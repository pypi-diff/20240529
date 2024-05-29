# Comparing `tmp/libbs-1.5.1.tar.gz` & `tmp/libbs-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.5.1.tar", last modified: Thu May 16 19:40:22 2024, max compression
+gzip compressed data, was "libbs-1.5.2.tar", last modified: Wed May 29 21:20:55 2024, max compression
```

## Comparing `libbs-1.5.1.tar` & `libbs-1.5.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.965549 libbs-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-16 19:40:19.000000 libbs-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 19:40:22.965549 libbs-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-16 19:40:19.000000 libbs-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.953548 libbs-1.5.1/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.957548 libbs-1.5.1/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.957548 libbs-1.5.1/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.957548 libbs-1.5.1/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.957548 libbs-1.5.1/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.957548 libbs-1.5.1/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.961549 libbs-1.5.1/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.965549 libbs-1.5.1/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32864 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.965549 libbs-1.5.1/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.965549 libbs-1.5.1/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-16 19:40:19.000000 libbs-1.5.1/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.965549 libbs-1.5.1/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 19:40:22.000000 libbs-1.5.1/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-16 19:40:22.000000 libbs-1.5.1/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:40:22.000000 libbs-1.5.1/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 19:40:22.000000 libbs-1.5.1/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 19:40:22.000000 libbs-1.5.1/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:40:22.000000 libbs-1.5.1/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-16 19:40:22.965549 libbs-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 19:40:19.000000 libbs-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:40:22.965549 libbs-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-16 19:40:19.000000 libbs-1.5.1/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-16 19:40:19.000000 libbs-1.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-16 19:40:19.000000 libbs-1.5.1/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-29 21:20:51.000000 libbs-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:20:55.293996 libbs-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-29 21:20:51.000000 libbs-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.281996 libbs-1.5.2/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32864 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 21:20:55.293996 libbs-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 21:20:51.000000 libbs-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-29 21:20:51.000000 libbs-1.5.2/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-29 21:20:51.000000 libbs-1.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-29 21:20:51.000000 libbs-1.5.2/tests/test_decompilers.py
```

### Comparing `libbs-1.5.1/LICENSE` & `libbs-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/PKG-INFO` & `libbs-1.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.5.1
+Version: 1.5.2
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -30,18 +30,16 @@
 for all BinSync based plugins.
 
 ## Install
 ```bash
 pip install libbs
 ```
 
-The minimum Python version is **3.8**.
-
-You can optionally also do `libbs --install` after to install generic plugins, but it's not required, since `libbs` 
-files will be installed with plugins that use it. 
+The minimum Python version is **3.8**. **If you plan on using libbs alone (without installing some other plugin), 
+you must do `libbs --install` after pip install**. This will copy the appropriate files to your decompiler. 
 
 ## Usage
 LibBS exposes all decompiler API through the abstract class `DecompilerInterface`. The `DecompilerInterface` 
 can be used in either the default mode, which assumes a GUI, or `headless` mode. In `headless` mode, the interface will 
 start a new process using a specified decompiler.
 
 You can find various examples using LibBS in the [examples](./examples) folder. Examples that are plugins show off
```

### Comparing `libbs-1.5.1/README.md` & `libbs-1.5.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 for all BinSync based plugins.
 
 ## Install
 ```bash
 pip install libbs
 ```
 
-The minimum Python version is **3.8**.
-
-You can optionally also do `libbs --install` after to install generic plugins, but it's not required, since `libbs` 
-files will be installed with plugins that use it. 
+The minimum Python version is **3.8**. **If you plan on using libbs alone (without installing some other plugin), 
+you must do `libbs --install` after pip install**. This will copy the appropriate files to your decompiler. 
 
 ## Usage
 LibBS exposes all decompiler API through the abstract class `DecompilerInterface`. The `DecompilerInterface` 
 can be used in either the default mode, which assumes a GUI, or `headless` mode. In `headless` mode, the interface will 
 start a new process using a specified decompiler.
 
 You can find various examples using LibBS in the [examples](./examples) folder. Examples that are plugins show off
```

### Comparing `libbs-1.5.1/libbs/__main__.py` & `libbs-1.5.2/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/api/artifact_dict.py` & `libbs-1.5.2/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/api/artifact_lifter.py` & `libbs-1.5.2/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/api/decompiler_interface.py` & `libbs-1.5.2/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/api/type_parser.py` & `libbs-1.5.2/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/api/utils.py` & `libbs-1.5.2/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/__init__.py` & `libbs-1.5.2/libbs/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/artifact.py` & `libbs-1.5.2/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/comment.py` & `libbs-1.5.2/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/decompilation.py` & `libbs-1.5.2/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/enum.py` & `libbs-1.5.2/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/func.py` & `libbs-1.5.2/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/global_variable.py` & `libbs-1.5.2/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/patch.py` & `libbs-1.5.2/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/stack_variable.py` & `libbs-1.5.2/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/artifacts/struct.py` & `libbs-1.5.2/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import subprocess
 import sys
-from jfx_bridge import bridge
-from ghidra_bridge_port import DEFAULT_SERVER_PORT
+from .jfx_bridge import bridge
+from .ghidra_bridge_port import DEFAULT_SERVER_PORT
 
 # NOTE: we definitely DON'T want to exclude ghidra from ghidra_bridge :P
 import ghidra
 
 
 class GhidraBridgeServer(object):
     """ Class mostly used to collect together functions and variables that we don't want contaminating the global namespace
```

### Comparing `libbs-1.5.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.5.2/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/angr/compat.py` & `libbs-1.5.2/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/angr/interface.py` & `libbs-1.5.2/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.5.2/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/binja/hooks.py` & `libbs-1.5.2/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/binja/interface.py` & `libbs-1.5.2/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.5.2/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.5.2/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ghidra/hooks.py` & `libbs-1.5.2/libbs/decompilers/ghidra/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ghidra/interface.py` & `libbs-1.5.2/libbs/decompilers/ghidra/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.5.2/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ida/compat.py` & `libbs-1.5.2/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ida/hooks.py` & `libbs-1.5.2/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/decompilers/ida/interface.py` & `libbs-1.5.2/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/logger.py` & `libbs-1.5.2/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/plugin_installer.py` & `libbs-1.5.2/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/ui/__init__.py` & `libbs-1.5.2/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/ui/qt_objects.py` & `libbs-1.5.2/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs/ui/utils.py` & `libbs-1.5.2/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/libbs.egg-info/PKG-INFO` & `libbs-1.5.2/libbs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.5.1
+Version: 1.5.2
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -30,18 +30,16 @@
 for all BinSync based plugins.
 
 ## Install
 ```bash
 pip install libbs
 ```
 
-The minimum Python version is **3.8**.
-
-You can optionally also do `libbs --install` after to install generic plugins, but it's not required, since `libbs` 
-files will be installed with plugins that use it. 
+The minimum Python version is **3.8**. **If you plan on using libbs alone (without installing some other plugin), 
+you must do `libbs --install` after pip install**. This will copy the appropriate files to your decompiler. 
 
 ## Usage
 LibBS exposes all decompiler API through the abstract class `DecompilerInterface`. The `DecompilerInterface` 
 can be used in either the default mode, which assumes a GUI, or `headless` mode. In `headless` mode, the interface will 
 start a new process using a specified decompiler.
 
 You can find various examples using LibBS in the [examples](./examples) folder. Examples that are plugins show off
```

### Comparing `libbs-1.5.1/libbs.egg-info/SOURCES.txt` & `libbs-1.5.2/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/setup.cfg` & `libbs-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/tests/test_artifacts.py` & `libbs-1.5.2/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/tests/test_cli.py` & `libbs-1.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.1/tests/test_decompilers.py` & `libbs-1.5.2/tests/test_decompilers.py`

 * *Files identical despite different names*

