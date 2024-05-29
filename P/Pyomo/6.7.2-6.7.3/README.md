# Comparing `tmp/Pyomo-6.7.2.tar.gz` & `tmp/Pyomo-6.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyomo-6.7.2.tar", last modified: Thu May  9 15:34:26 2024, max compression
+gzip compressed data, was "Pyomo-6.7.3.tar", last modified: Wed May 29 21:35:10 2024, max compression
```

## Comparing `Pyomo-6.7.2.tar` & `Pyomo-6.7.3.tar`

### file list

```diff
@@ -1,1510 +1,1511 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.571276 Pyomo-6.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-09 15:34:13.000000 Pyomo-6.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 15:34:13.000000 Pyomo-6.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-09 15:34:26.571276 Pyomo-6.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.367272 Pyomo-6.7.2/Pyomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-09 15:34:26.000000 Pyomo-6.7.2/Pyomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    53451 2024-05-09 15:34:26.000000 Pyomo-6.7.2/Pyomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:34:26.000000 Pyomo-6.7.2/Pyomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 15:34:26.000000 Pyomo-6.7.2/Pyomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-09 15:34:26.000000 Pyomo-6.7.2/Pyomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 15:34:26.000000 Pyomo-6.7.2/Pyomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-09 15:34:13.000000 Pyomo-6.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.367272 Pyomo-6.7.2/pyomo/
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/__future__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.371272 Pyomo-6.7.2/pyomo/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/autoslots.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/backports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/cmake_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.371272 Pyomo-6.7.2/pyomo/common/collections/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/collections/bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/collections/component_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/collections/component_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/collections/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (127)    95866 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    39759 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    21105 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/envvar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27265 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/gc_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/getGSL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/gsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/numeric_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/pyomo_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20308 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tee.py
--rw-r--r--   0 runner    (1001) docker     (127)    16192 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tempfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/config_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/dep_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/dep_mod_except.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/deps.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/import_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/relo_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/relo_mod_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/relocated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_component_map.py
--rw-r--r--   0 runner    (1001) docker     (127)   118848 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    23726 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_numeric_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_orderedset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_tee.py
--rw-r--r--   0 runner    (1001) docker     (127)    21463 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_tempfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    25880 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/tests/test_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)    37810 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    33700 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/common/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/FindASL.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/functions.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/contrib/appsi/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63435 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.379272 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.383272 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/common.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    67338 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/expression.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    32505 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/expression.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    32839 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/interval.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/interval.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/model_base.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/model_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.383272 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/tests/test_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.383272 Pyomo-6.7.2/pyomo/contrib/appsi/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/examples/getting_started.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.383272 Pyomo-6.7.2/pyomo/contrib/appsi/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/examples/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/examples/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/fbbt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.383272 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/cbc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/cplex.py
--rw-r--r--   0 runner    (1001) docker     (127)    60562 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/gurobi.py
--rw-r--r--   0 runner    (1001) docker     (127)    30217 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/highs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19812 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20101 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/maingo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/maingo_solvermodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25704 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_highs_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    57775 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_wntr_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/solvers/wntr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/appsi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/tests/test_fbbt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/tests/test_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/appsi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/utils/get_objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/appsi/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/appsi/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/writers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/writers/lp_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/writers/nl_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/appsi/writers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/writers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/appsi/writers/tests/test_nl_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/benders/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/benders_cuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/benders/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/examples/farmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/examples/grothey_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.387272 Pyomo-6.7.2/pyomo/contrib/benders/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/benders/tests/test_benders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.391272 Pyomo-6.7.2/pyomo/contrib/community_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/community_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    41445 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.391272 Pyomo-6.7.2/pyomo/contrib/community_detection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63466 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/community_detection/tests/test_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.391272 Pyomo-6.7.2/pyomo/contrib/cp/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/interval_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.391272 Pyomo-6.7.2/pyomo/contrib/cp/repn/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/repn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50331 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/repn/docplex_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.391272 Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/scheduling_logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/sequence_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/sequence_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.391272 Pyomo-6.7.2/pyomo/contrib/cp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67813 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_docplex_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_docplex_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_interval_var.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30065 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_precedence_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_sequence_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_sequence_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    19693 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/tests/test_step_function_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/cp/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/doe/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49775 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/doe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/doe/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_compute_FIM.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_optimize_doe.py
--rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/doe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    12406 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/tests/test_fim_doe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/doe/tests/test_reactor_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/example/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/example/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/plugins/ex_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/example/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/example/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.395273 Pyomo-6.7.2/pyomo/contrib/fbbt/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/expression_bounds_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    55929 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/fbbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24721 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.399273 Pyomo-6.7.2/pyomo/contrib/fbbt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/tests/test_expression_bounds_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    43511 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/tests/test_fbbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    17498 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fbbt/tests/test_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.399273 Pyomo-6.7.2/pyomo/contrib/fme/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32586 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fme/fourier_motzkin_elimination.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fme/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.399273 Pyomo-6.7.2/pyomo/contrib/fme/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fme/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38415 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.399273 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/compute_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.399273 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.403273 Pyomo-6.7.2/pyomo/contrib/gdpopt/
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/GDPopt.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/algorithm_base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/branch_and_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/config_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/create_oa_subproblems.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/cut_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/discrete_problem_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/enumerate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/gloa.py
--rw-r--r--   0 runner    (1001) docker     (127)    13252 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/loa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/nlp_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/oa_algorithm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/ric.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/solve_discrete_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/solve_subproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.403273 Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/test_LBB.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/test_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (127)    73110 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/test_gdpopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gdpopt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.403273 Pyomo-6.7.2/pyomo/contrib/gjh/
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gjh/GJH.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gjh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gjh/getGJH.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/gjh/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.403273 Pyomo-6.7.2/pyomo/contrib/iis/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/mis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.403273 Pyomo-6.7.2/pyomo/contrib/iis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/tests/test_iis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/tests/test_mis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/iis/tests/trivial_mis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.407273 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.407273 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.407273 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/incidence.py
--rw-r--r--   0 runner    (1001) docker     (127)    42797 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/scc_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.407273 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/models_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10051 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_incidence.py
--rw-r--r--   0 runner    (1001) docker     (127)    77033 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_triangularize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/triangularize.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/incidence_analysis/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.407273 Pyomo-6.7.2/pyomo/contrib/interior_point/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.407273 Pyomo-6.7.2/pyomo/contrib/interior_point/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/examples/ex1.py
--rw-r--r--   0 runner    (1001) docker     (127)    18758 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    27675 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/interior_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/inverse_reduced_hessian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.411273 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/ma27_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/mumps_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/scipy_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.411273 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/test_realloc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.411273 Pyomo-6.7.2/pyomo/contrib/interior_point/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_interior_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_realloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_reg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.411273 Pyomo-6.7.2/pyomo/contrib/latex_printer/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/latex_printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46955 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/latex_printer/latex_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.411273 Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/test_latex_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)   119853 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/test_latex_printer_vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.411273 Pyomo-6.7.2/pyomo/contrib/mcpp/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/getMCPP.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/mcppInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    17223 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/pyomo_mcpp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mcpp/test_mcpp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.415273 Pyomo-6.7.2/pyomo/contrib/mindtpy/
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/MindtPy.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   140954 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/algorithm_base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    26872 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/config_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/cut_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/extended_cutting_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/feasibility_pump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/global_outer_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/outer_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    43087 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/single_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tabu_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.419273 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP2_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP3_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP4_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP5_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP_simple_grey_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/eight_process_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/feasibility_pump1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/feasibility_pump2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/from_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/online_doc_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    21085 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_grey_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37557 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mindtpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.419273 Pyomo-6.7.2/pyomo/contrib/mpc/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.419273 Pyomo-6.7.2/pyomo/contrib/mpc/data/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/dynamic_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/find_nearest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/get_cuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/interval_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/scalar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/series_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_get_cuid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_interval_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_scalar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_series_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/run_mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/run_openloop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/copy_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/model_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/var_linker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.423273 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/cost_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.427273 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/test_terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.427273 Pyomo-6.7.2/pyomo/contrib/multistart/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/multistart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/multistart/high_conf_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/multistart/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/multistart/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/multistart/reinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/multistart/test_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.427273 Pyomo-6.7.2/pyomo/contrib/parmest/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.427273 Pyomo-6.7.2/pyomo/contrib/parmest/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.427273 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reaction_kinetics/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.431273 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/confidence_region_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.431273 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.431273 Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/parallel_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/scenario_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/semibatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21311 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/ipopt_solver_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    95547 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/parmest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/scenariocreator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.431273 Pyomo-6.7.2/pyomo/contrib/parmest/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)    77474 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_parmest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22344 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_scenariocreator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.435273 Pyomo-6.7.2/pyomo/contrib/parmest/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/utils/create_ef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/utils/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/parmest/utils/scenario_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.435273 Pyomo-6.7.2/pyomo/contrib/piecewise/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/piecewise_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    21052 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/piecewise_linear_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.435273 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/common_inner_repn_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_disaggregated_logarithmic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_nested_inner_repn_gdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.435273 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/convex_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/disaggregated_logarithmic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/inner_representation_gdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/nested_inner_repn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/outer_representation_gdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/piecewise_linear_transformation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.439273 Pyomo-6.7.2/pyomo/contrib/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.439273 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/constraint_tightener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/equality_propagate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/induced_linearity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/init_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/int_to_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/strip_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/var_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.443273 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_equality_propagate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_induced_linearity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_init_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_int_to_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_strip_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_var_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/preprocessing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.443273 Pyomo-6.7.2/pyomo/contrib/pynumero/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.443273 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.443273 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    24657 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.443273 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22682 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/asl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.447274 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.447274 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/reactor_design.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.447274 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.447274 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.447274 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17675 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/feasibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/mumps_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/nlp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/nlp_interface_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/parallel_matvec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/parallel_vector_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/sqp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.447274 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.451274 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33682 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/ampl_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/external_grey_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    18890 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/nlp_projections.py
--rw-r--r--   0 runner    (1001) docker     (127)    33401 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    59480 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.451274 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21711 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23094 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    86169 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    43312 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    43190 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35115 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py
--rw-r--r--   0 runner    (1001) docker     (127)   102434 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.455274 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma27.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma27_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma57.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma57_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/mumps_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/scipy_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.455274 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_ma27.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_ma57.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.455274 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/base_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    46318 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    59856 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/block_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    45374 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    56271 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/mpi_block_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.459274 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32251 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    36325 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)    53461 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    63243 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.459274 Pyomo-6.7.2/pyomo/contrib/pynumero/src/
--rw-r--r--   0 runner    (1001) docker     (127)    18075 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/AmplInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/AmplInterface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/AssertUtils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/ma27Interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/ma57Interface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.459274 Pyomo-6.7.2/pyomo/contrib/pynumero/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/tests/simple_nlp.nl
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/src/tests/simple_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.459274 Pyomo-6.7.2/pyomo/contrib/pynumero/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pynumero/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.459274 Pyomo-6.7.2/pyomo/contrib/pyros/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28898 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    33145 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/master_problem_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/pyros.py
--rw-r--r--   0 runner    (1001) docker     (127)    37868 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/pyros_algorithm_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    49923 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/separation_problem_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/solve_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/pyros/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20428 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   249981 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/tests/test_grcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    96732 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/uncertainty_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)    73256 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/pyros/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/satsolver/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/satsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/satsolver/satsolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/satsolver/test_satsolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9690 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/k_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    28361 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/sens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py
--rw-r--r--   0 runner    (1001) docker     (127)    35304 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/simplemodel/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplemodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/simplification/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/simplification/ginac/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/ginac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.463274 Pyomo-6.7.2/pyomo/contrib/simplification/ginac/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/ginac/src/ginac_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/ginac/src/ginac_interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.467274 Pyomo-6.7.2/pyomo/contrib/simplification/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/simplification/tests/test_simplification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.467274 Pyomo-6.7.2/pyomo/contrib/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23426 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14752 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    58164 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/gurobi.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/gurobi_direct.py
--rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20729 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/sol_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.467274 Pyomo-6.7.2/pyomo/contrib/solver/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.467274 Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/test_gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/test_ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    68410 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/test_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.467274 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.467274 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/sol_files/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/sol_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_sol_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/solver/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.471274 Pyomo-6.7.2/pyomo/contrib/trustregion/
--rw-r--r--   0 runner    (1001) docker     (127)    16856 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/TRF.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.471274 Pyomo-6.7.2/pyomo/contrib/trustregion/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2294 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.471274 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_TRF.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/trustregion/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.471274 Pyomo-6.7.2/pyomo/contrib/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/main.ui
--rw-r--r--   0 runner    (1001) docker     (127)    22054 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/model_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/model_browser.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/model_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/model_select.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/pyomo_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/qt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/residual_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/residual_table.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.475274 Pyomo-6.7.2/pyomo/contrib/viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_data_model_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_data_model_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/contrib/viewer/ui_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.475274 Pyomo-6.7.2/pyomo/core/
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.483274 Pyomo-6.7.2/pyomo/core/base/
--rw-r--r--   0 runner    (1001) docker     (127)    34707 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/PyomoModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    93464 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/blockutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    21419 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/boolean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    41048 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/component_namer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/component_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    26026 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/componentuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    36860 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/disable_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    16843 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    29704 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/global_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    48071 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/indexed_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    41781 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/indexed_component_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/instance2dat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/logical_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/numvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)    19191 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    37902 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/param.py
--rw-r--r--   0 runner    (1001) docker     (127)    58237 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/piecewise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    35898 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/range.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (127)    32908 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)   157776 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/set_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/sets.py
--rw-r--r--   0 runner    (1001) docker     (127)    21022 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/sos.py
--rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/symbol_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/template_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    58905 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/units_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    37253 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/base/var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.483274 Pyomo-6.7.2/pyomo/core/beta/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/beta/dict_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/beta/list_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.483274 Pyomo-6.7.2/pyomo/core/expr/
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/boolean_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.487274 Pyomo-6.7.2/pyomo/core/expr/calculus/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/calculus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/calculus/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/calculus/diff_with_pyomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/calculus/diff_with_sympy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/cnf_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/expr_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/expr_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/logical_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)   109971 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/numeric_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12940 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/numvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/relational_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/symbol_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/sympy_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/taylor_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    38237 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/template_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/expr/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.487274 Pyomo-6.7.2/pyomo/core/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/component_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/component_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/conic.py
--rw-r--r--   0 runner    (1001) docker     (127)    29572 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/container_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/dict_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/heterogeneous_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/homogeneous_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    15915 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.491274 Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45131 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/transforms_nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/register_numpy_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/set_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/sos.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/tuple_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/kernel/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.491274 Pyomo-6.7.2/pyomo/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.491274 Pyomo-6.7.2/pyomo/core/plugins/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/add_slack_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/discrete_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/eliminate_fixed_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/equality_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/expand_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/logical_to_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/nonnegative_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/radix_linearization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/relax_integrality.py
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/standard_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/plugins/transform/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/pyomoobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/staleflag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.491274 Pyomo-6.7.2/pyomo/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.491274 Pyomo-6.7.2/pyomo/core/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/data/test_odbc_ini.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.495274 Pyomo-6.7.2/pyomo/core/tests/diet/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/diet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/diet/test_diet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.495274 Pyomo-6.7.2/pyomo/core/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/pmedian.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/pmedian1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/pmedian2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/pmedian4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/pmedian_concrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/test_amplbook2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/test_kernel_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/test_pyomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/examples/test_tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.495274 Pyomo-6.7.2/pyomo/core/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23105 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/transform/test_add_slacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/transform/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    29458 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/transform/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.507274 Pyomo-6.7.2/pyomo/core/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.511275 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89754 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_component_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_component_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    30196 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_conic.py
--rw-r--r--   0 runner    (1001) docker     (127)    67770 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    37001 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_dict_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    40008 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    44784 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_sos.py
--rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    31639 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_tuple_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    37427 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)   122073 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_block_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    46512 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_componentuid.py
--rw-r--r--   0 runner    (1001) docker     (127)    56914 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_con.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_concrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    30317 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15985 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_derivs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_dict_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_disable_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_expr_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    35719 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    23167 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_external.py
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_indexed_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    27447 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_kernel_register_numpy_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_labelers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14855 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_list_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_logical_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_logical_expr_expanded.py
--rw-r--r--   0 runner    (1001) docker     (127)    33829 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_logical_to_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    36091 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_mutable.py
--rw-r--r--   0 runner    (1001) docker     (127)   188874 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    41414 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   275189 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)   249244 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_numpy_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    19349 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_numvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)    24637 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    76479 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_param.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    16809 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    34645 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_range.py
--rw-r--r--   0 runner    (1001) docker     (127)    46006 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    15319 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_relational_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)   224135 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_set.py
--rw-r--r--   0 runner    (1001) docker     (127)   129664 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_smap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_sos.py
--rw-r--r--   0 runner    (1001) docker     (127)    34102 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_sos_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    76333 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_symbol_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_taylor_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    27798 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_template_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    46156 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    64606 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_var_set_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    59887 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/test_xfrm_discrete_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/uninstantiated_model_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/tests/unit/uninstantiated_model_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.515275 Pyomo-6.7.2/pyomo/dae/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/contset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/diffvar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25259 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/integral.py
--rw-r--r--   0 runner    (1001) docker     (127)    18734 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.515275 Pyomo-6.7.2/pyomo/dae/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27260 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/plugins/colloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/plugins/finitedifference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    40990 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.515275 Pyomo-6.7.2/pyomo/dae/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_colloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_contset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_diffvar.py
--rw-r--r--   0 runner    (1001) docker     (127)    13717 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    79021 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_integral.py
--rw-r--r--   0 runner    (1001) docker     (127)    35439 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    49507 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/tests/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    71365 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dae/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.519275 Pyomo-6.7.2/pyomo/dataportal/
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/DataPortal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/TableData.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/parse_datacmds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.519275 Pyomo-6.7.2/pyomo/dataportal/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/csv_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/datacommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/db_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/json_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/plugins/xml_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    33443 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/process_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.519275 Pyomo-6.7.2/pyomo/dataportal/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/tests/test_dat_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    80503 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/dataportal/tests/test_dataportal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.519275 Pyomo-6.7.2/pyomo/duality/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/duality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/duality/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/duality/lagrangian_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/duality/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.519275 Pyomo-6.7.2/pyomo/duality/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/duality/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/duality/tests/test_linear_dual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.523275 Pyomo-6.7.2/pyomo/environ/
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/environ/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.523275 Pyomo-6.7.2/pyomo/environ/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/environ/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/environ/tests/standalone_minimal_pyomo_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/environ/tests/test_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/environ/tests/test_package_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.523275 Pyomo-6.7.2/pyomo/gdp/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/basic_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    29920 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/disjunct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.527275 Pyomo-6.7.2/pyomo/gdp/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/between_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    21683 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/bigm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/bigm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/bilinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/binary_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/bound_pretransformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/chull.py
--rw-r--r--   0 runner    (1001) docker     (127)    51943 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/cuttingplane.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/fix_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/gdp_to_mip_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/gdp_var_mover.py
--rw-r--r--   0 runner    (1001) docker     (127)    43373 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/hull.py
--rw-r--r--   0 runner    (1001) docker     (127)    32832 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/multiple_bigm.py
--rw-r--r--   0 runner    (1001) docker     (127)    38486 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/partition_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/plugins/transform_current_disjunctive_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.527275 Pyomo-6.7.2/pyomo/gdp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73755 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    38160 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_basic_step.py
--rw-r--r--   0 runner    (1001) docker     (127)   115559 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_bigm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_binary_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    38543 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_bound_pretransformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    49436 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_cuttingplane.py
--rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_disjunct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_fix_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_gdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_gdp_reclassification_error.py
--rw-r--r--   0 runner    (1001) docker     (127)   119545 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)    43576 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_mbigm.py
--rw-r--r--   0 runner    (1001) docker     (127)    88883 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_partition_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_reclassify.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_transform_current_disjunctive_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/transformed_disjunct.py
--rw-r--r--   0 runner    (1001) docker     (127)    24508 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/gdp/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.527275 Pyomo-6.7.2/pyomo/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/kernel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.531275 Pyomo-6.7.2/pyomo/mpec/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/complementarity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.531275 Pyomo-6.7.2/pyomo/mpec/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/mpec1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/mpec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/mpec3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/mpec4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/pathampl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/solver1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/plugins/solver2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.531275 Pyomo-6.7.2/pyomo/mpec/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/tests/test_complementarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/tests/test_minlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/tests/test_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/mpec/tests/test_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.531275 Pyomo-6.7.2/pyomo/neos/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/kestrel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.531275 Pyomo-6.7.2/pyomo/neos/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/plugins/NEOS.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/plugins/kestrel_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.531275 Pyomo-6.7.2/pyomo/neos/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/tests/model_min_lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/neos/tests/test_neos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/network/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39211 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    34799 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/foqus_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/network/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/plugins/expand_arcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/network/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86485 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/tests/test_arc.py
--rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    17236 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/tests/test_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/opt/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/opt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    28126 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/base/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/opt/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/parallel/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/parallel/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/parallel/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.535275 Pyomo-6.7.2/pyomo/opt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/plugins/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/plugins/res.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/plugins/sol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/problem/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/problem/ampl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/results/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/results/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/results/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/results/results_.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/results/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/results/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/solver/ilmcmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/solver/shellcmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/testing/pyunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/tests/base/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/test_ampl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/test_sol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9106 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/test_soln.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/base/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/opt/tests/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/opt/tests/solver/test_shellcmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.539275 Pyomo-6.7.2/pyomo/pysp/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/pysp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.543275 Pyomo-6.7.2/pyomo/repn/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.543275 Pyomo-6.7.2/pyomo/repn/beta/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24869 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/beta/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    27999 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.543275 Pyomo-6.7.2/pyomo/repn/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.543275 Pyomo-6.7.2/pyomo/repn/plugins/ampl/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/ampl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79843 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/ampl/ampl_.py
--rw-r--r--   0 runner    (1001) docker     (127)    32156 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/baron_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    39682 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/cpxlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    40619 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/gams_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/lp_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    32960 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)   120531 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/nl_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21877 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/plugins/standard_form.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/standard_aux.py
--rw-r--r--   0 runner    (1001) docker     (127)    60059 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/standard_repn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.543275 Pyomo-6.7.2/pyomo/repn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.547275 Pyomo-6.7.2/pyomo/repn/tests/ampl/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/nl_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small10_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small11_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small12_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small13_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small14_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small15_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small1_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small2_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small3_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small4_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small5_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small6_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small7_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small8_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/small9_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/test_ampl_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/test_ampl_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/test_ampl_repn.py
--rw-r--r--   0 runner    (1001) docker     (127)    73520 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/test_nlv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/ampl/test_suffixes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.547275 Pyomo-6.7.2/pyomo/repn/tests/baron/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/baron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/baron/small14a_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/baron/test_baron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/baron/test_baron_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.551275 Pyomo-6.7.2/pyomo/repn/tests/cpxlp/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/cpxlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/cpxlp/test_cpxlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/cpxlp/test_lpv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/diffutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.551275 Pyomo-6.7.2/pyomo/repn/tests/gams/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/gams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/gams/small14a_testCase.py
--rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/gams/test_gams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/gams/test_gams_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/lp_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.551275 Pyomo-6.7.2/pyomo/repn/tests/mps/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/mps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/mps/test_mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/nl_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    63527 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/test_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)   163906 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/test_standard_form.py
--rw-r--r--   0 runner    (1001) docker     (127)    32092 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    26171 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/repn/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.551275 Pyomo-6.7.2/pyomo/scripting/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/driver_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.551275 Pyomo-6.7.2/pyomo/scripting/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/plugins/build_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/plugins/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/plugins/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/plugins/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/plugins/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/pyomo_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/pyomo_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/pyomo_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/solve_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.551275 Pyomo-6.7.2/pyomo/scripting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/tests/test_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)    42654 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/scripting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.555276 Pyomo-6.7.2/pyomo/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/amplfunc_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/mockmip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.555276 Pyomo-6.7.2/pyomo/solvers/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.555276 Pyomo-6.7.2/pyomo/solvers/plugins/converter/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/converter/ampl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/converter/glpsol.py
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/converter/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/converter/pico.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.559275 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/ASL.py
--rw-r--r--   0 runner    (1001) docker     (127)    24289 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/BARON.py
--rw-r--r--   0 runner    (1001) docker     (127)    50930 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/CBCplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/CONOPT.py
--rw-r--r--   0 runner    (1001) docker     (127)    46074 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/CPLEX.py
--rw-r--r--   0 runner    (1001) docker     (127)    56796 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GAMS.py
--rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GLPK.py
--rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GUROBI.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GUROBI_RUN.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/IPOPT.py
--rw-r--r--   0 runner    (1001) docker     (127)    19887 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/SCIPAMPL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/XPRESS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41460 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/cplex_direct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/cplex_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/direct_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    46352 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/gurobi_direct.py
--rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    54326 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/mosek_direct.py
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/mosek_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/persistent_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/pywrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    43929 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/xpress_direct.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/plugins/solvers/xpress_persistent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.559275 Pyomo-6.7.2/pyomo/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.563276 Pyomo-6.7.2/pyomo/solvers/tests/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_BARON.py
--rw-r--r--   0 runner    (1001) docker     (127)    18940 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_CBCplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21968 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_CPLEXDirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_CPLEXPersistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19199 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_GAMS.py
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_MOSEKDirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_MOSEKPersistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_amplfunc_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_cbc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_cplex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_gurobi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_gurobi_direct.py
--rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_no_solution_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/checks/test_xpress_persistent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.563276 Pyomo-6.7.2/pyomo/solvers/tests/mip/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_asl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_mip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_qp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_scip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_scip_log_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_scip_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/mip/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.567276 Pyomo-6.7.2/pyomo/solvers/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_compiled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_constant_objective1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_constant_objective2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_duals_maximize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_duals_minimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_inactive_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_infeasible1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_infeasible2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_trivial_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_unbounded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_unique_duals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/LP_unused_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_infeasible1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_unbounded.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_unused_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MIQCP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/MIQP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/QCP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/QP_constant_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/QP_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/SOS1_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/SOS2_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18504 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.567276 Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/tests/testcases.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/solvers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.571276 Pyomo-6.7.2/pyomo/util/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/blockutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/calc_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/check_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/infeasible.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/model_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/report_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/slices.py
--rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/subsystems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.571276 Pyomo-6.7.2/pyomo/util/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_blockutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    17771 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_calc_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_check_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_infeasible.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_model_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_report_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    28108 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/tests/test_subsystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/util/vars_from_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.571276 Pyomo-6.7.2/pyomo/version/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/version/info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:34:26.571276 Pyomo-6.7.2/pyomo/version/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/version/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/version/tests/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-09 15:34:13.000000 Pyomo-6.7.2/pyomo/version/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-09 15:34:26.571276 Pyomo-6.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-05-09 15:34:13.000000 Pyomo-6.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.357447 Pyomo-6.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-29 21:35:00.000000 Pyomo-6.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 21:35:00.000000 Pyomo-6.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-29 21:35:10.357447 Pyomo-6.7.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.161447 Pyomo-6.7.3/Pyomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-29 21:35:09.000000 Pyomo-6.7.3/Pyomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    53496 2024-05-29 21:35:10.000000 Pyomo-6.7.3/Pyomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:35:09.000000 Pyomo-6.7.3/Pyomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 21:35:09.000000 Pyomo-6.7.3/Pyomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-29 21:35:09.000000 Pyomo-6.7.3/Pyomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 21:35:09.000000 Pyomo-6.7.3/Pyomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-29 21:35:00.000000 Pyomo-6.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.161447 Pyomo-6.7.3/pyomo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/__future__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.169448 Pyomo-6.7.3/pyomo/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/autoslots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/backports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/cmake_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.169448 Pyomo-6.7.3/pyomo/common/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/collections/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/collections/component_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/collections/component_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/collections/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95866 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39759 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21105 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27265 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/gc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/getGSL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/gsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/numeric_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/pyomo_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20308 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16192 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tempfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.173447 Pyomo-6.7.3/pyomo/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/config_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/dep_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/dep_mod_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/import_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/relo_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/relo_mod_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/relocated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_component_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118848 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23726 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_numeric_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_tee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21463 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25880 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/tests/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37810 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33700 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/common/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.173447 Pyomo-6.7.3/pyomo/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.173447 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.173447 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/FindASL.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/functions.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.173447 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.177447 Pyomo-6.7.3/pyomo/contrib/appsi/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63435 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.177447 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.177447 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    67338 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/expression.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32505 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/expression.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32839 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/interval.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/interval.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/model_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/model_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.177447 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.177447 Pyomo-6.7.3/pyomo/contrib/appsi/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/examples/getting_started.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.181447 Pyomo-6.7.3/pyomo/contrib/appsi/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/examples/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/examples/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.181447 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/cbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/cplex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60562 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30217 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/highs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19812 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20101 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/maingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/maingo_solvermodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.181447 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25704 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_highs_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57775 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_wntr_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/solvers/wntr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.181447 Pyomo-6.7.3/pyomo/contrib/appsi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/tests/test_fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/tests/test_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.181447 Pyomo-6.7.3/pyomo/contrib/appsi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/utils/get_objective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.181447 Pyomo-6.7.3/pyomo/contrib/appsi/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/appsi/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/writers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/writers/lp_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/writers/nl_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/appsi/writers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/writers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/appsi/writers/tests/test_nl_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/benders/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/benders_cuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/benders/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/examples/farmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/examples/grothey_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/benders/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/benders/tests/test_benders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/community_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/community_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41442 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/community_detection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63466 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/community_detection/tests/test_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.185447 Pyomo-6.7.3/pyomo/contrib/cp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/interval_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.189447 Pyomo-6.7.3/pyomo/contrib/cp/repn/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/repn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50331 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/repn/docplex_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.189447 Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/scheduling_logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/sequence_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/sequence_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.189447 Pyomo-6.7.3/pyomo/contrib/cp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67813 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_docplex_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_docplex_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_interval_var.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30065 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_precedence_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_sequence_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_sequence_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19693 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/tests/test_step_function_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.189447 Pyomo-6.7.3/pyomo/contrib/cp/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.189447 Pyomo-6.7.3/pyomo/contrib/doe/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57287 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/doe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/doe/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_compute_FIM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_optimize_doe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29606 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/doe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16222 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/tests/test_fim_doe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/doe/tests/test_reactor_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/example/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/plugins/ex_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/example/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/fbbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/expression_bounds_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55929 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24721 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.193447 Pyomo-6.7.3/pyomo/contrib/fbbt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/tests/test_expression_bounds_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43511 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/tests/test_fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17498 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fbbt/tests/test_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.197447 Pyomo-6.7.3/pyomo/contrib/fme/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32586 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fme/fourier_motzkin_elimination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fme/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.197447 Pyomo-6.7.3/pyomo/contrib/fme/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fme/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38415 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.197447 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/compute_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.197447 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.201447 Pyomo-6.7.3/pyomo/contrib/gdpopt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/GDPopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/algorithm_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/branch_and_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/config_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/create_oa_subproblems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/cut_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/discrete_problem_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/gloa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13252 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/loa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/nlp_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/oa_algorithm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/ric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/solve_discrete_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/solve_subproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.201447 Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/test_LBB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/test_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73110 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/test_gdpopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gdpopt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.201447 Pyomo-6.7.3/pyomo/contrib/gjh/
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gjh/GJH.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gjh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gjh/getGJH.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/gjh/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.201447 Pyomo-6.7.3/pyomo/contrib/iis/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/mis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.201447 Pyomo-6.7.3/pyomo/contrib/iis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/tests/test_iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/tests/test_mis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/iis/tests/trivial_mis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/incidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42797 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/scc_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/models_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10051 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_incidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77033 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_triangularize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/triangularize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/incidence_analysis/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/interior_point/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/interior_point/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/examples/ex1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18758 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27675 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/interior_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/inverse_reduced_hessian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.205447 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/ma27_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/mumps_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/scipy_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.209447 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/test_realloc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.209447 Pyomo-6.7.3/pyomo/contrib/interior_point/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_interior_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_realloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_reg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.209447 Pyomo-6.7.3/pyomo/contrib/latex_printer/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/latex_printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46955 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/latex_printer/latex_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.209447 Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/test_latex_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119853 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/test_latex_printer_vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.209447 Pyomo-6.7.3/pyomo/contrib/mcpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/getMCPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/mcppInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17223 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/pyomo_mcpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mcpp/test_mcpp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.213447 Pyomo-6.7.3/pyomo/contrib/mindtpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/MindtPy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140954 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/algorithm_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26872 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/config_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/cut_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/extended_cutting_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/feasibility_pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/global_outer_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/outer_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43087 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/single_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tabu_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.217447 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP3_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP4_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP5_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP_simple_grey_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/eight_process_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/feasibility_pump1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/feasibility_pump2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/from_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/online_doc_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21085 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_grey_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37557 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mindtpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.217447 Pyomo-6.7.3/pyomo/contrib/mpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.217447 Pyomo-6.7.3/pyomo/contrib/mpc/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/dynamic_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/find_nearest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/get_cuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/interval_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/scalar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/series_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.217447 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_get_cuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_interval_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_scalar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_series_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.217447 Pyomo-6.7.3/pyomo/contrib/mpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.217447 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/run_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/run_openloop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.221447 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.221447 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/copy_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/model_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.221447 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/var_linker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.221447 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/cost_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.221447 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/test_terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.221447 Pyomo-6.7.3/pyomo/contrib/multistart/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/multistart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/multistart/high_conf_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/multistart/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/multistart/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/multistart/reinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/multistart/test_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.225447 Pyomo-6.7.3/pyomo/contrib/parmest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.225447 Pyomo-6.7.3/pyomo/contrib/parmest/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.225447 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reaction_kinetics/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.225447 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/confidence_region_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.225447 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.229447 Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/parallel_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/scenario_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/semibatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21311 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/ipopt_solver_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95547 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/parmest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/scenariocreator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.229447 Pyomo-6.7.3/pyomo/contrib/parmest/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77474 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_parmest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22344 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_scenariocreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.229447 Pyomo-6.7.3/pyomo/contrib/parmest/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/utils/create_ef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/utils/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/parmest/utils/scenario_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.229447 Pyomo-6.7.3/pyomo/contrib/piecewise/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/piecewise_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21052 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/piecewise_linear_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.233447 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/common_inner_repn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_disaggregated_logarithmic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_nested_inner_repn_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.233447 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/convex_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/disaggregated_logarithmic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/inner_representation_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/nested_inner_repn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/outer_representation_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/piecewise_linear_transformation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.233447 Pyomo-6.7.3/pyomo/contrib/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.233447 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/constraint_tightener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/equality_propagate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/induced_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/int_to_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/strip_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/var_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.237447 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_equality_propagate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_induced_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_int_to_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_strip_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_var_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/preprocessing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.237447 Pyomo-6.7.3/pyomo/contrib/pynumero/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.237447 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.237447 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24657 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.241447 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22682 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/asl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.241447 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.241447 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/reactor_design.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.241447 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.241447 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.241447 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17675 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/feasibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/mumps_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/nlp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/nlp_interface_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/parallel_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/parallel_vector_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/sqp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.245447 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.245447 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33682 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/ampl_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/external_grey_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18890 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/nlp_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33401 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59480 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.249447 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21711 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23094 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86169 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43312 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43190 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35115 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102434 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.249447 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma27.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma27_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma57.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma57_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/mumps_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/scipy_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.249447 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_ma27.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_ma57.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.249447 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/base_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46318 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59856 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/block_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45374 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56271 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/mpi_block_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.253447 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32251 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36325 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53461 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63243 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.253447 Pyomo-6.7.3/pyomo/contrib/pynumero/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    18075 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/AmplInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/AmplInterface.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/AssertUtils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/ma27Interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/ma57Interface.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.253447 Pyomo-6.7.3/pyomo/contrib/pynumero/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/tests/simple_nlp.nl
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/src/tests/simple_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.253447 Pyomo-6.7.3/pyomo/contrib/pynumero/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pynumero/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.253447 Pyomo-6.7.3/pyomo/contrib/pyros/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28898 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33145 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/master_problem_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/pyros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37868 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/pyros_algorithm_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49923 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/separation_problem_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/solve_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.253447 Pyomo-6.7.3/pyomo/contrib/pyros/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20428 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249981 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/tests/test_grcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96732 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/uncertainty_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73256 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/pyros/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/satsolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/satsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/satsolver/satsolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/satsolver/test_satsolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9690 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/k_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28361 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/sens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35304 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/simplemodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplemodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/simplification/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/simplification/ginac/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/ginac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/simplification/ginac/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/ginac/src/ginac_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/ginac/src/ginac_interface.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.257447 Pyomo-6.7.3/pyomo/contrib/simplification/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/simplification/tests/test_simplification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.261447 Pyomo-6.7.3/pyomo/contrib/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23426 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14752 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58164 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/gurobi_direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20729 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/sol_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.261447 Pyomo-6.7.3/pyomo/contrib/solver/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.261447 Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/test_gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/test_ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68410 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/test_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.261447 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.261447 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/sol_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/sol_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_sol_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/solver/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.261447 Pyomo-6.7.3/pyomo/contrib/trustregion/
+-rw-r--r--   0 runner    (1001) docker     (127)    16856 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/TRF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.265447 Pyomo-6.7.3/pyomo/contrib/trustregion/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2294 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.265447 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_TRF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/trustregion/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.265447 Pyomo-6.7.3/pyomo/contrib/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/main.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    22054 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/model_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/model_browser.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/model_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/model_select.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/pyomo_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/residual_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/residual_table.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.265447 Pyomo-6.7.3/pyomo/contrib/viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_data_model_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_data_model_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/contrib/viewer/ui_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.269447 Pyomo-6.7.3/pyomo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.273447 Pyomo-6.7.3/pyomo/core/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    34707 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/PyomoModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93464 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/blockutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21419 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/boolean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41048 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/component_namer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/component_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26026 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/componentuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36860 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/disable_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16843 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29704 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/global_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48071 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/indexed_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41781 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/indexed_component_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/instance2dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/logical_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/numvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19191 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37902 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58237 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35898 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32908 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)   157776 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/set_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21022 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/sos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/symbol_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/template_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58905 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/units_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37253 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/base/var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.273447 Pyomo-6.7.3/pyomo/core/beta/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/beta/dict_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/beta/list_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.277447 Pyomo-6.7.3/pyomo/core/expr/
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/boolean_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.277447 Pyomo-6.7.3/pyomo/core/expr/calculus/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/calculus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/calculus/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/calculus/diff_with_pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/calculus/diff_with_sympy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/cnf_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/expr_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/expr_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/logical_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109971 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/numeric_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12940 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/numvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/relational_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/symbol_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/sympy_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/taylor_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38237 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/template_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/expr/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.281447 Pyomo-6.7.3/pyomo/core/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/component_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/component_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/conic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29572 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/container_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/dict_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/heterogeneous_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/homogeneous_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/list_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15915 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.281447 Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45131 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/transforms_nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/register_numpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/set_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/sos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/tuple_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/kernel/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.281447 Pyomo-6.7.3/pyomo/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.285447 Pyomo-6.7.3/pyomo/core/plugins/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/add_slack_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/discrete_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/eliminate_fixed_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/equality_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/expand_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/logical_to_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/nonnegative_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/radix_linearization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/relax_integrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/standard_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/plugins/transform/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/pyomoobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/staleflag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.285447 Pyomo-6.7.3/pyomo/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.285447 Pyomo-6.7.3/pyomo/core/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/data/test_odbc_ini.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.285447 Pyomo-6.7.3/pyomo/core/tests/diet/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/diet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/diet/test_diet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.285447 Pyomo-6.7.3/pyomo/core/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/pmedian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/pmedian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/pmedian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/pmedian4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/pmedian_concrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/test_amplbook2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/test_kernel_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/test_pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/examples/test_tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.285447 Pyomo-6.7.3/pyomo/core/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23105 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/transform/test_add_slacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/transform/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29458 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/transform/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.297447 Pyomo-6.7.3/pyomo/core/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.301447 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89754 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_component_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_component_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30196 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_conic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67770 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37001 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_dict_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40008 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_list_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44784 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_sos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31639 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_tuple_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37427 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122073 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_block_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46512 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_componentuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56914 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_con.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_concrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30317 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15985 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_derivs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_dict_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_disable_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_expr_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35719 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23167 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_indexed_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27447 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_kernel_register_numpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_labelers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14855 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_list_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_logical_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_logical_expr_expanded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33829 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_logical_to_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36091 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_mutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188874 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41414 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   275189 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249244 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_numpy_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19349 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_numvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24637 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76479 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16809 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34645 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46006 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15319 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_relational_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   224135 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129664 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_smap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_sos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34102 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_sos_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76333 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_symbol_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_taylor_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27798 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_template_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46156 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64606 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_var_set_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59887 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/test_xfrm_discrete_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/uninstantiated_model_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/tests/unit/uninstantiated_model_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.301447 Pyomo-6.7.3/pyomo/dae/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/contset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/diffvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25259 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18734 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.305447 Pyomo-6.7.3/pyomo/dae/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27260 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/plugins/colloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/plugins/finitedifference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40990 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.305447 Pyomo-6.7.3/pyomo/dae/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_colloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_contset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_diffvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13717 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79021 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35439 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49507 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/tests/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71365 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dae/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.305447 Pyomo-6.7.3/pyomo/dataportal/
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/DataPortal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/TableData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/parse_datacmds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/dataportal/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/csv_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/datacommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/db_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/plugins/xml_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33443 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/process_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/dataportal/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/tests/test_dat_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80503 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/dataportal/tests/test_dataportal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/duality/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/duality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/duality/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/duality/lagrangian_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/duality/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/duality/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/duality/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/duality/tests/test_linear_dual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/environ/
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/environ/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/environ/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/environ/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/environ/tests/standalone_minimal_pyomo_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/environ/tests/test_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/environ/tests/test_package_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.309447 Pyomo-6.7.3/pyomo/gdp/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/basic_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29920 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/disjunct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.313447 Pyomo-6.7.3/pyomo/gdp/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/between_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21683 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/bigm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/bigm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/bilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/binary_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/bound_pretransformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/chull.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51943 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/cuttingplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/fix_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/gdp_to_mip_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/gdp_var_mover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43373 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32832 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/multiple_bigm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38486 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/partition_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/plugins/transform_current_disjunctive_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/gdp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73755 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38160 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_basic_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115559 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_bigm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_binary_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38543 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_bound_pretransformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49436 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_cuttingplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_disjunct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_fix_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_gdp_reclassification_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119545 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43576 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_mbigm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88883 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_partition_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_reclassify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_transform_current_disjunctive_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/transformed_disjunct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24508 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/gdp/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/kernel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/mpec/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/complementarity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/mpec/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/mpec1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/mpec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/mpec3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/mpec4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/pathampl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/solver1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/plugins/solver2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/mpec/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/tests/test_complementarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/tests/test_minlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/tests/test_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/mpec/tests/test_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/neos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/kestrel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/neos/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/plugins/NEOS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/plugins/kestrel_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.317447 Pyomo-6.7.3/pyomo/neos/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/tests/model_min_lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/neos/tests/test_neos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39211 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34799 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/foqus_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/network/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/plugins/expand_arcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/network/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86485 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/tests/test_arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17236 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/tests/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/opt/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/opt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28126 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/base/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/opt/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/parallel/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/parallel/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/parallel/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.321447 Pyomo-6.7.3/pyomo/opt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/plugins/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/plugins/res.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/plugins/sol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/problem/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/problem/ampl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/results/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/results/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/results/results_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/results/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/results/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/solver/ilmcmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/solver/shellcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/testing/pyunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/test_ampl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/test_sol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9106 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/test_soln.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/base/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/opt/tests/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/opt/tests/solver/test_shellcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.325447 Pyomo-6.7.3/pyomo/pysp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/pysp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.329447 Pyomo-6.7.3/pyomo/repn/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.329447 Pyomo-6.7.3/pyomo/repn/beta/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24869 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/beta/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27999 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.329447 Pyomo-6.7.3/pyomo/repn/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.329447 Pyomo-6.7.3/pyomo/repn/plugins/ampl/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/ampl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79843 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/ampl/ampl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32156 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/baron_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39682 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/cpxlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40619 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/gams_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/lp_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32960 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129079 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/nl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21877 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/plugins/standard_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/standard_aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60059 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/standard_repn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.333447 Pyomo-6.7.3/pyomo/repn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.333447 Pyomo-6.7.3/pyomo/repn/tests/ampl/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/nl_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small10_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small11_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small12_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small13_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small14_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small15_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small1_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small2_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small3_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small4_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small5_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small6_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small7_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small8_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/small9_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/test_ampl_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/test_ampl_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/test_ampl_repn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84048 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/test_nlv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/ampl/test_suffixes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.337447 Pyomo-6.7.3/pyomo/repn/tests/baron/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/baron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/baron/small14a_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/baron/test_baron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/baron/test_baron_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.337447 Pyomo-6.7.3/pyomo/repn/tests/cpxlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/cpxlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/cpxlp/test_cpxlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/cpxlp/test_lpv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/diffutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.337447 Pyomo-6.7.3/pyomo/repn/tests/gams/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/gams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/gams/small14a_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/gams/test_gams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/gams/test_gams_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/lp_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.337447 Pyomo-6.7.3/pyomo/repn/tests/mps/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/mps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/mps/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/nl_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63527 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/test_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   163906 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/test_standard_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32092 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26171 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/repn/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.337447 Pyomo-6.7.3/pyomo/scripting/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/driver_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.341447 Pyomo-6.7.3/pyomo/scripting/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/plugins/build_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/plugins/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/plugins/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/plugins/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/plugins/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/pyomo_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/pyomo_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/pyomo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/solve_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.341447 Pyomo-6.7.3/pyomo/scripting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/tests/test_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42654 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/scripting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.341447 Pyomo-6.7.3/pyomo/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/amplfunc_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/mockmip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.341447 Pyomo-6.7.3/pyomo/solvers/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.341447 Pyomo-6.7.3/pyomo/solvers/plugins/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/converter/ampl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/converter/glpsol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/converter/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/converter/pico.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.345447 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/ASL.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24289 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/BARON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50791 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/CBCplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/CONOPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46074 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/CPLEX.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56796 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GAMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GLPK.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GUROBI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GUROBI_RUN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/IPOPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19887 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/SCIPAMPL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/XPRESS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41460 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/cplex_direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/cplex_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/direct_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46352 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/gurobi_direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54326 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/mosek_direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/mosek_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/persistent_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/pywrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43929 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/xpress_direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/plugins/solvers/xpress_persistent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.345447 Pyomo-6.7.3/pyomo/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.349447 Pyomo-6.7.3/pyomo/solvers/tests/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_BARON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18940 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_CBCplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21968 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_CPLEXDirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_CPLEXPersistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19199 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_GAMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_MOSEKDirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_MOSEKPersistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_amplfunc_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_cbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_cplex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_gurobi_direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_no_solution_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/checks/test_xpress_persistent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.349447 Pyomo-6.7.3/pyomo/solvers/tests/mip/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_asl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_mip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_qp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_scip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_scip_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_scip_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/mip/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.353447 Pyomo-6.7.3/pyomo/solvers/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_compiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_constant_objective1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_constant_objective2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_duals_maximize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_duals_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_inactive_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_infeasible1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_infeasible2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_trivial_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_unbounded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_unique_duals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/LP_unused_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_infeasible1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_unbounded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_unused_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MIQCP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/MIQP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/QCP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/QP_constant_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/QP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/SOS1_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/SOS2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18504 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.357447 Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/tests/testcases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/solvers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.357447 Pyomo-6.7.3/pyomo/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/blockutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/calc_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/check_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/infeasible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/model_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/report_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/subsystems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.357447 Pyomo-6.7.3/pyomo/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_blockutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17771 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_calc_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_check_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_infeasible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_model_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_report_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28108 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/tests/test_subsystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/util/vars_from_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.357447 Pyomo-6.7.3/pyomo/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/version/info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:35:10.357447 Pyomo-6.7.3/pyomo/version/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/version/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/version/tests/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-29 21:35:01.000000 Pyomo-6.7.3/pyomo/version/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-29 21:35:10.361446 Pyomo-6.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-29 21:35:01.000000 Pyomo-6.7.3/setup.py
```

### Comparing `Pyomo-6.7.2/LICENSE.md` & `Pyomo-6.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/PKG-INFO` & `Pyomo-6.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyomo
-Version: 6.7.2
+Version: 6.7.3
 Summary: Pyomo: Python Optimization Modeling Objects
 Home-page: http://pyomo.org
 Maintainer: Pyomo Developer Team
 Maintainer-email: pyomo-developers@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://pyomo.readthedocs.io/
 Project-URL: Source, https://github.com/Pyomo/pyomo
```

### Comparing `Pyomo-6.7.2/Pyomo.egg-info/PKG-INFO` & `Pyomo-6.7.3/Pyomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyomo
-Version: 6.7.2
+Version: 6.7.3
 Summary: Pyomo: Python Optimization Modeling Objects
 Home-page: http://pyomo.org
 Maintainer: Pyomo Developer Team
 Maintainer-email: pyomo-developers@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://pyomo.readthedocs.io/
 Project-URL: Source, https://github.com/Pyomo/pyomo
```

### Comparing `Pyomo-6.7.2/Pyomo.egg-info/SOURCES.txt` & `Pyomo-6.7.3/Pyomo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 pyomo/contrib/doe/__init__.py
 pyomo/contrib/doe/doe.py
 pyomo/contrib/doe/measurements.py
 pyomo/contrib/doe/result.py
 pyomo/contrib/doe/scenario.py
 pyomo/contrib/doe/examples/__init__.py
 pyomo/contrib/doe/examples/reactor_compute_FIM.py
+pyomo/contrib/doe/examples/reactor_design.py
 pyomo/contrib/doe/examples/reactor_grid_search.py
 pyomo/contrib/doe/examples/reactor_kinetics.py
 pyomo/contrib/doe/examples/reactor_optimize_doe.py
 pyomo/contrib/doe/tests/__init__.py
 pyomo/contrib/doe/tests/test_example.py
 pyomo/contrib/doe/tests/test_fim_doe.py
 pyomo/contrib/doe/tests/test_reactor_example.py
```

### Comparing `Pyomo-6.7.2/Pyomo.egg-info/requires.txt` & `Pyomo-6.7.3/Pyomo.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 enum_tools
 numpy<2.0.0
 scipy
 
 [optional]
 dill
 ipython
-matplotlib!=3.6.1
+matplotlib!=3.6.1,>=3.6.0
 numpy<2.0.0
 openpyxl
 pint
 plotly
 python-louvain
 pyyaml
 qtconsole
```

### Comparing `Pyomo-6.7.2/README.md` & `Pyomo-6.7.3/README.md`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/__future__.py` & `Pyomo-6.7.3/pyomo/__future__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/__init__.py` & `Pyomo-6.7.3/pyomo/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/__init__.py` & `Pyomo-6.7.3/pyomo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/_command.py` & `Pyomo-6.7.3/pyomo/common/_command.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/_common.py` & `Pyomo-6.7.3/pyomo/common/_common.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/autoslots.py` & `Pyomo-6.7.3/pyomo/common/autoslots.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/backports.py` & `Pyomo-6.7.3/pyomo/common/backports.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/cmake_builder.py` & `Pyomo-6.7.3/pyomo/common/cmake_builder.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/collections/__init__.py` & `Pyomo-6.7.3/pyomo/common/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/collections/bunch.py` & `Pyomo-6.7.3/pyomo/common/collections/bunch.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/collections/component_map.py` & `Pyomo-6.7.3/pyomo/common/collections/component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/collections/component_set.py` & `Pyomo-6.7.3/pyomo/common/collections/component_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/collections/orderedset.py` & `Pyomo-6.7.3/pyomo/common/collections/orderedset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/config.py` & `Pyomo-6.7.3/pyomo/common/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/dependencies.py` & `Pyomo-6.7.3/pyomo/common/dependencies.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/deprecation.py` & `Pyomo-6.7.3/pyomo/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/download.py` & `Pyomo-6.7.3/pyomo/common/download.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/enums.py` & `Pyomo-6.7.3/pyomo/common/enums.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/env.py` & `Pyomo-6.7.3/pyomo/common/env.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/envvar.py` & `Pyomo-6.7.3/pyomo/common/envvar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/errors.py` & `Pyomo-6.7.3/pyomo/common/errors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/extensions.py` & `Pyomo-6.7.3/pyomo/common/extensions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/factory.py` & `Pyomo-6.7.3/pyomo/common/factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/fileutils.py` & `Pyomo-6.7.3/pyomo/common/fileutils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/formatting.py` & `Pyomo-6.7.3/pyomo/common/formatting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/gc_manager.py` & `Pyomo-6.7.3/pyomo/common/gc_manager.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/getGSL.py` & `Pyomo-6.7.3/pyomo/common/getGSL.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/gsl.py` & `Pyomo-6.7.3/pyomo/common/gsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 @deprecated(
     "Use of get_gsl is deprecated and NO LONGER FUNCTIONS as of February 9, 2023. ",
     version='6.5.0',
 )
 def get_gsl(downloader):
     logger.info(
-        "As of February 9, 2023, AMPL GSL can no longer be downloaded\
-        through download-extensions. Visit https://portal.ampl.com/\
+        "As of February 9, 2023, AMPL GSL can no longer be downloaded \
+        through download-extensions. Visit https://portal.ampl.com/ \
         to download the AMPL GSL binaries."
     )
 
 
 def find_GSL():
     # FIXME: the GSL interface is currently broken in PyPy:
     if platform.python_implementation().lower().startswith('pypy'):
```

### Comparing `Pyomo-6.7.2/pyomo/common/log.py` & `Pyomo-6.7.3/pyomo/common/log.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/modeling.py` & `Pyomo-6.7.3/pyomo/common/modeling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/multithread.py` & `Pyomo-6.7.3/pyomo/common/multithread.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/numeric_types.py` & `Pyomo-6.7.3/pyomo/common/numeric_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/plugin.py` & `Pyomo-6.7.3/pyomo/common/plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/plugin_base.py` & `Pyomo-6.7.3/pyomo/common/plugin_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/plugins.py` & `Pyomo-6.7.3/pyomo/common/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/pyomo_typing.py` & `Pyomo-6.7.3/pyomo/common/pyomo_typing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/shutdown.py` & `Pyomo-6.7.3/pyomo/common/shutdown.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/sorting.py` & `Pyomo-6.7.3/pyomo/common/sorting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tee.py` & `Pyomo-6.7.3/pyomo/common/tee.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tempfiles.py` & `Pyomo-6.7.3/pyomo/common/tempfiles.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/__init__.py` & `Pyomo-6.7.3/pyomo/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/config_plugin.py` & `Pyomo-6.7.3/pyomo/common/tests/config_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/dep_mod.py` & `Pyomo-6.7.3/pyomo/common/tests/dep_mod.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/dep_mod_except.py` & `Pyomo-6.7.3/pyomo/common/tests/dep_mod_except.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/deps.py` & `Pyomo-6.7.3/pyomo/common/tests/deps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/import_ex.py` & `Pyomo-6.7.3/pyomo/common/tests/import_ex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/relo_mod.py` & `Pyomo-6.7.3/pyomo/common/tests/relo_mod.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/relo_mod_new.py` & `Pyomo-6.7.3/pyomo/common/tests/relo_mod_new.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/relocated.py` & `Pyomo-6.7.3/pyomo/common/tests/relocated.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_bunch.py` & `Pyomo-6.7.3/pyomo/common/tests/test_bunch.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_component_map.py` & `Pyomo-6.7.3/pyomo/common/tests/test_component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_config.py` & `Pyomo-6.7.3/pyomo/common/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_dependencies.py` & `Pyomo-6.7.3/pyomo/common/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_deprecated.py` & `Pyomo-6.7.3/pyomo/common/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_download.py` & `Pyomo-6.7.3/pyomo/common/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_enums.py` & `Pyomo-6.7.3/pyomo/common/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_env.py` & `Pyomo-6.7.3/pyomo/common/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_errors.py` & `Pyomo-6.7.3/pyomo/common/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_fileutils.py` & `Pyomo-6.7.3/pyomo/common/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_formatting.py` & `Pyomo-6.7.3/pyomo/common/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_gc.py` & `Pyomo-6.7.3/pyomo/common/tests/test_gc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_log.py` & `Pyomo-6.7.3/pyomo/common/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_modeling.py` & `Pyomo-6.7.3/pyomo/common/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_multithread.py` & `Pyomo-6.7.3/pyomo/common/tests/test_multithread.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_numeric_types.py` & `Pyomo-6.7.3/pyomo/common/tests/test_numeric_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_orderedset.py` & `Pyomo-6.7.3/pyomo/common/tests/test_orderedset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_plugin.py` & `Pyomo-6.7.3/pyomo/common/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_sorting.py` & `Pyomo-6.7.3/pyomo/common/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_tee.py` & `Pyomo-6.7.3/pyomo/common/tests/test_tee.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_tempfile.py` & `Pyomo-6.7.3/pyomo/common/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_timing.py` & `Pyomo-6.7.3/pyomo/common/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_typing.py` & `Pyomo-6.7.3/pyomo/common/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/tests/test_unittest.py` & `Pyomo-6.7.3/pyomo/common/tests/test_unittest.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/timing.py` & `Pyomo-6.7.3/pyomo/common/timing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/common/unittest.py` & `Pyomo-6.7.3/pyomo/common/unittest.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/build.py` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/FindASL.cmake` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/FindASL.cmake`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/src/functions.c` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/src/functions.c`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py` & `Pyomo-6.7.3/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/base.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/build.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/common.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/common.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/common.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/common.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/expression.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/expression.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/expression.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/expression.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/interval.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/interval.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/interval.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/interval.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/model_base.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/model_base.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/model_base.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/model_base.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/cmodel/tests/test_import.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/cmodel/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/examples/getting_started.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/examples/getting_started.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/examples/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/examples/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/examples/tests/test_examples.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/examples/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/fbbt.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/fbbt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/cbc.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/cbc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/cplex.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/cplex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/gurobi.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/gurobi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/highs.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/highs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/ipopt.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/maingo.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/maingo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/maingo_solvermodel.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/maingo_solvermodel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_highs_persistent.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_highs_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/tests/test_wntr_persistent.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/tests/test_wntr_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/solvers/wntr.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/solvers/wntr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/tests/test_base.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/tests/test_fbbt.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/tests/test_fbbt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/tests/test_interval.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/utils/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/utils/get_objective.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/utils/get_objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/utils/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/writers/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/writers/config.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/writers/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/writers/lp_writer.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/writers/lp_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/writers/nl_writer.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/writers/nl_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/writers/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/writers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/appsi/writers/tests/test_nl_writer.py` & `Pyomo-6.7.3/pyomo/contrib/appsi/writers/tests/test_nl_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/benders/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/benders_cuts.py` & `Pyomo-6.7.3/pyomo/contrib/benders/benders_cuts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/benders/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/examples/farmer.py` & `Pyomo-6.7.3/pyomo/contrib/benders/examples/farmer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/examples/grothey_ex.py` & `Pyomo-6.7.3/pyomo/contrib/benders/examples/grothey_ex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/benders/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/benders/tests/test_benders.py` & `Pyomo-6.7.3/pyomo/contrib/benders/tests/test_benders.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/community_graph.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/community_graph.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/detection.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,15 +576,15 @@
                         not_found = False
 
             # Note - there is no strong reason to choose spring layout; it just creates relatively clean graphs
             if pos is None:  # The case where the user has not provided their own layout
                 pos = nx.spring_layout(model_graph)
 
         # Define color_map
-        color_map = plt.cm.get_cmap('viridis', len(numbered_community_map))
+        color_map = plt.get_cmap('viridis', len(numbered_community_map))
 
         # Create the figure and draw the graph
         fig = plt.figure()
         nx.draw_networkx_nodes(
             model_graph,
             pos,
             nodelist=node_list,
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/event_log.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/event_log.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/community_detection/tests/test_detection.py` & `Pyomo-6.7.3/pyomo/contrib/community_detection/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/cp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/interval_var.py` & `Pyomo-6.7.3/pyomo/contrib/cp/interval_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/cp/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/repn/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/cp/repn/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/repn/docplex_writer.py` & `Pyomo-6.7.3/pyomo/contrib/cp/repn/docplex_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/scheduling_logic.py` & `Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/scheduling_logic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/sequence_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/sequence_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/sequence_var.py` & `Pyomo-6.7.3/pyomo/contrib/cp/sequence_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_docplex_walker.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_docplex_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_docplex_writer.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_docplex_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_interval_var.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_interval_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_precedence_constraints.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_precedence_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_sequence_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_sequence_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_sequence_var.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_sequence_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/tests/test_step_function_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/cp/tests/test_step_function_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/transform/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/cp/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py` & `Pyomo-6.7.3/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py` & `Pyomo-6.7.3/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/doe/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/doe.py` & `Pyomo-6.7.3/pyomo/contrib/doe/doe.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 from pyomo.contrib.sensitivity_toolbox.sens import get_dsdp
 from pyomo.contrib.doe.scenario import ScenarioGenerator, FiniteDifferenceStep
 from pyomo.contrib.doe.result import FisherResults, GridSearchResult
 import collections.abc
 
 import inspect
 
+from pyomo.common import DeveloperError
+
 
 class CalculationMode(Enum):
     sequential_finite = "sequential_finite"
     direct_kaug = "direct_kaug"
 
 
 class ObjectiveLib(Enum):
@@ -67,14 +69,16 @@
         design_vars,
         measurement_vars,
         create_model,
         solver=None,
         prior_FIM=None,
         discretize_model=None,
         args=None,
+        logger_level=logging.INFO,
+        only_compute_fim_lower=True,
     ):
         """
         This package enables model-based design of experiments analysis with Pyomo.
         Both direct optimization and enumeration modes are supported.
         NLP sensitivity tools, e.g.,  sipopt and k_aug, are supported to accelerate analysis via enumeration.
         It can be applied to dynamic models, where design variables are controlled throughout the experiment.
 
@@ -97,30 +101,56 @@
         prior_FIM:
             A 2D numpy array containing Fisher information matrix (FIM) for prior experiments.
             The default None means there is no prior information.
         discretize_model:
             A user-specified ``function`` that discretizes the model. Only use with Pyomo.DAE, default=None
         args:
             Additional arguments for the create_model function.
+        logger_level:
+            Specify the level of the logger. Change to logging.DEBUG for all messages.
+        only_compute_fim_lower:
+            If True, only the lower triangle of the FIM is computed. Default is True.
         """
 
         # parameters
         if not isinstance(param_init, collections.abc.Mapping):
             raise ValueError("param_init should be a dictionary.")
         self.param = param_init
         # design variable name
         self.design_name = design_vars.variable_names
         self.design_vars = design_vars
         self.create_model = create_model
+
+        # check if create model function conforms to the original
+        # Pyomo.DoE interface
+        model_option_arg = (
+            "model_option" in inspect.getfullargspec(self.create_model).args
+        )
+        mod_arg = "mod" in inspect.getfullargspec(self.create_model).args
+        if model_option_arg and mod_arg:
+            self._original_create_model_interface = True
+        else:
+            self._original_create_model_interface = False
+
+        if args is None:
+            args = {}
         self.args = args
 
         # create the measurement information object
         self.measurement_vars = measurement_vars
         self.measure_name = self.measurement_vars.variable_names
 
+        if (
+            self.measurement_vars.variable_names is None
+            or not self.measurement_vars.variable_names
+        ):
+            raise ValueError(
+                "There are no measurement variables. Check for a modeling mistake."
+            )
+
         # check if user-defined solver is given
         if solver:
             self.solver = solver
         # if not given, use default solver
         else:
             self.solver = self._get_default_ipopt_solver()
 
@@ -132,25 +162,27 @@
             self.prior_FIM = np.zeros((len(self.param), len(self.param)))
         else:
             self.prior_FIM = prior_FIM
         self._check_inputs()
 
         # if print statements
         self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(level=logging.INFO)
+        self.logger.setLevel(level=logger_level)
+
+        self.only_compute_fim_lower = only_compute_fim_lower
 
     def _check_inputs(self):
         """
         Check if the prior FIM is N*N matrix, where N is the number of parameter
         """
-        if type(self.prior_FIM) != type(None):
+        if self.prior_FIM is not None:
             if np.shape(self.prior_FIM)[0] != np.shape(self.prior_FIM)[1]:
-                raise ValueError('Found wrong prior information matrix shape.')
+                raise ValueError("Found wrong prior information matrix shape.")
             elif np.shape(self.prior_FIM)[0] != len(self.param):
-                raise ValueError('Found wrong prior information matrix shape.')
+                raise ValueError("Found wrong prior information matrix shape.")
 
     def stochastic_program(
         self,
         if_optimize=True,
         objective_option="det",
         scale_nominal_param_value=False,
         scale_constant_value=1,
@@ -319,14 +351,15 @@
         scale_nominal_param_value=False,
         scale_constant_value=1,
         store_output=None,
         read_output=None,
         extract_single_model=None,
         formula="central",
         step=0.001,
+        only_compute_fim_lower=False,
     ):
         """
         This function calculates the Fisher information matrix (FIM) using sensitivity information obtained
         from two possible modes (defined by the CalculationMode Enum):
 
             1.  sequential_finite: sequentially solve square problems and use finite difference approximation
             2.  direct_kaug: solve a single square problem then extract derivatives using NLP sensitivity theory
@@ -401,31 +434,41 @@
         return FIM_analysis
 
     def _sequential_finite(self, read_output, extract_single_model, store_output):
         """Sequential_finite mode uses Pyomo Block to evaluate the sensitivity information."""
 
         # if measurements are provided
         if read_output:
-            with open(read_output, 'rb') as f:
+            with open(read_output, "rb") as f:
                 output_record = pickle.load(f)
                 f.close()
             jac = self._finite_calculation(output_record)
 
         # if measurements are not provided
         else:
             mod = self._create_block()
 
             # dict for storing model outputs
             output_record = {}
 
+            # Deactivate any existing objective functions
+            for obj in mod.component_objects(pyo.Objective):
+                obj.deactivate()
+
+            # add zero (dummy/placeholder) objective function
+            mod.Obj = pyo.Objective(expr=0, sense=pyo.minimize)
+
             # solve model
             square_result = self._solve_doe(mod, fix=True)
 
+            # save model from optional post processing function
+            self._square_model_from_compute_FIM = mod
+
             if extract_single_model:
-                mod_name = store_output + '.csv'
+                mod_name = store_output + ".csv"
                 dataframe = extract_single_model(mod, square_result)
                 dataframe.to_csv(mod_name)
 
             # loop over blocks for results
             for s in range(len(self.scenario_list)):
                 # loop over measurement item and time to store model measurements
                 output_iter = []
@@ -439,18 +482,18 @@
                         raise ValueError(
                             f"measurement {r} cannot be found in the model."
                         )
                     output_iter.append(pyo.value(var_up))
 
                 output_record[s] = output_iter
 
-                output_record['design'] = self.design_values
+                output_record["design"] = self.design_values
 
                 if store_output:
-                    f = open(store_output, 'wb')
+                    f = open(store_output, "wb")
                     pickle.dump(output_record, f)
                     f.close()
 
             # calculate jacobian
             jac = self._finite_calculation(output_record)
 
             # return all models formed
@@ -477,35 +520,46 @@
             scale_constant_value=self.scale_constant_value,
         )
 
         return FIM_analysis
 
     def _direct_kaug(self):
         # create model
-        mod = self.create_model(model_option=ModelOptionLib.parmest)
+        if self._original_create_model_interface:
+            mod = self.create_model(model_option=ModelOptionLib.parmest, **self.args)
+        else:
+            mod = self.create_model(**self.args)
 
         # discretize if needed
-        if self.discretize_model:
+        if self.discretize_model is not None:
             mod = self.discretize_model(mod, block=False)
 
-        # add objective function
+        # Deactivate any existing objective functions
+        for obj in mod.component_objects(pyo.Objective):
+            obj.deactivate()
+
+        # add zero (dummy/placeholder) objective function
         mod.Obj = pyo.Objective(expr=0, sense=pyo.minimize)
 
         # set ub and lb to parameters
         for par in self.param.keys():
             cuid = pyo.ComponentUID(par)
             var = cuid.find_component_on(mod)
             var.setlb(self.param[par])
             var.setub(self.param[par])
 
         # generate parameter name list and value dictionary with index
         var_name = list(self.param.keys())
 
         # call k_aug get_dsdp function
         square_result = self._solve_doe(mod, fix=True)
+
+        # save model from optional post processing function
+        self._square_model_from_compute_FIM = mod
+
         dsdp_re, col = get_dsdp(
             mod, list(self.param.keys()), self.param, tee=self.tee_opt
         )
 
         # analyze result
         dsdp_array = dsdp_re.toarray().T
         self.dsdp = dsdp_array
@@ -520,15 +574,15 @@
             try:
                 kaug_no = col.index(mname)
                 measurement_index.append(kaug_no)
                 # get right line of dsdp
                 dsdp_extract.append(dsdp_array[kaug_no])
             except:
                 # k_aug does not provide value for fixed variables
-                self.logger.debug('The variable is fixed:  %s', mname)
+                self.logger.debug("The variable is fixed:  %s", mname)
                 # produce the sensitivity for fixed variables
                 zero_sens = np.zeros(len(self.param))
                 # for fixed variables, the sensitivity are a zero vector
                 dsdp_extract.append(zero_sens)
 
         # Extract and calculate sensitivity if scaled by constants or parameters.
         # Convert sensitivity to a dictionary
@@ -586,58 +640,97 @@
         self.scenario_list = self.scenario_data.scenario
         # dictionary, keys are parameter name, values are a list of scenario index where this parameter is perturbed.
         self.scenario_num = self.scenario_data.scena_num
         # dictionary, keys are parameter name, values are the perturbation step
         self.eps_abs = self.scenario_data.eps_abs
         self.scena_gen = scena_gen
 
-        # Create a global model
-        mod = pyo.ConcreteModel()
-
-        # Set for block/scenarios
-        mod.scenario = pyo.Set(initialize=self.scenario_data.scenario_indices)
-
         # Determine if create_model takes theta as an optional input
         pass_theta_to_initialize = (
-            'theta' in inspect.getfullargspec(self.create_model).args
+            "theta" in inspect.getfullargspec(self.create_model).args
         )
 
         # Allow user to self-define complex design variables
-        self.create_model(mod=mod, model_option=ModelOptionLib.stage1)
+        if self._original_create_model_interface:
+
+            # Create a global model
+            mod = pyo.ConcreteModel()
+
+            if pass_theta_to_initialize:
+                # Add model on block with theta values
+                self.create_model(
+                    mod=mod,
+                    model_option=ModelOptionLib.stage1,
+                    theta=self.param,
+                    **self.args,
+                )
+            else:
+                # Add model on block without theta values
+                self.create_model(
+                    mod=mod, model_option=ModelOptionLib.stage1, **self.args
+                )
+
+        else:
+            # Create a global model
+            mod = self.create_model(**self.args)
+
+        # Set for block/scenarios
+        mod.scenario = pyo.Set(initialize=self.scenario_data.scenario_indices)
 
         # Fix parameter values in the copy of the stage1 model (if they exist)
         for par in self.param:
             cuid = pyo.ComponentUID(par)
             var = cuid.find_component_on(mod)
             if var is not None:
                 # Fix the parameter value
                 # Otherwise, the parameter does not exist on the stage 1 model
                 var.fix(self.param[par])
 
         def block_build(b, s):
             # create block scenarios
             # idea: check if create_model takes theta as an optional input, if so, pass parameter values to create_model
 
-            if pass_theta_to_initialize:
-                # Grab the values of theta for this scenario/block
-                theta_initialize = self.scenario_data.scenario[s]
-                # Add model on block with theta values
-                self.create_model(
-                    mod=b, model_option=ModelOptionLib.stage2, theta=theta_initialize
-                )
+            if self._original_create_model_interface:
+                if pass_theta_to_initialize:
+                    # Grab the values of theta for this scenario/block
+                    theta_initialize = self.scenario_data.scenario[s]
+                    # Add model on block with theta values
+                    self.create_model(
+                        mod=b,
+                        model_option=ModelOptionLib.stage2,
+                        theta=theta_initialize,
+                        **self.args,
+                    )
+                else:
+                    # Otherwise add model on block without theta values
+                    self.create_model(
+                        mod=b, model_option=ModelOptionLib.stage2, **self.args
+                    )
+
+                # save block in a temporary variable
+                mod_ = b
             else:
-                # Otherwise add model on block without theta values
-                self.create_model(mod=b, model_option=ModelOptionLib.stage2)
+                # Add model on block
+                if pass_theta_to_initialize:
+                    # Grab the values of theta for this scenario/block
+                    theta_initialize = self.scenario_data.scenario[s]
+                    mod_ = self.create_model(theta=theta_initialize, **self.args)
+                else:
+                    mod_ = self.create_model(**self.args)
 
             # fix parameter values to perturbed values
             for par in self.param:
                 cuid = pyo.ComponentUID(par)
-                var = cuid.find_component_on(b)
+                var = cuid.find_component_on(mod_)
                 var.fix(self.scenario_data.scenario[s][par])
 
+            if not self._original_create_model_interface:
+                # for the "new"/"slim" interface, we need to add the block to the model
+                return mod_
+
         mod.block = pyo.Block(mod.scenario, rule=block_build)
 
         # discretize the model
         if self.discretize_model is not None:
             mod = self.discretize_model(mod)
 
         # force design variables in blocks to be equal to global design values
@@ -648,14 +741,21 @@
                 design_var_global = cuid.find_component_on(mod)
                 design_var = cuid.find_component_on(mod.block[s])
                 return design_var == design_var_global
 
             con_name = "con" + name
             mod.add_component(con_name, pyo.Constraint(mod.scenario, expr=fix1))
 
+            # Add user-defined design variable bounds
+            cuid = pyo.ComponentUID(name)
+            design_var_global = cuid.find_component_on(mod)
+            # Set the lower and upper bounds of the design variables
+            design_var_global.setlb(self.design_vars.lower_bounds[name])
+            design_var_global.setub(self.design_vars.upper_bounds[name])
+
         return mod
 
     def _finite_calculation(self, output_record):
         """
         Calculate Jacobian for sequential_finite mode
 
         Parameters
@@ -723,14 +823,15 @@
         scale_nominal_param_value=False,
         scale_constant_value=1,
         store_name=None,
         read_name=None,
         store_optimality_as_csv=None,
         formula="central",
         step=0.001,
+        post_processing_function=None,
     ):
         """
         Enumerate through full grid search for any number of design variables;
         solve square problems sequentially to compute FIMs.
         It calculates FIM with sensitivity information from two modes:
 
             1. sequential_finite: Calculates a one scenario model multiple times for multiple scenarios.
@@ -764,14 +865,18 @@
         store_optimality_as_csv:
             if True, the design criterion values of grid search results stored with this file name as a csv
         formula:
             choose from FiniteDifferenceStep.central, .forward, or .backward.
             This option is only used for CalculationMode.sequential_finite.
         step:
             Sensitivity perturbation step size, a fraction between [0,1]. default is 0.001
+        post_processing_function:
+            An optional function that executes after each solve of the grid search.
+            The function should take one input: the Pyomo model. This could be a plotting function.
+            Default is None.
 
         Returns
         -------
         figure_draw_object: a combined result object of class Grid_search_result
         """
         # Set the Objective Function to 0 helps solve square problem quickly
         self.objective_option = ObjectiveLib.zero
@@ -802,37 +907,48 @@
         search_design_set = product(*design_ranges_list)
 
         # loop over design value combinations
         for design_set_iter in search_design_set:
             # generate the design variable dictionary needed for running compute_FIM
             # first copy value from design_values
             design_iter = self.design_vars.variable_names_value.copy()
+
+            # convert to a list and cache
+            list_design_set_iter = list(design_set_iter)
+
             # update the controlled value of certain time points for certain design variables
             for i, names in enumerate(design_dimension_names):
-                # if the element is a list, all design variables in this list share the same values
-                if isinstance(names, collections.abc.Sequence):
+                if isinstance(names, str):
+                    # if 'names' is simply a string, copy the new value
+                    design_iter[names] = list_design_set_iter[i]
+                elif isinstance(names, collections.abc.Sequence):
+                    # if the element is a list, all design variables in this list share the same values
                     for n in names:
-                        design_iter[n] = list(design_set_iter)[i]
+                        design_iter[n] = list_design_set_iter[i]
                 else:
-                    design_iter[names] = list(design_set_iter)[i]
+                    # otherwise just copy the value
+                    # design_iter[names] = list(design_set_iter)[i]
+                    raise NotImplementedError(
+                        "You should not see this error message. Please report it to the Pyomo.DoE developers."
+                    )
 
             self.design_vars.variable_names_value = design_iter
             iter_timer = TicTocTimer()
-            self.logger.info('=======Iteration Number: %s =====', count + 1)
+            self.logger.info("=======Iteration Number: %s =====", count + 1)
             self.logger.debug(
-                'Design variable values of this iteration: %s', design_iter
+                "Design variable values of this iteration: %s", design_iter
             )
             iter_timer.tic(msg=None)
             # generate store name
             if store_name is None:
                 store_output_name = None
             else:
                 store_output_name = store_name + str(count)
 
-            if read_name:
+            if read_name is not None:
                 read_input_name = read_name + str(count)
             else:
                 read_input_name = None
 
             # call compute_FIM to get FIM
             try:
                 result_iter = self.compute_FIM(
@@ -851,45 +967,53 @@
                 result_iter.result_analysis()
 
                 # iteration time
                 iter_t = iter_timer.toc(msg=None)
                 time_set.append(iter_t)
 
                 # give run information at each iteration
-                self.logger.info('This is run %s out of %s.', count, total_count)
-                self.logger.info('The code has run  %s seconds.', sum(time_set))
+                self.logger.info("This is run %s out of %s.", count, total_count)
                 self.logger.info(
-                    'Estimated remaining time:  %s seconds',
-                    (sum(time_set) / (count + 1) * (total_count - count - 1)),
+                    "The code has run  %s seconds.", round(sum(time_set), 2)
                 )
+                self.logger.info(
+                    "Estimated remaining time:  %s seconds",
+                    round(
+                        sum(time_set) / (count) * (total_count - count), 2
+                    ),  # need to check this math... it gives a negative number for the final count
+                )
+
+                if post_processing_function is not None:
+                    # Call the post processing function
+                    post_processing_function(self._square_model_from_compute_FIM)
 
                 # the combined result object are organized as a dictionary, keys are a tuple of the design variable values, values are a result object
                 result_combine[tuple(design_set_iter)] = result_iter
 
             except:
                 self.logger.warning(
-                    ':::::::::::Warning: Cannot converge this run.::::::::::::'
+                    ":::::::::::Warning: Cannot converge this run.::::::::::::"
                 )
                 count += 1
                 failed_count += 1
-                self.logger.warning('failed count:', failed_count)
+                self.logger.warning("failed count:", failed_count)
                 result_combine[tuple(design_set_iter)] = None
 
         # For user's access
         self.all_fim = result_combine
 
         # Create figure drawing object
         figure_draw_object = GridSearchResult(
             design_ranges_list,
             design_dimension_names,
             result_combine,
             store_optimality_name=store_optimality_as_csv,
         )
 
-        self.logger.info('Overall wall clock time [s]:  %s', sum(time_set))
+        self.logger.info("Overall wall clock time [s]:  %s", sum(time_set))
 
         return figure_draw_object
 
     def _create_doe_model(self, no_obj=True):
         """
         Add equations to compute sensitivities, FIM, and objective.
 
@@ -897,14 +1021,26 @@
         -----------
         no_obj: if True, objective function is 0.
 
         Return
         -------
         model: the DOE model
         """
+
+        # Developer recommendation: use the Cholesky decomposition for D-optimality
+        # The explicit formula is available for benchmarking purposes and is NOT recommended
+        if (
+            self.only_compute_fim_lower
+            and self.objective_option == ObjectiveLib.det
+            and not self.Cholesky_option
+        ):
+            raise ValueError(
+                "Cannot compute determinant with explicit formula if only_compute_fim_lower is True."
+            )
+
         model = self._create_block()
 
         # variables for jacobian and FIM
         model.regression_parameters = pyo.Set(initialize=list(self.param.keys()))
         model.measured_variables = pyo.Set(initialize=self.measure_name)
 
         def identity_matrix(m, i, j):
@@ -939,18 +1075,19 @@
         model.sensitivity_jacobian = pyo.Var(
             model.regression_parameters,
             model.measured_variables,
             initialize=initialize_jac,
         )
 
         if self.fim_initial is not None:
-            dict_fim_initialize = {}
-            for i, bu in enumerate(model.regression_parameters):
-                for j, un in enumerate(model.regression_parameters):
-                    dict_fim_initialize[(bu, un)] = self.fim_initial[i][j]
+            dict_fim_initialize = {
+                (bu, un): self.fim_initial[i][j]
+                for i, bu in enumerate(model.regression_parameters)
+                for j, un in enumerate(model.regression_parameters)
+            }
 
         def initialize_fim(m, j, d):
             return dict_fim_initialize[(j, d)]
 
         if self.fim_initial is not None:
             model.fim = pyo.Var(
                 model.regression_parameters,
@@ -960,30 +1097,32 @@
         else:
             model.fim = pyo.Var(
                 model.regression_parameters,
                 model.regression_parameters,
                 initialize=identity_matrix,
             )
 
-        # move the L matrix initial point to a dictionary
-        if type(self.L_initial) != type(None):
-            dict_cho = {}
-            for i, bu in enumerate(model.regression_parameters):
-                for j, un in enumerate(model.regression_parameters):
-                    dict_cho[(bu, un)] = self.L_initial[i][j]
+        # if cholesky, define L elements as variables
+        if self.Cholesky_option and self.objective_option == ObjectiveLib.det:
 
-        # use the L dictionary to initialize L matrix
-        def init_cho(m, i, j):
-            return dict_cho[(i, j)]
+            # move the L matrix initial point to a dictionary
+            if self.L_initial is not None:
+                dict_cho = {
+                    (bu, un): self.L_initial[i][j]
+                    for i, bu in enumerate(model.regression_parameters)
+                    for j, un in enumerate(model.regression_parameters)
+                }
+
+            # use the L dictionary to initialize L matrix
+            def init_cho(m, i, j):
+                return dict_cho[(i, j)]
 
-        # if cholesky, define L elements as variables
-        if self.Cholesky_option:
             # Define elements of Cholesky decomposition matrix as Pyomo variables and either
             # Initialize with L in L_initial
-            if type(self.L_initial) != type(None):
+            if self.L_initial is not None:
                 model.L_ele = pyo.Var(
                     model.regression_parameters,
                     model.regression_parameters,
                     initialize=init_cho,
                 )
             # or initialize with the identity matrix
             else:
@@ -1026,79 +1165,108 @@
                 return (
                     m.sensitivity_jacobian[p, n]
                     == (var_up - var_lo) / self.eps_abs[p] * self.scale_constant_value
                 )
 
         # A constraint to calculate elements in Hessian matrix
         # transfer prior FIM to be Expressions
-        fim_initial_dict = {}
-        for i, bu in enumerate(model.regression_parameters):
-            for j, un in enumerate(model.regression_parameters):
-                fim_initial_dict[(bu, un)] = self.prior_FIM[i][j]
+        fim_initial_dict = {
+            (bu, un): self.prior_FIM[i][j]
+            for i, bu in enumerate(model.regression_parameters)
+            for j, un in enumerate(model.regression_parameters)
+        }
 
         def read_prior(m, i, j):
             return fim_initial_dict[(i, j)]
 
         model.priorFIM = pyo.Expression(
             model.regression_parameters, model.regression_parameters, rule=read_prior
         )
 
+        # The off-diagonal elements are symmetric, thus only half of the elements need to be calculated
         def fim_rule(m, p, q):
             """
             m: Pyomo model
             p: parameter
             q: parameter
             """
-            return (
-                m.fim[p, q]
-                == sum(
-                    1
-                    / self.measurement_vars.variance[n]
-                    * m.sensitivity_jacobian[p, n]
-                    * m.sensitivity_jacobian[q, n]
-                    for n in model.measured_variables
+
+            if p > q:
+                if self.only_compute_fim_lower:
+                    return pyo.Constraint.Skip
+                else:
+                    return m.fim[p, q] == m.fim[q, p]
+            else:
+                return (
+                    m.fim[p, q]
+                    == sum(
+                        1
+                        / self.measurement_vars.variance[n]
+                        * m.sensitivity_jacobian[p, n]
+                        * m.sensitivity_jacobian[q, n]
+                        for n in model.measured_variables
+                    )
+                    + m.priorFIM[p, q] * self.fim_scale_constant_value
                 )
-                + m.priorFIM[p, q] * self.fim_scale_constant_value
-            )
 
         model.jacobian_constraint = pyo.Constraint(
             model.regression_parameters, model.measured_variables, rule=jacobian_rule
         )
         model.fim_constraint = pyo.Constraint(
             model.regression_parameters, model.regression_parameters, rule=fim_rule
         )
 
+        if self.only_compute_fim_lower:
+            # Fix the upper half of the FIM matrix elements to be 0.0.
+            # This eliminates extra variables and ensures the expected number of
+            # degrees of freedom in the optimization problem.
+            for p in model.regression_parameters:
+                for q in model.regression_parameters:
+                    if p > q:
+                        model.fim[p, q].fix(0.0)
+
         return model
 
     def _add_objective(self, m):
 
-        ### Initialize the Cholesky decomposition matrix
-        if self.Cholesky_option:
+        small_number = 1e-10
+
+        # Assemble the FIM matrix. This is helpful for initialization!
+        #
+        # Suggestion from JS: "It might be more efficient to form the NP array in one shot
+        # (from a list or using fromiter), and then reshaping to the 2-D matrix"
+        #
+        fim = np.zeros((len(self.param), len(self.param)))
+        for i, bu in enumerate(m.regression_parameters):
+            for j, un in enumerate(m.regression_parameters):
+                # Copy value from Pyomo model into numpy array
+                fim[i][j] = m.fim[bu, un].value
+
+                # Set lower bound to ensure diagonal elements are (almost) non-negative
+                # if i == j:
+                #     m.fim[bu, un].setlb(-small_number)
 
-            # Assemble the FIM matrix
-            fim = np.zeros((len(self.param), len(self.param)))
-            for i, bu in enumerate(m.regression_parameters):
-                for j, un in enumerate(m.regression_parameters):
-                    fim[i][j] = m.fim[bu, un].value
+        ### Initialize the Cholesky decomposition matrix
+        if self.Cholesky_option and self.objective_option == ObjectiveLib.det:
 
             # Calculate the eigenvalues of the FIM matrix
             eig = np.linalg.eigvals(fim)
 
             # If the smallest eigenvalue is (practically) negative, add a diagonal matrix to make it positive definite
             small_number = 1e-10
             if min(eig) < small_number:
                 fim = fim + np.eye(len(self.param)) * (small_number - min(eig))
 
             # Compute the Cholesky decomposition of the FIM matrix
             L = np.linalg.cholesky(fim)
 
-        # Initialize the Cholesky matrix
-        for i, c in enumerate(m.regression_parameters):
-            for j, d in enumerate(m.regression_parameters):
-                m.L_ele[c, d].value = L[i, j]
+            # Initialize the Cholesky matrix
+            for i, c in enumerate(m.regression_parameters):
+                for j, d in enumerate(m.regression_parameters):
+                    m.L_ele[c, d].value = L[i, j]
 
         def cholesky_imp(m, c, d):
             """
             Calculate Cholesky L matrix using algebraic constraints
             """
             # If it is the left bottom half of L
             if list(self.param.keys()).index(c) >= list(self.param.keys()).index(d):
@@ -1115,15 +1283,15 @@
             """
             Calculate FIM elements. Can scale each element with 1000 for performance
             """
             return m.trace == sum(m.fim[j, j] for j in m.regression_parameters)
 
         def det_general(m):
             r"""Calculate determinant. Can be applied to FIM of any size.
-            det(A) = sum_{\sigma \in \S_n} (sgn(\sigma) * \Prod_{i=1}^n a_{i,\sigma_i})
+            det(A) = \sum_{\sigma in \S_n} (sgn(\sigma) * \Prod_{i=1}^n a_{i,\sigma_i})
             Use permutation() to get permutations, sgn() to get signature
             """
             r_list = list(range(len(m.regression_parameters)))
             # get all permutations
             object_p = permutations(r_list)
             list_p = list(object_p)
 
@@ -1145,32 +1313,44 @@
                     m.fim[each, name_order[b]]
                     for b, each in enumerate(m.regression_parameters)
                 )
                 for d in range(len(list_p))
             )
             return m.det == det_perm
 
-        if self.Cholesky_option:
+        if self.Cholesky_option and self.objective_option == ObjectiveLib.det:
             m.cholesky_cons = pyo.Constraint(
                 m.regression_parameters, m.regression_parameters, rule=cholesky_imp
             )
             m.Obj = pyo.Objective(
-                expr=2 * sum(pyo.log(m.L_ele[j, j]) for j in m.regression_parameters),
+                expr=2 * sum(pyo.log10(m.L_ele[j, j]) for j in m.regression_parameters),
                 sense=pyo.maximize,
             )
-        # if not cholesky but determinant, calculating det and evaluate the OBJ with det
+
         elif self.objective_option == ObjectiveLib.det:
+            # if not cholesky but determinant, calculating det and evaluate the OBJ with det
+            m.det = pyo.Var(initialize=np.linalg.det(fim), bounds=(small_number, None))
             m.det_rule = pyo.Constraint(rule=det_general)
-            m.Obj = pyo.Objective(expr=pyo.log(m.det), sense=pyo.maximize)
-        # if not determinant or cholesky, calculating the OBJ with trace
+            m.Obj = pyo.Objective(expr=pyo.log10(m.det), sense=pyo.maximize)
+
         elif self.objective_option == ObjectiveLib.trace:
+            # if not determinant or cholesky, calculating the OBJ with trace
+            m.trace = pyo.Var(initialize=np.trace(fim), bounds=(small_number, None))
             m.trace_rule = pyo.Constraint(rule=trace_calc)
-            m.Obj = pyo.Objective(expr=pyo.log(m.trace), sense=pyo.maximize)
+            m.Obj = pyo.Objective(expr=pyo.log10(m.trace), sense=pyo.maximize)
+            # m.Obj = pyo.Objective(expr=m.trace, sense=pyo.maximize)
+
         elif self.objective_option == ObjectiveLib.zero:
+            # add dummy objective function
             m.Obj = pyo.Objective(expr=0)
+        else:
+            # something went wrong!
+            raise DeveloperError(
+                "Objective option not recognized. Please contact the developers as you should not see this error."
+            )
 
         return m
 
     def _fix_design(self, m, design_val, fix_opt=True, optimize_option=None):
         """
         Fix design variable
 
@@ -1202,18 +1382,18 @@
                     # Otherwise, unfix only the design variables listed in optimize_option with value True
                     if optimize_option[name]:
                         var.unfix()
         return m
 
     def _get_default_ipopt_solver(self):
         """Default solver"""
-        solver = SolverFactory('ipopt')
-        solver.options['linear_solver'] = 'ma57'
-        solver.options['halt_on_ampl_error'] = 'yes'
-        solver.options['max_iter'] = 3000
+        solver = SolverFactory("ipopt")
+        solver.options["linear_solver"] = "ma57"
+        solver.options["halt_on_ampl_error"] = "yes"
+        solver.options["max_iter"] = 3000
         return solver
 
     def _solve_doe(self, m, fix=False, opt_option=None):
         """Solve DOE model.
         If it's a square problem, fix design variable and solve.
         Else, fix design variable and solve square problem first, then unfix them and solve the optimization problem
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/doe/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_compute_FIM.py` & `Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_compute_FIM.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_grid_search.py` & `Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_grid_search.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_kinetics.py` & `Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_kinetics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/examples/reactor_optimize_doe.py` & `Pyomo-6.7.3/pyomo/contrib/doe/examples/reactor_optimize_doe.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/measurements.py` & `Pyomo-6.7.3/pyomo/contrib/doe/measurements.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,24 +92,28 @@
             time_index_position,
             values,
             lower_bounds,
             upper_bounds,
         )
 
         if values is not None:
+            # if a scalar (int or float) is given, set it as the value for all variables
+            if type(values) in native_numeric_types:
+                values = [values] * len(added_names)
             # this dictionary keys are special set, values are its value
             self.variable_names_value.update(zip(added_names, values))
 
-        # if a scalar (int or float) is given, set it as the lower bound for all variables
         if lower_bounds is not None:
+            # if a scalar (int or float) is given, set it as the lower bound for all variables
             if type(lower_bounds) in native_numeric_types:
                 lower_bounds = [lower_bounds] * len(added_names)
             self.lower_bounds.update(zip(added_names, lower_bounds))
 
         if upper_bounds is not None:
+            # if a scalar (int or float) is given, set it as the upper bound for all variables
             if type(upper_bounds) in native_numeric_types:
                 upper_bounds = [upper_bounds] * len(added_names)
             self.upper_bounds.update(zip(added_names, upper_bounds))
 
         return added_names
 
     def _generate_variable_names_with_indices(
@@ -125,30 +129,36 @@
             if default (None), no extra indices needed for all var in var_name
             for e.g., {0:["CA", "CB", "CC"], 1: [1,2,3]}.
         time_index_position: an integer indicates which index is the time index
             for e.g., 1 is the time index position in the indices example.
         """
         # first combine all indices into a list
         all_index_list = []  # contains all index lists
-        if indices:
+        if indices is not None:
             for index_pointer in indices:
                 all_index_list.append(indices[index_pointer])
 
         # all index list for one variable, such as ["CA", 10, 1]
         # exhaustively enumerate over the full product of indices. For e.g.,
         # {0:["CA", "CB", "CC"], 1: [1,2,3]}
         # becomes ["CA", 1], ["CA", 2], ..., ["CC", 2], ["CC", 3]
         all_variable_indices = list(itertools.product(*all_index_list))
 
         # list store all names added this time
         added_names = []
         # iterate over index combinations ["CA", 1], ["CA", 2], ..., ["CC", 2], ["CC", 3]
         for index_instance in all_variable_indices:
-            var_name_index_string = var_name + "["
+            var_name_index_string = var_name
+            #
+            # Suggestion from JS: "Can you re-use name_repr and index_repr from pyomo.core.base.component_namer here?"
+            #
             for i, idx in enumerate(index_instance):
+                # if i is the first index, open the []
+                if i == 0:
+                    var_name_index_string += "["
                 # use repr() is different from using str()
                 # with repr(), "CA" is "CA", with str(), "CA" is CA. The first is not valid in our interface.
                 var_name_index_string += str(idx)
 
                 # if i is the last index, close the []. if not, add a "," for the next index.
                 if i == len(index_instance) - 1:
                     var_name_index_string += "]"
@@ -169,36 +179,53 @@
         values,
         lower_bounds,
         upper_bounds,
     ):
         """
         Check if the measurement information provided are valid to use.
         """
-        assert isinstance(var_name, str), "var_name should be a string."
+        if not isinstance(var_name, str):
+            raise TypeError("Variable name must be a string.")
 
-        if time_index_position not in indices:
+        # debugging note: what is an integer versus a list versus a dictionary here?
+        # check if time_index_position is in indices
+        if (
+            indices is not None  # ensure not None
+            and time_index_position is not None  # ensure not None
+            and time_index_position
+            not in indices.keys()  # ensure time_index_position is in indices
+        ):
             raise ValueError("time index cannot be found in indices.")
 
-        # if given a list, check if bounds have the same length with flattened variable
-        if values is not None and len(values) != len_indices:
+        # if given a list, check if values have the same length with flattened variable
+        if (
+            values is not None  # ensure not None
+            and not type(values)
+            in native_numeric_types  # skip this test if scalar (int or float)
+            and len(values) != len_indices
+        ):
             raise ValueError("Values is of different length with indices.")
 
         if (
             lower_bounds is not None  # ensure not None
+            and not type(lower_bounds)
+            in native_numeric_types  # skip this test if scalar (int or float)
             and isinstance(lower_bounds, collections.abc.Sequence)  # ensure list-like
             and len(lower_bounds) != len_indices  # ensure same length
         ):
-            raise ValueError("Lowerbounds is of different length with indices.")
+            raise ValueError("Lowerbounds have a different length with indices.")
 
         if (
-            upper_bounds is not None  # ensure None
+            upper_bounds is not None  # ensure not None
+            and not type(upper_bounds)
+            in native_numeric_types  # skip this test if scalar (int or float)
             and isinstance(upper_bounds, collections.abc.Sequence)  # ensure list-like
             and len(upper_bounds) != len_indices  # ensure same length
         ):
-            raise ValueError("Upperbounds is of different length with indices.")
+            raise ValueError("Upperbounds have a different length with indices.")
 
 
 class MeasurementVariables(VariablesWithIndices):
     def __init__(self):
         """
         This class stores information on which algebraic and differential variables in the Pyomo model are considered measurements.
         """
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/result.py` & `Pyomo-6.7.3/pyomo/contrib/doe/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,25 +119,25 @@
                 )  # Q.T @ Q for each measurement variable
             )
 
         # add prior information
         if self.prior_FIM is not None:
             try:
                 fim = fim + self.prior_FIM
-                self.logger.info('Existed information has been added.')
+                self.logger.info("Existed information has been added.")
             except:
-                raise ValueError('Check the shape of prior FIM.')
+                raise ValueError("Check the shape of prior FIM.")
 
         if np.linalg.cond(fim) > self.max_condition_number:
             self.logger.info(
                 "Warning: FIM is near singular. The condition number is: %s ;",
                 np.linalg.cond(fim),
             )
             self.logger.info(
-                'A condition number bigger than %s is considered near singular.',
+                "A condition number bigger than %s is considered near singular.",
                 self.max_condition_number,
             )
 
         # call private methods
         self._print_FIM_info(fim)
         if self.result is not None:
             self._get_solver_info()
@@ -235,18 +235,18 @@
         self.det = np.linalg.det(FIM)
         self.min_eig = min(eig)
         self.cond = max(eig) / min(eig)
         self.eig_vals = eig
         self.eig_vecs = np.linalg.eig(FIM)[1]
 
         self.logger.info(
-            'FIM: %s; \n Trace: %s; \n Determinant: %s;', self.FIM, self.trace, self.det
+            "FIM: %s; \n Trace: %s; \n Determinant: %s;", self.FIM, self.trace, self.det
         )
         self.logger.info(
-            'Condition number: %s; \n Min eigenvalue: %s.', self.cond, self.min_eig
+            "Condition number: %s; \n Min eigenvalue: %s.", self.cond, self.min_eig
         )
 
     def _solution_info(self, m, dv_set):
         """
         Solution information. Only for optimization problem
 
         Parameters
@@ -264,19 +264,19 @@
             -[design variable name]: a list of design variable solution
         """
         self.obj_value = value(m.obj)
 
         # When scaled with constant values, the effect of the scaling factors are removed here
         # For determinant, the scaling factor to determinant is scaling factor ** (Dim of FIM)
         # For trace, the scaling factor to trace is the scaling factor.
-        if self.obj == 'det':
+        if self.obj == "det":
             self.obj_det = np.exp(value(m.obj)) / (self.fim_scale_constant_value) ** (
                 len(self.parameter_names)
             )
-        elif self.obj == 'trace':
+        elif self.obj == "trace":
             self.obj_trace = np.exp(value(m.obj)) / (self.fim_scale_constant_value)
 
         design_variable_names = list(dv_set.keys())
         dv_times = list(dv_set.values())
 
         solution = {}
         for d, dname in enumerate(design_variable_names):
@@ -310,19 +310,19 @@
             -['square']: a string of square result solver status
             -['doe']: a string of doe result solver status
         """
 
         if (self.result.solver.status == SolverStatus.ok) and (
             self.result.solver.termination_condition == TerminationCondition.optimal
         ):
-            self.status = 'converged'
+            self.status = "converged"
         elif (
             self.result.solver.termination_condition == TerminationCondition.infeasible
         ):
-            self.status = 'infeasible'
+            self.status = "infeasible"
         else:
             self.status = self.result.solver.status
 
 
 class GridSearchResult:
     def __init__(
         self,
@@ -395,18 +395,18 @@
             # if design variables share the same value, use the first name as the column name
             if type(i) is list:
                 column_names.append(i[0])
             else:
                 column_names.append(i)
 
         # Each design criteria has a column to store values
-        column_names.append('A')
-        column_names.append('D')
-        column_names.append('E')
-        column_names.append('ME')
+        column_names.append("A")
+        column_names.append("D")
+        column_names.append("E")
+        column_names.append("ME")
         # generate the dataframe
         store_all_results = np.asarray(store_all_results)
         self.store_all_results_dataframe = pd.DataFrame(
             store_all_results, columns=column_names
         )
         # if needs to store the values
         if self.store_optimality_name is not None:
@@ -454,32 +454,32 @@
         self.fixed_design_values = list(fixed_design_dimensions.values())
         self.sensitivity_dimension = sensitivity_dimension
 
         if len(self.fixed_design_names) + len(self.sensitivity_dimension) != len(
             self.design_names
         ):
             raise ValueError(
-                'Error: All dimensions except for those the figures are drawn by should be fixed.'
+                "Error: All dimensions except for those the figures are drawn by should be fixed."
             )
 
         if len(self.sensitivity_dimension) not in [1, 2]:
             raise ValueError("Error: Either 1D or 2D figures can be drawn.")
 
         # generate a combination of logic sentences to filter the results of the DOF needed.
         # an example filter: (self.store_all_results_dataframe["CA0"]==5).
         if len(self.fixed_design_names) != 0:
-            filter = ''
+            filter = ""
             for i in range(len(self.fixed_design_names)):
-                filter += '(self.store_all_results_dataframe['
+                filter += "(self.store_all_results_dataframe["
                 filter += str(self.fixed_design_names[i])
-                filter += ']=='
+                filter += "]=="
                 filter += str(self.fixed_design_values[i])
-                filter += ')'
+                filter += ")"
                 if i != (len(self.fixed_design_names) - 1):
-                    filter += '&'
+                    filter += "&"
             # extract results with other dimensions fixed
             figure_result_data = self.store_all_results_dataframe.loc[eval(filter)]
         # if there is no other fixed dimensions
         else:
             figure_result_data = self.store_all_results_dataframe
 
         # add results for figures
@@ -522,86 +522,86 @@
         """
 
         # extract the range of the DOF design variable
         x_range = self.figure_result_data[self.sensitivity_dimension[0]].values.tolist()
 
         # decide if the results are log scaled
         if log_scale:
-            y_range_A = np.log10(self.figure_result_data['A'].values.tolist())
-            y_range_D = np.log10(self.figure_result_data['D'].values.tolist())
-            y_range_E = np.log10(self.figure_result_data['E'].values.tolist())
-            y_range_ME = np.log10(self.figure_result_data['ME'].values.tolist())
+            y_range_A = np.log10(self.figure_result_data["A"].values.tolist())
+            y_range_D = np.log10(self.figure_result_data["D"].values.tolist())
+            y_range_E = np.log10(self.figure_result_data["E"].values.tolist())
+            y_range_ME = np.log10(self.figure_result_data["ME"].values.tolist())
         else:
-            y_range_A = self.figure_result_data['A'].values.tolist()
-            y_range_D = self.figure_result_data['D'].values.tolist()
-            y_range_E = self.figure_result_data['E'].values.tolist()
-            y_range_ME = self.figure_result_data['ME'].values.tolist()
+            y_range_A = self.figure_result_data["A"].values.tolist()
+            y_range_D = self.figure_result_data["D"].values.tolist()
+            y_range_E = self.figure_result_data["E"].values.tolist()
+            y_range_ME = self.figure_result_data["ME"].values.tolist()
 
         # Draw A-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         # plt.rcParams.update(params)
         ax.plot(x_range, y_range_A)
         ax.scatter(x_range, y_range_A)
-        ax.set_ylabel('$log_{10}$ Trace')
+        ax.set_ylabel("$log_{10}$ Trace")
         ax.set_xlabel(xlabel_text)
-        plt.pyplot.title(title_text + ' - A optimality')
+        plt.pyplot.title(title_text + ": A-optimality")
         plt.pyplot.show()
 
         # Draw D-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         # plt.rcParams.update(params)
         ax.plot(x_range, y_range_D)
         ax.scatter(x_range, y_range_D)
-        ax.set_ylabel('$log_{10}$ Determinant')
+        ax.set_ylabel("$log_{10}$ Determinant")
         ax.set_xlabel(xlabel_text)
-        plt.pyplot.title(title_text + ' - D optimality')
+        plt.pyplot.title(title_text + ": D-optimality")
         plt.pyplot.show()
 
         # Draw E-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         # plt.rcParams.update(params)
         ax.plot(x_range, y_range_E)
         ax.scatter(x_range, y_range_E)
-        ax.set_ylabel('$log_{10}$ Minimal eigenvalue')
+        ax.set_ylabel("$log_{10}$ Minimal eigenvalue")
         ax.set_xlabel(xlabel_text)
-        plt.pyplot.title(title_text + ' - E optimality')
+        plt.pyplot.title(title_text + ": E-optimality")
         plt.pyplot.show()
 
         # Draw Modified E-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         # plt.rcParams.update(params)
         ax.plot(x_range, y_range_ME)
         ax.scatter(x_range, y_range_ME)
-        ax.set_ylabel('$log_{10}$ Condition number')
+        ax.set_ylabel("$log_{10}$ Condition number")
         ax.set_xlabel(xlabel_text)
-        plt.pyplot.title(title_text + ' - Modified E optimality')
+        plt.pyplot.title(title_text + ": Modified E-optimality")
         plt.pyplot.show()
 
     def _heatmap(
         self,
         title_text,
         xlabel_text,
         ylabel_text,
@@ -637,18 +637,18 @@
             elif name[0] in self.sensitivity_dimension:
                 sensitivity_dict[name[0]] = self.design_ranges[i]
 
         x_range = sensitivity_dict[self.sensitivity_dimension[0]]
         y_range = sensitivity_dict[self.sensitivity_dimension[1]]
 
         # extract the design criteria values
-        A_range = self.figure_result_data['A'].values.tolist()
-        D_range = self.figure_result_data['D'].values.tolist()
-        E_range = self.figure_result_data['E'].values.tolist()
-        ME_range = self.figure_result_data['ME'].values.tolist()
+        A_range = self.figure_result_data["A"].values.tolist()
+        D_range = self.figure_result_data["D"].values.tolist()
+        E_range = self.figure_result_data["E"].values.tolist()
+        ME_range = self.figure_result_data["ME"].values.tolist()
 
         # reshape the design criteria values for heatmaps
         cri_a = np.asarray(A_range).reshape(len(x_range), len(y_range))
         cri_d = np.asarray(D_range).reshape(len(x_range), len(y_range))
         cri_e = np.asarray(E_range).reshape(len(x_range), len(y_range))
         cri_e_cond = np.asarray(ME_range).reshape(len(x_range), len(y_range))
 
@@ -671,88 +671,88 @@
 
         # set heatmap x,y ranges
         xLabel = x_range
         yLabel = y_range
 
         # A-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         plt.pyplot.rcParams.update(params)
         ax.set_yticks(range(len(yLabel)))
         ax.set_yticklabels(yLabel)
         ax.set_ylabel(ylabel_text)
         ax.set_xticks(range(len(xLabel)))
         ax.set_xticklabels(xLabel)
         ax.set_xlabel(xlabel_text)
         im = ax.imshow(hes_a.T, cmap=plt.pyplot.cm.hot_r)
         ba = plt.pyplot.colorbar(im)
-        ba.set_label('log10(trace(FIM))')
-        plt.pyplot.title(title_text + ' - A optimality')
+        ba.set_label("log10(trace(FIM))")
+        plt.pyplot.title(title_text + ": A-optimality")
         plt.pyplot.show()
 
         # D-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         plt.pyplot.rcParams.update(params)
         ax.set_yticks(range(len(yLabel)))
         ax.set_yticklabels(yLabel)
         ax.set_ylabel(ylabel_text)
         ax.set_xticks(range(len(xLabel)))
         ax.set_xticklabels(xLabel)
         ax.set_xlabel(xlabel_text)
         im = ax.imshow(hes_d.T, cmap=plt.pyplot.cm.hot_r)
         ba = plt.pyplot.colorbar(im)
-        ba.set_label('log10(det(FIM))')
-        plt.pyplot.title(title_text + ' - D optimality')
+        ba.set_label("log10(det(FIM))")
+        plt.pyplot.title(title_text + ": D-optimality")
         plt.pyplot.show()
 
         # E-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         plt.pyplot.rcParams.update(params)
         ax.set_yticks(range(len(yLabel)))
         ax.set_yticklabels(yLabel)
         ax.set_ylabel(ylabel_text)
         ax.set_xticks(range(len(xLabel)))
         ax.set_xticklabels(xLabel)
         ax.set_xlabel(xlabel_text)
         im = ax.imshow(hes_e.T, cmap=plt.pyplot.cm.hot_r)
         ba = plt.pyplot.colorbar(im)
-        ba.set_label('log10(minimal eig(FIM))')
-        plt.pyplot.title(title_text + ' - E optimality')
+        ba.set_label("log10(minimal eig(FIM))")
+        plt.pyplot.title(title_text + ": E-optimality")
         plt.pyplot.show()
 
         # modified E-optimality
         fig = plt.pyplot.figure()
-        plt.pyplot.rc('axes', titlesize=font_axes)
-        plt.pyplot.rc('axes', labelsize=font_axes)
-        plt.pyplot.rc('xtick', labelsize=font_tick)
-        plt.pyplot.rc('ytick', labelsize=font_tick)
+        plt.pyplot.rc("axes", titlesize=font_axes)
+        plt.pyplot.rc("axes", labelsize=font_axes)
+        plt.pyplot.rc("xtick", labelsize=font_tick)
+        plt.pyplot.rc("ytick", labelsize=font_tick)
         ax = fig.add_subplot(111)
-        params = {'mathtext.default': 'regular'}
+        params = {"mathtext.default": "regular"}
         plt.pyplot.rcParams.update(params)
         ax.set_yticks(range(len(yLabel)))
         ax.set_yticklabels(yLabel)
         ax.set_ylabel(ylabel_text)
         ax.set_xticks(range(len(xLabel)))
         ax.set_xticklabels(xLabel)
         ax.set_xlabel(xlabel_text)
         im = ax.imshow(hes_e2.T, cmap=plt.pyplot.cm.hot_r)
         ba = plt.pyplot.colorbar(im)
-        ba.set_label('log10(cond(FIM))')
-        plt.pyplot.title(title_text + ' - Modified E-optimality')
+        ba.set_label("log10(cond(FIM))")
+        plt.pyplot.title(title_text + ": Modified E-optimality")
         plt.pyplot.show()
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/scenario.py` & `Pyomo-6.7.3/pyomo/contrib/doe/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,9 +146,9 @@
 
         self.ScenarioData = ScenarioData(
             scenario, scena_num, eps_abs, list(range(len(scenario)))
         )
 
         # store scenario
         if self.store:
-            with open('scenario_simultaneous.pickle', 'wb') as f:
+            with open("scenario_simultaneous.pickle", "wb") as f:
                 pickle.dump(self.scenario_data, f)
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/doe/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/tests/test_fim_doe.py` & `Pyomo-6.7.3/pyomo/contrib/doe/tests/test_fim_doe.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,35 +34,143 @@
     DesignOfExperiments,
     VariablesWithIndices,
 )
 from pyomo.contrib.doe.examples.reactor_kinetics import create_model, disc_for_measure
 
 
 class TestMeasurementError(unittest.TestCase):
-    def test(self):
-        t_control = [0, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1]
-        variable_name = "C"
-        indices = {0: ['CA', 'CB', 'CC'], 1: t_control}
-        # measurement object
-        measurements = MeasurementVariables()
+
+    def test_with_time_plus_one_extra_index(self):
+        """This tests confirms the typical usage with a time index plus one extra index.
+
+        This test should execute without throwing any errors.
+
+        """
+
+        MeasurementVariables().add_variables(
+            "C", indices={0: ["A", "B", "C"], 1: [0, 0.5, 1.0]}, time_index_position=1
+        )
+
+    def test_with_time_plus_two_extra_indices(self):
+        """This tests confirms the typical usage with a time index plus two extra indices.
+
+        This test should execute without throwing any errors.
+
+        """
+
+        MeasurementVariables().add_variables(
+            "C",
+            indices={
+                0: ["A", "B", "C"],  # species
+                1: [0, 0.5, 1.0],  # time
+                2: [1, 2, 3],
+            },  # position
+            time_index_position=1,
+        )
+
+    def test_time_index_position_out_of_bounds(self):
+        """This test confirms that an error is thrown when the time index position is out of bounds."""
+
         # if time index is not in indices, an value error is thrown.
         with self.assertRaises(ValueError):
-            measurements.add_variables(
-                variable_name, indices=indices, time_index_position=2
+            MeasurementVariables().add_variables(
+                "C",
+                indices={0: ["CA", "CB", "CC"], 1: [0, 0.5, 1.0]},  # species  # time
+                time_index_position=2,  # this is out of bounds
+            )
+
+    def test_single_measurement_variable(self):
+        """This test confirms we can specify a single measurement variable without
+        specifying the indices.
+
+        The test should execute with no errors.
+        """
+        measurements = MeasurementVariables()
+        measurements.add_variables("HelloWorld", indices=None, time_index_position=None)
+
+    def test_without_time_index(self):
+        """This test confirms we can add a measurement variable without specifying the time index.
+
+        The test should execute with no errors.
+
+        """
+
+        MeasurementVariables().add_variables(
+            "C",
+            indices={0: ["CA", "CB", "CC"]},  # species as only index
+            time_index_position=None,  # no time index
+        )
+
+    def test_only_time_index(self):
+        """This test confirms we can add a measurement variable without specifying the variable name.
+
+        The test should execute with no errors.
+
+        """
+
+        MeasurementVariables().add_variables(
+            "HelloWorld",  # name of the variable
+            indices={0: [0, 0.5, 1.0]},
+            time_index_position=0,
+        )
+
+    def test_with_no_measurement_name(self):
+        """This test confirms that an error is thrown when None is used as the measurement name."""
+
+        with self.assertRaises(TypeError):
+            MeasurementVariables().add_variables(
+                None, indices={0: [0, 0.5, 1.0]}, time_index_position=0
+            )
+
+    def test_with_non_string_measurement_name(self):
+        """This test confirms that an error is thrown when a non-string is used as the measurement name."""
+
+        with self.assertRaises(TypeError):
+            MeasurementVariables().add_variables(
+                1, indices={0: [0, 0.5, 1.0]}, time_index_position=0
+            )
+
+    def test_non_integer_index_keys(self):
+        """This test confirms that strings can be used as keys for specifying the indices.
+
+        Warning: it is possible this usage breaks something else in Pyomo.DoE.
+        There may be an implicit assumption that the order of the keys must match the order
+        of the indices in the Pyomo model.
+
+        """
+
+        MeasurementVariables().add_variables(
+            "C",
+            indices={"species": ["CA", "CB", "CC"], "time": [0, 0.5, 1.0]},
+            time_index_position="time",
+        )
+
+    def test_no_measurements(self):
+        """This test confirms that an error is thrown when the user forgets to add any measurements.
+
+        It's okay to have no decision variables. With no measurement variables, the FIM is the zero matrix.
+        This (no measurements) is a common user mistake.
+        """
+
+        with self.assertRaises(ValueError):
+            decisions = DesignVariables()
+            measurements = MeasurementVariables()
+            DesignOfExperiments(
+                {}, decisions, measurements, create_model, disc_for_measure
             )
 
 
 class TestDesignError(unittest.TestCase):
     def test(self):
         t_control = [0, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1]
         # design object
         exp_design = DesignVariables()
 
         # add T as design variable
-        var_T = 'T'
+        var_T = "T"
         indices_T = {0: t_control}
         exp1_T = [470, 300, 300, 300, 300, 300, 300, 300, 300]
 
         upper_bound = [
             700,
             700,
             700,
@@ -90,39 +198,39 @@
 @unittest.skipIf(not numpy_available, "Numpy is not available")
 class TestPriorFIMError(unittest.TestCase):
     def test(self):
         # Control time set [h]
         t_control = [0, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1]
         # measurement object
         variable_name = "C"
-        indices = {0: ['CA', 'CB', 'CC'], 1: t_control}
+        indices = {0: ["CA", "CB", "CC"], 1: t_control}
 
         measurements = MeasurementVariables()
         measurements.add_variables(
             variable_name, indices=indices, time_index_position=1
         )
 
         # design object
         exp_design = DesignVariables()
 
         # add CAO as design variable
-        var_C = 'CA0'
+        var_C = "CA0"
         indices_C = {0: [0]}
         exp1_C = [5]
         exp_design.add_variables(
             var_C,
             indices=indices_C,
             time_index_position=0,
             values=exp1_C,
             lower_bounds=1,
             upper_bounds=5,
         )
 
         # add T as design variable
-        var_T = 'T'
+        var_T = "T"
         indices_T = {0: t_control}
         exp1_T = [470, 300, 300, 300, 300, 300, 300, 300, 300]
 
         exp_design.add_variables(
             var_T,
             indices=indices_T,
             time_index_position=0,
@@ -161,57 +269,57 @@
         t_control2 = [0.2, 0.4, 0.6, 0.8]
 
         # measurement object
         measurements = MeasurementVariables()
 
         # add variable C
         variable_name = "C"
-        indices = {0: ['CA', 'CB', 'CC'], 1: t_control}
+        indices = {0: ["CA", "CB", "CC"], 1: t_control}
         measurements.add_variables(
             variable_name, indices=indices, time_index_position=1
         )
 
         # add variable T
         variable_name2 = "T"
         indices2 = {0: [1, 3, 5], 1: t_control2}
         measurements.add_variables(
             variable_name2, indices=indices2, time_index_position=1, variance=10
         )
 
         # check variable names
-        self.assertEqual(measurements.variable_names[0], 'C[CA,0]')
-        self.assertEqual(measurements.variable_names[1], 'C[CA,0.125]')
-        self.assertEqual(measurements.variable_names[-1], 'T[5,0.8]')
-        self.assertEqual(measurements.variable_names[-2], 'T[5,0.6]')
-        self.assertEqual(measurements.variance['T[5,0.4]'], 10)
-        self.assertEqual(measurements.variance['T[5,0.6]'], 10)
-        self.assertEqual(measurements.variance['T[5,0.4]'], 10)
-        self.assertEqual(measurements.variance['T[5,0.6]'], 10)
+        self.assertEqual(measurements.variable_names[0], "C[CA,0]")
+        self.assertEqual(measurements.variable_names[1], "C[CA,0.125]")
+        self.assertEqual(measurements.variable_names[-1], "T[5,0.8]")
+        self.assertEqual(measurements.variable_names[-2], "T[5,0.6]")
+        self.assertEqual(measurements.variance["T[5,0.4]"], 10)
+        self.assertEqual(measurements.variance["T[5,0.6]"], 10)
+        self.assertEqual(measurements.variance["T[5,0.4]"], 10)
+        self.assertEqual(measurements.variance["T[5,0.6]"], 10)
 
         ### specify function
         var_names = [
-            'C[CA,0]',
-            'C[CA,0.125]',
-            'C[CA,0.875]',
-            'C[CA,1]',
-            'C[CB,0]',
-            'C[CB,0.125]',
-            'C[CB,0.25]',
-            'C[CB,0.375]',
-            'C[CC,0]',
-            'C[CC,0.125]',
-            'C[CC,0.25]',
-            'C[CC,0.375]',
+            "C[CA,0]",
+            "C[CA,0.125]",
+            "C[CA,0.875]",
+            "C[CA,1]",
+            "C[CB,0]",
+            "C[CB,0.125]",
+            "C[CB,0.25]",
+            "C[CB,0.375]",
+            "C[CC,0]",
+            "C[CC,0.125]",
+            "C[CC,0.25]",
+            "C[CC,0.375]",
         ]
 
         measurements2 = MeasurementVariables()
         measurements2.set_variable_name_list(var_names)
 
-        self.assertEqual(measurements2.variable_names[1], 'C[CA,0.125]')
-        self.assertEqual(measurements2.variable_names[-1], 'C[CC,0.375]')
+        self.assertEqual(measurements2.variable_names[1], "C[CA,0.125]")
+        self.assertEqual(measurements2.variable_names[-1], "C[CC,0.375]")
 
         ### check_subset function
         self.assertTrue(measurements.check_subset(measurements2))
 
 
 class TestDesignVariable(unittest.TestCase):
     """Test the DesignVariable class, specify, add_element, add_bounds, update_values."""
@@ -219,28 +327,28 @@
     def test_setup(self):
         t_control = [0, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1]
 
         # design object
         exp_design = DesignVariables()
 
         # add CAO as design variable
-        var_C = 'CA0'
+        var_C = "CA0"
         indices_C = {0: [0]}
         exp1_C = [5]
         exp_design.add_variables(
             var_C,
             indices=indices_C,
             time_index_position=0,
             values=exp1_C,
             lower_bounds=1,
             upper_bounds=5,
         )
 
         # add T as design variable
-        var_T = 'T'
+        var_T = "T"
         indices_T = {0: t_control}
         exp1_T = [470, 300, 300, 300, 300, 300, 300, 300, 300]
 
         exp_design.add_variables(
             var_T,
             indices=indices_T,
             time_index_position=0,
@@ -248,83 +356,83 @@
             lower_bounds=300,
             upper_bounds=700,
         )
 
         self.assertEqual(
             exp_design.variable_names,
             [
-                'CA0[0]',
-                'T[0]',
-                'T[0.125]',
-                'T[0.25]',
-                'T[0.375]',
-                'T[0.5]',
-                'T[0.625]',
-                'T[0.75]',
-                'T[0.875]',
-                'T[1]',
+                "CA0[0]",
+                "T[0]",
+                "T[0.125]",
+                "T[0.25]",
+                "T[0.375]",
+                "T[0.5]",
+                "T[0.625]",
+                "T[0.75]",
+                "T[0.875]",
+                "T[1]",
             ],
         )
-        self.assertEqual(exp_design.variable_names_value['CA0[0]'], 5)
-        self.assertEqual(exp_design.variable_names_value['T[0]'], 470)
-        self.assertEqual(exp_design.upper_bounds['CA0[0]'], 5)
-        self.assertEqual(exp_design.upper_bounds['T[0]'], 700)
-        self.assertEqual(exp_design.lower_bounds['CA0[0]'], 1)
-        self.assertEqual(exp_design.lower_bounds['T[0]'], 300)
+        self.assertEqual(exp_design.variable_names_value["CA0[0]"], 5)
+        self.assertEqual(exp_design.variable_names_value["T[0]"], 470)
+        self.assertEqual(exp_design.upper_bounds["CA0[0]"], 5)
+        self.assertEqual(exp_design.upper_bounds["T[0]"], 700)
+        self.assertEqual(exp_design.lower_bounds["CA0[0]"], 1)
+        self.assertEqual(exp_design.lower_bounds["T[0]"], 300)
 
         design_names = exp_design.variable_names
         exp1 = [4, 600, 300, 300, 300, 300, 300, 300, 300, 300]
         exp1_design_dict = dict(zip(design_names, exp1))
         exp_design.update_values(exp1_design_dict)
-        self.assertEqual(exp_design.variable_names_value['CA0[0]'], 4)
-        self.assertEqual(exp_design.variable_names_value['T[0]'], 600)
+        self.assertEqual(exp_design.variable_names_value["CA0[0]"], 4)
+        self.assertEqual(exp_design.variable_names_value["T[0]"], 600)
 
 
 class TestParameter(unittest.TestCase):
     """Test the ScenarioGenerator class, generate_scenario function."""
 
     def test_setup(self):
         # set up parameter class
-        param_dict = {'A1': 84.79, 'A2': 371.72, 'E1': 7.78, 'E2': 15.05}
+        param_dict = {"A1": 84.79, "A2": 371.72, "E1": 7.78, "E2": 15.05}
 
         scenario_gene = ScenarioGenerator(param_dict, formula="central", step=0.1)
         parameter_set = scenario_gene.ScenarioData
 
-        self.assertAlmostEqual(parameter_set.eps_abs['A1'], 16.9582, places=1)
-        self.assertAlmostEqual(parameter_set.eps_abs['E1'], 1.5554, places=1)
-        self.assertEqual(parameter_set.scena_num['A2'], [2, 3])
-        self.assertEqual(parameter_set.scena_num['E1'], [4, 5])
-        self.assertAlmostEqual(parameter_set.scenario[0]['A1'], 93.2699, places=1)
-        self.assertAlmostEqual(parameter_set.scenario[2]['A2'], 408.8895, places=1)
-        self.assertAlmostEqual(parameter_set.scenario[-1]['E2'], 13.54, places=1)
-        self.assertAlmostEqual(parameter_set.scenario[-2]['E2'], 16.55, places=1)
+        self.assertAlmostEqual(parameter_set.eps_abs["A1"], 16.9582, places=1)
+        self.assertAlmostEqual(parameter_set.eps_abs["E1"], 1.5554, places=1)
+        self.assertEqual(parameter_set.scena_num["A2"], [2, 3])
+        self.assertEqual(parameter_set.scena_num["E1"], [4, 5])
+        self.assertAlmostEqual(parameter_set.scenario[0]["A1"], 93.2699, places=1)
+        self.assertAlmostEqual(parameter_set.scenario[2]["A2"], 408.8895, places=1)
+        self.assertAlmostEqual(parameter_set.scenario[-1]["E2"], 13.54, places=1)
+        self.assertAlmostEqual(parameter_set.scenario[-2]["E2"], 16.55, places=1)
 
 
 class TestVariablesWithIndices(unittest.TestCase):
     """Test the DesignVariable class, specify, add_element, add_bounds, update_values."""
 
     def test_setup(self):
         special = VariablesWithIndices()
         t_control = [0, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1]
         ### add_element function
         # add CAO as design variable
-        var_C = 'CA0'
+        var_C = "CA0"
         indices_C = {0: [0]}
         exp1_C = [5]
         special.add_variables(
             var_C,
             indices=indices_C,
             time_index_position=0,
             values=exp1_C,
             lower_bounds=1,
             upper_bounds=5,
         )
 
         # add T as design variable
-        var_T = 'T'
+        var_T = "T"
         indices_T = {0: t_control}
         exp1_T = [470, 300, 300, 300, 300, 300, 300, 300, 300]
 
         special.add_variables(
             var_T,
             indices=indices_T,
             time_index_position=0,
@@ -332,29 +440,29 @@
             lower_bounds=300,
             upper_bounds=700,
         )
 
         self.assertEqual(
             special.variable_names,
             [
-                'CA0[0]',
-                'T[0]',
-                'T[0.125]',
-                'T[0.25]',
-                'T[0.375]',
-                'T[0.5]',
-                'T[0.625]',
-                'T[0.75]',
-                'T[0.875]',
-                'T[1]',
+                "CA0[0]",
+                "T[0]",
+                "T[0.125]",
+                "T[0.25]",
+                "T[0.375]",
+                "T[0.5]",
+                "T[0.625]",
+                "T[0.75]",
+                "T[0.875]",
+                "T[1]",
             ],
         )
-        self.assertEqual(special.variable_names_value['CA0[0]'], 5)
-        self.assertEqual(special.variable_names_value['T[0]'], 470)
-        self.assertEqual(special.upper_bounds['CA0[0]'], 5)
-        self.assertEqual(special.upper_bounds['T[0]'], 700)
-        self.assertEqual(special.lower_bounds['CA0[0]'], 1)
-        self.assertEqual(special.lower_bounds['T[0]'], 300)
+        self.assertEqual(special.variable_names_value["CA0[0]"], 5)
+        self.assertEqual(special.variable_names_value["T[0]"], 470)
+        self.assertEqual(special.upper_bounds["CA0[0]"], 5)
+        self.assertEqual(special.upper_bounds["T[0]"], 700)
+        self.assertEqual(special.lower_bounds["CA0[0]"], 1)
+        self.assertEqual(special.lower_bounds["T[0]"], 300)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/doe/tests/test_reactor_example.py` & `Pyomo-6.7.3/pyomo/contrib/doe/tests/test_reactor_example.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,21 +30,20 @@
 from pyomo.common.dependencies import numpy as np, numpy_available, pandas_available
 import pyomo.common.unittest as unittest
 from pyomo.contrib.doe import DesignOfExperiments, MeasurementVariables, DesignVariables
 from pyomo.environ import value, ConcreteModel
 from pyomo.contrib.doe.examples.reactor_kinetics import create_model, disc_for_measure
 from pyomo.opt import SolverFactory
 
-ipopt_available = SolverFactory('ipopt').available()
+ipopt_available = SolverFactory("ipopt").available()
 
 
-class Test_example_options(unittest.TestCase):
-    """Test the three options in the kinetics example."""
-
-    def test_setUP(self):
+class Test_Reaction_Kinetics_Example(unittest.TestCase):
+    def test_reaction_kinetics_create_model(self):
+        """Test the three options in the kinetics example."""
         # parmest option
         mod = create_model(model_option="parmest")
 
         # global and block option
         mod = ConcreteModel()
         create_model(mod, model_option="stage1")
         create_model(mod, model_option="stage2")
@@ -52,169 +51,182 @@
         with self.assertRaises(ValueError):
             create_model(model_option="stage1")
 
         with self.assertRaises(ValueError):
             create_model(model_option="stage2")
 
         with self.assertRaises(ValueError):
-            create_model(model_option="NotDefine")
+            create_model(model_option="NotDefined")
+
+    @unittest.skipIf(not ipopt_available, "The 'ipopt' solver is not available")
+    @unittest.skipIf(not numpy_available, "Numpy is not available")
+    @unittest.skipIf(not pandas_available, "Pandas is not available")
+    def test_kinetics_example_sequential_finite_then_optimize(self):
+        """Test the kinetics example with sequential_finite mode and then optimization"""
+        doe_object = self.specify_reaction_kinetics()
+
+        # Test FIM calculation at nominal values
+        sensi_opt = "sequential_finite"
+        result = doe_object.compute_FIM(
+            mode=sensi_opt, scale_nominal_param_value=True, formula="central"
+        )
+        result.result_analysis()
+        self.assertAlmostEqual(np.log10(result.trace), 2.7885, places=2)
+        self.assertAlmostEqual(np.log10(result.det), 2.8218, places=2)
+        self.assertAlmostEqual(np.log10(result.min_eig), -1.0123, places=2)
+
+        ### check subset feature
+        sub_name = "C"
+        sub_indices = {0: ["CB", "CC"], 1: [0.125, 0.25, 0.5, 0.75, 0.875]}
+
+        measure_subset = MeasurementVariables()
+        measure_subset.add_variables(
+            sub_name, indices=sub_indices, time_index_position=1
+        )
+        sub_result = result.subset(measure_subset)
+        sub_result.result_analysis()
+
+        self.assertAlmostEqual(np.log10(sub_result.trace), 2.5535, places=2)
+        self.assertAlmostEqual(np.log10(sub_result.det), 1.3464, places=2)
+        self.assertAlmostEqual(np.log10(sub_result.min_eig), -1.5386, places=2)
+
+        ### Test stochastic_program mode
+        #  Prior information (scaled FIM with T=500 and T=300 experiments)
+        prior = np.asarray(
+            [
+                [28.67892806, 5.41249739, -81.73674601, -24.02377324],
+                [5.41249739, 26.40935036, -12.41816477, -139.23992532],
+                [-81.73674601, -12.41816477, 240.46276004, 58.76422806],
+                [-24.02377324, -139.23992532, 58.76422806, 767.25584508],
+            ]
+        )
+        doe_object2 = self.specify_reaction_kinetics(prior=prior)
 
+        square_result, optimize_result = doe_object2.stochastic_program(
+            if_optimize=True,
+            if_Cholesky=True,
+            scale_nominal_param_value=True,
+            objective_option="det",
+            L_initial=np.linalg.cholesky(prior),
+            jac_initial=result.jaco_information.copy(),
+            tee_opt=True,
+        )
 
-class Test_doe_object(unittest.TestCase):
-    """Test the kinetics example with both the sequential_finite mode and the direct_kaug mode"""
+        optimize_result.result_analysis()
+        ## 2024-May-26: changing this to test the objective instead of the optimal solution
+        ## It's possible the objective is flat and the optimal solution is not unique
+        # self.assertAlmostEqual(value(optimize_result.model.CA0[0]), 5.0, places=2)
+        # self.assertAlmostEqual(value(optimize_result.model.T[0.5]), 300, places=2)
+        self.assertAlmostEqual(np.log10(optimize_result.det), 5.744, places=2)
+
+        square_result, optimize_result = doe_object2.stochastic_program(
+            if_optimize=True,
+            scale_nominal_param_value=True,
+            objective_option="trace",
+            jac_initial=result.jaco_information.copy(),
+            tee_opt=True,
+        )
+
+        optimize_result.result_analysis()
+        ## 2024-May-26: changing this to test the objective instead of the optimal solution
+        ## It's possible the objective is flat and the optimal solution is not unique
+        # self.assertAlmostEqual(value(optimize_result.model.CA0[0]), 5.0, places=2)
+        # self.assertAlmostEqual(value(optimize_result.model.T[0.5]), 300, places=2)
+        self.assertAlmostEqual(np.log10(optimize_result.trace), 3.340, places=2)
 
     @unittest.skipIf(not ipopt_available, "The 'ipopt' solver is not available")
     @unittest.skipIf(not numpy_available, "Numpy is not available")
     @unittest.skipIf(not pandas_available, "Pandas is not available")
-    def test_setUP(self):
+    def test_kinetics_example_direct_k_aug(self):
+        doe_object = self.specify_reaction_kinetics()
+
+        # Test FIM calculation at nominal values
+        sensi_opt = "direct_kaug"
+        result = doe_object.compute_FIM(
+            mode=sensi_opt, scale_nominal_param_value=True, formula="central"
+        )
+        result.result_analysis()
+        self.assertAlmostEqual(np.log10(result.trace), 2.789, places=2)
+        self.assertAlmostEqual(np.log10(result.det), 2.8247, places=2)
+        self.assertAlmostEqual(np.log10(result.min_eig), -1.0112, places=2)
+
+        ### check subset feature
+        sub_name = "C"
+        sub_indices = {0: ["CB", "CC"], 1: [0.125, 0.25, 0.5, 0.75, 0.875]}
+
+        measure_subset = MeasurementVariables()
+        measure_subset.add_variables(
+            sub_name, indices=sub_indices, time_index_position=1
+        )
+        sub_result = result.subset(measure_subset)
+        sub_result.result_analysis()
+
+        self.assertAlmostEqual(np.log10(sub_result.trace), 2.5535, places=2)
+        self.assertAlmostEqual(np.log10(sub_result.det), 1.3464, places=2)
+        self.assertAlmostEqual(np.log10(sub_result.min_eig), -1.5386, places=2)
+
+    def specify_reaction_kinetics(self, prior=None):
         ### Define inputs
         # Control time set [h]
         t_control = [0, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1]
         # Define parameter nominal value
-        parameter_dict = {'A1': 84.79, 'A2': 371.72, 'E1': 7.78, 'E2': 15.05}
+        parameter_dict = {"A1": 84.79, "A2": 371.72, "E1": 7.78, "E2": 15.05}
 
         # measurement object
         variable_name = "C"
-        indices = {0: ['CA', 'CB', 'CC'], 1: t_control}
+        indices = {0: ["CA", "CB", "CC"], 1: t_control}
 
         measurements = MeasurementVariables()
         measurements.add_variables(
             variable_name, indices=indices, time_index_position=1
         )
 
         # design object
         exp_design = DesignVariables()
 
         # add CAO as design variable
-        var_C = 'CA0'
+        var_C = "CA0"
         indices_C = {0: [0]}
         exp1_C = [5]
         exp_design.add_variables(
             var_C,
             indices=indices_C,
             time_index_position=0,
             values=exp1_C,
             lower_bounds=1,
             upper_bounds=5,
         )
 
         # add T as design variable
-        var_T = 'T'
+        var_T = "T"
         indices_T = {0: t_control}
         exp1_T = [470, 300, 300, 300, 300, 300, 300, 300, 300]
 
         exp_design.add_variables(
             var_T,
             indices=indices_T,
             time_index_position=0,
             values=exp1_T,
             lower_bounds=300,
             upper_bounds=700,
         )
 
-        ### Test sequential_finite mode
-        sensi_opt = "sequential_finite"
-
         design_names = exp_design.variable_names
         exp1 = [5, 570, 300, 300, 300, 300, 300, 300, 300, 300]
         exp1_design_dict = dict(zip(design_names, exp1))
 
         exp_design.update_values(exp1_design_dict)
 
         doe_object = DesignOfExperiments(
             parameter_dict,
             exp_design,
             measurements,
             create_model,
             discretize_model=disc_for_measure,
-        )
-
-        result = doe_object.compute_FIM(
-            mode=sensi_opt, scale_nominal_param_value=True, formula="central"
-        )
-
-        result.result_analysis()
-
-        self.assertAlmostEqual(np.log10(result.trace), 2.7885, places=2)
-        self.assertAlmostEqual(np.log10(result.det), 2.8218, places=2)
-        self.assertAlmostEqual(np.log10(result.min_eig), -1.0123, places=2)
-
-        ### check subset feature
-        sub_name = "C"
-        sub_indices = {0: ["CB", "CC"], 1: [0.125, 0.25, 0.5, 0.75, 0.875]}
-
-        measure_subset = MeasurementVariables()
-        measure_subset.add_variables(
-            sub_name, indices=sub_indices, time_index_position=1
-        )
-        sub_result = result.subset(measure_subset)
-        sub_result.result_analysis()
-
-        self.assertAlmostEqual(np.log10(sub_result.trace), 2.5535, places=2)
-        self.assertAlmostEqual(np.log10(sub_result.det), 1.3464, places=2)
-        self.assertAlmostEqual(np.log10(sub_result.min_eig), -1.5386, places=2)
-
-        ### Test direct_kaug mode
-        sensi_opt = "direct_kaug"
-        # Define a new experiment
-
-        exp1 = [5, 570, 400, 300, 300, 300, 300, 300, 300, 300]
-        exp1_design_dict = dict(zip(design_names, exp1))
-        exp_design.update_values(exp1_design_dict)
-
-        doe_object = DesignOfExperiments(
-            parameter_dict,
-            exp_design,
-            measurements,
-            create_model,
-            discretize_model=disc_for_measure,
-        )
-
-        result = doe_object.compute_FIM(
-            mode=sensi_opt, scale_nominal_param_value=True, formula="central"
-        )
-
-        result.result_analysis()
-
-        self.assertAlmostEqual(np.log10(result.trace), 2.7211, places=2)
-        self.assertAlmostEqual(np.log10(result.det), 2.0845, places=2)
-        self.assertAlmostEqual(np.log10(result.min_eig), -1.3510, places=2)
-
-        ### Test stochastic_program mode
-
-        exp1 = [5, 570, 300, 300, 300, 300, 300, 300, 300, 300]
-        exp1_design_dict = dict(zip(design_names, exp1))
-        exp_design.update_values(exp1_design_dict)
-
-        # add a prior information (scaled FIM with T=500 and T=300 experiments)
-        prior = np.asarray(
-            [
-                [28.67892806, 5.41249739, -81.73674601, -24.02377324],
-                [5.41249739, 26.40935036, -12.41816477, -139.23992532],
-                [-81.73674601, -12.41816477, 240.46276004, 58.76422806],
-                [-24.02377324, -139.23992532, 58.76422806, 767.25584508],
-            ]
-        )
-
-        doe_object2 = DesignOfExperiments(
-            parameter_dict,
-            exp_design,
-            measurements,
-            create_model,
             prior_FIM=prior,
-            discretize_model=disc_for_measure,
-        )
-
-        square_result, optimize_result = doe_object2.stochastic_program(
-            if_optimize=True,
-            if_Cholesky=True,
-            scale_nominal_param_value=True,
-            objective_option="det",
-            L_initial=np.linalg.cholesky(prior),
         )
 
-        self.assertAlmostEqual(value(optimize_result.model.CA0[0]), 5.0, places=2)
-        self.assertAlmostEqual(value(optimize_result.model.T[0.5]), 300, places=2)
+        return doe_object
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/example/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/bar.py` & `Pyomo-6.7.3/pyomo/contrib/example/bar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/foo.py` & `Pyomo-6.7.3/pyomo/contrib/example/foo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/example/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/plugins/ex_plugin.py` & `Pyomo-6.7.3/pyomo/contrib/example/plugins/ex_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/example/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/example/tests/test_example.py` & `Pyomo-6.7.3/pyomo/contrib/example/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/expression_bounds_walker.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/expression_bounds_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/fbbt.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/fbbt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/interval.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/interval.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/tests/test_expression_bounds_walker.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/tests/test_expression_bounds_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/tests/test_fbbt.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/tests/test_fbbt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fbbt/tests/test_interval.py` & `Pyomo-6.7.3/pyomo/contrib/fbbt/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fme/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/fme/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fme/fourier_motzkin_elimination.py` & `Pyomo-6.7.3/pyomo/contrib/fme/fourier_motzkin_elimination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fme/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/fme/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fme/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/fme/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py` & `Pyomo-6.7.3/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdp_bounds/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/gdp_bounds/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdp_bounds/compute_bounds.py` & `Pyomo-6.7.3/pyomo/contrib/gdp_bounds/compute_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdp_bounds/info.py` & `Pyomo-6.7.3/pyomo/contrib/gdp_bounds/info.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdp_bounds/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/gdp_bounds/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdp_bounds/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/gdp_bounds/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py` & `Pyomo-6.7.3/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/GDPopt.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/GDPopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/algorithm_base_class.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/algorithm_base_class.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/branch_and_bound.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/branch_and_bound.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/config_options.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/config_options.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/create_oa_subproblems.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/create_oa_subproblems.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/cut_generation.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/cut_generation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/discrete_problem_initialize.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/discrete_problem_initialize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/enumerate.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/enumerate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/gloa.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/gloa.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/loa.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/loa.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/nlp_initialization.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/nlp_initialization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/oa_algorithm_utils.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/oa_algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/ric.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/ric.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/solve_discrete_problem.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/solve_discrete_problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/solve_subproblem.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/solve_subproblem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/common_tests.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/test_LBB.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/test_LBB.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/test_enumerate.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/test_enumerate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/tests/test_gdpopt.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/tests/test_gdpopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gdpopt/util.py` & `Pyomo-6.7.3/pyomo/contrib/gdpopt/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gjh/GJH.py` & `Pyomo-6.7.3/pyomo/contrib/gjh/GJH.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gjh/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/gjh/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gjh/getGJH.py` & `Pyomo-6.7.3/pyomo/contrib/gjh/getGJH.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/gjh/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/gjh/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/iis/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/iis.py` & `Pyomo-6.7.3/pyomo/contrib/iis/iis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/mis.py` & `Pyomo-6.7.3/pyomo/contrib/iis/mis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/iis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/tests/test_iis.py` & `Pyomo-6.7.3/pyomo/contrib/iis/tests/test_iis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/tests/test_mis.py` & `Pyomo-6.7.3/pyomo/contrib/iis/tests/test_mis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/iis/tests/trivial_mis.py` & `Pyomo-6.7.3/pyomo/contrib/iis/tests/trivial_mis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/config.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,28 +126,26 @@
 
     """
     if (
         kwds.get("method", None) is IncidenceMethod.ampl_repn
         and kwds.get("_ampl_repn_visitor", None) is None
     ):
         subexpression_cache = {}
-        subexpression_order = []
         external_functions = {}
         var_map = {}
         used_named_expressions = set()
         symbolic_solver_labels = False
         # TODO: Explore potential performance benefit of exporting defined variables.
         # This likely only shows up if we can preserve the subexpression cache across
         # multiple constraint expressions.
         export_defined_variables = False
         sorter = FileDeterminism_to_SortComponents(FileDeterminism.ORDERED)
         amplvisitor = AMPLRepnVisitor(
             text_nl_template,
             subexpression_cache,
-            subexpression_order,
             external_functions,
             var_map,
             used_named_expressions,
             symbolic_solver_labels,
             export_defined_variables,
             sorter,
         )
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/connected.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/connected.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/incidence.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/incidence.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,29 +79,40 @@
             if v_id not in id_set:
                 id_set.add(v_id)
                 unique_variables.append(var)
         return unique_variables
 
 
 def _get_incident_via_ampl_repn(expr, linear_only, visitor):
+    def _nonlinear_var_id_collector(idlist):
+        for _id in idlist:
+            if _id in visitor.subexpression_cache:
+                info = visitor.subexpression_cache[_id][1]
+                if info.nonlinear:
+                    yield from _nonlinear_var_id_collector(info.nonlinear[1])
+                if info.linear:
+                    yield from _nonlinear_var_id_collector(info.linear)
+            else:
+                yield _id
+
     var_map = visitor.var_map
     orig_activevisitor = AMPLRepn.ActiveVisitor
     AMPLRepn.ActiveVisitor = visitor
     try:
         repn = visitor.walk_expression((expr, None, 0, 1.0))
     finally:
         AMPLRepn.ActiveVisitor = orig_activevisitor
 
-    nonlinear_var_ids = [] if repn.nonlinear is None else repn.nonlinear[1]
     nonlinear_var_id_set = set()
     unique_nonlinear_var_ids = []
-    for v_id in nonlinear_var_ids:
-        if v_id not in nonlinear_var_id_set:
-            nonlinear_var_id_set.add(v_id)
-            unique_nonlinear_var_ids.append(v_id)
+    if repn.nonlinear:
+        for v_id in _nonlinear_var_id_collector(repn.nonlinear[1]):
+            if v_id not in nonlinear_var_id_set:
+                nonlinear_var_id_set.add(v_id)
+                unique_nonlinear_var_ids.append(v_id)
 
     nonlinear_vars = [var_map[v_id] for v_id in unique_nonlinear_var_ids]
     linear_only_vars = [
         var_map[v_id]
         for v_id, coef in repn.linear.items()
         if coef != 0.0 and v_id not in nonlinear_var_id_set
     ]
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/interface.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/matching.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/matching.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/scc_solver.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/scc_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/models_for_testing.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/models_for_testing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_connected.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_connected.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_incidence.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_incidence.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_interface.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_matching.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_triangularize.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_triangularize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/tests/test_visualize.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/triangularize.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/triangularize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/util.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/incidence_analysis/visualize.py` & `Pyomo-6.7.3/pyomo/contrib/incidence_analysis/visualize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/examples/ex1.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/examples/ex1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/interface.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/interior_point.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/interior_point.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/inverse_reduced_hessian.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/inverse_reduced_hessian.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/ma27_interface.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/ma27_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/mumps_interface.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/mumps_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/scipy_interface.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/scipy_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/linalg/tests/test_realloc.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/linalg/tests/test_realloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_interior_point.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_interior_point.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_realloc.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_realloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/interior_point/tests/test_reg.py` & `Pyomo-6.7.3/pyomo/contrib/interior_point/tests/test_reg.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/latex_printer/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/latex_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/latex_printer/latex_printer.py` & `Pyomo-6.7.3/pyomo/contrib/latex_printer/latex_printer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/test_latex_printer.py` & `Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/test_latex_printer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/latex_printer/tests/test_latex_printer_vartypes.py` & `Pyomo-6.7.3/pyomo/contrib/latex_printer/tests/test_latex_printer_vartypes.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mcpp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/build.py` & `Pyomo-6.7.3/pyomo/contrib/mcpp/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/getMCPP.py` & `Pyomo-6.7.3/pyomo/contrib/mcpp/getMCPP.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/mcppInterface.cpp` & `Pyomo-6.7.3/pyomo/contrib/mcpp/mcppInterface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/mcpp/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/pyomo_mcpp.py` & `Pyomo-6.7.3/pyomo/contrib/mcpp/pyomo_mcpp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mcpp/test_mcpp.py` & `Pyomo-6.7.3/pyomo/contrib/mcpp/test_mcpp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/MindtPy.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/MindtPy.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/algorithm_base_class.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/algorithm_base_class.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/config_options.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/config_options.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/cut_generation.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/cut_generation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/extended_cutting_plane.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/extended_cutting_plane.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/feasibility_pump.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/feasibility_pump.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/global_outer_approximation.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/global_outer_approximation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/outer_approximation.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/outer_approximation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/single_tree.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/single_tree.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tabu_list.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tabu_list.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP2_simple.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP2_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP3_simple.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP3_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP4_simple.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP4_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP5_simple.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP5_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP_simple.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/MINLP_simple_grey_box.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/MINLP_simple_grey_box.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/eight_process_problem.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/eight_process_problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/feasibility_pump1.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/feasibility_pump1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/feasibility_pump2.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/feasibility_pump2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/from_proposal.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/from_proposal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex1.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex2.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex3.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex3.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/nonconvex4.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/nonconvex4.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/online_doc_example.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/online_doc_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_grey_box.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_grey_box.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/tests/unit_test.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/tests/unit_test.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mindtpy/util.py` & `Pyomo-6.7.3/pyomo/contrib/mindtpy/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/convert.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/dynamic_data_base.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/dynamic_data_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/find_nearest_index.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/find_nearest_index.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/get_cuid.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/get_cuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/interval_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/interval_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/scalar_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/scalar_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/series_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/series_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_convert.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_get_cuid.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_get_cuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_interval_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_interval_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_scalar_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_scalar_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/data/tests/test_series_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/data/tests/test_series_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/model.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/run_mpc.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/run_mpc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/run_openloop.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/run_openloop.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/copy_values.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/copy_values.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/load_data.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/load_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/model_interface.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/model_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/test_interface.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/interfaces/var_linker.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/interfaces/var_linker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/constraints.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/cost_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/cost_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/terminal.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/terminal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/mpc/modeling/tests/test_terminal.py` & `Pyomo-6.7.3/pyomo/contrib/mpc/modeling/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/multistart/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/multistart/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/multistart/high_conf_stop.py` & `Pyomo-6.7.3/pyomo/contrib/multistart/high_conf_stop.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/multistart/multi.py` & `Pyomo-6.7.3/pyomo/contrib/multistart/multi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/multistart/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/multistart/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/multistart/reinit.py` & `Pyomo-6.7.3/pyomo/contrib/multistart/reinit.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/multistart/test_multi.py` & `Pyomo-6.7.3/pyomo/contrib/multistart/test_multi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/confidence_region_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/confidence_region_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/parallel_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/parallel_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/scenario_example.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/scenario_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/examples/semibatch/semibatch.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/examples/semibatch/semibatch.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/experiment.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/experiment.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/graphics.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/graphics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/ipopt_solver_wrapper.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/ipopt_solver_wrapper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/parmest.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/parmest.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/scenariocreator.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/scenariocreator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_examples.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_graphics.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_graphics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_parmest.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_parmest.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_scenariocreator.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_scenariocreator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_solver.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/tests/test_utils.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/utils/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/utils/create_ef.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/utils/create_ef.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/utils/model_utils.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/utils/mpi_utils.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/utils/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/parmest/utils/scenario_tree.py` & `Pyomo-6.7.3/pyomo/contrib/parmest/utils/scenario_tree.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/piecewise_linear_expression.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/piecewise_linear_expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/piecewise_linear_function.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/piecewise_linear_function.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/common_inner_repn_tests.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/common_inner_repn_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/common_tests.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/models.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_disaggregated_logarithmic.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_disaggregated_logarithmic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_nested_inner_repn_gdp.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_nested_inner_repn_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/convex_combination.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/convex_combination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/disaggregated_logarithmic.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/disaggregated_logarithmic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/inner_representation_gdp.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/inner_representation_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/multiple_choice.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/nested_inner_repn.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/nested_inner_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/outer_representation_gdp.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/outer_representation_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/piecewise_linear_transformation_base.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/piecewise_linear_transformation_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py` & `Pyomo-6.7.3/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/constraint_tightener.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/constraint_tightener.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/equality_propagate.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/equality_propagate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/induced_linearity.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/induced_linearity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/init_vars.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/init_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/int_to_binary.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/int_to_binary.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/strip_bounds.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/strip_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/var_aggregator.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/var_aggregator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_equality_propagate.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_equality_propagate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_induced_linearity.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_induced_linearity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_init_vars.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_init_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_int_to_binary.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_int_to_binary.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_strip_bounds.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_strip_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_var_aggregator.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_var_aggregator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/preprocessing/util.py` & `Pyomo-6.7.3/pyomo/contrib/preprocessing/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/asl.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/asl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/build.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/dependencies.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/dependencies.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/callback/reactor_design.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/callback/reactor_design.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/feasibility.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/feasibility.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/mumps_example.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/mumps_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/nlp_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/nlp_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/nlp_interface_2.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/nlp_interface_2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/parallel_matvec.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/parallel_matvec.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/parallel_vector_ops.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/parallel_vector_ops.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/sensitivity.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/sensitivity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/sqp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/sqp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/test_examples.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/exceptions.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/ampl_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/ampl_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/external_grey_box.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/external_grey_box.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/nlp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/nlp_projections.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/nlp_projections.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/tests/test_utils.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/interfaces/utils.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/intrinsic.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/intrinsic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/base.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma27.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma27.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma27_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma27_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma57.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma57.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/ma57_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/ma57_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/mumps_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/mumps_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/scipy_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/scipy_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_ma27.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_ma27.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_ma57.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_ma57.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/linalg/utils.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/linalg/utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/base_block.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/base_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/block_matrix.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/block_vector.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/mpi_block_vector.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/mpi_block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/AmplInterface.cpp` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/AmplInterface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/AmplInterface.hpp` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/AmplInterface.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/AssertUtils.hpp` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/AssertUtils.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/CMakeLists.txt` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/ma27Interface.cpp` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/ma27Interface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/ma57Interface.cpp` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/ma57Interface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/tests/simple_nlp.nl` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/tests/simple_nlp.nl`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/src/tests/simple_test.cpp` & `Pyomo-6.7.3/pyomo/contrib/pynumero/src/tests/simple_test.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pynumero/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pynumero/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/config.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/master_problem_methods.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/master_problem_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/pyros.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/pyros.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/pyros_algorithm_methods.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/pyros_algorithm_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/separation_problem_methods.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/separation_problem_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/solve_data.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/solve_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/tests/test_config.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/tests/test_grcs.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/tests/test_grcs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/uncertainty_sets.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/uncertainty_sets.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/pyros/util.py` & `Pyomo-6.7.3/pyomo/contrib/pyros/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/satsolver/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/satsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/satsolver/satsolver.py` & `Pyomo-6.7.3/pyomo/contrib/satsolver/satsolver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/satsolver/test_satsolver.py` & `Pyomo-6.7.3/pyomo/contrib/satsolver/test_satsolver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/parameter.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/parameter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/k_aug.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/k_aug.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/sens.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/sens.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py` & `Pyomo-6.7.3/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplemodel/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/simplemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/build.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/ginac/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/ginac/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/ginac/src/ginac_interface.cpp` & `Pyomo-6.7.3/pyomo/contrib/simplification/ginac/src/ginac_interface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/ginac/src/ginac_interface.hpp` & `Pyomo-6.7.3/pyomo/contrib/simplification/ginac/src/ginac_interface.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/simplify.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/simplify.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/simplification/tests/test_simplification.py` & `Pyomo-6.7.3/pyomo/contrib/simplification/tests/test_simplification.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/base.py` & `Pyomo-6.7.3/pyomo/contrib/solver/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/config.py` & `Pyomo-6.7.3/pyomo/contrib/solver/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/factory.py` & `Pyomo-6.7.3/pyomo/contrib/solver/factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/gurobi.py` & `Pyomo-6.7.3/pyomo/contrib/solver/gurobi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/gurobi_direct.py` & `Pyomo-6.7.3/pyomo/contrib/solver/gurobi_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/ipopt.py` & `Pyomo-6.7.3/pyomo/contrib/solver/ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/persistent.py` & `Pyomo-6.7.3/pyomo/contrib/solver/persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/solver/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/results.py` & `Pyomo-6.7.3/pyomo/contrib/solver/results.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/sol_reader.py` & `Pyomo-6.7.3/pyomo/contrib/solver/sol_reader.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/solution.py` & `Pyomo-6.7.3/pyomo/contrib/solver/solution.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/test_gurobi_persistent.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/test_gurobi_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/test_ipopt.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/test_ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/solvers/test_solvers.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/solvers/test_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/sol_files/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/sol_files/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_base.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_config.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_ipopt.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_results.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_results.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_sol_reader.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_sol_reader.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_solution.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_solution.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/tests/unit/test_util.py` & `Pyomo-6.7.3/pyomo/contrib/solver/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/solver/util.py` & `Pyomo-6.7.3/pyomo/contrib/solver/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/TRF.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/TRF.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/examples/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/examples/example1.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/examples/example1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/examples/example2.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/examples/example2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/filter.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/filter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/interface.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/plugins.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_TRF.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_TRF.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_examples.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_filter.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_interface.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/tests/test_util.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/trustregion/util.py` & `Pyomo-6.7.3/pyomo/contrib/trustregion/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/main.ui` & `Pyomo-6.7.3/pyomo/contrib/viewer/main.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/model_browser.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/model_browser.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/model_browser.ui` & `Pyomo-6.7.3/pyomo/contrib/viewer/model_browser.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/model_select.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/model_select.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/model_select.ui` & `Pyomo-6.7.3/pyomo/contrib/viewer/model_select.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/pyomo_viewer.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/pyomo_viewer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/qt.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/qt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/report.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/report.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/residual_table.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/residual_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/residual_table.ui` & `Pyomo-6.7.3/pyomo/contrib/viewer/residual_table.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/tests/__init__.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_data_model_item.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_data_model_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,18 @@
     sqrt,
     expr,
 )
 import pyomo.environ as pyo
 from pyomo.contrib.viewer.model_browser import ComponentDataItem
 from pyomo.contrib.viewer.ui_data import UIData
 from pyomo.common.dependencies import DeferredImportError
+from pyomo.core.base.units_container import pint_available
 
-try:
-    x = pyo.units.m
-    units_available = True
-except DeferredImportError:
-    units_available = False
 
-
-@unittest.skipIf(not units_available, "Pyomo units are not available")
+@unittest.skipIf(not pint_available, "Pyomo units are not available")
 class TestDataModelItem(unittest.TestCase):
     def setUp(self):
         # Borrowed this test model from the trust region tests
         m = ConcreteModel()
         m.y = BooleanVar(range(3), initialize=False)
         m.z = Var(range(3), domain=Reals, initialize=2.0, units=pyo.units.m)
         m.x = Var(range(4), initialize=2.0, units=pyo.units.m)
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_data_model_tree.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_data_model_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,20 +38,15 @@
     sin,
     sqrt,
 )
 import pyomo.environ as pyo
 from pyomo.contrib.viewer.model_browser import ComponentDataModel
 import pyomo.contrib.viewer.qt as myqt
 from pyomo.common.dependencies import DeferredImportError
-
-try:
-    _x = pyo.units.m
-    units_available = True
-except DeferredImportError:
-    units_available = False
+from pyomo.core.base.units_container import pint_available
 
 available = myqt.available
 
 if available:
     from pyomo.contrib.viewer.ui_data import UIData
     import pyomo.contrib.viewer.ui as ui
 else:
@@ -59,15 +54,15 @@
     class UIData(object):
         model = None
 
         def __init__(*args, **kwargs):
             pass
 
 
-@unittest.skipIf(not available or not units_available, "PyQt or units not available")
+@unittest.skipIf(not available or not pint_available, "PyQt or units not available")
 class TestDataModel(unittest.TestCase):
     def setUp(self):
         # Borrowed this test model from the trust region tests
         m = ConcreteModel(name="tm")
         m.y = BooleanVar(range(3), initialize=False)
         m.z = Var(
             range(3), domain=Reals, initialize=2.0, units=pyo.units.m, doc="test doc"
```

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_qt.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/tests/test_report.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/ui.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/ui.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/contrib/viewer/ui_data.py` & `Pyomo-6.7.3/pyomo/contrib/viewer/ui_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/__init__.py` & `Pyomo-6.7.3/pyomo/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/PyomoModel.py` & `Pyomo-6.7.3/pyomo/core/base/PyomoModel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/__init__.py` & `Pyomo-6.7.3/pyomo/core/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/action.py` & `Pyomo-6.7.3/pyomo/core/base/action.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/block.py` & `Pyomo-6.7.3/pyomo/core/base/block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/blockutil.py` & `Pyomo-6.7.3/pyomo/core/base/blockutil.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/boolean_var.py` & `Pyomo-6.7.3/pyomo/core/base/boolean_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/check.py` & `Pyomo-6.7.3/pyomo/core/base/check.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/component.py` & `Pyomo-6.7.3/pyomo/core/base/component.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/component_namer.py` & `Pyomo-6.7.3/pyomo/core/base/component_namer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/component_order.py` & `Pyomo-6.7.3/pyomo/core/base/component_order.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/componentuid.py` & `Pyomo-6.7.3/pyomo/core/base/componentuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/config.py` & `Pyomo-6.7.3/pyomo/core/base/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/connector.py` & `Pyomo-6.7.3/pyomo/core/base/connector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/constraint.py` & `Pyomo-6.7.3/pyomo/core/base/constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/disable_methods.py` & `Pyomo-6.7.3/pyomo/core/base/disable_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/enums.py` & `Pyomo-6.7.3/pyomo/core/base/enums.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/expression.py` & `Pyomo-6.7.3/pyomo/core/base/expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/external.py` & `Pyomo-6.7.3/pyomo/core/base/external.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/global_set.py` & `Pyomo-6.7.3/pyomo/core/base/global_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/indexed_component.py` & `Pyomo-6.7.3/pyomo/core/base/indexed_component.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/indexed_component_slice.py` & `Pyomo-6.7.3/pyomo/core/base/indexed_component_slice.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/initializer.py` & `Pyomo-6.7.3/pyomo/core/base/initializer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/instance2dat.py` & `Pyomo-6.7.3/pyomo/core/base/instance2dat.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/label.py` & `Pyomo-6.7.3/pyomo/core/base/label.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/logical_constraint.py` & `Pyomo-6.7.3/pyomo/core/base/logical_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/matrix_constraint.py` & `Pyomo-6.7.3/pyomo/core/base/matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/misc.py` & `Pyomo-6.7.3/pyomo/core/base/misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/numvalue.py` & `Pyomo-6.7.3/pyomo/core/base/numvalue.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/objective.py` & `Pyomo-6.7.3/pyomo/core/base/objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/param.py` & `Pyomo-6.7.3/pyomo/core/base/param.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/piecewise.py` & `Pyomo-6.7.3/pyomo/core/base/piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/plugin.py` & `Pyomo-6.7.3/pyomo/core/base/plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/range.py` & `Pyomo-6.7.3/pyomo/core/base/range.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/rangeset.py` & `Pyomo-6.7.3/pyomo/core/base/rangeset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/reference.py` & `Pyomo-6.7.3/pyomo/core/base/reference.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/set.py` & `Pyomo-6.7.3/pyomo/core/base/set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/set_types.py` & `Pyomo-6.7.3/pyomo/core/base/set_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/sets.py` & `Pyomo-6.7.3/pyomo/core/base/sets.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/sos.py` & `Pyomo-6.7.3/pyomo/core/base/sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/suffix.py` & `Pyomo-6.7.3/pyomo/core/base/suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/symbol_map.py` & `Pyomo-6.7.3/pyomo/core/base/symbol_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/symbolic.py` & `Pyomo-6.7.3/pyomo/core/base/symbolic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/template_expr.py` & `Pyomo-6.7.3/pyomo/core/base/template_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/transformation.py` & `Pyomo-6.7.3/pyomo/core/base/transformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/units_container.py` & `Pyomo-6.7.3/pyomo/core/base/units_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/util.py` & `Pyomo-6.7.3/pyomo/core/base/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/base/var.py` & `Pyomo-6.7.3/pyomo/core/base/var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/beta/__init__.py` & `Pyomo-6.7.3/pyomo/core/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/beta/dict_objects.py` & `Pyomo-6.7.3/pyomo/core/beta/dict_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/beta/list_objects.py` & `Pyomo-6.7.3/pyomo/core/beta/list_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/__init__.py` & `Pyomo-6.7.3/pyomo/core/expr/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/base.py` & `Pyomo-6.7.3/pyomo/core/expr/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/boolean_value.py` & `Pyomo-6.7.3/pyomo/core/expr/boolean_value.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/calculus/__init__.py` & `Pyomo-6.7.3/pyomo/core/expr/calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/calculus/derivatives.py` & `Pyomo-6.7.3/pyomo/core/expr/calculus/derivatives.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/calculus/diff_with_pyomo.py` & `Pyomo-6.7.3/pyomo/core/expr/calculus/diff_with_pyomo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/calculus/diff_with_sympy.py` & `Pyomo-6.7.3/pyomo/core/expr/calculus/diff_with_sympy.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/cnf_walker.py` & `Pyomo-6.7.3/pyomo/core/expr/cnf_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/compare.py` & `Pyomo-6.7.3/pyomo/core/expr/compare.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/current.py` & `Pyomo-6.7.3/pyomo/core/expr/current.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/expr_common.py` & `Pyomo-6.7.3/pyomo/core/expr/expr_common.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/expr_errors.py` & `Pyomo-6.7.3/pyomo/core/expr/expr_errors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/logical_expr.py` & `Pyomo-6.7.3/pyomo/core/expr/logical_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/ndarray.py` & `Pyomo-6.7.3/pyomo/core/expr/ndarray.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/numeric_expr.py` & `Pyomo-6.7.3/pyomo/core/expr/numeric_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/numvalue.py` & `Pyomo-6.7.3/pyomo/core/expr/numvalue.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/relational_expr.py` & `Pyomo-6.7.3/pyomo/core/expr/relational_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/symbol_map.py` & `Pyomo-6.7.3/pyomo/core/expr/symbol_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/sympy_tools.py` & `Pyomo-6.7.3/pyomo/core/expr/sympy_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,33 +5,52 @@
 #  National Technology and Engineering Solutions of Sandia, LLC
 #  Under the terms of Contract DE-NA0003525 with National Technology and
 #  Engineering Solutions of Sandia, LLC, the U.S. Government retains certain
 #  rights in this software.
 #  This software is distributed under the 3-clause BSD License.
 #  ___________________________________________________________________________
 import operator
-import sys
+from math import prod as _prod
 
+import pyomo.core.expr as EXPR
 from pyomo.common import DeveloperError
 from pyomo.common.collections import ComponentMap
 from pyomo.common.dependencies import attempt_import
 from pyomo.common.errors import NondifferentiableError
-import pyomo.core.expr as EXPR
 from pyomo.core.expr.numvalue import value, native_types
 
 #
 # Sympy takes a significant time to load; defer importing it unless
 # someone actually needs the interface.
 #
 
 _operatorMap = {}
 _pyomo_operator_map = {}
 _functionMap = {}
 
 
+def _nondifferentiable(x):
+    if type(x[1]) is tuple:
+        # sympy >= 1.3 returns tuples (var, order)
+        wrt = x[1][0]
+    else:
+        # early versions of sympy returned the bare var
+        wrt = x[1]
+    raise NondifferentiableError(
+        "The sub-expression '%s' is not differentiable with respect to %s" % (x[0], wrt)
+    )
+
+
+def _external_fcn(*x):
+    raise TypeError(
+        "Expressions containing external functions are not convertible to "
+        f"sympy expressions (found 'f{x}')"
+    )
+
+
 def _configure_sympy(sympy, available):
     if not available:
         return
 
     _operatorMap.update(
         {
             sympy.Add: sum,
@@ -109,45 +128,14 @@
         }
     )
 
 
 sympy, sympy_available = attempt_import('sympy', callback=_configure_sympy)
 
 
-if sys.version_info[:2] < (3, 8):
-
-    def _prod(args):
-        ans = 1
-        for arg in args:
-            ans *= arg
-        return ans
-
-else:
-    from math import prod as _prod
-
-
-def _nondifferentiable(x):
-    if type(x[1]) is tuple:
-        # sympy >= 1.3 returns tuples (var, order)
-        wrt = x[1][0]
-    else:
-        # early versions of sympy returned the bare var
-        wrt = x[1]
-    raise NondifferentiableError(
-        "The sub-expression '%s' is not differentiable with respect to %s" % (x[0], wrt)
-    )
-
-
-def _external_fcn(*x):
-    raise TypeError(
-        "Expressions containing external functions are not convertible to "
-        f"sympy expressions (found 'f{x}')"
-    )
-
-
 class PyomoSympyBimap(object):
     def __init__(self):
         self.pyomo2sympy = ComponentMap()
         self.sympy2pyomo = {}
         self.i = 0
 
     def getPyomoSymbol(self, sympy_object, default=None):
```

### Comparing `Pyomo-6.7.2/pyomo/core/expr/taylor_series.py` & `Pyomo-6.7.3/pyomo/core/expr/taylor_series.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/template_expr.py` & `Pyomo-6.7.3/pyomo/core/expr/template_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/expr/visitor.py` & `Pyomo-6.7.3/pyomo/core/expr/visitor.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/__init__.py` & `Pyomo-6.7.3/pyomo/core/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/base.py` & `Pyomo-6.7.3/pyomo/core/kernel/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/block.py` & `Pyomo-6.7.3/pyomo/core/kernel/block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/component_map.py` & `Pyomo-6.7.3/pyomo/core/kernel/component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/component_set.py` & `Pyomo-6.7.3/pyomo/core/kernel/component_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/conic.py` & `Pyomo-6.7.3/pyomo/core/kernel/conic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/constraint.py` & `Pyomo-6.7.3/pyomo/core/kernel/constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/container_utils.py` & `Pyomo-6.7.3/pyomo/core/kernel/container_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/dict_container.py` & `Pyomo-6.7.3/pyomo/core/kernel/dict_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/expression.py` & `Pyomo-6.7.3/pyomo/core/kernel/expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/heterogeneous_container.py` & `Pyomo-6.7.3/pyomo/core/kernel/heterogeneous_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/homogeneous_container.py` & `Pyomo-6.7.3/pyomo/core/kernel/homogeneous_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/list_container.py` & `Pyomo-6.7.3/pyomo/core/kernel/list_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/matrix_constraint.py` & `Pyomo-6.7.3/pyomo/core/kernel/matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/objective.py` & `Pyomo-6.7.3/pyomo/core/kernel/objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/parameter.py` & `Pyomo-6.7.3/pyomo/core/kernel/parameter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/__init__.py` & `Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/transforms.py` & `Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/transforms.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/transforms_nd.py` & `Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/transforms_nd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/piecewise_library/util.py` & `Pyomo-6.7.3/pyomo/core/kernel/piecewise_library/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/register_numpy_types.py` & `Pyomo-6.7.3/pyomo/core/kernel/register_numpy_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/set_types.py` & `Pyomo-6.7.3/pyomo/core/kernel/set_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/sos.py` & `Pyomo-6.7.3/pyomo/core/kernel/sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/suffix.py` & `Pyomo-6.7.3/pyomo/core/kernel/suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/tuple_container.py` & `Pyomo-6.7.3/pyomo/core/kernel/tuple_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/kernel/variable.py` & `Pyomo-6.7.3/pyomo/core/kernel/variable.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/core/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/__init__.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/add_slack_vars.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/add_slack_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/discrete_vars.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/discrete_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/eliminate_fixed_vars.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/eliminate_fixed_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/equality_transform.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/equality_transform.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/expand_connectors.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/expand_connectors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/hierarchy.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/hierarchy.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/logical_to_linear.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/logical_to_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/model.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,25 @@
 #
 # NOTE: deprecated code
 #
 # This code is here for historical purposes, and
 # because we may support an explicit matrix representation for models.
 #
 
+from pyomo.common.deprecation import deprecated
 from pyomo.core.base import Objective, Constraint
 import array
 
 
+@deprecated(
+    "to_standard_form() is deprecated.  "
+    "Please use WriterFactory('compile_standard_form')",
+    version='6.7.3',
+    remove_in='6.8.0',
+)
 def to_standard_form(self):
     """
     Produces a standard-form representation of the model. Returns
     the coefficient matrix (A), the cost vector (c), and the
     constraint vector (b), where the 'standard form' problem is
 
     min/max c'x
```

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/nonnegative_transform.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/nonnegative_transform.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/radix_linearization.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/radix_linearization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/relax_integrality.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/relax_integrality.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/scaling.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/standard_form.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/standard_form.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/plugins/transform/util.py` & `Pyomo-6.7.3/pyomo/core/plugins/transform/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/pyomoobject.py` & `Pyomo-6.7.3/pyomo/core/pyomoobject.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/staleflag.py` & `Pyomo-6.7.3/pyomo/core/staleflag.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/data/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/data/test_odbc_ini.py` & `Pyomo-6.7.3/pyomo/core/tests/data/test_odbc_ini.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/diet/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/diet/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/diet/test_diet.py` & `Pyomo-6.7.3/pyomo/core/tests/diet/test_diet.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/pmedian.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/pmedian.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/pmedian1.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/pmedian1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/pmedian2.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/pmedian2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/pmedian4.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/pmedian4.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/pmedian_concrete.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/pmedian_concrete.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/test_amplbook2.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/test_amplbook2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/test_kernel_examples.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/test_kernel_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/test_pyomo.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/test_pyomo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/examples/test_tutorials.py` & `Pyomo-6.7.3/pyomo/core/tests/examples/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/transform/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/transform/test_add_slacks.py` & `Pyomo-6.7.3/pyomo/core/tests/transform/test_add_slacks.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/transform/test_scaling.py` & `Pyomo-6.7.3/pyomo/core/tests/transform/test_scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/transform/test_transform.py` & `Pyomo-6.7.3/pyomo/core/tests/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/__init__.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_block.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_component_map.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_component_set.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_component_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_conic.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_conic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_constraint.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_dict_container.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_dict_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_expression.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_kernel.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_kernel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_list_container.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_list_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_matrix_constraint.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_objective.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_parameter.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_parameter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_piecewise.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_sos.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_suffix.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_tuple_container.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_tuple_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/kernel/test_variable.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/kernel/test_variable.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_action.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_block.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_block_model.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_block_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_bounds.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_check.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_check.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_compare.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_component.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_component.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_componentuid.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_componentuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_con.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_con.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_concrete.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_concrete.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_connector.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_connector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_deprecation.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_derivs.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_derivs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_dict_objects.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_dict_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_disable_methods.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_disable_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_enums.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_expr_misc.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_expr_misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_expression.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_external.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_external.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_indexed.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_indexed.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_indexed_slice.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_indexed_slice.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_initializer.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_initializer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_kernel_register_numpy_types.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_kernel_register_numpy_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_labelers.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_labelers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_list_objects.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_list_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_logical_constraint.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_logical_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_logical_expr_expanded.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_logical_expr_expanded.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_logical_to_linear.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_logical_to_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_matrix_constraint.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_misc.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_model.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_mutable.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_mutable.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr_api.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr_api.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_numpy_expr.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_numpy_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_numvalue.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_numvalue.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_obj.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_obj.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_param.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_param.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_pickle.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_pickle.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_piecewise.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_preprocess.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_range.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_range.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_reference.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_reference.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_relational_expr.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_relational_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_set.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_sets.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_sets.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_smap.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_smap.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_sos.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_sos_v2.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_sos_v2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_suffix.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_symbol_map.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_symbol_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_symbolic.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_taylor_series.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_taylor_series.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_template_expr.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_template_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_units.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_units.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_var.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_var_set_bounds.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_var_set_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_visitor.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_visitor.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/test_xfrm_discrete_vars.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/test_xfrm_discrete_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/uninstantiated_model_linear.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/uninstantiated_model_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/tests/unit/uninstantiated_model_quadratic.py` & `Pyomo-6.7.3/pyomo/core/tests/unit/uninstantiated_model_quadratic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/core/util.py` & `Pyomo-6.7.3/pyomo/core/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/__init__.py` & `Pyomo-6.7.3/pyomo/dae/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/contset.py` & `Pyomo-6.7.3/pyomo/dae/contset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/diffvar.py` & `Pyomo-6.7.3/pyomo/dae/diffvar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/flatten.py` & `Pyomo-6.7.3/pyomo/dae/flatten.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/initialization.py` & `Pyomo-6.7.3/pyomo/dae/initialization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/integral.py` & `Pyomo-6.7.3/pyomo/dae/integral.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/misc.py` & `Pyomo-6.7.3/pyomo/dae/misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/dae/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/plugins/colloc.py` & `Pyomo-6.7.3/pyomo/dae/plugins/colloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/plugins/finitedifference.py` & `Pyomo-6.7.3/pyomo/dae/plugins/finitedifference.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/set_utils.py` & `Pyomo-6.7.3/pyomo/dae/set_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/simulator.py` & `Pyomo-6.7.3/pyomo/dae/simulator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/__init__.py` & `Pyomo-6.7.3/pyomo/dae/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_colloc.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_colloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_contset.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_contset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_diffvar.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_diffvar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_finite_diff.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_finite_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_flatten.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_initialization.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_integral.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_integral.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_misc.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_set_utils.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_set_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/tests/test_simulator.py` & `Pyomo-6.7.3/pyomo/dae/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dae/utilities.py` & `Pyomo-6.7.3/pyomo/dae/utilities.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/DataPortal.py` & `Pyomo-6.7.3/pyomo/dataportal/DataPortal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/TableData.py` & `Pyomo-6.7.3/pyomo/dataportal/TableData.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/__init__.py` & `Pyomo-6.7.3/pyomo/dataportal/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/factory.py` & `Pyomo-6.7.3/pyomo/dataportal/factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/parse_datacmds.py` & `Pyomo-6.7.3/pyomo/dataportal/parse_datacmds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/csv_table.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/csv_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/datacommands.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/datacommands.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/db_table.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/db_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,16 +381,17 @@
         Create a new ODBC config instance, loading data from
         the given file and/or data string. Once initialized, the
         new config will contain the data represented in both
         arguments, if any. Data specified as a string argument
         will override that in the file.
         """
 
-        # ugh hardcoded strings. See following URL for info:
-        # http://publib.boulder.ibm.com/infocenter/idshelp/v10/index.jsp?topic=/com.ibm.odbc.doc/odbc58.htm
+        # Hardcoded string required here.
+        # See documentation:
+        # https://www.ibm.com/docs/en/informix-servers/12.10?topic=SSGU8G_12.1.0/com.ibm.odbc.doc/ids_odbc_062.html
         self.ODBC_DS_KEY = 'ODBC Data Sources'
         self.ODBC_INFO_KEY = 'ODBC'
 
         self.file = filename
 
         self.sources = {}
         self.source_specs = {}
```

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/json_dict.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/json_dict.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/sheet.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/sheet.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/text.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/text.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/plugins/xml_table.py` & `Pyomo-6.7.3/pyomo/dataportal/plugins/xml_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/process_data.py` & `Pyomo-6.7.3/pyomo/dataportal/process_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/tests/__init__.py` & `Pyomo-6.7.3/pyomo/dataportal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/tests/test_dat_parser.py` & `Pyomo-6.7.3/pyomo/dataportal/tests/test_dat_parser.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/dataportal/tests/test_dataportal.py` & `Pyomo-6.7.3/pyomo/dataportal/tests/test_dataportal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/duality/__init__.py` & `Pyomo-6.7.3/pyomo/duality/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/duality/collect.py` & `Pyomo-6.7.3/pyomo/duality/collect.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/duality/lagrangian_dual.py` & `Pyomo-6.7.3/pyomo/duality/lagrangian_dual.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/duality/plugins.py` & `Pyomo-6.7.3/pyomo/duality/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/duality/tests/__init__.py` & `Pyomo-6.7.3/pyomo/duality/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/duality/tests/test_linear_dual.py` & `Pyomo-6.7.3/pyomo/duality/tests/test_linear_dual.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/environ/__init__.py` & `Pyomo-6.7.3/pyomo/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/environ/tests/__init__.py` & `Pyomo-6.7.3/pyomo/environ/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/environ/tests/standalone_minimal_pyomo_driver.py` & `Pyomo-6.7.3/pyomo/environ/tests/standalone_minimal_pyomo_driver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/environ/tests/test_environ.py` & `Pyomo-6.7.3/pyomo/environ/tests/test_environ.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/environ/tests/test_package_layout.py` & `Pyomo-6.7.3/pyomo/environ/tests/test_package_layout.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/__init__.py` & `Pyomo-6.7.3/pyomo/gdp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/basic_step.py` & `Pyomo-6.7.3/pyomo/gdp/basic_step.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/disjunct.py` & `Pyomo-6.7.3/pyomo/gdp/disjunct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/between_steps.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/between_steps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/bigm.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/bigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/bigm_mixin.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/bigm_mixin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/bilinear.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/bilinear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/binary_multiplication.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/binary_multiplication.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/bound_pretransformation.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/bound_pretransformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/chull.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/chull.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/cuttingplane.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/cuttingplane.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/fix_disjuncts.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/fix_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/gdp_to_mip_transformation.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/gdp_to_mip_transformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/gdp_var_mover.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/gdp_var_mover.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/hull.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/hull.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/multiple_bigm.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/multiple_bigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/partition_disjuncts.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/partition_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/plugins/transform_current_disjunctive_state.py` & `Pyomo-6.7.3/pyomo/gdp/plugins/transform_current_disjunctive_state.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/__init__.py` & `Pyomo-6.7.3/pyomo/gdp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/common_tests.py` & `Pyomo-6.7.3/pyomo/gdp/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/models.py` & `Pyomo-6.7.3/pyomo/gdp/tests/models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_basic_step.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_basic_step.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_bigm.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_bigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_binary_multiplication.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_binary_multiplication.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_bound_pretransformation.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_bound_pretransformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_cuttingplane.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_cuttingplane.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_disjunct.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_disjunct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_fix_disjuncts.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_fix_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_gdp.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_gdp_reclassification_error.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_gdp_reclassification_error.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_hull.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_hull.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_mbigm.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_mbigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_partition_disjuncts.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_partition_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_reclassify.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_reclassify.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_transform_current_disjunctive_state.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_transform_current_disjunctive_state.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/tests/test_util.py` & `Pyomo-6.7.3/pyomo/gdp/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/transformed_disjunct.py` & `Pyomo-6.7.3/pyomo/gdp/transformed_disjunct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/gdp/util.py` & `Pyomo-6.7.3/pyomo/gdp/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/kernel/__init__.py` & `Pyomo-6.7.3/pyomo/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/kernel/util.py` & `Pyomo-6.7.3/pyomo/kernel/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/__init__.py` & `Pyomo-6.7.3/pyomo/mpec/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/complementarity.py` & `Pyomo-6.7.3/pyomo/mpec/complementarity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/mpec1.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/mpec1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/mpec2.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/mpec2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/mpec3.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/mpec3.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/mpec4.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/mpec4.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/pathampl.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/pathampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/solver1.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/solver1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/plugins/solver2.py` & `Pyomo-6.7.3/pyomo/mpec/plugins/solver2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/tests/__init__.py` & `Pyomo-6.7.3/pyomo/mpec/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/tests/test_complementarity.py` & `Pyomo-6.7.3/pyomo/mpec/tests/test_complementarity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/tests/test_minlp.py` & `Pyomo-6.7.3/pyomo/mpec/tests/test_minlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/tests/test_nlp.py` & `Pyomo-6.7.3/pyomo/mpec/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/mpec/tests/test_path.py` & `Pyomo-6.7.3/pyomo/mpec/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/__init__.py` & `Pyomo-6.7.3/pyomo/neos/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/kestrel.py` & `Pyomo-6.7.3/pyomo/neos/kestrel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/plugins/NEOS.py` & `Pyomo-6.7.3/pyomo/neos/plugins/NEOS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/neos/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/plugins/kestrel_plugin.py` & `Pyomo-6.7.3/pyomo/neos/plugins/kestrel_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/tests/__init__.py` & `Pyomo-6.7.3/pyomo/neos/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/tests/model_min_lp.py` & `Pyomo-6.7.3/pyomo/neos/tests/model_min_lp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/neos/tests/test_neos.py` & `Pyomo-6.7.3/pyomo/neos/tests/test_neos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/__init__.py` & `Pyomo-6.7.3/pyomo/network/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/arc.py` & `Pyomo-6.7.3/pyomo/network/arc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/decomposition.py` & `Pyomo-6.7.3/pyomo/network/decomposition.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/foqus_graph.py` & `Pyomo-6.7.3/pyomo/network/foqus_graph.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/network/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/plugins/expand_arcs.py` & `Pyomo-6.7.3/pyomo/network/plugins/expand_arcs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/port.py` & `Pyomo-6.7.3/pyomo/network/port.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/tests/__init__.py` & `Pyomo-6.7.3/pyomo/network/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/tests/test_arc.py` & `Pyomo-6.7.3/pyomo/network/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/tests/test_decomposition.py` & `Pyomo-6.7.3/pyomo/network/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/tests/test_port.py` & `Pyomo-6.7.3/pyomo/network/tests/test_port.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/network/util.py` & `Pyomo-6.7.3/pyomo/network/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/__init__.py` & `Pyomo-6.7.3/pyomo/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/__init__.py` & `Pyomo-6.7.3/pyomo/opt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/convert.py` & `Pyomo-6.7.3/pyomo/opt/base/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/error.py` & `Pyomo-6.7.3/pyomo/opt/base/error.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/formats.py` & `Pyomo-6.7.3/pyomo/opt/base/formats.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/opt_config.py` & `Pyomo-6.7.3/pyomo/opt/base/opt_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/problem.py` & `Pyomo-6.7.3/pyomo/opt/base/problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/results.py` & `Pyomo-6.7.3/pyomo/opt/base/results.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/base/solvers.py` & `Pyomo-6.7.3/pyomo/opt/base/solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/parallel/__init__.py` & `Pyomo-6.7.3/pyomo/opt/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/parallel/async_solver.py` & `Pyomo-6.7.3/pyomo/opt/parallel/async_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/parallel/local.py` & `Pyomo-6.7.3/pyomo/opt/parallel/local.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/parallel/manager.py` & `Pyomo-6.7.3/pyomo/opt/parallel/manager.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/opt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/plugins/driver.py` & `Pyomo-6.7.3/pyomo/opt/plugins/driver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/plugins/res.py` & `Pyomo-6.7.3/pyomo/opt/plugins/res.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/plugins/sol.py` & `Pyomo-6.7.3/pyomo/opt/plugins/sol.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/problem/__init__.py` & `Pyomo-6.7.3/pyomo/opt/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/problem/ampl.py` & `Pyomo-6.7.3/pyomo/opt/problem/ampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/results/__init__.py` & `Pyomo-6.7.3/pyomo/opt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/results/container.py` & `Pyomo-6.7.3/pyomo/opt/results/container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/results/problem.py` & `Pyomo-6.7.3/pyomo/opt/results/problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/results/results_.py` & `Pyomo-6.7.3/pyomo/opt/results/results_.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/results/solution.py` & `Pyomo-6.7.3/pyomo/opt/results/solution.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/results/solver.py` & `Pyomo-6.7.3/pyomo/opt/results/solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/solver/__init__.py` & `Pyomo-6.7.3/pyomo/opt/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/solver/ilmcmd.py` & `Pyomo-6.7.3/pyomo/opt/solver/ilmcmd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/solver/shellcmd.py` & `Pyomo-6.7.3/pyomo/opt/solver/shellcmd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/testing/__init__.py` & `Pyomo-6.7.3/pyomo/opt/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/testing/pyunit.py` & `Pyomo-6.7.3/pyomo/opt/testing/pyunit.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/__init__.py` & `Pyomo-6.7.3/pyomo/opt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/__init__.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/test_ampl.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/test_ampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/test_convert.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/test_convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/test_factory.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/test_factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/test_sol.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/test_sol.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/test_soln.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/test_soln.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/base/test_solver.py` & `Pyomo-6.7.3/pyomo/opt/tests/base/test_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/solver/__init__.py` & `Pyomo-6.7.3/pyomo/opt/tests/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/opt/tests/solver/test_shellcmd.py` & `Pyomo-6.7.3/pyomo/opt/tests/solver/test_shellcmd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/pysp/__init__.py` & `Pyomo-6.7.3/pyomo/pysp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/__init__.py` & `Pyomo-6.7.3/pyomo/repn/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/beta/__init__.py` & `Pyomo-6.7.3/pyomo/repn/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/beta/matrix.py` & `Pyomo-6.7.3/pyomo/repn/beta/matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/linear.py` & `Pyomo-6.7.3/pyomo/repn/linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/repn/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/ampl/__init__.py` & `Pyomo-6.7.3/pyomo/repn/plugins/ampl/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/ampl/ampl_.py` & `Pyomo-6.7.3/pyomo/repn/plugins/ampl/ampl_.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/baron_writer.py` & `Pyomo-6.7.3/pyomo/repn/plugins/baron_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/cpxlp.py` & `Pyomo-6.7.3/pyomo/repn/plugins/cpxlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/gams_writer.py` & `Pyomo-6.7.3/pyomo/repn/plugins/gams_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/lp_writer.py` & `Pyomo-6.7.3/pyomo/repn/plugins/lp_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/mps.py` & `Pyomo-6.7.3/pyomo/repn/plugins/mps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/nl_writer.py` & `Pyomo-6.7.3/pyomo/repn/plugins/nl_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 #  Engineering Solutions of Sandia, LLC, the U.S. Government retains certain
 #  rights in this software.
 #  This software is distributed under the 3-clause BSD License.
 #  ___________________________________________________________________________
 
 import ctypes
 import logging
+import math
+import operator
 import os
 from collections import deque, defaultdict, namedtuple
 from contextlib import nullcontext
-from itertools import filterfalse, product
+from itertools import filterfalse, product, chain
 from math import log10 as _log10
 from operator import itemgetter, attrgetter, setitem
 
 from pyomo.common.collections import ComponentMap, ComponentSet
 from pyomo.common.config import (
     ConfigBlock,
     ConfigValue,
@@ -538,23 +540,23 @@
         self.config = config
         self.symbolic_solver_labels = config.symbolic_solver_labels
         if self.symbolic_solver_labels:
             self.template = text_nl_debug_template
         else:
             self.template = text_nl_template
         self.subexpression_cache = {}
-        self.subexpression_order = []
+        self.subexpression_order = None  # set to [] later
         self.external_functions = {}
         self.used_named_expressions = set()
         self.var_map = {}
+        self.var_id_to_nl_map = {}
         self.sorter = FileDeterminism_to_SortComponents(config.file_determinism)
         self.visitor = AMPLRepnVisitor(
             self.template,
             self.subexpression_cache,
-            self.subexpression_order,
             self.external_functions,
             self.var_map,
             self.used_named_expressions,
             self.symbolic_solver_labels,
             self.config.export_defined_variables,
             self.sorter,
         )
@@ -616,14 +618,15 @@
 
         # Caching some frequently-used objects into the locals()
         symbolic_solver_labels = self.symbolic_solver_labels
         visitor = self.visitor
         ostream = self.ostream
         linear_presolve = self.config.linear_presolve
 
+        nl_map = self.var_id_to_nl_map
         var_map = self.var_map
         initialize_var_map_from_column_order(model, self.config, var_map)
         timer.toc('Initialized column order', level=logging.DEBUG)
 
         # Collect all defined EXPORT suffixes on the model
         suffix_data = {}
         if component_map[Suffix]:
@@ -696,16 +699,15 @@
 
         # Order the objectives, moving all nonlinear objectives to
         # the beginning
         n_nonlinear_objs = len(objectives)
         objectives.extend(linear_objs)
         n_objs = len(objectives)
 
-        constraints = []
-        linear_cons = []
+        all_constraints = []
         n_ranges = 0
         n_equality = 0
         n_complementarity_nonlin = 0
         n_complementarity_lin = 0
         # TODO: update the writer to tabulate and report the range and
         # nzlb values.  Low priority, as they do not appear to be
         # required for solvers like PATH.
@@ -734,75 +736,100 @@
             if scale != 1:
                 if lb is not None:
                     lb = lb * scale
                 if ub is not None:
                     ub = ub * scale
                 if scale < 0:
                     lb, ub = ub, lb
-            if expr_info.nonlinear:
-                constraints.append((con, expr_info, lb, ub))
-            elif expr_info.linear:
-                linear_cons.append((con, expr_info, lb, ub))
-            elif not self.config.skip_trivial_constraints:
-                linear_cons.append((con, expr_info, lb, ub))
-            else:  # constant constraint and skip_trivial_constraints
-                c = expr_info.const
-                if (lb is not None and lb - c > TOL) or (
-                    ub is not None and ub - c < -TOL
-                ):
-                    raise InfeasibleConstraintException(
-                        "model contains a trivially infeasible "
-                        f"constraint '{con.name}' (fixed body value "
-                        f"{c} outside bounds [{lb}, {ub}])."
-                    )
+            all_constraints.append((con, expr_info, lb, ub))
             if linear_presolve:
                 con_id = id(con)
                 if not expr_info.nonlinear and lb == ub and lb is not None:
                     lcon_by_linear_nnz[len(expr_info.linear)][con_id] = expr_info, lb
                 for _id in expr_info.linear:
                     comp_by_linear_var[_id].append((con_id, expr_info))
         if with_debug_timing:
             # report the last constraint
             timer.toc('Constraint %s', last_parent, level=logging.DEBUG)
         else:
-            timer.toc('Processed %s constraints', len(constraints))
+            timer.toc('Processed %s constraints', len(all_constraints))
+
+        # We have identified all the external functions (resolving them
+        # by name).  Now we may need to resolve the function by the
+        # (local) FID, which we know is indexed by integers starting at
+        # 0.  We will convert the dict to a list for efficient lookup.
+        self.external_functions = list(self.external_functions.values())
 
         # This may fetch more bounds than needed, but only in the cases
         # where variables were completely eliminated while walking the
         # expressions, or when users provide superfluous variables in
         # the column ordering.
         var_bounds = {_id: v.bounds for _id, v in var_map.items()}
+        var_values = {_id: v.value for _id, v in var_map.items()}
 
         eliminated_cons, eliminated_vars = self._linear_presolve(
-            comp_by_linear_var, lcon_by_linear_nnz, var_bounds
+            comp_by_linear_var, lcon_by_linear_nnz, var_bounds, var_values
         )
         del comp_by_linear_var
         del lcon_by_linear_nnz
 
-        # Order the constraints, moving all nonlinear constraints to
-        # the beginning
-        n_nonlinear_cons = len(constraints)
+        # Note: defer categorizing constraints until after presolve, as
+        # the presolver could result in nonlinear constraints becoming
+        # linear (or trivial)
+        constraints = []
+        linear_cons = []
         if eliminated_cons:
             _removed = eliminated_cons.__contains__
-            constraints.extend(filterfalse(lambda c: _removed(id(c[0])), linear_cons))
+            _constraints = filterfalse(lambda c: _removed(id(c[0])), all_constraints)
         else:
-            constraints.extend(linear_cons)
+            _constraints = all_constraints
+        for info in _constraints:
+            expr_info = info[1]
+            if expr_info.nonlinear:
+                nl, args = expr_info.nonlinear
+                if any(vid not in nl_map for vid in args):
+                    constraints.append(info)
+                    continue
+                expr_info.const += _evaluate_constant_nl(
+                    nl % tuple(nl_map[i] for i in args), self.external_functions
+                )
+                expr_info.nonlinear = None
+            if expr_info.linear:
+                linear_cons.append(info)
+            elif not self.config.skip_trivial_constraints:
+                linear_cons.append(info)
+            else:  # constant constraint and skip_trivial_constraints
+                c = expr_info.const
+                con, expr_info, lb, ub = info
+                if (lb is not None and lb - c > TOL) or (
+                    ub is not None and ub - c < -TOL
+                ):
+                    raise InfeasibleConstraintException(
+                        "model contains a trivially infeasible "
+                        f"constraint '{con.name}' (fixed body value "
+                        f"{c} outside bounds [{lb}, {ub}])."
+                    )
+
+        # Order the constraints, moving all nonlinear constraints to
+        # the beginning
+        n_nonlinear_cons = len(constraints)
+        constraints.extend(linear_cons)
         n_cons = len(constraints)
 
         #
         # Collect variables from constraints and objectives into the
         # groupings necessary for AMPL
         #
         # For efficiency, we will do everything with ids (and not the
         # var objects themselves)
         #
 
         # Filter out any unused named expressions
         self.subexpression_order = list(
-            filter(self.used_named_expressions.__contains__, self.subexpression_order)
+            filter(self.used_named_expressions.__contains__, self.subexpression_cache)
         )
 
         # linear contribution by (constraint, objective, variable) component.
         # Keys are component id(), Values are dicts mapping variable
         # id() to linear coefficient.  All nonzeros in the component
         # (variables appearing in the linear and/or nonlinear
         # subexpressions) will appear in the dict.
@@ -816,18 +843,15 @@
         # nonlinear equality constraints), then this logic will need to
         # be revisited.
         linear_by_comp = {_id: info.linear for _id, info in eliminated_vars.items()}
 
         # We need to categorize the named subexpressions first so that
         # we know their linear / nonlinear vars when we encounter them
         # in constraints / objectives
-        self._categorize_vars(
-            map(self.subexpression_cache.__getitem__, self.subexpression_order),
-            linear_by_comp,
-        )
+        self._categorize_vars(self.subexpression_cache.values(), linear_by_comp)
         n_subexpressions = self._count_subexpression_occurrences()
         obj_vars_linear, obj_vars_nonlinear, obj_nnz_by_var = self._categorize_vars(
             objectives, linear_by_comp
         )
         con_vars_linear, con_vars_nonlinear, con_nnz_by_var = self._categorize_vars(
             constraints, linear_by_comp
         )
@@ -843,14 +867,15 @@
                 else:
                     _iter = (v,)
                 for _v in _iter:
                     _id = id(_v)
                     if _id not in var_map:
                         var_map[_id] = _v
                         var_bounds[_id] = _v.bounds
+                        var_values[_id] = _v.value
                     con_vars_nonlinear.add(_id)
 
         con_nnz = sum(con_nnz_by_var.values())
         timer.toc('Categorized model variables: %s nnz', con_nnz, level=logging.DEBUG)
 
         n_lcons = 0  # We do not yet support logical constraints
 
@@ -1037,33 +1062,34 @@
             labeler = NameLabeler()
             row_labels = [labeler(info[0]) for info in constraints] + [
                 labeler(info[0]) for info in objectives
             ]
             row_comments = [f'\t#{lbl}' for lbl in row_labels]
             col_labels = [labeler(var_map[_id]) for _id in variables]
             col_comments = [f'\t#{lbl}' for lbl in col_labels]
-            self.var_id_to_nl = {
-                _id: f'v{var_idx}{col_comments[var_idx]}'
+            id2nl = {
+                _id: f'v{var_idx}{col_comments[var_idx]}\n'
                 for var_idx, _id in enumerate(variables)
             }
             # Write out the .row and .col data
             if self.rowstream is not None:
                 self.rowstream.write('\n'.join(row_labels))
                 self.rowstream.write('\n')
             if self.colstream is not None:
                 self.colstream.write('\n'.join(col_labels))
                 self.colstream.write('\n')
         else:
             row_labels = row_comments = [''] * (n_cons + n_objs)
             col_labels = col_comments = [''] * len(variables)
-            self.var_id_to_nl = {
-                _id: f"v{var_idx}" for var_idx, _id in enumerate(variables)
-            }
+            id2nl = {_id: f"v{var_idx}\n" for var_idx, _id in enumerate(variables)}
 
-        _vmap = self.var_id_to_nl
+        if nl_map:
+            nl_map.update(id2nl)
+        else:
+            self.var_id_to_nl_map = nl_map = id2nl
         if scale_model:
             template = self.template
             objective_scaling = [scaling_cache[id(info[0])] for info in objectives]
             constraint_scaling = [scaling_cache[id(info[0])] for info in constraints]
             variable_scaling = [scaling_factor(var_map[_id]) for _id in variables]
             for _id, scale in zip(variables, variable_scaling):
                 if scale == 1:
@@ -1075,52 +1101,50 @@
                 else:
                     lb, ub = var_bounds[_id]
                 if lb is not None:
                     lb *= scale
                 if ub is not None:
                     ub *= scale
                 var_bounds[_id] = lb, ub
-                # Update _vmap to output scaled variables in NL expressions
-                _vmap[_id] = (
-                    template.division + _vmap[_id] + '\n' + template.const % scale
-                ).rstrip()
+                # Update nl_map to output scaled variables in NL expressions
+                nl_map[_id] = template.division + nl_map[_id] + template.const % scale
 
         # Update any eliminated variables to point to the (potentially
         # scaled) substituted variables
         for _id, expr_info in list(eliminated_vars.items()):
             nl, args, _ = expr_info.compile_repn(visitor)
             for _i in args:
                 # It is possible that the eliminated variable could
                 # reference another variable that is no longer part of
-                # the model and therefore does not have a _vmap entry.
+                # the model and therefore does not have a nl_map entry.
                 # This can happen when there is an underdetermined
                 # independent linear subsystem and the presolve removed
                 # all the constraints from the subsystem.  Because the
                 # free variables in the subsystem are not referenced
                 # anywhere else in the model, they are not part of the
                 # `variables` list.  Implicitly "fix" it to an arbitrary
                 # valid value from the presolved domain (see #3192).
-                if _i not in _vmap:
+                if _i not in nl_map:
                     lb, ub = var_bounds[_i]
                     if lb is None:
                         lb = -inf
                     if ub is None:
                         ub = inf
                     if lb <= 0 <= ub:
                         val = 0
                     else:
                         val = lb if abs(lb) < abs(ub) else ub
                     eliminated_vars[_i] = AMPLRepn(val, {}, None)
-                    _vmap[_i] = expr_info.compile_repn(visitor)[0]
+                    nl_map[_i] = expr_info.compile_repn(visitor)[0]
                     logger.warning(
                         "presolve identified an underdetermined independent "
                         "linear subsystem that was removed from the model.  "
                         f"Setting '{var_map[_i]}' == {val}"
                     )
-            _vmap[_id] = nl.rstrip() % tuple(_vmap[_i] for _i in args)
+            nl_map[_id] = nl % tuple(nl_map[_i] for _i in args)
 
         r_lines = [None] * n_cons
         for idx, (con, expr_info, lb, ub) in enumerate(constraints):
             if lb == ub:  # TBD: should this be within tolerance?
                 if lb is None:
                     # type = 3  # -inf <= c <= inf
                     r_lines[idx] = "3"
@@ -1311,15 +1335,15 @@
             " %d %d %d %d %d\t# common exprs: b,c,o,c1,o1\n" % tuple(n_subexpressions)
         )
 
         #
         # "F" lines (external function definitions)
         #
         amplfunc_libraries = set()
-        for fid, fcn in sorted(self.external_functions.values()):
+        for fid, fcn in self.external_functions:
             amplfunc_libraries.add(fcn._library)
             ostream.write("F%d 1 -1 %s\n" % (fid, fcn._function))
 
         #
         # "S" lines (suffixes)
         #
         for name, data in suffix_data.items():
@@ -1465,15 +1489,15 @@
                 )
 
         #
         # "x" lines (variable initialization)
         #
         _init_lines = [
             (var_idx, val if val.__class__ in int_float else float(val))
-            for var_idx, val in enumerate(var_map[_id].value for _id in variables)
+            for var_idx, val in enumerate(map(var_values.__getitem__, variables))
             if val is not None
         ]
         if scale_model:
             _init_lines = [
                 (var_idx, val * variable_scaling[var_idx])
                 for var_idx, val in _init_lines
             ]
@@ -1686,20 +1710,21 @@
                         expr_info.linear[i] = 0
                 else:
                     # All variables are nonlinear; generate the linear
                     # dict with all zeros
                     expr_info.linear = dict.fromkeys(nonlinear_vars, 0)
                 all_nonlinear_vars.update(nonlinear_vars)
 
-            # Update the count of components that each variable appears in
-            for v in expr_info.linear:
-                if v in nnz_by_var:
-                    nnz_by_var[v] += 1
-                else:
-                    nnz_by_var[v] = 1
+            if expr_info.linear:
+                # Update the count of components that each variable appears in
+                for v in expr_info.linear:
+                    if v in nnz_by_var:
+                        nnz_by_var[v] += 1
+                    else:
+                        nnz_by_var[v] = 1
             # Record all nonzero variable ids for this component
             linear_by_comp[id(comp_info[0])] = expr_info.linear
         # Linear models (or objectives) are common.  Avoid the set
         # difference if possible
         if all_nonlinear_vars:
             all_linear_vars -= all_nonlinear_vars
         return all_linear_vars, all_nonlinear_vars, nnz_by_var
@@ -1731,15 +1756,17 @@
                 n_subexpressions[3 if info[0] else 1] += 1
             elif info[0] is None:
                 n_subexpressions[4 if info[1] else 2] += 1
             else:
                 n_subexpressions[0] += 1
         return n_subexpressions
 
-    def _linear_presolve(self, comp_by_linear_var, lcon_by_linear_nnz, var_bounds):
+    def _linear_presolve(
+        self, comp_by_linear_var, lcon_by_linear_nnz, var_bounds, var_values
+    ):
         eliminated_vars = {}
         eliminated_cons = set()
         if not self.config.linear_presolve:
             return eliminated_cons, eliminated_vars
 
         # We need to record all named expressions with linear components
         # so that any eliminated variables are removed from them.
@@ -1752,32 +1779,35 @@
 
         fixed_vars = [
             _id for _id, (lb, ub) in var_bounds.items() if lb == ub and lb is not None
         ]
         var_map = self.var_map
         substitutions_by_linear_var = defaultdict(set)
         template = self.template
+        nl_map = self.var_id_to_nl_map
         one_var = lcon_by_linear_nnz[1]
         two_var = lcon_by_linear_nnz[2]
         while 1:
             if fixed_vars:
                 _id = fixed_vars.pop()
                 a = x = None
                 b, _ = var_bounds[_id]
                 logger.debug("NL presolve: bounds fixed %s := %s", var_map[_id], b)
                 eliminated_vars[_id] = AMPLRepn(b, {}, None)
+                nl_map[_id] = template.const % b
             elif one_var:
                 con_id, info = one_var.popitem()
                 expr_info, lb = info
                 _id, coef = expr_info.linear.popitem()
                 # substituting _id with a*x + b
                 a = x = None
                 b = expr_info.const = (lb - expr_info.const) / coef
                 logger.debug("NL presolve: substituting %s := %s", var_map[_id], b)
                 eliminated_vars[_id] = expr_info
+                nl_map[_id] = template.const % b
                 lb, ub = var_bounds[_id]
                 if (lb is not None and lb - b > TOL) or (
                     ub is not None and ub - b < -TOL
                 ):
                     raise InfeasibleConstraintException(
                         "model contains a trivially infeasible variable "
                         f"'{var_map[_id].name}' (presolved to a value of "
@@ -1804,15 +1834,15 @@
                     log_coef = _log10(abs(coef))
                     log_coef2 = _log10(abs(coef2))
                     if abs(log_coef2) < abs(log_coef) or (
                         log_coef2 == -log_coef and log_coef2 < log_coef
                     ):
                         _id, id2 = id2, _id
                         coef, coef2 = coef2, coef
-                # substituting _id with a*x + b
+                # eliminating _id and replacing it with a*x + b
                 a = -coef2 / coef
                 x = id2
                 b = expr_info.const = (lb - expr_info.const) / coef
                 expr_info.linear[x] = a
                 substitutions_by_linear_var[x].add(_id)
                 eliminated_vars[_id] = expr_info
                 logger.debug(
@@ -1834,17 +1864,36 @@
                 if x_lb is None or (lb is not None and lb > x_lb):
                     x_lb = lb
                 if x_ub is None or (ub is not None and ub < x_ub):
                     x_ub = ub
                 var_bounds[x] = x_lb, x_ub
                 if x_lb == x_ub and x_lb is not None:
                     fixed_vars.append(x)
+                # Given that we are eliminating a variable, we want to
+                # attempt to sanely resolve the initial variable values.
+                y_init = var_values[_id]
+                if y_init is not None:
+                    # Y has a value
+                    x_init = var_values[x]
+                    if x_init is None:
+                        # X does not; just use the one calculated from Y
+                        x_init = (y_init - b) / a
+                    else:
+                        # X does too, use the average of the two values
+                        x_init = (x_init + (y_init - b) / a) / 2.0
+                    # Ensure that the initial value respects the
+                    # tightened bounds
+                    if x_ub is not None and x_init > x_ub:
+                        x_init = x_ub
+                    if x_lb is not None and x_init < x_lb:
+                        x_init = x_lb
+                    var_values[x] = x_init
                 eliminated_cons.add(con_id)
             else:
-                return eliminated_cons, eliminated_vars
+                break
             for con_id, expr_info in comp_by_linear_var[_id]:
                 # Note that if we were aggregating (i.e., _id was
                 # from two_var), then one of these info's will be
                 # for the constraint we just eliminated.  In this
                 # case, _id will no longer be in expr_info.linear - so c
                 # will be 0 - thereby preventing us from re-updating
                 # the expression.  We still want it to persist so
@@ -1888,14 +1937,50 @@
                 expr_info = eliminated_vars[resubst]
                 c = expr_info.linear.pop(_id, 0)
                 expr_info.const += c * b
                 if x in expr_info.linear:
                     expr_info.linear[x] += c * a
                 elif a:
                     expr_info.linear[x] = c * a
+                elif not expr_info.linear:
+                    nl_map[resubst] = template.const % expr_info.const
+
+        # Note: the ASL will (silently) produce incorrect answers if the
+        # nonlinear portion of a defined variable is a constant
+        # expression.  This may not be the case if all the variables in
+        # the original nonlinear expression have been fixed.
+        for _id, (expr, info, sub) in self.subexpression_cache.items():
+            if info.nonlinear:
+                nl, args = info.nonlinear
+                # Note: 'not args' skips string arguments
+                # Note: 'vid in nl_map' skips eliminated
+                #   variables and defined variables reduced to constants
+                if not args or any(vid not in nl_map for vid in args):
+                    continue
+                # Ideally, we would just evaluate the named expression.
+                # However, there might be a linear portion of the named
+                # expression that still has free variables, and there is no
+                # guarantee that the user actually initialized the
+                # variables.  So, we will fall back on parsing the (now
+                # constant) nonlinear fragment and evaluating it.
+                info.nonlinear = None
+                info.const += _evaluate_constant_nl(
+                    nl % tuple(nl_map[i] for i in args), self.external_functions
+                )
+            if not info.linear:
+                # This has resolved to a constant: the ASL will fail for
+                # defined variables containing ONLY a constant.  We
+                # need to substitute the constant directly into the
+                # original constraint/objective expression(s)
+                info.linear = {}
+                self.used_named_expressions.discard(_id)
+                nl_map[_id] = template.const % info.const
+                self.subexpression_cache[_id] = (expr, info, [None, None, True])
+
+        return eliminated_cons, eliminated_vars
 
     def _record_named_expression_usage(self, named_exprs, src, comp_type):
         self.used_named_expressions.update(named_exprs)
         src = id(src)
         for _id in named_exprs:
             info = self.subexpression_cache[_id][2]
             if info[comp_type] is None:
@@ -1913,29 +1998,46 @@
         # already been compiled)
         if repn.nonlinear:
             nl, args = repn.nonlinear
             if include_const and repn.const:
                 # Add the constant to the NL expression.  AMPL adds the
                 # constant as the second argument, so we will too.
                 nl = self.template.binary_sum + nl + self.template.const % repn.const
-            self.ostream.write(nl % tuple(map(self.var_id_to_nl.__getitem__, args)))
+            try:
+                self.ostream.write(
+                    nl % tuple(map(self.var_id_to_nl_map.__getitem__, args))
+                )
+            except KeyError:
+                final_args = []
+                for arg in args:
+                    if arg in self.var_id_to_nl_map:
+                        final_args.append(self.var_id_to_nl_map[arg])
+                    else:
+                        _nl, _ids, _ = self.subexpression_cache[arg][1].compile_repn(
+                            self.visitor
+                        )
+                        final_args.append(
+                            _nl % tuple(map(self.var_id_to_nl_map.__getitem__, _ids))
+                        )
+                self.ostream.write(nl % tuple(final_args))
+
         elif include_const:
             self.ostream.write(self.template.const % repn.const)
         else:
             self.ostream.write(self.template.const % 0)
 
     def _write_v_line(self, expr_id, k):
         ostream = self.ostream
         column_order = self.column_order
         info = self.subexpression_cache[expr_id]
         if self.symbolic_solver_labels:
             lbl = '\t#%s' % info[0].name
         else:
             lbl = ''
-        self.var_id_to_nl[expr_id] = f"v{self.next_V_line_id}{lbl}"
+        self.var_id_to_nl_map[expr_id] = f"v{self.next_V_line_id}{lbl}\n"
         # Do NOT write out 0 coefficients here: doing so fouls up the
         # ASL's logic for calculating derivatives, leading to 'nan' in
         # the Hessian results.
         linear = dict(item for item in info[1].linear.items() if item[1])
         #
         ostream.write(f'V{self.next_V_line_id} {len(linear)} {k}{lbl}\n')
         for _id in sorted(linear, key=column_order.__getitem__):
@@ -2010,15 +2112,15 @@
     def duplicate(self):
         ans = self.__class__.__new__(self.__class__)
         ans.nl = self.nl
         ans.mult = self.mult
         ans.const = self.const
         ans.linear = None if self.linear is None else dict(self.linear)
         ans.nonlinear = self.nonlinear
-        ans.named_exprs = self.named_exprs
+        ans.named_exprs = None if self.named_exprs is None else set(self.named_exprs)
         return ans
 
     def compile_repn(self, visitor, prefix='', args=None, named_exprs=None):
         template = visitor.template
         if self.mult != 1:
             if self.mult == -1:
                 prefix += template.negation
@@ -2255,25 +2357,64 @@
     nary_sum = 'o54\t# sumlist\n%d\t# (n)\n'
     exprif = 'o35\t# if\n'
     and_expr = 'o21\t# and\n'
     less_than = 'o22\t# lt\n'
     less_equal = 'o23\t# le\n'
     equality = 'o24\t# eq\n'
     external_fcn = 'f%d %d%s\n'
-    var = '%s\n'  # NOTE: to support scaling, we do NOT include the 'v' here
+    # NOTE: to support scaling and substitutions, we do NOT include the
+    # 'v' or the EOL here:
+    var = '%s'
     const = 'n%r\n'
     string = 'h%d:%s\n'
     monomial = product + const + var.replace('%', '%%')
     multiplier = product + const
 
     _create_strict_inequality_map(vars())
 
 
+nl_operators = {
+    0: (2, operator.add),
+    2: (2, operator.mul),
+    3: (2, operator.truediv),
+    5: (2, operator.pow),
+    15: (1, operator.abs),
+    16: (1, operator.neg),
+    54: (None, lambda *x: sum(x)),
+    35: (3, lambda a, b, c: b if a else c),
+    21: (2, operator.and_),
+    22: (2, operator.lt),
+    23: (2, operator.le),
+    24: (2, operator.eq),
+    43: (1, math.log),
+    42: (1, math.log10),
+    41: (1, math.sin),
+    46: (1, math.cos),
+    38: (1, math.tan),
+    40: (1, math.sinh),
+    45: (1, math.cosh),
+    37: (1, math.tanh),
+    51: (1, math.asin),
+    53: (1, math.acos),
+    49: (1, math.atan),
+    44: (1, math.exp),
+    39: (1, math.sqrt),
+    50: (1, math.asinh),
+    52: (1, math.acosh),
+    47: (1, math.atanh),
+    14: (1, math.ceil),
+    13: (1, math.floor),
+}
+
+
 def _strip_template_comments(vars_, base_):
-    vars_['unary'] = {k: v[: v.find('\t#')] + '\n' for k, v in base_.unary.items()}
+    vars_['unary'] = {
+        k: v[: v.find('\t#')] + '\n' if v[-1] == '\n' else ''
+        for k, v in base_.unary.items()
+    }
     for k, v in base_.__dict__.items():
         if type(v) is str and '\t#' in v:
             v_lines = v.split('\n')
             for i, l in enumerate(v_lines):
                 comment_start = l.find('\t#')
                 if comment_start >= 0:
                     v_lines[i] = l[:comment_start]
@@ -2516,35 +2657,35 @@
         # 1: the common subexpression (to be written out)
         repn,
         # 2: the source usage information for this subexpression:
         #    [(con_id, obj_id, substitute); see above]
         expression_source,
     )
 
+    # As we will eventually need the compiled form of any nonlinear
+    # expression, we will go ahead and compile it here.  We do not
+    # do the same for the linear component as we will only need the
+    # linear component compiled to a dict if we are emitting the
+    # original (linear + nonlinear) V line (which will not happen if
+    # the V line is part of a larger linear operator).
+    if repn.nonlinear.__class__ is list:
+        repn.compile_nonlinear_fragment(visitor)
+
     if not visitor.use_named_exprs:
         return _GENERAL, repn.duplicate()
 
     mult, repn.mult = repn.mult, 1
     if repn.named_exprs is None:
         repn.named_exprs = set()
 
     # When converting this shared subexpression to a (nonlinear)
     # node, we want to just reference this subexpression:
     repn.nl = (visitor.template.var, (_id,))
 
     if repn.nonlinear:
-        # As we will eventually need the compiled form of any nonlinear
-        # expression, we will go ahead and compile it here.  We do not
-        # do the same for the linear component as we will only need the
-        # linear component compiled to a dict if we are emitting the
-        # original (linear + nonlinear) V line (which will not happen if
-        # the V line is part of a larger linear operator).
-        if repn.nonlinear.__class__ is list:
-            repn.compile_nonlinear_fragment(visitor)
-
         if repn.linear:
             # If this expression has both linear and nonlinear
             # components, we will follow the ASL convention and break
             # the named subexpression into two named subexpressions: one
             # that is only the nonlinear component and one that has the
             # const/linear component (and references the first).  This
             # will allow us to propagate linear coefficients up from
@@ -2559,16 +2700,18 @@
             repn.named_exprs.add(sub_id)
             repn.nonlinear = sub_repn.nl
 
             # See above for the meaning of this source information
             nl_info = list(expression_source)
             visitor.subexpression_cache[sub_id] = (sub_node, sub_repn, nl_info)
             # It is important that the NL subexpression comes before the
-            # main named expression:
-            visitor.subexpression_order.append(sub_id)
+            # main named expression: re-insert the original named
+            # expression (so that the nonlinear sub_node comes first
+            # when iterating over subexpression_cache)
+            visitor.subexpression_cache[_id] = visitor.subexpression_cache.pop(_id)
         else:
             nl_info = expression_source
     else:
         repn.nonlinear = None
         if repn.linear:
             if (
                 not repn.const
@@ -2599,33 +2742,32 @@
                 prefix = visitor.template.negation
             else:
                 prefix = visitor.template.multiplier % mult
             repn.nonlinear = prefix + repn.nonlinear[0], repn.nonlinear[1]
 
     if expression_source[2]:
         if repn.linear:
-            return (_MONOMIAL, next(iter(repn.linear)), 1)
+            assert len(repn.linear) == 1 and not repn.const
+            return (_MONOMIAL,) + next(iter(repn.linear.items()))
         else:
             return (_CONSTANT, repn.const)
 
-    # Defer recording this _id until after we know that this repn will
-    # not be directly substituted (and to ensure that the NL fragment is
-    # added to the order first).
-    visitor.subexpression_order.append(_id)
-
     return (_GENERAL, repn.duplicate())
 
 
 def handle_external_function_node(visitor, node, *args):
     func = node._fcn._function
     # There is a special case for external functions: these are the only
     # expressions that can accept string arguments. As we currently pass
-    # these as 'precompiled' general NL fragments, the normal trap for
-    # constant subexpressions will miss constant external function calls
-    # that contain strings.  We will catch that case here.
+    # these as 'precompiled' GENERAL AMPLRepns, the normal trap for
+    # constant subexpressions will miss string arguments.  We will catch
+    # that case here by looking for NL fragments with no variable
+    # references.  Note that the NL fragment is NOT the raw string
+    # argument that we want to evaluate: the raw string is in the
+    # `const` field.
     if all(
         arg[0] is _CONSTANT or (arg[0] is _GENERAL and arg[1].nl and not arg[1].nl[1])
         for arg in args
     ):
         arg_list = [arg[1] if arg[0] is _CONSTANT else arg[1].const for arg in args]
         return _CONSTANT, apply_node_operation(node, arg_list)
     if func in visitor.external_functions:
@@ -2633,31 +2775,50 @@
             raise RuntimeError(
                 "The same external function name (%s) is associated "
                 "with two different libraries (%s through %s, and %s "
                 "through %s).  The ASL solver will fail to link "
                 "correctly."
                 % (
                     func,
-                    visitor.external_byFcn[func]._library,
-                    visitor.external_byFcn[func]._library.name,
+                    visitor.external_functions[func]._library,
+                    visitor.external_functions[func]._library.name,
                     node._fcn._library,
                     node._fcn.name,
                 )
             )
     else:
         visitor.external_functions[func] = (len(visitor.external_functions), node._fcn)
     comment = f'\t#{node.local_name}' if visitor.symbolic_solver_labels else ''
-    nonlin = node_result_to_amplrepn(args[0]).compile_repn(
-        visitor,
-        visitor.template.external_fcn
-        % (visitor.external_functions[func][0], len(args), comment),
+    nl = visitor.template.external_fcn % (
+        visitor.external_functions[func][0],
+        len(args),
+        comment,
+    )
+    arg_ids = []
+    named_exprs = set()
+    for arg in args:
+        _id = id(arg)
+        arg_ids.append(_id)
+        visitor.subexpression_cache[_id] = (
+            arg,
+            AMPLRepn(
+                0,
+                None,
+                node_result_to_amplrepn(arg).compile_repn(
+                    visitor, named_exprs=named_exprs
+                ),
+            ),
+            (None, None, True),
+        )
+    if not named_exprs:
+        named_exprs = None
+    return (
+        _GENERAL,
+        AMPLRepn(0, None, (nl + '%s' * len(arg_ids), arg_ids, named_exprs)),
     )
-    for arg in args[1:]:
-        nonlin = node_result_to_amplrepn(arg).compile_repn(visitor, *nonlin)
-    return (_GENERAL, AMPLRepn(0, None, nonlin))
 
 
 _operator_handles = ExitNodeDispatcher(
     {
         NegationExpression: handle_negation_node,
         ProductExpression: handle_product_node,
         DivisionExpression: handle_division_node,
@@ -2857,26 +3018,24 @@
 
 
 class AMPLRepnVisitor(StreamBasedExpressionVisitor):
     def __init__(
         self,
         template,
         subexpression_cache,
-        subexpression_order,
         external_functions,
         var_map,
         used_named_expressions,
         symbolic_solver_labels,
         use_named_exprs,
         sorter,
     ):
         super().__init__()
         self.template = template
         self.subexpression_cache = subexpression_cache
-        self.subexpression_order = subexpression_order
         self.external_functions = external_functions
         self.active_expression_source = None
         self.var_map = var_map
         self.used_named_expressions = used_named_expressions
         self.symbolic_solver_labels = symbolic_solver_labels
         self.use_named_exprs = use_named_exprs
         self.encountered_string_arguments = False
@@ -3017,7 +3176,64 @@
                     prefix = self.template.negation
                 else:
                     prefix = self.template.multiplier % mult
                 ans.nonlinear = prefix + ans.nonlinear[0], ans.nonlinear[1]
         #
         self.active_expression_source = None
         return ans
+
+
+def _evaluate_constant_nl(nl, external_functions):
+    expr = nl.splitlines()
+    stack = []
+    while expr:
+        line = expr.pop()
+        tokens = line.split()
+        # remove tokens after the first comment
+        for i, t in enumerate(tokens):
+            if t.startswith('#'):
+                tokens = tokens[:i]
+                break
+        if len(tokens) != 1:
+            # skip blank lines
+            if not tokens:
+                continue
+            if tokens[0][0] == 'f':
+                # external function
+                fid, nargs = tokens
+                fid = int(fid[1:])
+                nargs = int(nargs)
+                fcn_id, ef = external_functions[fid]
+                assert fid == fcn_id
+                stack.append(ef.evaluate(tuple(stack.pop() for i in range(nargs))))
+                continue
+            raise DeveloperError(
+                f"Unsupported line format _evaluate_constant_nl() "
+                f"(we expect each line to contain a single token): '{line}'"
+            )
+        term = tokens[0]
+        # the "command" can be determined by the first character on the line
+        cmd = term[0]
+        # Note that we will unpack the line into the expected number of
+        # explicit arguments as a form of error checking
+        if cmd == 'n':
+            # numeric constant
+            stack.append(float(term[1:]))
+        elif cmd == 'o':
+            # operator
+            nargs, fcn = nl_operators[int(term[1:])]
+            if nargs is None:
+                nargs = int(stack.pop())
+            stack.append(fcn(*(stack.pop() for i in range(nargs))))
+        elif cmd in '1234567890':
+            # this is either a single int (e.g., the nargs in a nary
+            # sum) or a string argument.  Preserve it as-is until later
+            # when we know which we are expecting.
+            stack.append(term)
+        elif cmd == 'h':
+            stack.append(term.split(':', 1)[1])
+        else:
+            raise DeveloperError(
+                f"Unsupported NL operator in _evaluate_constant_nl(): '{line}'"
+            )
+    assert len(stack) == 1
+    return stack[0]
```

### Comparing `Pyomo-6.7.2/pyomo/repn/plugins/standard_form.py` & `Pyomo-6.7.3/pyomo/repn/plugins/standard_form.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/quadratic.py` & `Pyomo-6.7.3/pyomo/repn/quadratic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/standard_aux.py` & `Pyomo-6.7.3/pyomo/repn/standard_aux.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/standard_repn.py` & `Pyomo-6.7.3/pyomo/repn/standard_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/__init__.py` & `Pyomo-6.7.3/pyomo/repn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/__init__.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/helper.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/helper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/nl_diff.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/nl_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small10_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small10_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small11_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small11_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small12_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small12_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small13_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small13_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small14_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small14_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small15_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small15_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small1_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small1_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small2_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small2_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small3_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small3_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small4_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small4_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small5_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small5_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small6_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small6_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small7_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small7_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small8_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small8_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/small9_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/small9_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/test_ampl_comparison.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/test_ampl_comparison.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/test_ampl_nl.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/test_ampl_nl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/test_ampl_repn.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/test_ampl_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/test_nlv2.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/test_nlv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import pyomo.repn.util as repn_util
 import pyomo.repn.plugins.nl_writer as nl_writer
 from pyomo.repn.util import InvalidNumber
 from pyomo.repn.tests.nl_diff import nl_diff
 
 from pyomo.common.dependencies import numpy, numpy_available
 from pyomo.common.errors import MouseTrap
+from pyomo.common.gsl import find_GSL
 from pyomo.common.log import LoggingIntercept
 from pyomo.common.tee import capture_output
 from pyomo.common.tempfiles import TempfileManager
 from pyomo.common.timing import report_timing
 from pyomo.core.expr import Expr_if, inequality, LinearExpression
 from pyomo.core.base.expression import ScalarExpression
 from pyomo.environ import (
@@ -53,24 +54,22 @@
 class INFO(object):
     def __init__(self, symbolic=False):
         if symbolic:
             self.template = nl_writer.text_nl_debug_template
         else:
             self.template = nl_writer.text_nl_template
         self.subexpression_cache = {}
-        self.subexpression_order = []
         self.external_functions = {}
         self.var_map = {}
         self.used_named_expressions = set()
         self.symbolic_solver_labels = symbolic
 
         self.visitor = nl_writer.AMPLRepnVisitor(
             self.template,
             self.subexpression_cache,
-            self.subexpression_order,
             self.external_functions,
             self.var_map,
             self.used_named_expressions,
             self.symbolic_solver_labels,
             True,
             None,
         )
@@ -95,15 +94,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((m.x**2 / m.p, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o5\n%s\nn2\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o5\n%sn2\n', [id(m.x)]))
 
         m.p = 2
 
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((4 / m.p, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
@@ -147,25 +146,25 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((m.x**2 / m.p, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o2\nn0.5\no5\n%s\nn2\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o2\nn0.5\no5\n%sn2\n', [id(m.x)]))
 
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((log(m.x) / m.x, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o3\no43\n%s\n%s\n', [id(m.x), id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o3\no43\n%s%s', [id(m.x), id(m.x)]))
 
     def test_errors_divide_by_0(self):
         m = ConcreteModel()
         m.p = Param(mutable=True, initialize=0)
         m.x = Var()
 
         info = INFO()
@@ -252,15 +251,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((m.x**m.p, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o5\n%s\nn2\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o5\n%sn2\n', [id(m.x)]))
 
         m.p = 1
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((m.x**m.p, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
@@ -539,15 +538,15 @@
         expr = m.z[1] - ((m.z[2] * m.z[3]) * m.z[4])
         with INFO() as info:
             repn = info.visitor.walk_expression((expr, None, None, 1))
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, InvalidNumber(None))
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear[0], 'o16\no2\no2\n%s\n%s\n%s\n')
+        self.assertEqual(repn.nonlinear[0], 'o16\no2\no2\n%s%s%s')
         self.assertEqual(repn.nonlinear[1], [id(m.z[2]), id(m.z[3]), id(m.z[4])])
 
         m.z[3].fix(float('nan'))
         with INFO() as info:
             repn = info.visitor.walk_expression((expr, None, None, 1))
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
@@ -589,15 +588,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((m.x ** (0.5), None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o5\n%s\nn0.5\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o5\n%sn0.5\n', [id(m.x)]))
 
         m.x.fix()
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((m.x ** (0.5), None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
@@ -614,15 +613,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((abs(m.x), None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o15\n%s\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o15\n%s', [id(m.x)]))
 
         m.x.fix()
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((abs(m.x), None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
@@ -639,15 +638,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((log(m.x), None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o43\n%s\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o43\n%s', [id(m.x)]))
 
         m.x.fix()
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((log(m.x), None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
@@ -668,15 +667,15 @@
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
         self.assertEqual(
             repn.nonlinear,
-            ('o35\no23\n%s\nn4\no5\n%s\nn2\n%s\n', [id(m.x), id(m.x), id(m.y)]),
+            ('o35\no23\n%sn4\no5\n%sn2\n%s', [id(m.x), id(m.x), id(m.y)]),
         )
 
         m.x.fix()
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((expr, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
@@ -709,15 +708,15 @@
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
         self.assertEqual(
             repn.nonlinear,
-            ('o35\no24\n%s\nn4\no5\n%s\nn2\n%s\n', [id(m.x), id(m.x), id(m.y)]),
+            ('o35\no24\n%sn4\no5\n%sn2\n%s', [id(m.x), id(m.x), id(m.y)]),
         )
 
         m.x.fix()
         info = INFO()
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((expr, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
@@ -751,15 +750,15 @@
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
         self.assertEqual(
             repn.nonlinear,
             (
-                'o35\no21\no23\nn1\n%s\no23\n%s\nn4\no5\n%s\nn2\n%s\n',
+                'o35\no21\no23\nn1\n%so23\n%sn4\no5\n%sn2\n%s',
                 [id(m.x), id(m.x), id(m.x), id(m.y)],
             ),
         )
 
         m.x.fix()
         info = INFO()
         with LoggingIntercept() as LOG:
@@ -812,15 +811,15 @@
         self.assertEqual(repn.const, 6)
         self.assertEqual(repn.linear, {id(m.x): 2})
         self.assertEqual(repn.nonlinear, None)
 
         self.assertEqual(len(info.subexpression_cache), 1)
         obj, repn, info = info.subexpression_cache[id(m.e)]
         self.assertIs(obj, m.e)
-        self.assertEqual(repn.nl, ('%s\n', (id(m.e),)))
+        self.assertEqual(repn.nl, ('%s', (id(m.e),)))
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 3)
         self.assertEqual(repn.linear, {id(m.x): 1})
         self.assertEqual(repn.nonlinear, None)
         self.assertEqual(info, [None, None, False])
 
     def test_nested_operator_zero_arg(self):
@@ -839,15 +838,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((expr, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {})
-        self.assertEqual(repn.nonlinear, ('o24\no3\nn1\n%s\nn0\n', [id(m.x)]))
+        self.assertEqual(repn.nonlinear, ('o24\no3\nn1\n%sn0\n', [id(m.x)]))
 
     def test_duplicate_shared_linear_expressions(self):
         # This tests an issue where AMPLRepn.duplicate() was not copying
         # the linear dict, allowing certain operations (like finalizing
         # a bare expression multiplied by something other than 1) to
         # change the compiled shared expression
         m = ConcreteModel()
@@ -926,15 +925,15 @@
         with LoggingIntercept() as LOG:
             repn = info.visitor.walk_expression((e, None, None, 1))
         self.assertEqual(LOG.getvalue(), "")
         self.assertEqual(repn.nl, None)
         self.assertEqual(repn.mult, 1)
         self.assertEqual(repn.const, 0)
         self.assertEqual(repn.linear, {id(m.x[2]): 4, id(m.x[3]): 9, id(m.x[4]): 16})
-        self.assertEqual(repn.nonlinear, ('o5\n%s\nn2\n', [id(m.x[2])]))
+        self.assertEqual(repn.nonlinear, ('o5\n%sn2\n', [id(m.x[2])]))
         with self.assertRaisesRegex(
             MouseTrap, "Cannot convert nonlinear AMPLRepn to Pyomo Expression"
         ):
             ee = repn.to_expr(info.var_map)
 
 
 class Test_NLWriter(unittest.TestCase):
@@ -1760,15 +1759,19 @@
                 )
         self.assertEqual(LOG.getvalue(), "")
 
         m.c1.set_value(m.x >= m.y + m.z + 1.5)
         OUT = io.StringIO()
         with LoggingIntercept() as LOG:
             nlinfo = nl_writer.NLWriter().write(
-                m, OUT, symbolic_solver_labels=True, linear_presolve=True
+                m,
+                OUT,
+                symbolic_solver_labels=True,
+                linear_presolve=True,
+                skip_trivial_constraints=False,
             )
         self.assertEqual(LOG.getvalue(), "")
 
         self.assertIs(nlinfo.eliminated_vars[0][0], m.y)
         self.assertExpressionsEqual(
             nlinfo.eliminated_vars[0][1], LinearExpression([-1.0 * m.z])
         )
@@ -1810,14 +1813,64 @@
 G0 1	#obj
 0 0
 """,
                 OUT.getvalue(),
             )
         )
 
+        OUT = io.StringIO()
+        with LoggingIntercept() as LOG:
+            nlinfo = nl_writer.NLWriter().write(
+                m, OUT, symbolic_solver_labels=True, linear_presolve=True
+            )
+        self.assertEqual(LOG.getvalue(), "")
+
+        self.assertIs(nlinfo.eliminated_vars[0][0], m.y)
+        self.assertExpressionsEqual(
+            nlinfo.eliminated_vars[0][1], LinearExpression([-1.0 * m.z])
+        )
+        self.assertEqual(nlinfo.eliminated_vars[1], (m.x, 2))
+
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0	# problem unknown
+ 1 0 1 0 0	#vars, constraints, objectives, ranges, eqns
+ 0 1 0 0 0 0	#nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0	#network constraints: nonlinear, linear
+ 0 1 0	#nonlinear vars in constraints, objectives, both
+ 0 0 0 1	#linear network variables; functions; arith, flags
+ 0 0 0 0 0	#discrete variables: binary, integer, nonlinear (b,c,o)
+ 0 1	#nonzeros in Jacobian, obj. gradient
+ 3 1	#max name lengths: constraints, variables
+ 0 0 0 0 0	#common exprs: b,c,o,c1,o1
+O0 0	#obj
+o54	#sumlist
+3	#(n)
+o5	#^
+n2
+n2
+o5	#^
+o16	#-
+v0	#z
+n2
+o5	#^
+v0	#z
+n2
+x0	#initial guess
+r	#1 ranges (rhs's)
+b	#1 bounds (on variables)
+3	#z
+k0	#intermediate Jacobian column lengths
+G0 1	#obj
+0 0
+""",
+                OUT.getvalue(),
+            )
+        )
+
     def test_presolve_independent_subsystem(self):
         # This is derived from the example in #3192
         m = ConcreteModel()
         m.x = Var()
         m.y = Var()
         m.z = Var()
         m.d = Constraint(expr=m.z == m.y)
@@ -2304,7 +2357,349 @@
 10 1
 11 1
 12 1
 """,
                 OUT.getvalue(),
             )
         )
+
+    def test_presolve_fixes_nl_defined_variables(self):
+        # This tests a workaround for a bug in the ASL where defined
+        # variables with constant expressions in the NL portion are not
+        # evaluated correctly.
+        m = ConcreteModel()
+        m.x = Var()
+        m.y = Var(bounds=(3, None))
+        m.z = Var(bounds=(None, 3))
+        m.e = Expression(expr=m.x + m.y * m.z + m.y**2 + 3 / m.z)
+        m.c1 = Constraint(expr=m.y * m.e + m.x >= 0)
+        m.c2 = Constraint(expr=m.y == m.z)
+
+        OUT = io.StringIO()
+        nl_writer.NLWriter().write(
+            m,
+            OUT,
+            symbolic_solver_labels=True,
+            linear_presolve=True,
+            export_defined_variables=True,
+        )
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0	# problem unknown
+ 1 1 0 0 0	#vars, constraints, objectives, ranges, eqns
+ 1 0 0 0 0 0	#nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0	#network constraints: nonlinear, linear
+ 1 0 0	#nonlinear vars in constraints, objectives, both
+ 0 0 0 1	#linear network variables; functions; arith, flags
+ 0 0 0 0 0	#discrete variables: binary, integer, nonlinear (b,c,o)
+ 1 0	#nonzeros in Jacobian, obj. gradient
+ 2 1	#max name lengths: constraints, variables
+ 0 0 0 1 0	#common exprs: b,c,o,c1,o1
+V1 1 1	#e
+0 1
+n19
+C0	#c1
+o2	#*
+n3
+v1	#e
+x0	#initial guess
+r	#1 ranges (rhs's)
+2 0	#c1
+b	#1 bounds (on variables)
+3	#x
+k0	#intermediate Jacobian column lengths
+J0 1	#c1
+0 1
+""",
+                OUT.getvalue(),
+            )
+        )
+
+        OUT = io.StringIO()
+        nl_writer.NLWriter().write(
+            m,
+            OUT,
+            symbolic_solver_labels=True,
+            linear_presolve=True,
+            export_defined_variables=False,
+        )
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0	# problem unknown
+ 1 1 0 0 0	#vars, constraints, objectives, ranges, eqns
+ 1 0 0 0 0 0	#nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0	#network constraints: nonlinear, linear
+ 1 0 0	#nonlinear vars in constraints, objectives, both
+ 0 0 0 1	#linear network variables; functions; arith, flags
+ 0 0 0 0 0	#discrete variables: binary, integer, nonlinear (b,c,o)
+ 1 0	#nonzeros in Jacobian, obj. gradient
+ 2 1	#max name lengths: constraints, variables
+ 0 0 0 0 0	#common exprs: b,c,o,c1,o1
+C0	#c1
+o2	#*
+n3
+o0	#+
+v0	#x
+o54	#sumlist
+3	#(n)
+o2	#*
+n3
+n3
+o5	#^
+n3
+n2
+o3	#/
+n3
+n3
+x0	#initial guess
+r	#1 ranges (rhs's)
+2 0	#c1
+b	#1 bounds (on variables)
+3	#x
+k0	#intermediate Jacobian column lengths
+J0 1	#c1
+0 1
+""",
+                OUT.getvalue(),
+            )
+        )
+
+        OUT = io.StringIO()
+        nl_writer.NLWriter().write(
+            m,
+            OUT,
+            symbolic_solver_labels=True,
+            linear_presolve=False,
+            export_defined_variables=True,
+        )
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0	# problem unknown
+ 3 2 0 0 1	#vars, constraints, objectives, ranges, eqns
+ 1 0 0 0 0 0	#nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0	#network constraints: nonlinear, linear
+ 3 0 0	#nonlinear vars in constraints, objectives, both
+ 0 0 0 1	#linear network variables; functions; arith, flags
+ 0 0 0 0 0	#discrete variables: binary, integer, nonlinear (b,c,o)
+ 5 0	#nonzeros in Jacobian, obj. gradient
+ 2 1	#max name lengths: constraints, variables
+ 0 0 0 2 0	#common exprs: b,c,o,c1,o1
+V3 0 1	#nl(e)
+o54	#sumlist
+3	#(n)
+o2	#*
+v0	#y
+v2	#z
+o5	#^
+v0	#y
+n2
+o3	#/
+n3
+v2	#z
+V4 1 1	#e
+1 1
+v3	#nl(e)
+C0	#c1
+o2	#*
+v0	#y
+v4	#e
+C1	#c2
+n0
+x0	#initial guess
+r	#2 ranges (rhs's)
+2 0	#c1
+4 0	#c2
+b	#3 bounds (on variables)
+2 3	#y
+3	#x
+1 3	#z
+k2	#intermediate Jacobian column lengths
+2
+3
+J0 3	#c1
+0 0
+1 1
+2 0
+J1 2	#c2
+0 1
+2 -1
+""",
+                OUT.getvalue(),
+            )
+        )
+
+    def test_presolve_fixes_nl_external_function(self):
+        # This tests a workaround for a bug in the ASL where external
+        # functions with constant argument expressions are not
+        # evaluated correctly.
+        DLL = find_GSL()
+        if not DLL:
+            self.skipTest("Could not find the amplgsl.dll library")
+
+        m = ConcreteModel()
+        m.hypot = ExternalFunction(library=DLL, function="gsl_hypot")
+        m.p = Param(initialize=1, mutable=True)
+        m.x = Var(bounds=(None, 3))
+        m.y = Var(bounds=(3, None))
+        m.z = Var(initialize=1)
+        m.o = Objective(expr=m.z**2 * m.hypot(m.p * m.x, m.p + m.y) ** 2)
+        m.c = Constraint(expr=m.x == m.y)
+
+        OUT = io.StringIO()
+        nl_writer.NLWriter().write(
+            m, OUT, symbolic_solver_labels=True, linear_presolve=False
+        )
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0       #problem unknown
+ 3 1 1 0 1     #vars, constraints, objectives, ranges, eqns
+ 0 1 0 0 0 0   #nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0   #network constraints: nonlinear, linear
+ 0 3 0 #nonlinear vars in constraints, objectives, both
+ 0 1 0 1       #linear network variables; functions; arith, flags
+ 0 0 0 0 0     #discrete variables: binary, integer, nonlinear (b,c,o)
+ 2 3   #nonzeros in Jacobian, obj. gradient
+ 1 1   #max name lengths: constraints, variables
+ 0 0 0 0 0     #common exprs: b,c,o,c1,o1
+F0 1 -1 gsl_hypot
+C0     #c
+n0
+O0 0   #o
+o2     #*
+o5     #^
+v0     #z
+n2
+o5     #^
+f0 2   #hypot
+v1     #x
+o0     #+
+v2     #y
+n1
+n2
+x1     #initial guess
+0 1    #z
+r      #1 ranges (rhs's)
+4 0    #c
+b      #3 bounds (on variables)
+3      #z
+1 3    #x
+2 3    #y
+k2     #intermediate Jacobian column lengths
+0
+1
+J0 2   #c
+1 1
+2 -1
+G0 3   #o
+0 0
+1 0
+2 0
+""",
+                OUT.getvalue(),
+            )
+        )
+
+        OUT = io.StringIO()
+        nl_writer.NLWriter().write(
+            m, OUT, symbolic_solver_labels=True, linear_presolve=True
+        )
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0       #problem unknown
+ 1 0 1 0 0     #vars, constraints, objectives, ranges, eqns
+ 0 1 0 0 0 0   #nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0   #network constraints: nonlinear, linear
+ 0 1 0 #nonlinear vars in constraints, objectives, both
+ 0 1 0 1       #linear network variables; functions; arith, flags
+ 0 0 0 0 0     #discrete variables: binary, integer, nonlinear (b,c,o)
+ 0 1   #nonzeros in Jacobian, obj. gradient
+ 1 1   #max name lengths: constraints, variables
+ 0 0 0 0 0     #common exprs: b,c,o,c1,o1
+F0 1 -1 gsl_hypot
+O0 0   #o
+o2     #*
+o5     #^
+v0     #z
+n2
+o5     #^
+f0 2   #hypot
+n3
+n4
+n2
+x1     #initial guess
+0 1    #z
+r      #0 ranges (rhs's)
+b      #1 bounds (on variables)
+3      #z
+k0     #intermediate Jacobian column lengths
+G0 1   #o
+0 0
+""",
+                OUT.getvalue(),
+            )
+        )
+
+    def test_presolve_defined_var_to_const(self):
+        # This test is derived from a step in an IDAES initialization
+        # where the presolver is able to fix enough variables to cause
+        # the defined variable to be reduced to a constant.  We must not
+        # emit the defined variable (because doing so generates an error
+        # in the ASL)
+        m = ConcreteModel()
+        m.eq = Var(initialize=100)
+        m.co2 = Var()
+        m.n2 = Var()
+        m.E = Expression(expr=60 / (3 * m.co2 - 4 * m.n2 - 5))
+        m.con1 = Constraint(expr=m.co2 == 6)
+        m.con2 = Constraint(expr=m.n2 == 7)
+        m.con3 = Constraint(expr=8 / m.E == m.eq)
+
+        OUT = io.StringIO()
+        nl_writer.NLWriter().write(
+            m, OUT, symbolic_solver_labels=True, linear_presolve=True
+        )
+        # Note that the presolve will end up recognizing con3 as a
+        # linear constraint; however, it does not do so until processing
+        # the constraints after presolve (so the constraint is not
+        # actually removed and the eq variable still appears in the model)
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0	#problem unknown
+ 1 1 0 0 1	#vars, constraints, objectives, ranges, eqns
+ 0 0 0 0 0 0	#nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0	#network constraints: nonlinear, linear
+ 0 0 0	#nonlinear vars in constraints, objectives, both
+ 0 0 0 1	#linear network variables; functions; arith, flags
+ 0 0 0 0 0	#discrete variables: binary, integer, nonlinear (b,c,o)
+ 1 0	#nonzeros in Jacobian, obj. gradient
+ 4 2	#max name lengths: constraints, variables
+ 0 0 0 0 0	#common exprs: b,c,o,c1,o1
+C0	#con3
+n0
+x1	#initial guess
+0 100	#eq
+r	#1 ranges (rhs's)
+4 2.0	#con3
+b	#1 bounds (on variables)
+3	#eq
+k0	#intermediate Jacobian column lengths
+J0 1	#con3
+0 -1
+""",
+                OUT.getvalue(),
+            )
+        )
+
+    def test_presolve_check_invalid_monomial_constraints(self):
+        # This checks issue #3272
+        m = ConcreteModel()
+        m.x = Var()
+        m.c = Constraint(expr=m.x == 5)
+        m.d = Constraint(expr=m.x >= 10)
+
+        OUT = io.StringIO()
+        with self.assertRaisesRegex(
+            nl_writer.InfeasibleConstraintException,
+            r"model contains a trivially infeasible constraint 'd' "
+            r"\(fixed body value 5.0 outside bounds \[10, None\]\)\.",
+        ):
+            nl_writer.NLWriter().write(m, OUT, linear_presolve=True)
```

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/ampl/test_suffixes.py` & `Pyomo-6.7.3/pyomo/repn/tests/ampl/test_suffixes.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/baron/__init__.py` & `Pyomo-6.7.3/pyomo/repn/tests/baron/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/baron/small14a_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/baron/small14a_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/baron/test_baron.py` & `Pyomo-6.7.3/pyomo/repn/tests/baron/test_baron.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/baron/test_baron_comparison.py` & `Pyomo-6.7.3/pyomo/repn/tests/baron/test_baron_comparison.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/cpxlp/__init__.py` & `Pyomo-6.7.3/pyomo/repn/tests/cpxlp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/cpxlp/test_cpxlp.py` & `Pyomo-6.7.3/pyomo/repn/tests/cpxlp/test_cpxlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/cpxlp/test_lpv2.py` & `Pyomo-6.7.3/pyomo/repn/tests/cpxlp/test_lpv2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/diffutils.py` & `Pyomo-6.7.3/pyomo/repn/tests/diffutils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/gams/__init__.py` & `Pyomo-6.7.3/pyomo/repn/tests/gams/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/gams/small14a_testCase.py` & `Pyomo-6.7.3/pyomo/repn/tests/gams/small14a_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/gams/test_gams.py` & `Pyomo-6.7.3/pyomo/repn/tests/gams/test_gams.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/gams/test_gams_comparison.py` & `Pyomo-6.7.3/pyomo/repn/tests/gams/test_gams_comparison.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/lp_diff.py` & `Pyomo-6.7.3/pyomo/repn/tests/lp_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/mps/__init__.py` & `Pyomo-6.7.3/pyomo/repn/tests/mps/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/mps/test_mps.py` & `Pyomo-6.7.3/pyomo/repn/tests/mps/test_mps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/nl_diff.py` & `Pyomo-6.7.3/pyomo/repn/tests/nl_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/test_linear.py` & `Pyomo-6.7.3/pyomo/repn/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/test_quadratic.py` & `Pyomo-6.7.3/pyomo/repn/tests/test_quadratic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/test_standard.py` & `Pyomo-6.7.3/pyomo/repn/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/test_standard_form.py` & `Pyomo-6.7.3/pyomo/repn/tests/test_standard_form.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/tests/test_util.py` & `Pyomo-6.7.3/pyomo/repn/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/repn/util.py` & `Pyomo-6.7.3/pyomo/repn/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/__init__.py` & `Pyomo-6.7.3/pyomo/scripting/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/commands.py` & `Pyomo-6.7.3/pyomo/scripting/commands.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/convert.py` & `Pyomo-6.7.3/pyomo/scripting/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/driver_help.py` & `Pyomo-6.7.3/pyomo/scripting/driver_help.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/interface.py` & `Pyomo-6.7.3/pyomo/scripting/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/scripting/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/plugins/build_ext.py` & `Pyomo-6.7.3/pyomo/scripting/plugins/build_ext.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/plugins/convert.py` & `Pyomo-6.7.3/pyomo/scripting/plugins/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/plugins/download.py` & `Pyomo-6.7.3/pyomo/scripting/plugins/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     def _call_impl(self, args, unparsed, logger):
         results = []
         result_fmt = "[%s]  %s"
         returncode = 0
         self.downloader.cacert = args.cacert
         self.downloader.insecure = args.insecure
         logger.info(
-            "As of February 9, 2023, AMPL GSL can no longer be downloaded\
-                    through download-extensions. Visit https://portal.ampl.com/\
-                    to download the AMPL GSL binaries."
+            "As of February 9, 2023, AMPL GSL can no longer be downloaded \
+            through download-extensions. Visit https://portal.ampl.com/ \
+            to download the AMPL GSL binaries."
         )
         for target in DownloadFactory:
             try:
                 ext = DownloadFactory(target, downloader=self.downloader)
                 if hasattr(ext, 'skip') and ext.skip():
                     result = 'SKIP'
                 elif hasattr(ext, '__call__'):
```

### Comparing `Pyomo-6.7.2/pyomo/scripting/plugins/extras.py` & `Pyomo-6.7.3/pyomo/scripting/plugins/extras.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/plugins/solve.py` & `Pyomo-6.7.3/pyomo/scripting/plugins/solve.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/pyomo_command.py` & `Pyomo-6.7.3/pyomo/scripting/pyomo_command.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/pyomo_main.py` & `Pyomo-6.7.3/pyomo/scripting/pyomo_main.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/pyomo_parser.py` & `Pyomo-6.7.3/pyomo/scripting/pyomo_parser.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/solve_config.py` & `Pyomo-6.7.3/pyomo/scripting/solve_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/tests/__init__.py` & `Pyomo-6.7.3/pyomo/scripting/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/tests/test_cmds.py` & `Pyomo-6.7.3/pyomo/scripting/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/scripting/util.py` & `Pyomo-6.7.3/pyomo/scripting/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/amplfunc_merge.py` & `Pyomo-6.7.3/pyomo/solvers/amplfunc_merge.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/mockmip.py` & `Pyomo-6.7.3/pyomo/solvers/mockmip.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/converter/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/converter/ampl.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/converter/ampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/converter/glpsol.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/converter/glpsol.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/converter/model.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/converter/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/converter/pico.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/converter/pico.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/ASL.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/ASL.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/BARON.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/BARON.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/CBCplugin.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/CBCplugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -451,15 +451,15 @@
         gap = None
         nodes = None
         # See https://www.coin-or.org/Cbc/cbcuserguide.html#messages
         for line in output.split("\n"):
             tokens = tuple(re.split('[ \t]+', line.strip()))
             n_tokens = len(tokens)
             if n_tokens > 1:
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L3769
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L3769
                 if n_tokens > 4 and tokens[:4] == (
                     'Continuous',
                     'objective',
                     'value',
                     'is',
                 ):
                     lower_bound = _float(tokens[4])
@@ -535,39 +535,39 @@
                             results.problem.name = '.'.join(parts[:-1])
                         else:
                             results.problem.name = results.problem.name.split('.')[0]
                     if '/' in results.problem.name:
                         results.problem.name = results.problem.name.split('/')[-1]
                     if '\\' in results.problem.name:
                         results.problem.name = results.problem.name.split('\\')[-1]
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L10840
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L10840
                 elif tokens[0] == 'Presolve':
                     if n_tokens > 9 and tokens[3] == 'rows,' and tokens[6] == 'columns':
                         results.problem.number_of_variables = int(tokens[4]) - int(
                             tokens[5][1:-1]
                         )
                         results.problem.number_of_constraints = int(tokens[1]) - int(
                             tokens[2][1:-1]
                         )
                         results.problem.number_of_objectives = 1
                     elif n_tokens > 6 and tokens[6] == 'infeasible':
                         soln.status = SolutionStatus.infeasible
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L11105
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L11105
                 elif (
                     n_tokens > 11
                     and tokens[:2] == ('Problem', 'has')
                     and tokens[3] == 'rows,'
                     and tokens[5] == 'columns'
                     and tokens[7:9] == ('with', 'objective)')
                 ):
                     results.problem.number_of_variables = int(tokens[4])
                     results.problem.number_of_constraints = int(tokens[2])
                     results.problem.number_of_nonzeros = int(tokens[6][1:])
                     results.problem.number_of_objectives = 1
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L10814
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L10814
                 elif (
                     n_tokens > 8
                     and tokens[:3] == ('Original', 'problem', 'has')
                     and tokens[4] == 'integers'
                     and tokens[6:9] == ('of', 'which', 'binary)')
                 ):
                     results.problem.number_of_integer_variables = int(tokens[3])
@@ -575,15 +575,15 @@
                 elif n_tokens == 5 and tokens[3] == "NAME":
                     results.problem.name = tokens[4]
                 elif (
                     'CoinLpIO::readLp(): Maximization problem reformulated as minimization'
                     in ' '.join(tokens)
                 ):
                     results.problem.sense = maximize
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L3047
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L3047
                 elif n_tokens > 3 and tokens[:2] == ('Result', '-'):
                     if tokens[2:4] in [('Run', 'abandoned'), ('User', 'ctrl-c')]:
                         results.solver.termination_condition = (
                             TerminationCondition.userInterrupt
                         )
                     if n_tokens > 4:
                         if tokens[2:5] == ('Optimal', 'solution', 'found'):
@@ -605,54 +605,54 @@
                         ):
                             results.solver.termination_condition = {
                                 'node': TerminationCondition.maxEvaluations,
                                 'time': TerminationCondition.maxTimeLimit,
                                 'solution': TerminationCondition.other,
                                 'iterations': TerminationCondition.maxIterations,
                             }.get(tokens[4], TerminationCondition.other)
-                    # perhaps from https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L12318
+                    # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L12318
                     elif n_tokens > 3 and tokens[2] == "Finished":
                         soln.status = SolutionStatus.optimal
                         optim_value = _float(tokens[4])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7904
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7904
                 elif n_tokens >= 3 and tokens[:2] == ('Objective', 'value:'):
                     # parser for log file generetated with discrete variable
                     optim_value = _float(tokens[2])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7904
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7904
                 elif n_tokens >= 4 and tokens[:4] == (
                     'No',
                     'feasible',
                     'solution',
                     'found',
                 ):
                     soln.status = SolutionStatus.infeasible
                 elif n_tokens > 2 and tokens[:2] == ('Lower', 'bound:'):
                     if (
                         lower_bound is None
                     ):  # Only use if not already found since this is to less decimal places
                         results.problem.lower_bound = _float(tokens[2])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7918
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7918
                 elif tokens[0] == 'Gap:':
                     # This is relative and only to 2 decimal places - could calculate explicitly using lower bound
                     gap = _float(tokens[1])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7923
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7923
                 elif n_tokens > 2 and tokens[:2] == ('Enumerated', 'nodes:'):
                     nodes = int(tokens[2])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7926
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7926
                 elif n_tokens > 2 and tokens[:2] == ('Total', 'iterations:'):
                     results.solver.statistics.black_box.number_of_iterations = int(
                         tokens[2]
                     )
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7930
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7930
                 elif n_tokens > 3 and tokens[:3] == ('Time', '(CPU', 'seconds):'):
                     results.solver.system_time = _float(tokens[3])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L7933
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L7933
                 elif n_tokens > 3 and tokens[:3] == ('Time', '(Wallclock', 'Seconds):'):
                     results.solver.wallclock_time = _float(tokens[3])
-                # https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp?rev=2497#L10477
+                # https://github.com/coin-or/Cbc/blob/cb6bf98/Cbc/src/CbcSolver.cpp#L10477
                 elif n_tokens > 4 and tokens[:4] == (
                     'Total',
                     'time',
                     '(CPU',
                     'seconds):',
                 ):
                     results.solver.system_time = _float(tokens[4])
@@ -828,19 +828,23 @@
             _ver and _ver[:3] < (2, 10, 2)
         )
 
         for line in INPUT:
             tokens = tuple(re.split('[ \t]+', line.strip()))
             n_tokens = len(tokens)
             #
-            # These are the only header entries CBC will generate (identified via browsing CbcSolver.cpp)
-            # See https://projects.coin-or.org/Cbc/browser/trunk/Cbc/src/CbcSolver.cpp
-            # Search for (no integer solution - continuous used)      Currently line 9912 as of rev2497
-            # Note that since this possibly also covers old CBC versions, we shall not be removing any functionality,
-            # even if it is not seen in the current revision
+            # These are the only header entries CBC will generate
+            # (identified via browsing CbcSolver.cpp).  See
+            #     https://github.com/coin-or/Cbc/tree/master/src/CbcSolver.cpp
+            # Search for "(no integer solution - continuous used)"
+            # (L10796 as of cb855c7)
+            #
+            # Note that since this possibly also supports old CBC
+            # versions, we shall not be removing any functionality, even
+            # if it is not seen in the current revision
             #
             if not header_processed:
                 if tokens[0] == 'Optimal':
                     results.solver.termination_condition = TerminationCondition.optimal
                     results.solver.status = SolverStatus.ok
                     results.solver.termination_message = (
                         "Model was solved to optimality (subject to tolerances), "
```

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/CONOPT.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/CONOPT.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/CPLEX.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/CPLEX.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GAMS.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GAMS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GLPK.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GLPK.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GUROBI.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GUROBI.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/GUROBI_RUN.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/GUROBI_RUN.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/IPOPT.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/IPOPT.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/SCIPAMPL.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/SCIPAMPL.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/XPRESS.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/XPRESS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/cplex_direct.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/cplex_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/cplex_persistent.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/cplex_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/direct_solver.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/direct_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/gurobi_direct.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/gurobi_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/gurobi_persistent.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/gurobi_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/mosek_direct.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/mosek_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/mosek_persistent.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/mosek_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/persistent_solver.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/persistent_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/pywrapper.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/pywrapper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/xpress_direct.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/xpress_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/plugins/solvers/xpress_persistent.py` & `Pyomo-6.7.3/pyomo/solvers/plugins/solvers/xpress_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_BARON.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_BARON.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_CBCplugin.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_CBCplugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_CPLEXDirect.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_CPLEXDirect.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_CPLEXPersistent.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_CPLEXPersistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_GAMS.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_GAMS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_MOSEKDirect.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_MOSEKDirect.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_MOSEKPersistent.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_MOSEKPersistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_amplfunc_merge.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_amplfunc_merge.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_cbc.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_cbc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_cplex.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_cplex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_gurobi.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_gurobi_direct.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_gurobi_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_gurobi_persistent.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_gurobi_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_no_solution_behavior.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_no_solution_behavior.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_pickle.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_pickle.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_writers.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_writers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/checks/test_xpress_persistent.py` & `Pyomo-6.7.3/pyomo/solvers/tests/checks/test_xpress_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/model.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_asl.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_asl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_convert.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_factory.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_ipopt.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_mip.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_mip.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_qp.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_qp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_scip.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_scip.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_scip_log_data.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_scip_log_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_scip_version.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_scip_version.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/mip/test_solver.py` & `Pyomo-6.7.3/pyomo/solvers/tests/mip/test_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_block.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_compiled.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_compiled.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_constant_objective1.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_constant_objective1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_constant_objective2.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_constant_objective2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_duals_maximize.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_duals_maximize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_duals_minimize.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_duals_minimize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_inactive_index.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_inactive_index.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_infeasible1.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_infeasible1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_infeasible2.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_infeasible2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_piecewise.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_trivial_constraints.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_trivial_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_unbounded.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_unbounded.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_unique_duals.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_unique_duals.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/LP_unused_vars.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/LP_unused_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_infeasible1.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_infeasible1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_unbounded.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_unbounded.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MILP_unused_vars.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MILP_unused_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MIQCP_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MIQCP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/MIQP_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/MIQP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/QCP_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/QCP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/QP_constant_objective.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/QP_constant_objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/QP_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/QP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/SOS1_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/SOS1_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/SOS2_simple.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/SOS2_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/models/base.py` & `Pyomo-6.7.3/pyomo/solvers/tests/models/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/__init__.py` & `Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/test_examples.py` & `Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py` & `Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py` & `Pyomo-6.7.3/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/solvers.py` & `Pyomo-6.7.3/pyomo/solvers/tests/solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/tests/testcases.py` & `Pyomo-6.7.3/pyomo/solvers/tests/testcases.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/solvers/wrappers.py` & `Pyomo-6.7.3/pyomo/solvers/wrappers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/__init__.py` & `Pyomo-6.7.3/pyomo/util/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/blockutil.py` & `Pyomo-6.7.3/pyomo/util/blockutil.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/calc_var_value.py` & `Pyomo-6.7.3/pyomo/util/calc_var_value.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/check_units.py` & `Pyomo-6.7.3/pyomo/util/check_units.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/components.py` & `Pyomo-6.7.3/pyomo/util/components.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/diagnostics.py` & `Pyomo-6.7.3/pyomo/util/diagnostics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/infeasible.py` & `Pyomo-6.7.3/pyomo/util/infeasible.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/model_size.py` & `Pyomo-6.7.3/pyomo/util/model_size.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/report_scaling.py` & `Pyomo-6.7.3/pyomo/util/report_scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/slices.py` & `Pyomo-6.7.3/pyomo/util/slices.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/subsystems.py` & `Pyomo-6.7.3/pyomo/util/subsystems.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/__init__.py` & `Pyomo-6.7.3/pyomo/util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_blockutil.py` & `Pyomo-6.7.3/pyomo/util/tests/test_blockutil.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_calc_var_value.py` & `Pyomo-6.7.3/pyomo/util/tests/test_calc_var_value.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_check_units.py` & `Pyomo-6.7.3/pyomo/util/tests/test_check_units.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_components.py` & `Pyomo-6.7.3/pyomo/util/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_infeasible.py` & `Pyomo-6.7.3/pyomo/util/tests/test_infeasible.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_model_size.py` & `Pyomo-6.7.3/pyomo/util/tests/test_model_size.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_report_scaling.py` & `Pyomo-6.7.3/pyomo/util/tests/test_report_scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_slices.py` & `Pyomo-6.7.3/pyomo/util/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/tests/test_subsystems.py` & `Pyomo-6.7.3/pyomo/util/tests/test_subsystems.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/util/vars_from_expressions.py` & `Pyomo-6.7.3/pyomo/util/vars_from_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/version/__init__.py` & `Pyomo-6.7.3/pyomo/version/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/version/info.py` & `Pyomo-6.7.3/pyomo/version/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 # The VOTD zipbuilder will automatically change releaselevel to "VOTD
 # {hash}" and set the serial number to YYMMDDhhmm.  The serial number
 # should generally be left at 0, unless a downstream package is tracking
 # main and needs a hard reference to "suitably new" development.
 major = 6
 minor = 7
-micro = 2
+micro = 3
 # releaselevel = 'invalid'
 releaselevel = 'final'
 serial = 0
 
 if releaselevel == 'final':
     pass
 elif '/tags/' in _init_url:  # pragma:nocover
```

### Comparing `Pyomo-6.7.2/pyomo/version/tests/__init__.py` & `Pyomo-6.7.3/pyomo/version/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/version/tests/check.py` & `Pyomo-6.7.3/pyomo/version/tests/check.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/pyomo/version/tests/test_version.py` & `Pyomo-6.7.3/pyomo/version/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/setup.cfg` & `Pyomo-6.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `Pyomo-6.7.2/setup.py` & `Pyomo-6.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,17 @@
             'scipy',  # Needed by autodoc for pynumero
         ],
         'optional': [
             'dill',  # No direct use, but improves lambda pickle
             'ipython',  # contrib.viewer
             # Note: matplotlib 3.6.1 has bug #24127, which breaks
             # seaborn's histplot (triggering parmest failures)
-            'matplotlib!=3.6.1',
+            # Note: minimum version from community_detection use of
+            # matplotlib.pyplot.get_cmap()
+            'matplotlib>=3.6.0,!=3.6.1',
             # network, incidence_analysis, community_detection
             # Note: networkx 3.2 is Python>-3.9, but there is a broken
             # 3.2 package on conda-forge that will get implicitly
             # installed on python 3.8
             'networkx<3.2; python_version<"3.9"',
             'networkx; python_version>="3.9"',
             'numpy<2.0.0',
```

