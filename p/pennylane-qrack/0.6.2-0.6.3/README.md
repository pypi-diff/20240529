# Comparing `tmp/pennylane_qrack-0.6.2.tar.gz` & `tmp/pennylane_qrack-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane_qrack-0.6.2.tar", last modified: Sun May 26 15:20:44 2024, max compression
+gzip compressed data, was "pennylane_qrack-0.6.3.tar", last modified: Wed May 29 19:16:11 2024, max compression
```

## Comparing `pennylane_qrack-0.6.2.tar` & `pennylane_qrack-0.6.3.tar`

### file list

```diff
@@ -1,59 +1,35 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.175918 pennylane_qrack-0.6.2/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     4189 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/CHANGELOG.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      507 2024-05-24 10:23:28.000000 pennylane_qrack-0.6.2/CMakeLists.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1335 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/Makefile
--rw-r--r--   0 iamu      (1000) iamu      (1000)     4563 2024-05-26 15:20:44.175918 pennylane_qrack-0.6.2/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3364 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/README.rst
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.169917 pennylane_qrack-0.6.2/_skbuild/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.169917 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.171918 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     4189 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/CHANGELOG.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      507 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/CMakeLists.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1335 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/Makefile
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3364 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/README.rst
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.169917 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.169917 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.169917 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/lib/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.169917 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/lib/backend/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.171918 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/lib/backend/common/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     6135 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/lib/backend/common/CacheManager.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     4596 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/lib/backend/common/QubitManager.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    13170 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/catalyst/runtime/lib/backend/common/Utils.hpp
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.173918 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     6144 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/QrackDeviceConfig.toml
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/_version.py
--rw-r--r--   0 iamu      (1000) iamu      (1000)  4159848 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/libqrack_device.so
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    39277 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/qrack_device.cpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    22662 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/qrack_device.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       57 2024-05-26 15:20:41.000000 pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/requirements.txt
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.170918 pennylane_qrack-0.6.2/catalyst/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.170918 pennylane_qrack-0.6.2/catalyst/runtime/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.170918 pennylane_qrack-0.6.2/catalyst/runtime/lib/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.170918 pennylane_qrack-0.6.2/catalyst/runtime/lib/backend/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.174918 pennylane_qrack-0.6.2/catalyst/runtime/lib/backend/common/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     6135 2024-05-26 15:06:28.000000 pennylane_qrack-0.6.2/catalyst/runtime/lib/backend/common/CacheManager.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     4596 2024-05-26 15:06:28.000000 pennylane_qrack-0.6.2/catalyst/runtime/lib/backend/common/QubitManager.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    13170 2024-05-26 15:06:28.000000 pennylane_qrack-0.6.2/catalyst/runtime/lib/backend/common/Utils.hpp
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.174918 pennylane_qrack-0.6.2/pennylane_qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     6144 2024-05-25 13:36:03.000000 pennylane_qrack-0.6.2/pennylane_qrack/QrackDeviceConfig.toml
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/pennylane_qrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2024-05-26 15:15:01.000000 pennylane_qrack-0.6.2/pennylane_qrack/_version.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    39277 2024-05-26 14:47:58.000000 pennylane_qrack-0.6.2/pennylane_qrack/qrack_device.cpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    22662 2024-05-26 14:30:40.000000 pennylane_qrack-0.6.2/pennylane_qrack/qrack_device.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.175918 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/
--rw-r--r--   0 iamu      (1000) iamu      (1000)     4563 2024-05-26 15:20:44.000000 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1730 2024-05-26 15:20:44.000000 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-05-26 15:20:44.000000 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       79 2024-05-26 15:20:44.000000 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/entry_points.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       64 2024-05-26 15:20:44.000000 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       16 2024-05-26 15:20:44.000000 pennylane_qrack-0.6.2/pennylane_qrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       57 2024-05-24 10:23:28.000000 pennylane_qrack-0.6.2/requirements.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-05-26 15:20:44.175918 pennylane_qrack-0.6.2/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2401 2024-05-25 17:54:38.000000 pennylane_qrack-0.6.2/setup.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:20:44.175918 pennylane_qrack-0.6.2/tests/
--rwxrwxr-x   0 iamu      (1000) iamu      (1000)    17655 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/tests/test_apply.py
--rwxrwxr-x   0 iamu      (1000) iamu      (1000)     1715 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/tests/test_integration.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3783 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.2/tests/test_units.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.982662 pennylane_qrack-0.6.3/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     4189 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.3/CHANGELOG.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      898 2024-05-29 19:12:58.000000 pennylane_qrack-0.6.3/CMakeLists.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2024-05-28 19:56:38.000000 pennylane_qrack-0.6.3/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1335 2024-05-28 19:56:38.000000 pennylane_qrack-0.6.3/Makefile
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     5775 2024-05-29 19:16:11.982662 pennylane_qrack-0.6.3/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     4576 2024-05-29 19:13:00.000000 pennylane_qrack-0.6.3/README.rst
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.979662 pennylane_qrack-0.6.3/catalyst/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.979662 pennylane_qrack-0.6.3/catalyst/runtime/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.980662 pennylane_qrack-0.6.3/catalyst/runtime/include/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     5069 2024-05-29 16:48:23.000000 pennylane_qrack-0.6.3/catalyst/runtime/include/DataView.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2919 2024-05-29 16:48:23.000000 pennylane_qrack-0.6.3/catalyst/runtime/include/Exception.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11733 2024-05-29 16:48:23.000000 pennylane_qrack-0.6.3/catalyst/runtime/include/QuantumDevice.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     5187 2024-05-29 16:48:23.000000 pennylane_qrack-0.6.3/catalyst/runtime/include/RuntimeCAPI.h
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3354 2024-05-29 16:48:23.000000 pennylane_qrack-0.6.3/catalyst/runtime/include/Types.h
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.981662 pennylane_qrack-0.6.3/pennylane_qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     6144 2024-05-25 13:36:03.000000 pennylane_qrack-0.6.3/pennylane_qrack/QrackDeviceConfig.toml
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.3/pennylane_qrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2024-05-29 19:15:49.000000 pennylane_qrack-0.6.3/pennylane_qrack/_version.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    39277 2024-05-26 14:47:58.000000 pennylane_qrack-0.6.3/pennylane_qrack/qrack_device.cpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    25186 2024-05-29 19:12:58.000000 pennylane_qrack-0.6.3/pennylane_qrack/qrack_device.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.982662 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     5775 2024-05-29 19:16:11.000000 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      735 2024-05-29 19:16:11.000000 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-05-29 19:16:11.000000 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       79 2024-05-29 19:16:11.000000 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/entry_points.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       64 2024-05-29 19:16:11.000000 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       16 2024-05-29 19:16:11.000000 pennylane_qrack-0.6.3/pennylane_qrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       57 2024-05-24 10:23:28.000000 pennylane_qrack-0.6.3/requirements.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-05-29 19:16:11.982662 pennylane_qrack-0.6.3/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2434 2024-05-29 19:12:58.000000 pennylane_qrack-0.6.3/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-29 19:16:11.982662 pennylane_qrack-0.6.3/tests/
+-rwxrwxr-x   0 iamu      (1000) iamu      (1000)    18234 2024-05-29 19:12:58.000000 pennylane_qrack-0.6.3/tests/test_apply.py
+-rwxrwxr-x   0 iamu      (1000) iamu      (1000)     1747 2024-05-28 11:59:09.000000 pennylane_qrack-0.6.3/tests/test_integration.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2978 2024-05-29 19:12:58.000000 pennylane_qrack-0.6.3/tests/test_units.py
```

### Comparing `pennylane_qrack-0.6.2/CHANGELOG.md` & `pennylane_qrack-0.6.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.2/LICENSE` & `pennylane_qrack-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.2/Makefile` & `pennylane_qrack-0.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.2/PKG-INFO` & `pennylane_qrack-0.6.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qrack
-Version: 0.6.2
+Version: 0.6.3
 Summary: PennyLane plugin for Qrack.
 Home-page: http://github.com/vm6502q
 Maintainer: vm6502q
 Maintainer-email: stranoj@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -35,41 +35,58 @@
 
 The PennyLane-Qrack plugin integrates the Qrack quantum computing framework with PennyLane's quantum machine learning capabilities.
 
 This plugin is addapted from the `PennyLane-Qulacs plugin, <https://github.com/PennyLaneAI/pennylane-qulacs>`__ under the Apache License 2.0, with many thanks to the original developers!
 
 `PennyLane <https://pennylane.readthedocs.io>`__ is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
-`vm6502q/qrack <https://github.com/vm6502q>`__ is a software library for quantum computing, written in C++ and with GPU support.
+`unitaryfund/qrack <https://github.com/unitaryfund/qrack>`__ (formerly **vm6502q/qrack**) is a software library for quantum computing, written in C++ and with GPU support.
 
 Features
 ========
 
 * Provides access to a PyQrack simulator backend via the ``qrack.simulator`` device
+* Provides access to a (C++) Qrack simulator backend for Catalyst (also) via the ``qrack.simulator`` device
 
 Installation
 ============
 
-This plugin requires Python version 3.6 or above, as well as PennyLane. Installation of this plugin, as well as all dependencies, can be done using ``pip``:
+This plugin requires Python version 3.6 or above, as well as PennyLane and the Qrack library.
+
+You can choose to go the `releases <https://github.com/unitaryfund/qrack/releases>`__ page of Qrack to download a packaged artifact for your system and **install it in your system directories** (like `/usr` or `/usr/local` on Linux and UNIX based systems, including Mac), **or** you can opt to **build and install from source**, which might be easier, and this gives you maximum control over build configurations, like choice of CUDA over OpenCL GPU acceleration!
+
+See the Qrack README and documentation for the many build options of qrack, but, after checking out the Qrack repository and entering its root folder, this might be the best and simplest way to build and install Qrack:
+
+.. code-block:: bash
+
+    $ mkdir _build
+    $ cd _build
+    $ cmake -DCPP_STD=14 ..
+    $ make all -j$(nproc --all)
+    $ sudo make install
+
+After installing Qrack, installation of this plugin as well as all its Python dependencies can be done using ``pip`` (or ``pip3``, as appropriate):
 
 .. code-block:: bash
 
-    $ pip install pennylane-qrack
+    $ pip3 install pennylane-qrack
 
 Dependencies
 ~~~~~~~~~~~~
 
 PennyLane-Qrack requires the following libraries be installed:
 
 * `Python <http://python.org/>`__ >= 3.8
+* `Qrack <https://github.com/unitaryfund/qrack>`__ >= 9.0
 
 as well as the following Python packages:
 
 * `PennyLane <http://pennylane.readthedocs.io/>`__ >= 0.32
-* `PyQrack <https://github.com/vm6502q/pyqrack>`__  >= 0.13.0
+* `Catalyst <https://docs.pennylane.ai/projects/catalyst/en/stable/index.html>`__ >= 0.6
+* `PyQrack <https://github.com/vm6502q/pyqrack>`__  >= 1.28.0
 
 
 If you currently do not have Python 3 installed, we recommend
 `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed version of Python packaged
 for scientific computation.
```

### Comparing `pennylane_qrack-0.6.2/README.rst` & `pennylane_qrack-0.6.3/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -3,41 +3,58 @@
 
 The PennyLane-Qrack plugin integrates the Qrack quantum computing framework with PennyLane's quantum machine learning capabilities.
 
 This plugin is addapted from the `PennyLane-Qulacs plugin, <https://github.com/PennyLaneAI/pennylane-qulacs>`__ under the Apache License 2.0, with many thanks to the original developers!
 
 `PennyLane <https://pennylane.readthedocs.io>`__ is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
-`vm6502q/qrack <https://github.com/vm6502q>`__ is a software library for quantum computing, written in C++ and with GPU support.
+`unitaryfund/qrack <https://github.com/unitaryfund/qrack>`__ (formerly **vm6502q/qrack**) is a software library for quantum computing, written in C++ and with GPU support.
 
 Features
 ========
 
 * Provides access to a PyQrack simulator backend via the ``qrack.simulator`` device
+* Provides access to a (C++) Qrack simulator backend for Catalyst (also) via the ``qrack.simulator`` device
 
 Installation
 ============
 
-This plugin requires Python version 3.6 or above, as well as PennyLane. Installation of this plugin, as well as all dependencies, can be done using ``pip``:
+This plugin requires Python version 3.6 or above, as well as PennyLane and the Qrack library.
+
+You can choose to go the `releases <https://github.com/unitaryfund/qrack/releases>`__ page of Qrack to download a packaged artifact for your system and **install it in your system directories** (like `/usr` or `/usr/local` on Linux and UNIX based systems, including Mac), **or** you can opt to **build and install from source**, which might be easier, and this gives you maximum control over build configurations, like choice of CUDA over OpenCL GPU acceleration!
+
+See the Qrack README and documentation for the many build options of qrack, but, after checking out the Qrack repository and entering its root folder, this might be the best and simplest way to build and install Qrack:
+
+.. code-block:: bash
+
+    $ mkdir _build
+    $ cd _build
+    $ cmake -DCPP_STD=14 ..
+    $ make all -j$(nproc --all)
+    $ sudo make install
+
+After installing Qrack, installation of this plugin as well as all its Python dependencies can be done using ``pip`` (or ``pip3``, as appropriate):
 
 .. code-block:: bash
 
-    $ pip install pennylane-qrack
+    $ pip3 install pennylane-qrack
 
 Dependencies
 ~~~~~~~~~~~~
 
 PennyLane-Qrack requires the following libraries be installed:
 
 * `Python <http://python.org/>`__ >= 3.8
+* `Qrack <https://github.com/unitaryfund/qrack>`__ >= 9.0
 
 as well as the following Python packages:
 
 * `PennyLane <http://pennylane.readthedocs.io/>`__ >= 0.32
-* `PyQrack <https://github.com/vm6502q/pyqrack>`__  >= 0.13.0
+* `Catalyst <https://docs.pennylane.ai/projects/catalyst/en/stable/index.html>`__ >= 0.6
+* `PyQrack <https://github.com/vm6502q/pyqrack>`__  >= 1.28.0
 
 
 If you currently do not have Python 3 installed, we recommend
 `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed version of Python packaged
 for scientific computation.
```

### Comparing `pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/QrackDeviceConfig.toml` & `pennylane_qrack-0.6.3/pennylane_qrack/QrackDeviceConfig.toml`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/__init__.py` & `pennylane_qrack-0.6.3/pennylane_qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/_version.py` & `pennylane_qrack-0.6.3/pennylane_qrack/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
```

### Comparing `pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/qrack_device.cpp` & `pennylane_qrack-0.6.3/pennylane_qrack/qrack_device.cpp`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.2/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/qrack_device.py` & `pennylane_qrack-0.6.3/pennylane_qrack/qrack_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,32 @@
 import pathlib
 import sys
 import itertools as it
 
 import numpy as np
 
 from pennylane import QubitDevice, DeviceError
-from pennylane.ops import QubitStateVector, BasisState, QubitUnitary, CRZ, PhaseShift, Adjoint
+from pennylane.ops import (
+    QubitStateVector,
+    BasisState,
+    QubitUnitary,
+    CRZ,
+    PhaseShift,
+    Adjoint,
+)
 from pennylane.wires import Wires
 
 from pyqrack import QrackSimulator, Pauli
 
 from ._version import __version__
 
 # tolerance for numerical errors
 tolerance = 1e-10
 
+
 def _reverse_state(state_vector):
     """Reverse the qubit order for a vector of amplitudes.
     Args:
         state_vector (iterable[complex]): vector containing the amplitudes
     Returns:
         list[complex]
     """
@@ -65,15 +73,15 @@
     }
 
     _observable_map = {
         "PauliX": Pauli.PauliX,
         "PauliY": Pauli.PauliY,
         "PauliZ": Pauli.PauliZ,
         "Identity": Pauli.PauliI,
-        "Prod": None
+        "Prod": None,
         # "Hadamard": None,
         # "Hermitian": None,
         # "Sum": None,
         # "SProd": None,
         # "Exp": None,
         # "Projector": None,
         # "Hamiltonian": None,
@@ -142,22 +150,27 @@
         "C(Rot)",
         "ControlledPhaseShift",
         "CPhase",
         "C(ControlledPhaseShift)",
         "C(CPhase)",
         "MultiControlledX",
         "C(MultiControlledX)",
-        "QFT"
+        "QFT",
     }
 
-    config = pathlib.Path(os.path.dirname(sys.modules[__name__].__file__) + "/QrackDeviceConfig.toml")
+    config = pathlib.Path(
+        os.path.dirname(sys.modules[__name__].__file__) + "/QrackDeviceConfig.toml"
+    )
 
     @staticmethod
     def get_c_interface():
-        return "QrackDevice", os.path.dirname(sys.modules[__name__].__file__) + "/libqrack_device.so"
+        return (
+            "QrackDevice",
+            os.path.dirname(sys.modules[__name__].__file__) + "/libqrack_device.so",
+        )
 
     def __init__(self, wires=0, shots=None, **kwargs):
         super().__init__(wires=wires, shots=shots)
 
         if "isTensorNetwork" in kwargs:
             self._state = QrackSimulator(self.num_wires, **kwargs)
         else:
@@ -191,15 +204,15 @@
             if isinstance(op, QubitStateVector):
                 self._apply_qubit_state_vector(op)
             elif isinstance(op, BasisState):
                 self._apply_basis_state(op)
             elif isinstance(op, QubitUnitary):
                 if len(op.wires) > 1:
                     raise DeviceError(
-                        "Operation {} is not supported on a {} device, except for single wires.".format(op.name, self.short_name)
+                        f"Operation {op.name} is not supported on a {self.short_name} device, except for single wires."
                     )
                 self._apply_qubit_unitary(op)
             else:
                 self._apply_gate(op)
 
     def _expand_state(self, state_vector, wires):
         """Expands state vector to more wires"""
@@ -268,75 +281,132 @@
         elif opname == "C(MultiRZ)":
             device_wires = self.map_wires(op.wires)
             control_wires = self.map_wires(op.control_wires)
             for q in device_wires:
                 self._state.mcr(Pauli.PauliZ, par[0], control_wires, q)
 
         # translate op wire labels to consecutive wire labels used by the device
-        device_wires = self.map_wires((op.control_wires + op.wires) if op.control_wires else op.wires)
+        device_wires = self.map_wires(
+            (op.control_wires + op.wires) if op.control_wires else op.wires
+        )
         par = op.parameters
 
-        if opname in [''.join(p) for p in it.product(["Toffoli", "C(Toffoli)", "CNOT", "C(CNOT)", "MultiControlledX", "C(PauliX)"], ["", ".inv"])]:
+        if opname in [
+            "".join(p)
+            for p in it.product(
+                [
+                    "Toffoli",
+                    "C(Toffoli)",
+                    "CNOT",
+                    "C(CNOT)",
+                    "MultiControlledX",
+                    "C(PauliX)",
+                ],
+                ["", ".inv"],
+            )
+        ]:
             self._state.mcx(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["C(PauliY)", "C(PauliY).inv"]:
             self._state.mcy(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["C(PauliZ)", "C(PauliZ).inv"]:
             self._state.mcz(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["C(Hadamard)", "C(Hadamard).inv"]:
             self._state.mch(device_wires.labels[:-1], device_wires.labels[-1])
-        elif opname in ["CSWAP", "CSWAP.inv", "C(SWAP)", "C(SWAP).inv", "C(CSWAP)", "C(CSWAP).inv"]:
-            self._state.cswap(device_wires.labels[:-2], device_wires.labels[-2], device_wires.labels[-1])
+        elif opname in [
+            "CSWAP",
+            "CSWAP.inv",
+            "C(SWAP)",
+            "C(SWAP).inv",
+            "C(CSWAP)",
+            "C(CSWAP).inv",
+        ]:
+            self._state.cswap(
+                device_wires.labels[:-2],
+                device_wires.labels[-2],
+                device_wires.labels[-1],
+            )
         elif opname in ["CRX", "C(RX)", "C(CRX)"]:
             self._state.mcr(Pauli.PauliX, par[0], device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["CRX.inv", "C(RX).inv", "C(CRX).inv"]:
-            self._state.mcr(Pauli.PauliX, -par[0], device_wires.labels[:-1], device_wires.labels[-1])
+            self._state.mcr(
+                Pauli.PauliX, -par[0], device_wires.labels[:-1], device_wires.labels[-1]
+            )
         elif opname in ["CRY", "C(RY)", "C(CRY)"]:
             self._state.mcr(Pauli.PauliY, par[0], device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["CRY.inv", "C(RY).inv", "C(CRY).inv"]:
-            self._state.mcr(Pauli.PauliY, -par[0], device_wires.labels[:-1], device_wires.labels[-1])
+            self._state.mcr(
+                Pauli.PauliY, -par[0], device_wires.labels[:-1], device_wires.labels[-1]
+            )
         elif opname in ["CRZ", "C(RZ)", "C(CRZ)"]:
             self._state.mcr(Pauli.PauliZ, par[0], device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["CRZ.inv", "C(RZ).inv", "C(CRZ).inv"]:
-            self._state.mcr(Pauli.PauliZ, -par[0], device_wires.labels[:-1], device_wires.labels[-1])
-        elif opname in ["CRot", "CRot.inv", "C(Rot)", "C(Rot).inv", "C(CRot)", "C(CRot).inv"]:
+            self._state.mcr(
+                Pauli.PauliZ, -par[0], device_wires.labels[:-1], device_wires.labels[-1]
+            )
+        elif opname in [
+            "CRot",
+            "CRot.inv",
+            "C(Rot)",
+            "C(Rot).inv",
+            "C(CRot)",
+            "C(CRot).inv",
+        ]:
             phi = par[0]
             theta = par[1]
             omega = par[2]
             if ".inv" in opname:
                 phi = -phi
                 theta = -theta
                 omega = -omega
             c = math.cos(theta / 2)
             s = math.sin(theta / 2)
             mtrx = [
-                cmath.exp(-0.5j * (phi + omega)) * c, cmath.exp(0.5j * (phi - omega)) * s,
-                cmath.exp(-0.5j * (phi - omega)) * s, cmath.exp(0.5j * (phi + omega)) * c
+                cmath.exp(-0.5j * (phi + omega)) * c,
+                cmath.exp(0.5j * (phi - omega)) * s,
+                cmath.exp(-0.5j * (phi - omega)) * s,
+                cmath.exp(0.5j * (phi + omega)) * c,
             ]
             self._state.mcmtrx(device_wires.labels[:-1], mtrx, device_wires.labels[-1])
         elif opname in ["SWAP", "SWAP.inv"]:
             self._state.swap(device_wires.labels[0], device_wires.labels[1])
         elif opname == "ISWAP":
             self._state.iswap(device_wires.labels[0], device_wires.labels[1])
         elif opname == "ISWAP.inv":
             self._state.adjiswap(device_wires.labels[0], device_wires.labels[1])
         elif opname == "C(ISWAP)":
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, 1j)
-            self._state.cswap(device_wires.labels[:-2], device_wires.labels[-2], device_wires.labels[-1])
+            self._state.cswap(
+                device_wires.labels[:-2],
+                device_wires.labels[-2],
+                device_wires.labels[-1],
+            )
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, 1j)
         elif opname == "C(ISWAP).inv":
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, -1j)
-            self._state.cswap(device_wires.labels[:-2], device_wires.labels[-2], device_wires.labels[-1])
+            self._state.cswap(
+                device_wires.labels[:-2],
+                device_wires.labels[-2],
+                device_wires.labels[-1],
+            )
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, -1j)
         elif opname == "C(PSWAP)":
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, par[0])
-            self._state.cswap(device_wires.labels[:-2], device_wires.labels[-2], device_wires.labels[-1])
+            self._state.cswap(
+                device_wires.labels[:-2],
+                device_wires.labels[-2],
+                device_wires.labels[-1],
+            )
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, par[0])
         elif opname == "C(PSWAP).inv":
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, -par[0])
-            self._state.cswap(device_wires.labels[:-2], device_wires.labels[-2], device_wires.labels[-1])
+            self._state.cswap(
+                device_wires.labels[:-2],
+                device_wires.labels[-2],
+                device_wires.labels[-1],
+            )
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], 0, 0, -par[0])
         elif opname in ["CY", "CY.inv", "C(CY)", "C(CY).inv"]:
             self._state.mcy(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["CZ", "CZ.inv", "C(CZ)", "C(CZ).inv"]:
             self._state.mcz(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname == "S":
             self._state.s(device_wires.labels[0])
@@ -383,68 +453,162 @@
         elif opname in ["PauliY", "PauliY.inv"]:
             self._state.y(device_wires.labels[0])
         elif opname in ["PauliZ", "PauliZ.inv"]:
             self._state.z(device_wires.labels[0])
         elif opname in ["Hadamard", "Hadamard.inv"]:
             self._state.h(device_wires.labels[0])
         elif opname == "SX":
-            self._state.mtrx([(1+1j)/2, (1-1j)/2, (1-1j)/2, (1+1j)/2], device_wires.labels[0])
+            self._state.mtrx(
+                [(1 + 1j) / 2, (1 - 1j) / 2, (1 - 1j) / 2, (1 + 1j) / 2],
+                device_wires.labels[0],
+            )
         elif opname == "SX.inv":
-            self._state.mtrx([(1-1j)/2, (1+1j)/2, (1+1j)/2, (1-1j)/2], device_wires.labels[0])
+            self._state.mtrx(
+                [(1 - 1j) / 2, (1 + 1j) / 2, (1 + 1j) / 2, (1 - 1j) / 2],
+                device_wires.labels[0],
+            )
         elif opname == "C(SX)":
-            self._state.mcmtrx(device_wires.labels[:-1], [(1+1j)/2, (1-1j)/2, (1-1j)/2, (1+1j)/2], device_wires.labels[-1])
+            self._state.mcmtrx(
+                device_wires.labels[:-1],
+                [(1 + 1j) / 2, (1 - 1j) / 2, (1 - 1j) / 2, (1 + 1j) / 2],
+                device_wires.labels[-1],
+            )
         elif opname == "SX.inv":
-            self._state.mtrx([(1-1j)/2, (1+1j)/2, (1+1j)/2, (1-1j)/2], device_wires.labels[0])
+            self._state.mtrx(
+                [(1 - 1j) / 2, (1 + 1j) / 2, (1 + 1j) / 2, (1 - 1j) / 2],
+                device_wires.labels[0],
+            )
         elif opname == "C(SX).inc":
-            self._state.mcmtrx(device_wires.labels[:-1], [(1-1j)/2, (1+1j)/2, (1+1j)/2, (1-1j)/2], device_wires.labels[-1])
+            self._state.mcmtrx(
+                device_wires.labels[:-1],
+                [(1 - 1j) / 2, (1 + 1j) / 2, (1 + 1j) / 2, (1 - 1j) / 2],
+                device_wires.labels[-1],
+            )
         elif opname in ["PhaseShift", "U1"]:
             self._state.mtrx([1, 0, 0, cmath.exp(1j * par[0])], device_wires.labels[0])
         elif opname in ["PhaseShift.inv", "U1.inv"]:
             self._state.mtrx([1, 0, 0, cmath.exp(1j * -par[0])], device_wires.labels[0])
         elif opname in ["C(PhaseShift)", "C(U1)"]:
-            self._state.mtrx(device_wires.labels[:-1], [1, 0, 0, cmath.exp(1j * par[0])], device_wires.labels[-1])
+            self._state.mtrx(
+                device_wires.labels[:-1],
+                [1, 0, 0, cmath.exp(1j * par[0])],
+                device_wires.labels[-1],
+            )
         elif opname in ["C(PhaseShift).inv", "C(U1).inv"]:
-            self._state.mtrx(device_wires.labels[:-1], [1, 0, 0, cmath.exp(1j * -par[0])], device_wires.labels[-1])
-        elif opname in ["ControlledPhaseShift", "C(ControlledPhaseShift)", "CPhase", "C(CPhase)"]:
-            self._state.mcmtrx(device_wires.labels[:-1], [1, 0, 0, cmath.exp(1j * par[0])], device_wires.labels[-1])
-        elif opname in ["ControlledPhaseShift.inv", "C(ControlledPhaseShift).inv", "CPhase.inv", "C(CPhase).inv"]:
-            self._state.mcmtrx(device_wires.labels[:-1], [1, 0, 0, cmath.exp(1j * -par[0])], device_wires.labels[-1])
+            self._state.mtrx(
+                device_wires.labels[:-1],
+                [1, 0, 0, cmath.exp(1j * -par[0])],
+                device_wires.labels[-1],
+            )
+        elif opname in [
+            "ControlledPhaseShift",
+            "C(ControlledPhaseShift)",
+            "CPhase",
+            "C(CPhase)",
+        ]:
+            self._state.mcmtrx(
+                device_wires.labels[:-1],
+                [1, 0, 0, cmath.exp(1j * par[0])],
+                device_wires.labels[-1],
+            )
+        elif opname in [
+            "ControlledPhaseShift.inv",
+            "C(ControlledPhaseShift).inv",
+            "CPhase.inv",
+            "C(CPhase).inv",
+        ]:
+            self._state.mcmtrx(
+                device_wires.labels[:-1],
+                [1, 0, 0, cmath.exp(1j * -par[0])],
+                device_wires.labels[-1],
+            )
         elif opname == "U2":
-            self._state.mtrx([1, cmath.exp(1j * par[1]), cmath.exp(1j * par[0]), cmath.exp(1j * (par[0] + par[1]))], device_wires.labels[0])
+            self._state.mtrx(
+                [
+                    1,
+                    cmath.exp(1j * par[1]),
+                    cmath.exp(1j * par[0]),
+                    cmath.exp(1j * (par[0] + par[1])),
+                ],
+                device_wires.labels[0],
+            )
         elif opname == "U2.inv":
-            self._state.mtrx([1, cmath.exp(1j * -par[1]), cmath.exp(1j * -par[0]), cmath.exp(1j * (-par[0] - par[1]))], device_wires.labels[0])
+            self._state.mtrx(
+                [
+                    1,
+                    cmath.exp(1j * -par[1]),
+                    cmath.exp(1j * -par[0]),
+                    cmath.exp(1j * (-par[0] - par[1])),
+                ],
+                device_wires.labels[0],
+            )
         elif opname == "C(U2)":
-            self._state.mcmtrx(device_wires.labels[:-1], [1, cmath.exp(1j * par[1]), cmath.exp(1j * par[0]), cmath.exp(1j * (par[0] + par[1]))], device_wires.labels[-1])
+            self._state.mcmtrx(
+                device_wires.labels[:-1],
+                [
+                    1,
+                    cmath.exp(1j * par[1]),
+                    cmath.exp(1j * par[0]),
+                    cmath.exp(1j * (par[0] + par[1])),
+                ],
+                device_wires.labels[-1],
+            )
         elif opname == "C(U2).inv":
-            self._state.mcmtrx(device_wires.labels[:-1], [1, cmath.exp(1j * -par[1]), cmath.exp(1j * -par[0]), cmath.exp(1j * (-par[0] - par[1]))], device_wires.labels[-1])
+            self._state.mcmtrx(
+                device_wires.labels[:-1],
+                [
+                    1,
+                    cmath.exp(1j * -par[1]),
+                    cmath.exp(1j * -par[0]),
+                    cmath.exp(1j * (-par[0] - par[1])),
+                ],
+                device_wires.labels[-1],
+            )
         elif opname == "U3":
             self._state.u(device_wires.labels[-1], par[0], par[1], par[2])
         elif opname == "U3.inv":
             self._state.u(device_wires.labels[-1], -par[0], -par[1], -par[2])
         elif opname == "Rot":
             self._state.r(Pauli.PauliZ, par[0], device_wires.labels[-1])
             self._state.r(Pauli.PauliY, par[1], device_wires.labels[-1])
             self._state.r(Pauli.PauliZ, par[2], device_wires.labels[-1])
         elif opname == "Rot.inv":
             self._state.r(Pauli.PauliZ, -par[2], device_wires.labels[-1])
             self._state.r(Pauli.PauliY, -par[1], device_wires.labels[-1])
             self._state.r(Pauli.PauliZ, -par[0], device_wires.labels[-1])
         elif opname == "C(U3)":
-            self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], par[0], par[1], par[2])
+            self._state.mcu(
+                device_wires.labels[:-1],
+                device_wires.labels[-1],
+                par[0],
+                par[1],
+                par[2],
+            )
         elif opname == "C(U3).inv":
-            self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], -par[0], -par[1], -par[2])
+            self._state.mcu(
+                device_wires.labels[:-1],
+                device_wires.labels[-1],
+                -par[0],
+                -par[1],
+                -par[2],
+            )
         elif opname == "QFT":
             self._state.qft(device_wires.labels)
             for i in range(len(wires) >> 1):
                 self._state.swap(wires[i], wires[-i])
         elif opname == "QFT.inv":
             for i in range(len(wires) >> 1):
                 self._state.swap(wires[i], wires[-i])
             self._state.iqft(device_wires.labels)
-        elif opname not in ["Identity", "Identity.inv", "C(Identity)", "C(Identity).inv"]:
+        elif opname not in [
+            "Identity",
+            "Identity.inv",
+            "C(Identity)",
+            "C(Identity).inv",
+        ]:
             raise DeviceError(f"Operation {opname} is not supported on a {self.short_name} device.")
 
     def _apply_qubit_unitary(self, op):
         """Apply unitary to state"""
         # translate op wire labels to consecutive wire labels used by the device
         device_wires = self.map_wires(op.wires)
         par = op.parameters
@@ -462,20 +626,20 @@
         """Return the (marginal) analytic probability of each computational basis state."""
         if self._state is None:
             return None
 
         all_probs = _reverse_state(self._abs(self.state) ** 2)
         prob = self.marginal_prob(all_probs, wires)
 
-        if (not "QRACK_FPPOW" in os.environ) or (6 > int(os.environ.get('QRACK_FPPOW'))):
+        if (not "QRACK_FPPOW" in os.environ) or (6 > int(os.environ.get("QRACK_FPPOW"))):
             tot_prob = 0
             for p in prob:
                 tot_prob = tot_prob + p
 
-            if tot_prob != 1.:
+            if tot_prob != 1.0:
                 for i in range(len(prob)):
                     prob[i] = prob[i] / tot_prob
 
         return prob
 
     def expval(self, observable, **kwargs):
         if self.shots is None:
@@ -504,15 +668,17 @@
     def generate_samples(self):
         if self.shots is None:
             raise qml.QuantumFunctionError(
                 "The number of shots has to be explicitly set on the device "
                 "when using sample-based measurements."
             )
 
-        samples = np.array(self._state.measure_shots(list(range(self.num_wires - 1, -1, -1)), self.shots))
+        samples = np.array(
+            self._state.measure_shots(list(range(self.num_wires - 1, -1, -1)), self.shots)
+        )
         self._samples = QubitDevice.states_to_binary(samples, self.num_wires)
 
         return self._samples
 
     @property
     def state(self):
         # returns the state after all operations are applied
```

### Comparing `pennylane_qrack-0.6.2/pennylane_qrack.egg-info/PKG-INFO` & `pennylane_qrack-0.6.3/pennylane_qrack.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qrack
-Version: 0.6.2
+Version: 0.6.3
 Summary: PennyLane plugin for Qrack.
 Home-page: http://github.com/vm6502q
 Maintainer: vm6502q
 Maintainer-email: stranoj@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -35,41 +35,58 @@
 
 The PennyLane-Qrack plugin integrates the Qrack quantum computing framework with PennyLane's quantum machine learning capabilities.
 
 This plugin is addapted from the `PennyLane-Qulacs plugin, <https://github.com/PennyLaneAI/pennylane-qulacs>`__ under the Apache License 2.0, with many thanks to the original developers!
 
 `PennyLane <https://pennylane.readthedocs.io>`__ is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
-`vm6502q/qrack <https://github.com/vm6502q>`__ is a software library for quantum computing, written in C++ and with GPU support.
+`unitaryfund/qrack <https://github.com/unitaryfund/qrack>`__ (formerly **vm6502q/qrack**) is a software library for quantum computing, written in C++ and with GPU support.
 
 Features
 ========
 
 * Provides access to a PyQrack simulator backend via the ``qrack.simulator`` device
+* Provides access to a (C++) Qrack simulator backend for Catalyst (also) via the ``qrack.simulator`` device
 
 Installation
 ============
 
-This plugin requires Python version 3.6 or above, as well as PennyLane. Installation of this plugin, as well as all dependencies, can be done using ``pip``:
+This plugin requires Python version 3.6 or above, as well as PennyLane and the Qrack library.
+
+You can choose to go the `releases <https://github.com/unitaryfund/qrack/releases>`__ page of Qrack to download a packaged artifact for your system and **install it in your system directories** (like `/usr` or `/usr/local` on Linux and UNIX based systems, including Mac), **or** you can opt to **build and install from source**, which might be easier, and this gives you maximum control over build configurations, like choice of CUDA over OpenCL GPU acceleration!
+
+See the Qrack README and documentation for the many build options of qrack, but, after checking out the Qrack repository and entering its root folder, this might be the best and simplest way to build and install Qrack:
+
+.. code-block:: bash
+
+    $ mkdir _build
+    $ cd _build
+    $ cmake -DCPP_STD=14 ..
+    $ make all -j$(nproc --all)
+    $ sudo make install
+
+After installing Qrack, installation of this plugin as well as all its Python dependencies can be done using ``pip`` (or ``pip3``, as appropriate):
 
 .. code-block:: bash
 
-    $ pip install pennylane-qrack
+    $ pip3 install pennylane-qrack
 
 Dependencies
 ~~~~~~~~~~~~
 
 PennyLane-Qrack requires the following libraries be installed:
 
 * `Python <http://python.org/>`__ >= 3.8
+* `Qrack <https://github.com/unitaryfund/qrack>`__ >= 9.0
 
 as well as the following Python packages:
 
 * `PennyLane <http://pennylane.readthedocs.io/>`__ >= 0.32
-* `PyQrack <https://github.com/vm6502q/pyqrack>`__  >= 0.13.0
+* `Catalyst <https://docs.pennylane.ai/projects/catalyst/en/stable/index.html>`__ >= 0.6
+* `PyQrack <https://github.com/vm6502q/pyqrack>`__  >= 1.28.0
 
 
 If you currently do not have Python 3 installed, we recommend
 `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed version of Python packaged
 for scientific computation.
```

### Comparing `pennylane_qrack-0.6.2/setup.py` & `pennylane_qrack-0.6.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,47 +8,49 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #!/usr/bin/env python3
+import os
 import re
 from skbuild import setup
 
 
 with open("./pennylane_qrack/_version.py") as f:
     (version,) = re.findall('__version__ = "(.*)"', f.read())
 
-
 requirements = [
     "pennylane>=0.32",
     "pyqrack>=0.13.0",
     "numpy~=1.16",
-    "scikit-build>=0.1.0"
+    "scikit-build>=0.1.0",
 ]
 
 info = {
     "name": "pennylane-qrack",
     "version": version,
     "maintainer": "vm6502q",
     "maintainer_email": "stranoj@gmail.com",
     "url": "http://github.com/vm6502q",
     "license": "Apache License 2.0",
     "packages": ["pennylane_qrack"],
     "entry_points": {
-        "pennylane.plugins": ["qrack.simulator = pennylane_qrack.qrack_device:QrackDevice"]
+        "pennylane.plugins": [
+            "qrack.simulator = pennylane_qrack.qrack_device:QrackDevice"
+        ]
     },
     "description": "PennyLane plugin for Qrack.",
     "long_description": open("README.rst").read(),
     "long_description_content_type": "text/x-rst",
     "provides": ["pennylane_qrack"],
     "install_requires": requirements,
-    "package_data": {'pennylane_qrack': ['QrackDeviceConfig.toml']},
-    "include_package_data": True
+    "package_data": {"pennylane_qrack": ["QrackDeviceConfig.toml"]},
+    "include_package_data": True,
 }
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `pennylane_qrack-0.6.2/tests/test_apply.py` & `pennylane_qrack-0.6.3/tests/test_apply.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 I = np.identity(2)
 X = np.array([[0, 1], [1, 0]])
 Y = np.array([[0, -1j], [1j, 0]])
 Z = np.array([[1, 0], [0, -1]])
 H = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
 S = np.diag([1, 1j])
 T = np.diag([1, np.exp(1j * np.pi / 4)])
-SX = np.array([[(1+1j)/2, (1-1j)/2], [(1-1j)/2, (1+1j)/2]])
+SX = np.array([[(1 + 1j) / 2, (1 - 1j) / 2], [(1 - 1j) / 2, (1 + 1j) / 2]])
 SWAP = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
 CNOT = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
 CZ = np.diag([1, 1, 1, -1])
 ISWAP = np.array([[1, 0, 0, 0], [0, 0, 1j, 0], [0, 1j, 0, 0], [0, 0, 0, 1]])
 toffoli = np.diag([1 for i in range(8)])
 toffoli[6:8, 6:8] = np.array([[0, 1], [1, 0]])
 multix4 = np.diag([1 for i in range(16)])
@@ -48,16 +48,26 @@
 
 # parametrized qubit gates
 phase_shift = lambda phi: np.diag([1, np.exp(1j * phi)])
 c_phase_shift = lambda phi: np.diag([1, 1, 1, np.exp(1j * phi)])
 rx = lambda theta: np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * X
 ry = lambda theta: np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * Y
 rz = lambda theta: np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * Z
-u2 = lambda phi, delta: np.array([[1, np.exp(1j * delta)], [np.exp(1j * phi), np.exp(1j * (phi + delta))]])
-u3 = lambda theta, phi, delta: np.array([[np.cos(theta / 2), -np.exp(1j * delta) * np.sin(theta / 2)], [np.exp(1j * phi) * np.sin(theta / 2), np.exp(1j * (phi + delta)) * np.cos(theta / 2)]])
+u2 = lambda phi, delta: np.array(
+    [[1, np.exp(1j * delta)], [np.exp(1j * phi), np.exp(1j * (phi + delta))]]
+)
+u3 = lambda theta, phi, delta: np.array(
+    [
+        [np.cos(theta / 2), -np.exp(1j * delta) * np.sin(theta / 2)],
+        [
+            np.exp(1j * phi) * np.sin(theta / 2),
+            np.exp(1j * (phi + delta)) * np.cos(theta / 2),
+        ],
+    ]
+)
 
 # CRX/CRY/CRZ in the PennyLane convention
 crx = lambda theta: np.array(
     [
         [1, 0, 0, 0],
         [0, 1, 0, 0],
         [0, 0, np.cos(theta / 2), -1j * np.sin(theta / 2)],
@@ -80,16 +90,26 @@
         [0, 0, 0, np.exp(1j * theta / 2)],
     ]
 )
 crot = lambda phi, theta, omega: np.array(
     [
         [1, 0, 0, 0],
         [0, 1, 0, 0],
-        [0, 0, np.exp(-0.5j * (phi + omega)) * np.cos(theta / 2), np.exp(0.5j * (phi - omega)) * np.sin(theta / 2)],
-        [0, 0, np.exp(-0.5j * (phi - omega)) * np.sin(theta / 2), np.exp(0.5j * (phi + omega)) * np.cos(theta / 2)]
+        [
+            0,
+            0,
+            np.exp(-0.5j * (phi + omega)) * np.cos(theta / 2),
+            np.exp(0.5j * (phi - omega)) * np.sin(theta / 2),
+        ],
+        [
+            0,
+            0,
+            np.exp(-0.5j * (phi - omega)) * np.sin(theta / 2),
+            np.exp(0.5j * (phi + omega)) * np.cos(theta / 2),
+        ],
     ]
 )
 
 # list of all non-parametrized single-qubit gates,
 # along with the PennyLane operation name
 single_qubit = [
     (qml.PauliX(wires=0), X),
@@ -101,15 +121,15 @@
     (qml.SX(wires=0), SX),
     (qml.adjoint(qml.PauliX(wires=0)), X.conj().T),
     (qml.adjoint(qml.PauliY(wires=0)), Y.conj().T),
     (qml.adjoint(qml.PauliZ(wires=0)), Z.conj().T),
     (qml.adjoint(qml.Hadamard(wires=0)), H.conj().T),
     (qml.adjoint(qml.S(wires=0)), S.conj().T),
     (qml.adjoint(qml.T(wires=0)), T.conj().T),
-    (qml.adjoint(qml.SX(wires=0)), SX.conj().T)
+    (qml.adjoint(qml.SX(wires=0)), SX.conj().T),
 ]
 
 # list of all parametrized single-qubit gates
 single_qubit_param = [
     (qml.RX(0, wires=0), rx),
     (qml.RY(0, wires=0), ry),
     (qml.RZ(0, wires=0), rz),
@@ -121,53 +141,62 @@
 ]
 single_qubit_two_param = [
     (qml.U2(0, 0, wires=0), u2),
     (qml.adjoint(qml.U2(0, 0, wires=0)), lambda phi, delta: u2(-phi, -delta)),
 ]
 single_qubit_three_param = [
     (qml.U3(0, 0, 0, wires=0), u3),
-    (qml.adjoint(qml.U3(0, 0, 0, wires=0)), lambda theta, phi, delta: u3(-theta, -phi, -delta)),
+    (
+        qml.adjoint(qml.U3(0, 0, 0, wires=0)),
+        lambda theta, phi, delta: u3(-theta, -phi, -delta),
+    ),
 ]
 # list of all non-parametrized two-qubit gates
 two_qubit = [
     (qml.CNOT(wires=[0, 1]), CNOT),
     (qml.SWAP(wires=[0, 1]), SWAP),
     (qml.CZ(wires=[0, 1]), CZ),
     (qml.ISWAP(wires=[0, 1]), ISWAP),
     (qml.adjoint(qml.CNOT(wires=[0, 1])), CNOT.conj().T),
     (qml.adjoint(qml.SWAP(wires=[0, 1])), SWAP.conj().T),
     (qml.adjoint(qml.CZ(wires=[0, 1])), CZ.conj().T),
-    (qml.adjoint(qml.ISWAP(wires=[0, 1])), ISWAP.conj().T)
+    (qml.adjoint(qml.ISWAP(wires=[0, 1])), ISWAP.conj().T),
 ]
 # list of all parametrized two-qubit gates
 two_qubit_param = [
     (qml.CRX(0, wires=[0, 1]), crx),
     (qml.CRY(0, wires=[0, 1]), cry),
     (qml.CRZ(0, wires=[0, 1]), crz),
     (qml.ControlledPhaseShift(0, wires=[0, 1]), c_phase_shift),
     (qml.adjoint(qml.CRX(0, wires=[0, 1])), lambda theta: crx(-theta)),
     (qml.adjoint(qml.CRY(0, wires=[0, 1])), lambda theta: cry(-theta)),
     (qml.adjoint(qml.CRZ(0, wires=[0, 1])), lambda theta: crz(-theta)),
-    (qml.adjoint(qml.ControlledPhaseShift(0, wires=[0, 1])), lambda theta: c_phase_shift(-theta))
+    (
+        qml.adjoint(qml.ControlledPhaseShift(0, wires=[0, 1])),
+        lambda theta: c_phase_shift(-theta),
+    ),
 ]
 two_qubit_three_param = [
     (qml.CRot(0, 0, 0, wires=[0, 1]), crot),
-    (qml.adjoint(qml.CRot(0, 0, 0, wires=[0, 1])), lambda phi, theta, omega: crot(-phi, -theta, -omega)),
+    (
+        qml.adjoint(qml.CRot(0, 0, 0, wires=[0, 1])),
+        lambda phi, theta, omega: crot(-phi, -theta, -omega),
+    ),
 ]
 # list of all three-qubit gates
 three_qubit = [
     (qml.Toffoli(wires=[0, 1, 2]), toffoli),
     (qml.CSWAP(wires=[0, 1, 2]), CSWAP),
     (qml.adjoint(qml.Toffoli(wires=[0, 1, 2])), toffoli.conj().T),
     (qml.adjoint(qml.CSWAP(wires=[0, 1, 2])), CSWAP.conj().T),
 ]
 # list of all four-qubit gates
 four_qubit = [
     (qml.MultiControlledX(wires=[0, 1, 2, 3]), multix4),
-    (qml.adjoint(qml.MultiControlledX(wires=[0, 1, 2, 3])), multix4.conj().T)
+    (qml.adjoint(qml.MultiControlledX(wires=[0, 1, 2, 3])), multix4.conj().T),
 ]
 
 
 class TestStateApply:
     """Test the device's state after application of gates."""
 
     @pytest.mark.parametrize(
@@ -177,23 +206,23 @@
             np.array([0, 0, 1, 0]),
             np.array([1, 0, 1, 0]),
             np.array([1, 1, 1, 1]),
         ],
     )
     def test_basis_state(self, state, tol):
         """Test basis state initialization"""
-        dev = QrackDevice(4, isTensorNetwork=False)
+        dev = QrackDevice(4, isOpenCL=False)
 
         op = qml.BasisState(state, wires=[0, 1, 2, 3])
         dev.apply([op])
         dev._obs_queue = []
 
         res = np.abs(dev.state) ** 2
         # compute expected probabilities
-        expected = np.zeros([2 ** 4])
+        expected = np.zeros([2**4])
         expected[np.ravel_multi_index(state, [2] * 4)] = 1
 
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize(
         "state",
         [
@@ -203,15 +232,15 @@
             np.array([1, 1]),
         ],
     )
     @pytest.mark.parametrize("device_wires", [3, 4, 5])
     @pytest.mark.parametrize("op_wires", [[0, 1], [1, 0], [2, 0]])
     def test_basis_state_on_wires_subset(self, state, device_wires, op_wires, tol):
         """Test basis state initialization on a subset of device wires"""
-        dev = QrackDevice(device_wires, isTensorNetwork=False)
+        dev = QrackDevice(device_wires, isOpenCL=False)
 
         op = qml.BasisState(state, wires=op_wires)
         dev.apply([op])
         dev._obs_queue = []
 
         res = np.abs(dev.state) ** 2
         # compute expected probabilities
@@ -219,69 +248,74 @@
         expected[np.ravel_multi_index(state, [2] * len(op_wires))] = 1
 
         expected = dev._expand_state(expected, op_wires)
         assert np.allclose(res, expected, tol)
 
     def test_qubit_state_vector(self, init_state, tol):
         """Test QubitStateVector application"""
-        dev = QrackDevice(1, isTensorNetwork=False)
+        dev = QrackDevice(1, isOpenCL=False)
         state = init_state(1)
 
         op = qml.QubitStateVector(state, wires=[0])
         dev.apply([op])
         dev._obs_queue = []
 
         res = dev.state
         expected = state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("device_wires", [3, 4, 5])
     @pytest.mark.parametrize("op_wires", [[0], [2], [0, 1], [1, 0], [2, 0]])
-    def test_qubit_state_vector_on_wires_subset(self, init_state, device_wires, op_wires, tol):
+    def test_qubit_state_vector_on_wires_subset(
+        self, init_state, device_wires, op_wires, tol
+    ):
         """Test QubitStateVector application on a subset of device wires"""
-        dev = QrackDevice(device_wires, isTensorNetwork=False)
+        dev = QrackDevice(device_wires, isOpenCL=False)
         state = init_state(len(op_wires))
 
         op = qml.QubitStateVector(state, wires=op_wires)
         dev.apply([op])
         dev._obs_queue = []
 
         res = dev.state
         expected = dev._expand_state(state, op_wires)
 
         assert np.allclose(res, expected, tol)
 
     def test_invalid_qubit_state_vector(self):
         """Test that an exception is raised if the state
         vector is the wrong size"""
-        dev = QrackDevice(2, isTensorNetwork=False)
+        dev = QrackDevice(2, isOpenCL=False)
         state = np.array([0, 123.432])
 
-        with pytest.raises(ValueError, match="State vector must have shape \\(2\\*\\*wires,\\) or \\(batch_size, 2\\*\\*wires\\)."):
+        with pytest.raises(
+            ValueError,
+            match="State vector must have shape \\(2\\*\\*wires,\\) or \\(batch_size, 2\\*\\*wires\\).",
+        ):
             op = qml.QubitStateVector(state, wires=[0, 1])
             dev.apply([op])
 
     @pytest.mark.parametrize("op,mat", single_qubit)
     def test_single_qubit_no_parameters(self, init_state, op, mat, tol):
         """Test PauliX application"""
-        dev = QrackDevice(1, isTensorNetwork=False)
+        dev = QrackDevice(1, isOpenCL=False)
         state = init_state(1)
 
         dev.apply([qml.QubitStateVector(state, wires=[0]), op])
         dev._obs_queue = []
 
         res = dev.state
         expected = mat @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("theta", [0.5432, -0.232])
     @pytest.mark.parametrize("op,func", single_qubit_param)
     def test_single_qubit_parameters(self, init_state, op, func, theta, tol):
         """Test PauliX application"""
-        dev = QrackDevice(1, isTensorNetwork=False)
+        dev = QrackDevice(1, isOpenCL=False)
         state = init_state(1)
 
         op.data = [theta]
         dev.apply([qml.QubitStateVector(state, wires=[0]), op])
         dev._obs_queue = []
 
         res = dev.state
@@ -289,61 +323,63 @@
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("phi", [0.126, -0.721])
     @pytest.mark.parametrize("delta", [0.5432, -0.232])
     @pytest.mark.parametrize("op,func", single_qubit_two_param)
     def test_single_qubit_two_parameters(self, init_state, op, func, phi, delta, tol):
         """Test PauliX application"""
-        dev = QrackDevice(1, isTensorNetwork=False)
+        dev = QrackDevice(1, isOpenCL=False)
         state = init_state(1)
 
         op.data = [phi, delta]
         dev.apply([qml.QubitStateVector(state, wires=[0]), op])
         dev._obs_queue = []
 
         res = dev.state
         expected = func(phi, delta) @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("phi", [0.126, -0.721])
     @pytest.mark.parametrize("theta", [0.5432, -0.232])
     @pytest.mark.parametrize("omega", [1.213, -0.221])
     @pytest.mark.parametrize("op,func", single_qubit_three_param)
-    def test_single_qubit_three_parameters(self, init_state, op, func, phi, theta, omega, tol):
+    def test_single_qubit_three_parameters(
+        self, init_state, op, func, phi, theta, omega, tol
+    ):
         """Test PauliX application"""
-        dev = QrackDevice(1, isTensorNetwork=False)
+        dev = QrackDevice(1, isOpenCL=False)
         state = init_state(1)
 
         op.data = [phi, theta, omega]
         dev.apply([qml.QubitStateVector(state, wires=[0]), op])
         dev._obs_queue = []
 
         res = dev.state
         expected = func(phi, theta, omega) @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("op, mat", two_qubit)
     def test_two_qubit_no_parameters(self, init_state, op, mat, tol):
         """Test PauliX application"""
-        dev = QrackDevice(2, isTensorNetwork=False)
+        dev = QrackDevice(2, isOpenCL=False)
         state = init_state(2)
 
         dev.apply([qml.QubitStateVector(state, wires=[0, 1]), op])
         dev._obs_queue = []
 
         res = dev.state
         expected = mat @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("mat", [U])
     def test_qubit_unitary(self, init_state, mat, tol):
         """Test QubitUnitary application"""
 
         N = int(np.log2(len(mat)))
-        dev = QrackDevice(N, isTensorNetwork=False)
+        dev = QrackDevice(N, isOpenCL=False)
         state = init_state(N)
 
         op = qml.QubitUnitary(mat, wires=list(range(N)))
         dev.apply([qml.QubitStateVector(state, wires=list(range(N))), op])
         dev._obs_queue = []
 
         res = dev.state
@@ -356,41 +392,41 @@
         state = np.array([[0, 123.432], [-0.432, 023.4]])
 
         with pytest.raises(ValueError, match=r"Input unitary must be of shape"):
             qml.QubitUnitary(state, wires=[0, 1])
 
     @pytest.mark.parametrize("op, mat", three_qubit)
     def test_three_qubit_no_parameters(self, init_state, op, mat, tol):
-        dev = QrackDevice(3, isTensorNetwork=False)
+        dev = QrackDevice(3, isOpenCL=False)
         state = init_state(3)
 
         dev.apply([qml.QubitStateVector(state, wires=[0, 1, 2]), op])
         dev._obs_queue = []
 
         res = dev.state
         expected = mat @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("op, mat", four_qubit)
     def test_four_qubit_no_parameters(self, init_state, op, mat, tol):
-        dev = QrackDevice(4, isTensorNetwork=False)
+        dev = QrackDevice(4, isOpenCL=False)
         state = init_state(4)
 
         dev.apply([qml.QubitStateVector(state, wires=[0, 1, 2, 3]), op])
         dev._obs_queue = []
 
         res = dev.state
         expected = mat @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("theta", [0.5432, -0.232])
     @pytest.mark.parametrize("op,func", two_qubit_param)
     def test_two_qubit_parameters(self, init_state, op, func, theta, tol):
         """Test parametrized two qubit gates application"""
-        dev = QrackDevice(2, isTensorNetwork=False)
+        dev = QrackDevice(2, isOpenCL=False)
         state = init_state(2)
 
         op.data = [theta]
         dev.apply([qml.QubitStateVector(state, wires=[0, 1]), op])
 
         dev._obs_queue = []
 
@@ -398,43 +434,50 @@
         expected = func(theta) @ state
         assert np.allclose(res, expected, tol)
 
     @pytest.mark.parametrize("phi", [0.126, -0.721])
     @pytest.mark.parametrize("theta", [0.5432, -0.232])
     @pytest.mark.parametrize("omega", [1.213, -0.221])
     @pytest.mark.parametrize("op,func", two_qubit_three_param)
-    def test_two_qubit_three_parameters(self, init_state, op, func, phi, theta, omega, tol):
+    def test_two_qubit_three_parameters(
+        self, init_state, op, func, phi, theta, omega, tol
+    ):
         """Test parametrized two qubit gates application"""
-        dev = QrackDevice(2, isTensorNetwork=False)
+        dev = QrackDevice(2, isOpenCL=False)
         state = init_state(2)
 
         op.data = [phi, theta, omega]
         dev.apply([qml.QubitStateVector(state, wires=[0, 1]), op])
 
         dev._obs_queue = []
 
         res = dev.state
         expected = func(phi, theta, omega) @ state
         assert np.allclose(res, expected, tol)
 
     def test_apply_errors_qubit_state_vector(self):
         """Test that apply fails for incorrect state preparation."""
-        dev = QrackDevice(2, isTensorNetwork=False)
+        dev = QrackDevice(2, isOpenCL=False)
 
-        with pytest.raises(ValueError, match="Sum of amplitudes-squared does not equal one."):
+        with pytest.raises(
+            ValueError, match="Sum of amplitudes-squared does not equal one."
+        ):
             dev.apply([qml.QubitStateVector(np.array([1, -1]), wires=[0])])
 
-        with pytest.raises(ValueError, match="State vector must have shape \\(2\\*\\*wires,\\) or \\(batch_size, 2\\*\\*wires\\)."):
+        with pytest.raises(
+            ValueError,
+            match="State vector must have shape \\(2\\*\\*wires,\\) or \\(batch_size, 2\\*\\*wires\\).",
+        ):
             p = np.array([1, 0, 1, 1, 0]) / np.sqrt(3)
             dev.reset()
             dev.apply([qml.QubitStateVector(p, wires=[0, 1])])
 
     def test_apply_errors_basis_state(self):
         """Test that apply fails for incorrect basis state preparation."""
-        dev = QrackDevice(2, isTensorNetwork=False)
+        dev = QrackDevice(2, isOpenCL=False)
 
         with pytest.raises(
             ValueError, match="BasisState parameter must consist of 0 or 1 integers."
         ):
             dev.apply([qml.BasisState(np.array([-0.2, 4.2]), wires=[0, 1])])
 
         with pytest.raises(
@@ -445,20 +488,45 @@
 
 @pytest.mark.parametrize(
     "state, device_wires, op_wires, expected",
     [
         (np.array([1, 0]), 2, [0], [1, 0, 0, 0]),
         (np.array([0, 1]), 2, [0], [0, 0, 1, 0]),
         (np.array([1, 1]) / np.sqrt(2), 2, [1], np.array([1, 1, 0, 0]) / np.sqrt(2)),
-        (np.array([1, 1]) / np.sqrt(2), 3, [0], np.array([1, 0, 0, 0, 1, 0, 0, 0]) / np.sqrt(2)),
-        (np.array([1, 2, 3, 4]) / np.sqrt(48), 3, [0, 1], np.array([1, 0, 2, 0, 3, 0, 4, 0]) / np.sqrt(48)),
-        (np.array([1, 2, 3, 4]) / np.sqrt(48), 3, [1, 0], np.array([1, 0, 3, 0, 2, 0, 4, 0]) / np.sqrt(48)),
-        (np.array([1, 2, 3, 4]) / np.sqrt(48), 3, [0, 2], np.array([1, 2, 0, 0, 3, 4, 0, 0]) / np.sqrt(48)),
-        (np.array([1, 2, 3, 4]) / np.sqrt(48), 3, [1, 2], np.array([1, 2, 3, 4, 0, 0, 0, 0]) / np.sqrt(48)),
+        (
+            np.array([1, 1]) / np.sqrt(2),
+            3,
+            [0],
+            np.array([1, 0, 0, 0, 1, 0, 0, 0]) / np.sqrt(2),
+        ),
+        (
+            np.array([1, 2, 3, 4]) / np.sqrt(48),
+            3,
+            [0, 1],
+            np.array([1, 0, 2, 0, 3, 0, 4, 0]) / np.sqrt(48),
+        ),
+        (
+            np.array([1, 2, 3, 4]) / np.sqrt(48),
+            3,
+            [1, 0],
+            np.array([1, 0, 3, 0, 2, 0, 4, 0]) / np.sqrt(48),
+        ),
+        (
+            np.array([1, 2, 3, 4]) / np.sqrt(48),
+            3,
+            [0, 2],
+            np.array([1, 2, 0, 0, 3, 4, 0, 0]) / np.sqrt(48),
+        ),
+        (
+            np.array([1, 2, 3, 4]) / np.sqrt(48),
+            3,
+            [1, 2],
+            np.array([1, 2, 3, 4, 0, 0, 0, 0]) / np.sqrt(48),
+        ),
     ],
 )
 def test_expand_state(state, op_wires, device_wires, expected, tol):
     """Test that the expand_state method works as expected."""
-    dev = QrackDevice(device_wires, isTensorNetwork=False)
+    dev = QrackDevice(device_wires, isOpenCL=False)
     res = dev._expand_state(state, op_wires)
 
     assert np.allclose(res, expected, tol)
```

### Comparing `pennylane_qrack-0.6.2/tests/test_integration.py` & `pennylane_qrack-0.6.3/tests/test_integration.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
 
 class TestIntegration:
     """Some basic integration tests."""
 
     def test_load_device(self):
         """Test that the Qrack device loads correctly."""
-        dev = QrackDevice(2, shots=int(1e6))
+        dev = QrackDevice(2, shots=int(1e6), isOpenCL=False)
 
         assert dev.num_wires == 2
         assert dev.shots == int(1e6)
         assert dev.short_name == "qrack.simulator"
         assert "model" in dev.__class__.capabilities()
 
     def test_expectation(self):
         """Test that expectation of a non-trivial circuit is correct."""
-        dev = QrackDevice(2, shots=int(1e6))
+        dev = QrackDevice(2, shots=int(1e6), isOpenCL=False)
 
         theta = 0.432
         phi = 0.123
 
         @qml.qnode(dev)
         def circuit():
             qml.adjoint(qml.RY(theta, wires=[0]))
```

### Comparing `pennylane_qrack-0.6.2/tests/test_units.py` & `pennylane_qrack-0.6.3/tests/test_units.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,85 +19,63 @@
 from pennylane_qrack.qrack_device import QrackDevice
 from pyqrack import QrackSimulator
 
 
 class TestDeviceUnits:
     """Unit tests for the plugin."""
 
-    @pytest.mark.parametrize(
-        "num_wires, shots", [(1, None), (2, 184), (3, 1)]
-    )
+    @pytest.mark.parametrize("num_wires, shots", [(1, None), (2, 184), (3, 1)])
     def test_device_attributes(self, num_wires, shots):
         """Test that attributes are set as expected."""
-        dev = QrackDevice(wires=num_wires, shots=shots)
+        dev = QrackDevice(wires=num_wires, shots=shots, isOpenCL=False)
 
         assert dev.num_wires == num_wires
         assert dev.shots == shots
         assert dev._samples is None
         assert dev._capabilities["model"] == "qubit"
         assert dev._capabilities["tensor_observables"]
-        assert not dev._capabilities["returns_state"]
+        assert dev._capabilities["returns_state"]
         assert isinstance(dev._state, QrackSimulator)
 
     # def test_no_gpu_support(self, monkeypatch):
     #     """Test that error thrown when gpu set to True but no gpu support found."""
     #
-    #     monkeypatch.setattr(QrackDevice, "gpu_supported", False)
+    #     monkeypatch.setattr(QrackDevice, "gpu_supported", False, isOpenCL=False)
     #
     #     with pytest.raises(
     #         qml.DeviceError, match="GPU not supported with installed version of qrack"
     #     ):
-    #         QrackDevice(3, gpu=True)
+    #         QrackDevice(3, gpu=True, isOpenCL=False)
 
     @pytest.mark.parametrize(
         "wires, prob",
-        [([0], [1.0, 0.0]), ([0, 1], [0.0, 1.0, 0.0, 0.0]), ([1, 3], [0.0, 0.0, 0.0, 1.0])],
+        [
+            ([0], [1.0, 0.0]),
+            ([0, 1], [0.0, 1.0, 0.0, 0.0]),
+            ([1, 3], [0.0, 0.0, 0.0, 1.0]),
+        ],
     )
     def test_analytic_probability(self, wires, prob, tol):
         """Test the analytic_probability() function."""
-        dev = QrackDevice(4)
+        dev = QrackDevice(4, isOpenCL=False)
         state = np.array((0, 1, 0, 1))
         op = qml.BasisState(state, wires=[0, 1, 2, 3])
         dev.apply([op])
 
         res = dev.analytic_probability(wires=wires)
         res = list(res)
         assert np.allclose(res, prob, atol=tol)
 
     def test_reset(self, tol):
         """Test the reset() function."""
-        dev = QrackDevice(4)
+        dev = QrackDevice(4, isOpenCL=False)
         state = np.array((0, 1, 0, 1))
         op = qml.BasisState(state, wires=[0, 1, 2, 3])
         dev.apply([op])
         dev.reset()
 
         expected = [0.0] * 16
         expected[0] = 1.0
         actual = dev._state.out_ket()
         for i in range(16):
             actual[i] = actual[i] * np.conjugate(actual[i])
         assert np.allclose(actual, expected)
-
-    @pytest.mark.parametrize("obs,args,wires,supported", [
-        (qml.PauliX, [], [0], True),
-        (qml.Hadamard, [], [0], False),
-        (qml.Hermitian, [
-            np.array([
-                [1.02789352, 1.61296440 - 0.3498192j],
-                [1.61296440 + 0.3498192j, 1.23920938 + 0j]
-            ])
-        ], [0], False),
-        (lambda wires: qml.PauliX(wires[0]) @ qml.Hadamard(wires[1]), [], [0, 1], False),
-        (lambda wires: qml.PauliZ(wires[0]) @ qml.PauliY(wires[1]), [], [0, 1], True)
-        ])
-    def test_expval_hadamard(self, obs, args, wires, supported, mocker):
-        """Test that QrackDevice.expval() uses native calculations when possible"""
-        dev = QrackDevice(4)
-
-        spy = mocker.spy(dev, "probability")
-        dev.expval(obs(*args, wires=wires))
-
-        # if supported:
-        #     spy.assert_not_called()
-        # else:
-        spy.assert_called_once()
```

