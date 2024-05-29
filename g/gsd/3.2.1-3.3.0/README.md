# Comparing `tmp/gsd-3.2.1.tar.gz` & `tmp/gsd-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsd-3.2.1.tar", last modified: Mon Jan 22 22:16:08 2024, max compression
+gzip compressed data, was "gsd-3.3.0.tar", last modified: Wed May 29 16:07:46 2024, max compression
```

## Comparing `gsd-3.2.1.tar` & `gsd-3.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:16:08.952503 gsd-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-01-22 22:15:56.000000 gsd-3.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-22 22:15:56.000000 gsd-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-22 22:15:56.000000 gsd-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-01-22 22:16:08.952503 gsd-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-01-22 22:15:56.000000 gsd-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:16:08.952503 gsd-3.2.1/gsd/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)   976607 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd/fl.c
--rw-r--r--   0 runner    (1001) docker     (127)    37102 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/fl.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    73998 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/gsd.c
--rw-r--r--   0 runner    (1001) docker     (127)    22342 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/gsd.h
--rw-r--r--   0 runner    (1001) docker     (127)    45325 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/libgsd.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/pygsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/pytest_plugin_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:16:08.952503 gsd-3.2.1/gsd/test/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)    36771 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/test/test_fl.py
--rw-r--r--   0 runner    (1001) docker     (127)    72428 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/test/test_gsd_v1.gsd
--rw-r--r--   0 runner    (1001) docker     (127)    38509 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/test/test_hoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/test/test_largefile.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-22 22:15:56.000000 gsd-3.2.1/gsd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:16:08.952503 gsd-3.2.1/gsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-22 22:16:08.000000 gsd-3.2.1/gsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-01-22 22:15:56.000000 gsd-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 22:16:08.952503 gsd-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-22 22:15:56.000000 gsd-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:07:46.469859 gsd-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-05-29 16:07:17.000000 gsd-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-29 16:07:17.000000 gsd-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 16:07:17.000000 gsd-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-29 16:07:46.469859 gsd-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-29 16:07:17.000000 gsd-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:07:46.465860 gsd-3.3.0/gsd/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1001886 2024-05-29 16:07:45.000000 gsd-3.3.0/gsd/fl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    37102 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/fl.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    73998 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/gsd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22342 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/gsd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45384 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/libgsd.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/pygsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/pytest_plugin_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:07:46.469859 gsd-3.3.0/gsd/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    36785 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/test/test_fl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72428 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/test/test_gsd_v1.gsd
+-rw-r--r--   0 runner    (1001) docker     (127)    38509 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/test/test_hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/test/test_largefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 16:07:17.000000 gsd-3.3.0/gsd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:07:46.469859 gsd-3.3.0/gsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-29 16:07:46.000000 gsd-3.3.0/gsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-29 16:07:46.000000 gsd-3.3.0/gsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:07:46.000000 gsd-3.3.0/gsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 16:07:46.000000 gsd-3.3.0/gsd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 16:07:46.000000 gsd-3.3.0/gsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 16:07:46.000000 gsd-3.3.0/gsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-29 16:07:17.000000 gsd-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:07:46.469859 gsd-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 16:07:17.000000 gsd-3.3.0/setup.py
```

### Comparing `gsd-3.2.1/CHANGELOG.rst` & `gsd-3.3.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,41 @@
-.. Copyright (c) 2016-2023 The Regents of the University of Michigan
+.. Copyright (c) 2016-2024 The Regents of the University of Michigan
 .. Part of GSD, released under the BSD 2-Clause License.
 
 Change Log
 ==========
 
 `GSD <https://github.com/glotzerlab/gsd>`_ releases follow `semantic versioning
 <https://semver.org/>`_.
 
 3.x
 ---
 
+3.3.0 (2024-05-29)
+^^^^^^^^^^^^^^^^^^
+
+*Added:*
+
+* Support numpy 2.0
+  (`#367 <https://github.com/glotzerlab/gsd/pull/367>`__).
+
+*Changed:*
+
+* Navigate the documentation with arrow keys
+  (`#365 <https://github.com/glotzerlab/gsd/pull/365>`__).
+* Add button to copy code snippets from the documentation
+  (`#365 <https://github.com/glotzerlab/gsd/pull/365>`__).
+* Remove singularity reference from the documentation
+  (`#365 <https://github.com/glotzerlab/gsd/pull/365>`__).
+
+*Removed:*
+
+* Support for Python 3.8
+  (`#367 <https://github.com/glotzerlab/gsd/pull/367>`__).
+
 3.2.1 (2024-01-22)
 ^^^^^^^^^^^^^^^^^^
 
 *Fixed:*
 
 * Write all pending index entries to the file when ``gsd_flush()`` is called after
   ``gsd_write_chunk()`` and before ``gsd_end_frame()``
```

### Comparing `gsd-3.2.1/LICENSE` & `gsd-3.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016-2023 The Regents of the University of Michigan
+Copyright (c) 2016-2024 The Regents of the University of Michigan
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `gsd-3.2.1/PKG-INFO` & `gsd-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 3.2.1
+Version: 3.3.0
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.2.1/gsd-3.2.1.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.3.0/gsd-3.3.0.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.9.3
+Requires-Dist: numpy>=1.19.0
 
 # GSD
 
 The **GSD** file format is the native file format for [HOOMD-blue](https://glotzerlab.engin.umich.edu/hoomd-blue/).
 **GSD** files store trajectories of the **HOOMD-blue** system state in a binary file with efficient random access to
 frames. **GSD** allows all particle and topology properties to vary from one frame to the next. Use the **GSD** Python
 API to specify the initial condition for a **HOOMD-blue** simulation or analyze trajectory output with a script. Read a
```

### Comparing `gsd-3.2.1/README.md` & `gsd-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gsd-3.2.1/gsd/__init__.py` & `gsd-3.3.0/gsd/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """The GSD main module.
 
 The main package :py:mod:`gsd` is the root package. It holds the submodules
 :py:mod:`gsd.fl` and :py:mod:`gsd.hoomd`, but does not import them by default.
 You must explicitly import these modules before use::
```

### Comparing `gsd-3.2.1/gsd/__main__.py` & `gsd-3.3.0/gsd/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """The GSD command line interface.
 
 To simplify ad hoc usage of :py:mod:`gsd`, this module provides a command line
 interface for interacting with GSD files. The primary entry point is a single
 command for starting a Python interpreter with a GSD file pre-loaded::
```

### Comparing `gsd-3.2.1/gsd/fl.c` & `gsd-3.3.0/gsd/fl.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/_core/include/numpy/arrayobject.h",
+            "/tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/_core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/_core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/_core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/_core/include/numpy/ufuncobject.h",
             "gsd/gsd.h"
         ],
         "include_dirs": [
             "gsd",
-            "/tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/_core/include"
         ],
         "name": "gsd.fl",
         "sources": [
             "gsd/fl.pyx",
             "gsd/gsd.c"
         ]
     },
@@ -51,18 +51,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -146,14 +146,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -207,14 +209,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -268,60 +272,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -404,14 +431,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -747,16 +777,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1100,15 +1135,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1187,15 +1222,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1303,32 +1338,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1565,200 +1583,164 @@
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":770
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":784
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
- * # The int types are mapped a bit surprising --
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
- * ctypedef npy_longlong   longlong_t
- */
-typedef npy_long __pyx_t_5numpy_int_t;
-
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+ * ctypedef double complex complex128_t
  * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_ulonglong  ulonglong_t
  * 
- * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
- * ctypedef npy_longlong   longlong_t
- * 
- * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
- * ctypedef npy_ulonglong  ulonglong_t
- */
-typedef npy_ulong __pyx_t_5numpy_uint_t;
-
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":793
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
+ * ctypedef npy_longlong   longlong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":795
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":796
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":798
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":799
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":800
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
- * ctypedef npy_cfloat      cfloat_t
+ * ctypedef float complex       cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 /* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
@@ -1778,54 +1760,48 @@
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* Declarations.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    typedef ::std::complex< long double > __pyx_t_long_double_complex;
+  #else
+    typedef long double _Complex __pyx_t_long_double_complex;
+  #endif
+#else
+    typedef struct { long double real, imag; } __pyx_t_long_double_complex;
+#endif
+static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double, long double);
+
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_3gsd_2fl_GSDFile;
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
- * ctypedef npy_longdouble longdouble_t
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1096
  * 
- * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t
- */
-typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
-
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
- * 
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
- * ctypedef npy_clongdouble clongdouble_t
- * 
- */
-typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
-
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil             # <<<<<<<<<<<<<<
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil
  * 
- * ctypedef npy_cdouble     complex_t
  */
-typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
+typedef int (*__pyx_t_5numpy_NpyIter_IterNextFunc)(NpyIter *);
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
- * ctypedef npy_clongdouble clongdouble_t
- * 
- * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1097
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil             # <<<<<<<<<<<<<<
  * 
- * cdef inline object PyArray_MultiIterNew1(a):
+ * cdef extern from "numpy/arrayobject.h":
  */
-typedef npy_cdouble __pyx_t_5numpy_complex_t;
+typedef void (*__pyx_t_5numpy_NpyIter_GetMultiIndexFunc)(NpyIter *, npy_intp *);
 
 /* "gsd/fl.pyx":229
  * 
  * 
  * cdef class GSDFile:             # <<<<<<<<<<<<<<
  *     """GSDFile
  * 
@@ -2362,30 +2338,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2686,14 +2662,52 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
+/* Arithmetic.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+    #define __Pyx_c_eq_long__double(a, b)   ((a)==(b))
+    #define __Pyx_c_sum_long__double(a, b)  ((a)+(b))
+    #define __Pyx_c_diff_long__double(a, b) ((a)-(b))
+    #define __Pyx_c_prod_long__double(a, b) ((a)*(b))
+    #define __Pyx_c_quot_long__double(a, b) ((a)/(b))
+    #define __Pyx_c_neg_long__double(a)     (-(a))
+  #ifdef __cplusplus
+    #define __Pyx_c_is_zero_long__double(z) ((z)==(long double)0)
+    #define __Pyx_c_conj_long__double(z)    (::std::conj(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (::std::abs(z))
+        #define __Pyx_c_pow_long__double(a, b)  (::std::pow(a, b))
+    #endif
+  #else
+    #define __Pyx_c_is_zero_long__double(z) ((z)==0)
+    #define __Pyx_c_conj_long__double(z)    (conjl(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (cabsl(z))
+        #define __Pyx_c_pow_long__double(a, b)  (cpowl(a, b))
+    #endif
+ #endif
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex);
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex);
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    #endif
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__gsd_error(enum gsd_error value);
 
 /* CIntToPy.proto */
@@ -2757,14 +2771,26 @@
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
@@ -2973,23 +2999,23 @@
 static const char __pyx_k_File_must_be_readable[] = "File must be readable: ";
 static const char __pyx_k_File_must_be_writable[] = "File must be writable: ";
 static const char __pyx_k_invalid_type_for_chunk[] = "invalid type for chunk: ";
 static const char __pyx_k_Memory_allocation_failed[] = "Memory allocation failed: ";
 static const char __pyx_k_find_matching_chunk_names[] = "find_matching_chunk_names";
 static const char __pyx_k_Unsupported_GSD_file_version[] = "Unsupported GSD file version: ";
 static const char __pyx_k_implicit_data_copy_when_writing[] = "implicit data copy when writing chunk: ";
-static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_GSDFile_find_matching_chunk_name[] = "GSDFile.find_matching_chunk_names";
 static const char __pyx_k_GSD_can_only_write_1_or_2_dimens[] = "GSD can only write 1 or 2 dimensional arrays: ";
 static const char __pyx_k_GSD_file_layer_API_Low_level_acc[] = "GSD file layer API.\n\nLow level access to gsd files. :py:mod:`gsd.fl` allows direct access to create,\nread, and write ``gsd`` files. The module is implemented in C and is optimized.\nSee :ref:`fl-examples` for detailed example code.\n\n* :py:class:`GSDFile` - Class interface to read and write gsd files.\n* :py:func:`open` - Open a gsd file.\n\n";
 static const char __pyx_k_Only_read_only_GSDFiles_can_be_p[] = "Only read only GSDFiles can be pickled.";
 static const char __pyx_k_Provide_application_when_creatin[] = "Provide application when creating a file";
 static const char __pyx_k_Provide_schema_version_when_crea[] = "Provide schema_version when creating a file";
 static const char __pyx_k_Provide_schema_when_creating_a_f[] = "Provide schema when creating a file";
-static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_numpy__core_multiarray_failed_to[] = "numpy._core.multiarray failed to import";
+static const char __pyx_k_numpy__core_umath_failed_to_impo[] = "numpy._core.umath failed to import";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_3gsd_2fl_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name, PyObject *__pyx_v_mode, PyObject *__pyx_v_application, PyObject *__pyx_v_schema, PyObject *__pyx_v_schema_version); /* proto */
 static int __pyx_pf_3gsd_2fl_7GSDFile___init__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_mode, PyObject *__pyx_v_application, PyObject *__pyx_v_schema, PyObject *__pyx_v_schema_version); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_2close(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4truncate(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_6end_frame(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_8flush(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
@@ -3193,16 +3219,16 @@
   PyObject *__pyx_n_s_match_e;
   PyObject *__pyx_n_s_mode;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_name_e;
   PyObject *__pyx_kp_u_not_found_in;
   PyObject *__pyx_n_s_numpy;
-  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_kp_u_numpy__core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy__core_umath_failed_to_impo;
   PyObject *__pyx_n_s_open;
   PyObject *__pyx_kp_u_opening_file;
   PyObject *__pyx_n_s_os;
   PyObject *__pyx_kp_u_overwriting_file;
   PyObject *__pyx_n_s_path;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_u_r;
@@ -3439,16 +3465,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_match_e);
   Py_CLEAR(clear_module_state->__pyx_n_s_mode);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_e);
   Py_CLEAR(clear_module_state->__pyx_kp_u_not_found_in);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_CLEAR(clear_module_state->__pyx_n_s_open);
   Py_CLEAR(clear_module_state->__pyx_kp_u_opening_file);
   Py_CLEAR(clear_module_state->__pyx_n_s_os);
   Py_CLEAR(clear_module_state->__pyx_kp_u_overwriting_file);
   Py_CLEAR(clear_module_state->__pyx_n_s_path);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_u_r);
@@ -3663,16 +3689,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_match_e);
   Py_VISIT(traverse_module_state->__pyx_n_s_mode);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_e);
   Py_VISIT(traverse_module_state->__pyx_kp_u_not_found_in);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_VISIT(traverse_module_state->__pyx_n_s_open);
   Py_VISIT(traverse_module_state->__pyx_kp_u_opening_file);
   Py_VISIT(traverse_module_state->__pyx_n_s_os);
   Py_VISIT(traverse_module_state->__pyx_kp_u_overwriting_file);
   Py_VISIT(traverse_module_state->__pyx_n_s_path);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_u_r);
@@ -3921,16 +3947,16 @@
 #define __pyx_n_s_match_e __pyx_mstate_global->__pyx_n_s_match_e
 #define __pyx_n_s_mode __pyx_mstate_global->__pyx_n_s_mode
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_name_e __pyx_mstate_global->__pyx_n_s_name_e
 #define __pyx_kp_u_not_found_in __pyx_mstate_global->__pyx_kp_u_not_found_in
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
-#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
-#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_kp_u_numpy__core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy__core_multiarray_failed_to
+#define __pyx_kp_u_numpy__core_umath_failed_to_impo __pyx_mstate_global->__pyx_kp_u_numpy__core_umath_failed_to_impo
 #define __pyx_n_s_open __pyx_mstate_global->__pyx_n_s_open
 #define __pyx_kp_u_opening_file __pyx_mstate_global->__pyx_kp_u_opening_file
 #define __pyx_n_s_os __pyx_mstate_global->__pyx_n_s_os
 #define __pyx_kp_u_overwriting_file __pyx_mstate_global->__pyx_kp_u_overwriting_file
 #define __pyx_n_s_path __pyx_mstate_global->__pyx_n_s_path
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_u_r __pyx_mstate_global->__pyx_n_u_r
@@ -3997,262 +4023,686 @@
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":287
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:
+ *             return PyDataType_ELSIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_ELSIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":291
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:
+ *             return PyDataType_ALIGNMENT(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use fields/names with care as they may be NULL.  You must check
+ */
+  __pyx_r = PyDataType_ALIGNMENT(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("fields", 1);
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":297
+ *         @property
+ *         cdef inline object fields(self):
+ *             return <object>PyDataType_FIELDS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_FIELDS(__pyx_v_self);
+  __Pyx_INCREF(((PyObject *)__pyx_t_1));
+  __pyx_r = ((PyObject *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("names", 1);
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":301
+ *         @property
+ *         cdef inline tuple names(self):
+ *             return <tuple>PyDataType_NAMES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use PyDataType_HASSUBARRAY to test whether this field is
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_NAMES(__pyx_v_self);
+  __Pyx_INCREF(((PyObject*)__pyx_t_1));
+  __pyx_r = ((PyObject*)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self) {
+  PyArray_ArrayDescr *__pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":308
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:
+ *             return PyDataType_SUBARRAY(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_SUBARRAY(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self) {
+  npy_uint64 __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":313
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyDataType_FLAGS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":325
+ *         cdef inline int numiter(self) noexcept nogil:
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NUMITER(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":330
+ *         cdef inline npy_intp size(self) noexcept nogil:
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":335
+ *         cdef inline npy_intp index(self) noexcept nogil:
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_INDEX(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":340
+ *         cdef inline int nd(self) noexcept nogil:
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":345
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self) {
+  void **__pyx_r;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":351
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ *             return PyArray_MultiIter_ITERS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyArray_MultiIter_ITERS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":369
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":375
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":381
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":389
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":396
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":402
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":411
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
- *     ctypedef unsigned char      npy_bool
+ * 
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
- * ctypedef npy_cdouble     complex_t
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
@@ -4260,30 +4710,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":808
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
- * ctypedef npy_cdouble     complex_t
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
   /* function exit code */
@@ -4293,15 +4743,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4310,29 +4760,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":811
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4343,15 +4793,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4360,29 +4810,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":814
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4393,15 +4843,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4410,29 +4860,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":817
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4443,15 +4893,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4460,29 +4910,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":820
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4493,209 +4943,219 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  PyObject *__pyx_t_2;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":824
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    __pyx_t_2 = __pyx_f_5numpy_5dtype_8subarray_subarray(__pyx_v_d)->shape;
+    __Pyx_INCREF(((PyObject*)__pyx_t_2));
+    __pyx_r = ((PyObject*)__pyx_t_2);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":826
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  * 
- * cdef inline void set_array_base(ndarray arr, object base):
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
- * cdef inline void set_array_base(ndarray arr, object base):
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1012
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 1012, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1015
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1017
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1018
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4711,15 +5171,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4727,68 +5187,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1024
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1024, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1025
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1025, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1026, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 986, __pyx_L5_except_error)
+      __PYX_ERR(1, 1026, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4796,15 +5256,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4819,16 +5279,16 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
- *         raise ImportError("numpy.core.multiarray failed to import")
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
@@ -4843,15 +5303,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4859,68 +5319,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1030
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1030, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1031
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1031, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1032, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 992, __pyx_L5_except_error)
+      __PYX_ERR(1, 1032, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4928,16 +5388,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
- *         raise ImportError("numpy.core.multiarray failed to import")
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -4951,16 +5411,16 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
- *         raise ImportError("numpy.core.umath failed to import")
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
@@ -4975,15 +5435,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4991,68 +5451,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1036, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1037
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1037, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1038
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1038, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 998, __pyx_L5_except_error)
+      __PYX_ERR(1, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5060,16 +5520,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -5083,173 +5543,175 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1053
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1068
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1078
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1085
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1092
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -15162,16 +15624,16 @@
     {&__pyx_n_s_match_e, __pyx_k_match_e, sizeof(__pyx_k_match_e), 0, 0, 1, 1},
     {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_name_e, __pyx_k_name_e, sizeof(__pyx_k_name_e), 0, 0, 1, 1},
     {&__pyx_kp_u_not_found_in, __pyx_k_not_found_in, sizeof(__pyx_k_not_found_in), 0, 1, 0, 0},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_multiarray_failed_to, __pyx_k_numpy__core_multiarray_failed_to, sizeof(__pyx_k_numpy__core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_umath_failed_to_impo, __pyx_k_numpy__core_umath_failed_to_impo, sizeof(__pyx_k_numpy__core_umath_failed_to_impo), 0, 1, 0, 0},
     {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
     {&__pyx_kp_u_opening_file, __pyx_k_opening_file, sizeof(__pyx_k_opening_file), 0, 1, 0, 0},
     {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
     {&__pyx_kp_u_overwriting_file, __pyx_k_overwriting_file, sizeof(__pyx_k_overwriting_file), 0, 1, 0, 0},
     {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
@@ -15216,44 +15678,44 @@
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_IOError = __Pyx_GetBuiltinName(__pyx_n_s_IOError); if (!__pyx_builtin_IOError) __PYX_ERR(0, 43, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 51, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 314, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 753, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 986, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1026, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy__core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 1026, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-ueh7eqhp/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-tvetsta_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_umath_failed_to_impo); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 1032, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "gsd/fl.pyx":326
  *         if overwrite:
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")             # <<<<<<<<<<<<<<
@@ -15567,41 +16029,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 812, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 814, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 816, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 818, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 820, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 822, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 824, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 826, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 828, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 830, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 868, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 271, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 316, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 320, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 359, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 848, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 850, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 852, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 854, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 856, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 858, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 860, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 862, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 864, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 930, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -16155,15 +16617,15 @@
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3gsd_2fl_7GSDFile_25__reduce__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_GSDFile___reduce, NULL, __pyx_n_s_gsd_fl, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 925, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile, __pyx_n_s_reduce, __pyx_t_3) < 0) __PYX_ERR(0, 925, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3gsd_2fl_GSDFile);
 
   /* "gsd/fl.pyx":1
- * # Copyright (c) 2016-2023 The Regents of the University of Michigan             # <<<<<<<<<<<<<<
+ * # Copyright (c) 2016-2024 The Regents of the University of Michigan             # <<<<<<<<<<<<<<
  * # Part of GSD, released under the BSD 2-Clause License.
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -18985,18 +19447,18 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -19042,23 +19504,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -20279,15 +20741,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -21142,14 +21604,168 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
+/* Declarations */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return ::std::complex< long double >(x, y);
+    }
+  #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return x + y*(__pyx_t_long_double_complex)_Complex_I;
+    }
+  #endif
+#else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      __pyx_t_long_double_complex z;
+      z.real = x;
+      z.imag = y;
+      return z;
+    }
+#endif
+
+/* Arithmetic */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+       return (a.real == b.real) && (a.imag == b.imag);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real + b.real;
+        z.imag = a.imag + b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real - b.real;
+        z.imag = a.imag - b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real * b.real - a.imag * b.imag;
+        z.imag = a.real * b.imag + a.imag * b.real;
+        return z;
+    }
+    #if 1
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else if (fabsl(b.real) >= fabsl(b.imag)) {
+            if (b.real == 0 && b.imag == 0) {
+                return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.imag);
+            } else {
+                long double r = b.imag / b.real;
+                long double s = (long double)(1.0) / (b.real + b.imag * r);
+                return __pyx_t_long_double_complex_from_parts(
+                    (a.real + a.imag * r) * s, (a.imag - a.real * r) * s);
+            }
+        } else {
+            long double r = b.real / b.imag;
+            long double s = (long double)(1.0) / (b.imag + b.real * r);
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * r + a.imag) * s, (a.imag * r - a.real) * s);
+        }
+    }
+    #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else {
+            long double denom = b.real * b.real + b.imag * b.imag;
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * b.real + a.imag * b.imag) / denom,
+                (a.imag * b.real - a.real * b.imag) / denom);
+        }
+    }
+    #endif
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real = -a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex a) {
+       return (a.real == 0) && (a.imag == 0);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real =  a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex z) {
+          #if !defined(HAVE_HYPOT) || defined(_MSC_VER)
+            return sqrtl(z.real*z.real + z.imag*z.imag);
+          #else
+            return hypotl(z.real, z.imag);
+          #endif
+        }
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+            __pyx_t_long_double_complex z;
+            long double r, lnr, theta, z_r, z_theta;
+            if (b.imag == 0 && b.real == (int)b.real) {
+                if (b.real < 0) {
+                    long double denom = a.real * a.real + a.imag * a.imag;
+                    a.real = a.real / denom;
+                    a.imag = -a.imag / denom;
+                    b.real = -b.real;
+                }
+                switch ((int)b.real) {
+                    case 0:
+                        z.real = 1;
+                        z.imag = 0;
+                        return z;
+                    case 1:
+                        return a;
+                    case 2:
+                        return __Pyx_c_prod_long__double(a, a);
+                    case 3:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, a);
+                    case 4:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, z);
+                }
+            }
+            if (a.imag == 0) {
+                if (a.real == 0) {
+                    return a;
+                } else if ((b.imag == 0) && (a.real >= 0)) {
+                    z.real = powl(a.real, b.real);
+                    z.imag = 0;
+                    return z;
+                } else if (a.real > 0) {
+                    r = a.real;
+                    theta = 0;
+                } else {
+                    r = -a.real;
+                    theta = atan2l(0.0, -1.0);
+                }
+            } else {
+                r = __Pyx_c_abs_long__double(a);
+                theta = atan2l(a.imag, a.real);
+            }
+            lnr = logl(r);
+            z_r = expl(lnr * b.real - theta * b.imag);
+            z_theta = theta * b.real + lnr * b.imag;
+            z.real = z_r * cosl(z_theta);
+            z.imag = z_r * sinl(z_theta);
+            return z;
+        }
+    #endif
+#endif
+
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
```

### Comparing `gsd-3.2.1/gsd/fl.pyx` & `gsd-3.3.0/gsd/fl.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """GSD file layer API.
 
 Low level access to gsd files. :py:mod:`gsd.fl` allows direct access to create,
 read, and write ``gsd`` files. The module is implemented in C and is optimized.
 See :ref:`fl-examples` for detailed example code.
```

### Comparing `gsd-3.2.1/gsd/gsd.c` & `gsd-3.3.0/gsd/gsd.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2023 The Regents of the University of Michigan
+// Copyright (c) 2016-2024 The Regents of the University of Michigan
 // Part of GSD, released under the BSD 2-Clause License.
 
 #include <sys/stat.h>
 #ifdef _WIN32
 
 #pragma warning(push)
 #pragma warning(disable : 4996)
```

### Comparing `gsd-3.2.1/gsd/gsd.h` & `gsd-3.3.0/gsd/gsd.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2016-2023 The Regents of the University of Michigan
+// Copyright (c) 2016-2024 The Regents of the University of Michigan
 // Part of GSD, released under the BSD 2-Clause License.
 
 #ifndef GSD_H
 #define GSD_H
 
 #include <stdbool.h>
 #include <stdint.h>
```

### Comparing `gsd-3.2.1/gsd/hoomd.py` & `gsd-3.3.0/gsd/hoomd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Read and write HOOMD schema GSD files.
 
 :py:mod:`gsd.hoomd` reads and writes GSD files with the ``hoomd`` schema.
 
 * `HOOMDTrajectory` - Read and write hoomd schema GSD files.
@@ -547,28 +547,29 @@
                 self.state['hpmc/convex_spheropolyhedron/N'], dtype=numpy.uint32
             )
             self.state['hpmc/convex_spheropolyhedron/N'] = self.state[
                 'hpmc/convex_spheropolyhedron/N'
             ].reshape([NT])
             sumN = numpy.sum(self.state['hpmc/convex_spheropolyhedron/N'])
 
-            self.state[
-                'hpmc/convex_spheropolyhedron/sweep_radius'
-            ] = numpy.ascontiguousarray(
-                self.state['hpmc/convex_spheropolyhedron/sweep_radius'],
-                dtype=numpy.float32,
+            self.state['hpmc/convex_spheropolyhedron/sweep_radius'] = (
+                numpy.ascontiguousarray(
+                    self.state['hpmc/convex_spheropolyhedron/sweep_radius'],
+                    dtype=numpy.float32,
+                )
             )
             self.state['hpmc/convex_spheropolyhedron/sweep_radius'] = self.state[
                 'hpmc/convex_spheropolyhedron/sweep_radius'
             ].reshape([NT])
 
-            self.state[
-                'hpmc/convex_spheropolyhedron/vertices'
-            ] = numpy.ascontiguousarray(
-                self.state['hpmc/convex_spheropolyhedron/vertices'], dtype=numpy.float32
+            self.state['hpmc/convex_spheropolyhedron/vertices'] = (
+                numpy.ascontiguousarray(
+                    self.state['hpmc/convex_spheropolyhedron/vertices'],
+                    dtype=numpy.float32,
+                )
             )
             self.state['hpmc/convex_spheropolyhedron/vertices'] = self.state[
                 'hpmc/convex_spheropolyhedron/vertices'
             ].reshape([sumN, 3])
 
         if 'hpmc/convex_polygon/N' in self.state:
             self.state['hpmc/convex_polygon/N'] = numpy.ascontiguousarray(
@@ -591,19 +592,19 @@
                 self.state['hpmc/convex_spheropolygon/N'], dtype=numpy.uint32
             )
             self.state['hpmc/convex_spheropolygon/N'] = self.state[
                 'hpmc/convex_spheropolygon/N'
             ].reshape([NT])
             sumN = numpy.sum(self.state['hpmc/convex_spheropolygon/N'])
 
-            self.state[
-                'hpmc/convex_spheropolygon/sweep_radius'
-            ] = numpy.ascontiguousarray(
-                self.state['hpmc/convex_spheropolygon/sweep_radius'],
-                dtype=numpy.float32,
+            self.state['hpmc/convex_spheropolygon/sweep_radius'] = (
+                numpy.ascontiguousarray(
+                    self.state['hpmc/convex_spheropolygon/sweep_radius'],
+                    dtype=numpy.float32,
+                )
             )
             self.state['hpmc/convex_spheropolygon/sweep_radius'] = self.state[
                 'hpmc/convex_spheropolygon/sweep_radius'
             ].reshape([NT])
 
             self.state['hpmc/convex_spheropolygon/vertices'] = numpy.ascontiguousarray(
                 self.state['hpmc/convex_spheropolygon/vertices'], dtype=numpy.float32
```

### Comparing `gsd-3.2.1/gsd/libgsd.pxd` & `gsd-3.3.0/gsd/libgsd.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 from libc.stdint cimport uint8_t, int8_t, uint16_t, int16_t, uint32_t, int32_t,\
     uint64_t, int64_t
 
 cdef extern from "gsd.h" nogil:
     cdef enum gsd_type:
```

### Comparing `gsd-3.2.1/gsd/pygsd.py` & `gsd-3.3.0/gsd/pygsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """GSD reader written in pure Python.
 
 :file:`pygsd.py` is a pure Python implementation of a GSD reader. If your
 analysis tool is written in Python and you want to embed a GSD reader without
 requiring C code compilation or require the **gsd** Python package as a
@@ -32,15 +32,15 @@
 import logging
 import struct
 import sys
 from collections import namedtuple
 
 import numpy
 
-version = '3.2.1'
+version = '3.3.0'
 
 logger = logging.getLogger('gsd.pygsd')
 
 gsd_header = namedtuple(
     'gsd_header',
     'magic index_location index_allocated_entries '
     'namelist_location namelist_allocated_entries '
```

### Comparing `gsd-3.2.1/gsd/pytest_plugin_validate.py` & `gsd-3.3.0/gsd/pytest_plugin_validate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Command line options for pytest."""
 
 import pytest
```

### Comparing `gsd-3.2.1/gsd/test/conftest.py` & `gsd-3.3.0/gsd/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Pytest fixtures common to all tests."""
 
 import collections
 
 import pytest
```

### Comparing `gsd-3.2.1/gsd/test/test_fl.py` & `gsd-3.3.0/gsd/test/test_fl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Test gsd.fl."""
 
 import os
 import pathlib
 import platform
@@ -401,17 +401,16 @@
             f.write_chunk(name='chunk1', data=data)
 
         f.end_frame()
 
 
 def test_truncate(tmp_path):
     """Test that the truncate method functions."""
-    data = numpy.ascontiguousarray(
-        numpy.random.random(size=(1000, 3)), dtype=numpy.float32
-    )
+    rng = numpy.random.default_rng()
+    data = numpy.ascontiguousarray(rng.random(size=(1000, 3)), dtype=numpy.float32)
     with gsd.fl.open(
         name=tmp_path / 'test_truncate.gsd',
         mode='w',
         application='test_truncate',
         schema='none',
         schema_version=[1, 2],
     ) as f:
```

### Comparing `gsd-3.2.1/gsd/test/test_gsd_v1.gsd` & `gsd-3.3.0/gsd/test/test_gsd_v1.gsd`

 * *Files identical despite different names*

### Comparing `gsd-3.2.1/gsd/test/test_hoomd.py` & `gsd-3.3.0/gsd/test/test_hoomd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Test the gsd.hoomd API."""
 
 import pickle
 
 import numpy
```

### Comparing `gsd-3.2.1/gsd/test/test_largefile.py` & `gsd-3.3.0/gsd/test/test_largefile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Test the gsd.fl API with large files."""
 
 import gc
 
 import numpy
```

### Comparing `gsd-3.2.1/gsd.egg-info/PKG-INFO` & `gsd-3.3.0/gsd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 3.2.1
+Version: 3.3.0
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.2.1/gsd-3.2.1.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.3.0/gsd-3.3.0.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.9.3
+Requires-Dist: numpy>=1.19.0
 
 # GSD
 
 The **GSD** file format is the native file format for [HOOMD-blue](https://glotzerlab.engin.umich.edu/hoomd-blue/).
 **GSD** files store trajectories of the **HOOMD-blue** system state in a binary file with efficient random access to
 frames. **GSD** allows all particle and topology properties to vary from one frame to the next. Use the **GSD** Python
 API to specify the initial condition for a **HOOMD-blue** simulation or analyze trajectory output with a script. Read a
```

### Comparing `gsd-3.2.1/gsd.egg-info/SOURCES.txt` & `gsd-3.3.0/gsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsd-3.2.1/pyproject.toml` & `gsd-3.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">=3.6"
 name = "gsd"
-version = "3.2.1"
+version = "3.3.0"
 description = "General simulation data file format."
 readme = "README.md"
 license = {text = "BSD-2-Clause"}
 authors = [
     {name = "Joshua A. Anderson", email = "joaander@umich.edu"},
 ]
 classifiers=[
@@ -13,47 +13,38 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX",
     "License :: OSI Approved :: BSD License",
     "Topic :: Scientific/Engineering :: Physics",
     ]
-dependencies = ["numpy>=1.9.3"]
+dependencies = ["numpy>=1.19.0"]
 
 [project.scripts]
 gsd = "gsd.__main__:main"
 
 [project.urls]
 Homepage = "https://gsd.readthedocs.io"
 Documentation = "https://gsd.readthedocs.io"
-Download = "https://github.com/glotzerlab/gsd/releases/download/v3.2.1/gsd-3.2.1.tar.gz"
+Download = "https://github.com/glotzerlab/gsd/releases/download/v3.3.0/gsd-3.3.0.tar.gz"
 Source = "https://github.com/glotzerlab/gsd"
 Issues = "https://github.com/glotzerlab/gsd/issues"
 
 [tool.setuptools]
 packages = ["gsd", "gsd.test"]
 
 [build-system]
 requires = ["setuptools>=64.0.0",
             "wheel",
             "Cython",
-            "oldest-supported-numpy"]
+            "numpy>=2.0.0rc1"]
 
 [tool.cibuildwheel]
-# Build for cpython only
-skip =  "pp*"
-
 # Test the wheels.
 test-command = "pytest --pyargs gsd -v --log-level=DEBUG"
-test-skip = "*-macosx_arm64"
-test-requires = "pytest"
 
-# Build only on 64-bit architectures.
+# Build on 64-bit architectures.
 archs = ["auto64"]
 
-[tool.cibuildwheel.macos]
-# Build for x86_64 and arm64
-archs = ["x86_64", "arm64"]
-
 [tool.cibuildwheel.linux]
 # dependencies do not build for musl
 skip = ["pp* *musllinux*"]
```

### Comparing `gsd-3.2.1/setup.py` & `gsd-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2023 The Regents of the University of Michigan
+# Copyright (c) 2016-2024 The Regents of the University of Michigan
 # Part of GSD, released under the BSD 2-Clause License.
 
 """Install gsd."""
 
 import numpy
 from Cython.Build import cythonize
 from setuptools import setup
```

