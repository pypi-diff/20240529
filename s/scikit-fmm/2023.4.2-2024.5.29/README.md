# Comparing `tmp/scikit-fmm-2023.4.2.tar.gz` & `tmp/scikit_fmm-2024.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-fmm-2023.4.2.tar", last modified: Mon Apr  3 14:01:20 2023, max compression
+gzip compressed data, was "scikit_fmm-2024.5.29.tar", last modified: Wed May 29 20:06:46 2024, max compression
```

## Comparing `scikit-fmm-2023.4.2.tar` & `scikit_fmm-2024.5.29.tar`

### file list

```diff
@@ -1,55 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:01:20.443215 scikit-fmm-2023.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-03 14:01:20.443215 scikit-fmm-2023.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:01:20.439215 scikit-fmm-2023.4.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/2d_phi.png
--rw-r--r--   0 runner    (1001) docker     (123)    37689 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/2d_phi_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)    47191 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/2d_phi_distance_narrow.png
--rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/2d_phi_travel_time.png
--rw-r--r--   0 runner    (1001) docker     (123)    54550 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/2d_phi_travel_time_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26693 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/extension_velocity.png
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/periodic.png
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/doc/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:01:20.439215 scikit-fmm-2023.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/examples/2d_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/examples/boundaryconditions_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/examples/extension_velocities_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:01:20.439215 scikit-fmm-2023.4.2/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/profile/prof.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/profile/prof.sh
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/profile/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:01:20.443215 scikit-fmm-2023.4.2/scikit_fmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-03 14:01:20.000000 scikit-fmm-2023.4.2/scikit_fmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-03 14:01:20.000000 scikit-fmm-2023.4.2/scikit_fmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:01:20.000000 scikit-fmm-2023.4.2/scikit_fmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-03 14:01:20.000000 scikit-fmm-2023.4.2/scikit_fmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-03 14:01:20.000000 scikit-fmm-2023.4.2/scikit_fmm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:01:20.443215 scikit-fmm-2023.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:01:20.443215 scikit-fmm-2023.4.2/skfmm/
--rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/base_marcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/base_marcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/distance_marcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/distance_marcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/extension_velocity_marcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/extension_velocity_marcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/fmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/heap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/heap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/pfmm.py
--rw-r--r--   0 runner    (1001) docker     (123)   166640 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/pheap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/pheap.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/travel_time_marcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/skfmm/travel_time_marcher.h
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-03 14:00:45.000000 scikit-fmm-2023.4.2/static_analysis.sh
+-rw-r--r--   0        0        0     1018 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1092 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/.github/workflows/windows_build.yaml
+-rw-r--r--   0        0        0      249 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/.gitignore
+-rw-r--r--   0        0        0      577 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/.readthedocs.yaml
+-rw-r--r--   0        0        0      326 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/CONTRIBUTORS.txt
+-rw-r--r--   0        0        0     1540 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/LICENSE.txt
+-rw-r--r--   0        0        0      456 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/MANIFEST.in
+-rw-r--r--   0        0        0     5561 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/Makefile
+-rw-r--r--   0        0        0    10229 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/README.md
+-rw-r--r--   0        0        0     1404 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/dev_notes.org
+-rw-r--r--   0        0        0    16540 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/2d_phi.png
+-rw-r--r--   0        0        0    37689 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/2d_phi_distance.png
+-rw-r--r--   0        0        0    47191 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/2d_phi_distance_narrow.png
+-rw-r--r--   0        0        0    50648 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/2d_phi_travel_time.png
+-rw-r--r--   0        0        0    54550 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/2d_phi_travel_time_mask.png
+-rw-r--r--   0        0        0     8634 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/conf.py
+-rw-r--r--   0        0        0        8 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/doc.pip
+-rw-r--r--   0        0        0      385 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/examples.rst
+-rw-r--r--   0        0        0    26693 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/extension_velocity.png
+-rw-r--r--   0        0        0     5531 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/index.rst
+-rw-r--r--   0        0        0   153658 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/periodic.png
+-rw-r--r--   0        0        0       15 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/requirements.txt
+-rw-r--r--   0        0        0       60 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/doc/testing.rst
+-rw-r--r--   0        0        0     1617 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/examples/2d_example.py
+-rw-r--r--   0        0        0     1092 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/examples/boundaryconditions_example.py
+-rw-r--r--   0        0        0      764 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/examples/extension_velocities_example.py
+-rw-r--r--   0        0        0     1224 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/meson.build
+-rw-r--r--   0        0        0      169 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/profile/.gitignore
+-rw-r--r--   0        0        0      706 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/profile/prof.cpp
+-rw-r--r--   0        0        0     1339 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/profile/prof.sh
+-rw-r--r--   0        0        0      714 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/profile/profile.py
+-rw-r--r--   0        0        0      935 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/pyproject.toml
+-rw-r--r--   0        0        0    33496 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/__init__.py
+-rw-r--r--   0        0        0     5704 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/base_marcher.cpp
+-rw-r--r--   0        0        0     3072 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/base_marcher.h
+-rw-r--r--   0        0        0     4284 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/distance_marcher.cpp
+-rw-r--r--   0        0        0      782 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/distance_marcher.h
+-rw-r--r--   0        0        0     4184 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/extension_velocity_marcher.cpp
+-rw-r--r--   0        0        0      907 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/extension_velocity_marcher.h
+-rw-r--r--   0        0        0     8807 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/fmm.cpp
+-rw-r--r--   0        0        0     5728 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/heap.cpp
+-rw-r--r--   0        0        0     2936 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/heap.h
+-rw-r--r--   0        0        0     4872 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/heap.py
+-rw-r--r--   0        0        0     9689 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/pfmm.py
+-rw-r--r--   0        0        0   335061 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/pheap.cpp
+-rw-r--r--   0        0        0      941 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/pheap.pyx
+-rw-r--r--   0        0        0     3533 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/travel_time_marcher.cpp
+-rw-r--r--   0        0        0     1132 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/skfmm/travel_time_marcher.h
+-rw-r--r--   0        0        0       77 2024-05-29 20:05:40.000000 scikit_fmm-2024.5.29/static_analysis.sh
+-rw-r--r--   0        0        0    12660 2024-05-29 20:06:46.147436 scikit_fmm-2024.5.29/PKG-INFO
```

### Comparing `scikit-fmm-2023.4.2/LICENSE.txt` & `scikit_fmm-2024.5.29/LICENSE.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Unless otherwise specified by LICENSE.txt files in individual
 directories, all code is
 
-Copyright (C) 2022 the scikit-fmm team
+Copyright (C) 2024 the scikit-fmm team
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
  1. Redistributions of source code must retain the above copyright
```

### Comparing `scikit-fmm-2023.4.2/Makefile` & `scikit_fmm-2024.5.29/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/README.md` & `scikit_fmm-2024.5.29/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Linux build](https://github.com/scikit-fmm/scikit-fmm/actions/workflows/build.yaml/badge.svg) ![Windows build](https://github.com/scikit-fmm/scikit-fmm/actions/workflows/windows_build.yaml/badge.svg) [![PyPI version](https://badge.fury.io/py/scikit-fmm.svg)](http://pypi.python.org/pypi/scikit-fmm)[![Documentation Status](https://readthedocs.org/projects/scikit-fmm/badge/?version=latest)](https://scikit-fmm.readthedocs.io/en/latest/?badge=latest)<a href="https://pepy.tech/project/scikit-fmm"><img alt="Downloads" src="https://pepy.tech/badge/scikit-fmm"></a>
+![Linux build](https://github.com/scikit-fmm/scikit-fmm/actions/workflows/build.yaml/badge.svg) ![Windows build](https://github.com/scikit-fmm/scikit-fmm/actions/workflows/windows_build.yaml/badge.svg) [![PyPI version](https://badge.fury.io/py/scikit-fmm.svg)](http://pypi.python.org/pypi/scikit-fmm)[![Documentation Status](https://readthedocs.org/projects/scikit-fmm/badge/?version=latest)](https://scikit-fmm.readthedocs.io/en/latest/?badge=latest) ![Contributors](https://img.shields.io/github/contributors/scikit-fmm/scikit-fmm.svg)<a href="https://pepy.tech/project/scikit-fmm"><img alt="Downloads" src="https://pepy.tech/badge/scikit-fmm"></a>
 
 # scikit-fmm: the fast marching method for Python
 
 `scikit-fmm` is a Python extension module which implements the fast marching method.
 The fast marching method is used to model the evolution of boundaries
 and interfaces in a variety of application areas. More specifically,
 the fast marching method is a numerical technique for finding
@@ -46,44 +46,47 @@
    ```
 ---
 
 The input array can be of 1, 2, 3 or higher dimensions and can be a
 masked array. A function is provided to compute extension velocities.
 
 ### Documentation
-* http://scikit-fmm.readthedocs.org/en/latest/
+* http://scikit-fmm.readthedocs.org/en/master/
 
 ### PyPI
 * http://pypi.python.org/pypi/scikit-fmm
 
 ### Requirements
 * Numpy >= 1.0.2
-* Building requires a C/C++ compiler (gcc, MinGW, MSVC)
-
+* Building requires the pypa/build module
+  (https://github.com/pypa/build) and a C/C++ compiler
 ### Bugs, questions, patches, feature requests, discussion & cetera
 * Open a GitHub pull request or a GitHub issue
 * Email list: http://groups.google.com/group/scikit-fmm
   * Send an email to scikit-fmm+subscribe@googlegroups.com to subscribe.
 
 ### Installing
 * Via pip: `pip install scikit-fmm`
-* From source:
-  * `python setup.py install`
 * 64-bit Windows binaries from Christoph Gohlke:
   * http://www.lfd.uci.edu/~gohlke/pythonlibs/#scikit-fmm
 * Anaconda linux-64 and linux-ppc64le packages:
   * `conda install scikit-fmm`
 * Ubuntu PPA
   * https://launchpad.net/~nvidia-digits/+archive/ubuntu/dev
 * Debian
   * https://tracker.debian.org/pkg/scikit-fmm
 
+### Building and installing from Source
+* `pip install build`
+* `python -m build`
+* `pip install .`
+
+
 ### Running Tests
-* `python -c "import skfmm; skfmm.test(True)"`
-* When running the tests from the source directory use `python setup.py develop`
+* `python -c "import skfmm; skfmm.test(True)"` (Do not run the tests from the source directory.)
 * Tests are doctests in `skfmm/__init__.py`
 
 ### Building documentation
 * Requires sphinx and numpydoc
 * `make html`
 
 ### Publications using scikit-fmm
@@ -225,12 +228,16 @@
 * 2022.08.15 August 15th 2022
    * Following the breaking changes in setuptools v65 pin setuptools
      to v64
    * (DorSSS)
 * 2022.04.02 April 2nd 2023
    * Build fixes for Python 3.11 (update pheap cython wrapper)
    * No solver changes
+* 2024.05.29 May 29th 2024
+   * Update build system to use meson
+   * Python 3.12 support
+   * No solver changes
 
 
 Copyright 2023 The scikit-fmm team.
 
 BSD-style license. See LICENSE.txt in the source directory.
```

#### html2text {}

```diff
@@ -1,57 +1,59 @@
 ![Linux build](https://github.com/scikit-fmm/scikit-fmm/actions/workflows/
 build.yaml/badge.svg) ![Windows build](https://github.com/scikit-fmm/scikit-
 fmm/actions/workflows/windows_build.yaml/badge.svg) [![PyPI version](https://
 badge.fury.io/py/scikit-fmm.svg)](http://pypi.python.org/pypi/scikit-fmm)[!
 [Documentation Status](https://readthedocs.org/projects/scikit-fmm/badge/
-?version=latest)](https://scikit-fmm.readthedocs.io/en/latest/?badge=latest)
-_[_D_o_w_n_l_o_a_d_s_] # scikit-fmm: the fast marching method for Python `scikit-fmm` is a
-Python extension module which implements the fast marching method. The fast
-marching method is used to model the evolution of boundaries and interfaces in
-a variety of application areas. More specifically, the fast marching method is
-a numerical technique for finding approximate solutions to boundary value
-problems of the Eikonal equation: F(x) | grad T(x) | = 1 Typically, such a
-problem describes the evolution of a closed curve as a function of time T with
-speed F(x)>0 in the normal direction at a point x on the curve. The speed
-function is specified, and the time at which the contour crosses a point x is
-obtained by solving the equation. scikit-fmm is a simple module which provides
-functions to calculate the signed distance and travel time to an interface
-described by the zero contour of the input array phi. ```python import skfmm
-import numpy as np phi = np.ones((3, 3)) phi[1, 1] = -1 skfmm.distance(phi) ```
-```python array([[ 1.20710678, 0.5 , 1.20710678], [ 0.5 , -0.35355339, 0.5 ],
-[ 1.20710678, 0.5 , 1.20710678]]) ``` --- ```python skfmm.travel_time(phi,
-speed = 3.0 * np.ones_like(phi)) ``` ```python array([[ 0.40236893, 0.16666667,
-0.40236893], [ 0.16666667, 0.11785113, 0.16666667], [ 0.40236893, 0.16666667,
-0.40236893]]) ``` --- The input array can be of 1, 2, 3 or higher dimensions
-and can be a masked array. A function is provided to compute extension
-velocities. ### Documentation * http://scikit-fmm.readthedocs.org/en/latest/
-### PyPI * http://pypi.python.org/pypi/scikit-fmm ### Requirements * Numpy >=
-1.0.2 * Building requires a C/C++ compiler (gcc, MinGW, MSVC) ### Bugs,
-questions, patches, feature requests, discussion & cetera * Open a GitHub pull
-request or a GitHub issue * Email list: http://groups.google.com/group/scikit-
-fmm * Send an email to scikit-fmm+subscribe@googlegroups.com to subscribe. ###
-Installing * Via pip: `pip install scikit-fmm` * From source: * `python
-setup.py install` * 64-bit Windows binaries from Christoph Gohlke: * http://
-www.lfd.uci.edu/~gohlke/pythonlibs/#scikit-fmm * Anaconda linux-64 and linux-
-ppc64le packages: * `conda install scikit-fmm` * Ubuntu PPA * https://
-launchpad.net/~nvidia-digits/+archive/ubuntu/dev * Debian * https://
-tracker.debian.org/pkg/scikit-fmm ### Running Tests * `python -c "import skfmm;
-skfmm.test(True)"` * When running the tests from the source directory use
-`python setup.py develop` * Tests are doctests in `skfmm/__init__.py` ###
-Building documentation * Requires sphinx and numpydoc * `make html` ###
-Publications using scikit-fmm * Akinola, I., J Varley, B. Chen, and P.K. Allen
-(2018) "Workspace Aware Online Grasp Planning" arXiv:1806.11402v1 [cs.RO] 29
-Jun 2018 https://arxiv.org/pdf/1806.11402.pdf * Bortolussi, V., B. Figliuzzi,
-F. Willot, M. Faessel, M. Jeandin (2018) "Morphological modeling of cold spray
-coatings" Image Anal Stereol 2018;37:145-158 doi:10.5566/ias.1894 https://
-hal.archives-ouvertes.fr/hal-01837906/document * Chalmers, S., C.D. Saunter,
-J.M. Girkin and J.G. McCarron (2016) "Age decreases mitochondrial motility and
-increases mitochondrial size in vascular smooth muscle." Journal of Physiology,
-594.15 pp 4283â4295. * Diogo BrandÃ£o Amorim (2014) "Efficient path planning
-of a mobile robot on rough terrain" Master's Thesis, Department of Aerospace
+?version=latest)](https://scikit-fmm.readthedocs.io/en/latest/?badge=latest) !
+[Contributors](https://img.shields.io/github/contributors/scikit-fmm/scikit-
+fmm.svg)_[_D_o_w_n_l_o_a_d_s_] # scikit-fmm: the fast marching method for Python `scikit-
+fmm` is a Python extension module which implements the fast marching method.
+The fast marching method is used to model the evolution of boundaries and
+interfaces in a variety of application areas. More specifically, the fast
+marching method is a numerical technique for finding approximate solutions to
+boundary value problems of the Eikonal equation: F(x) | grad T(x) | = 1
+Typically, such a problem describes the evolution of a closed curve as a
+function of time T with speed F(x)>0 in the normal direction at a point x on
+the curve. The speed function is specified, and the time at which the contour
+crosses a point x is obtained by solving the equation. scikit-fmm is a simple
+module which provides functions to calculate the signed distance and travel
+time to an interface described by the zero contour of the input array phi.
+```python import skfmm import numpy as np phi = np.ones((3, 3)) phi[1, 1] = -
+1 skfmm.distance(phi) ``` ```python array([[ 1.20710678, 0.5 , 1.20710678],
+[ 0.5 , -0.35355339, 0.5 ], [ 1.20710678, 0.5 , 1.20710678]]) ``` --- ```python
+skfmm.travel_time(phi, speed = 3.0 * np.ones_like(phi)) ``` ```python array([
+[ 0.40236893, 0.16666667, 0.40236893], [ 0.16666667, 0.11785113, 0.16666667],
+[ 0.40236893, 0.16666667, 0.40236893]]) ``` --- The input array can be of 1, 2,
+3 or higher dimensions and can be a masked array. A function is provided to
+compute extension velocities. ### Documentation * http://scikit-
+fmm.readthedocs.org/en/master/ ### PyPI * http://pypi.python.org/pypi/scikit-
+fmm ### Requirements * Numpy >= 1.0.2 * Building requires the pypa/build module
+(https://github.com/pypa/build) and a C/C++ compiler ### Bugs, questions,
+patches, feature requests, discussion & cetera * Open a GitHub pull request or
+a GitHub issue * Email list: http://groups.google.com/group/scikit-fmm * Send
+an email to scikit-fmm+subscribe@googlegroups.com to subscribe. ### Installing
+* Via pip: `pip install scikit-fmm` * 64-bit Windows binaries from Christoph
+Gohlke: * http://www.lfd.uci.edu/~gohlke/pythonlibs/#scikit-fmm * Anaconda
+linux-64 and linux-ppc64le packages: * `conda install scikit-fmm` * Ubuntu PPA
+* https://launchpad.net/~nvidia-digits/+archive/ubuntu/dev * Debian * https://
+tracker.debian.org/pkg/scikit-fmm ### Building and installing from Source *
+`pip install build` * `python -m build` * `pip install .` ### Running Tests *
+`python -c "import skfmm; skfmm.test(True)"` (Do not run the tests from the
+source directory.) * Tests are doctests in `skfmm/__init__.py` ### Building
+documentation * Requires sphinx and numpydoc * `make html` ### Publications
+using scikit-fmm * Akinola, I., J Varley, B. Chen, and P.K. Allen (2018)
+"Workspace Aware Online Grasp Planning" arXiv:1806.11402v1 [cs.RO] 29 Jun 2018
+https://arxiv.org/pdf/1806.11402.pdf * Bortolussi, V., B. Figliuzzi, F. Willot,
+M. Faessel, M. Jeandin (2018) "Morphological modeling of cold spray coatings"
+Image Anal Stereol 2018;37:145-158 doi:10.5566/ias.1894 https://hal.archives-
+ouvertes.fr/hal-01837906/document * Chalmers, S., C.D. Saunter, J.M. Girkin and
+J.G. McCarron (2016) "Age decreases mitochondrial motility and increases
+mitochondrial size in vascular smooth muscle." Journal of Physiology, 594.15 pp
+4283â4295. * Diogo BrandÃ£o Amorim (2014) "Efficient path planning of a
+mobile robot on rough terrain" Master's Thesis, Department of Aerospace
 Engineering, University of Lisbon. * Giometto, A., D.R. Nelson, and A.W. Murray
 (2018) "Physical interactions reduce the power of natural selection in growing
 yeast colonies", PNAS November 6, 2018 115 (45) 11448-11453; published ahead of
 print October 23, 2018 https://doi.org/10.1073/pnas.1809587115 * Joshua A.
 Taillon, Christopher Pellegrinelli, Yilin Huang, Eric D. Wachsman, and Lourdes
 G. Salamanca-Riba (2014) "Three Dimensional Microstructural Characterization of
 Cathode Degradation in SOFCs Using Focused Ion Beam and SEM" ECS Trans. 2014 61
@@ -116,9 +118,10 @@
 when discriminant becomes negative * (Joshua Gehre) * 2022.02.02 February 2nd
 2022 * Fixes for Python 3.10 compatibility * (Amin Sadeghi, Xylar Asay-Davis,
 David Parsson) * 2022.03.26 March 26th 2022 * Following the breaking changes in
 setuptools v61.0.0 it is suggested to set py_modules to disable auto-discovery
 behavior. * (Daniel Ammar) * 2022.08.15 August 15th 2022 * Following the
 breaking changes in setuptools v65 pin setuptools to v64 * (DorSSS) *
 2022.04.02 April 2nd 2023 * Build fixes for Python 3.11 (update pheap cython
-wrapper) * No solver changes Copyright 2023 The scikit-fmm team. BSD-style
-license. See LICENSE.txt in the source directory.
+wrapper) * No solver changes * 2024.05.29 May 29th 2024 * Update build system
+to use meson * Python 3.12 support * No solver changes Copyright 2023 The
+scikit-fmm team. BSD-style license. See LICENSE.txt in the source directory.
```

### Comparing `scikit-fmm-2023.4.2/doc/2d_phi.png` & `scikit_fmm-2024.5.29/doc/2d_phi.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/2d_phi_distance.png` & `scikit_fmm-2024.5.29/doc/2d_phi_distance.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/2d_phi_distance_narrow.png` & `scikit_fmm-2024.5.29/doc/2d_phi_distance_narrow.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/2d_phi_travel_time.png` & `scikit_fmm-2024.5.29/doc/2d_phi_travel_time.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/2d_phi_travel_time_mask.png` & `scikit_fmm-2024.5.29/doc/2d_phi_travel_time_mask.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/conf.py` & `scikit_fmm-2024.5.29/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,22 +59,22 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'scikit-fmm'
-copyright = u'2023, the scikit-fmm team'
+copyright = u'2024, the scikit-fmm team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '2023.04.02'
+version = '2024.05.29'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `scikit-fmm-2023.4.2/doc/extension_velocity.png` & `scikit_fmm-2024.5.29/doc/extension_velocity.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/index.rst` & `scikit_fmm-2024.5.29/doc/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/doc/periodic.png` & `scikit_fmm-2024.5.29/doc/periodic.png`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/examples/2d_example.py` & `scikit_fmm-2024.5.29/examples/2d_example.py`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/examples/boundaryconditions_example.py` & `scikit_fmm-2024.5.29/examples/boundaryconditions_example.py`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/examples/extension_velocities_example.py` & `scikit_fmm-2024.5.29/examples/extension_velocities_example.py`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/profile/prof.cpp` & `scikit_fmm-2024.5.29/profile/prof.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/profile/prof.sh` & `scikit_fmm-2024.5.29/profile/prof.sh`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/profile/profile.py` & `scikit_fmm-2024.5.29/profile/profile.py`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/__init__.py` & `scikit_fmm-2024.5.29/skfmm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 :Copyright: Copyright 2023 The scikit-fmm team.
 :License: BSD-style license. See LICENSE.txt in the source directory.
 
 """
 
 from __future__ import print_function
 
-__version__ = "2023.04.02"
+__version__ = "2024.05.29"
 __docformat__ = 'restructuredtext'
 
 from .pfmm import distance, travel_time, extension_velocities
 from .heap import heap
 
 def testing():
     r"""
```

### Comparing `scikit-fmm-2023.4.2/skfmm/base_marcher.cpp` & `scikit_fmm-2024.5.29/skfmm/base_marcher.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/base_marcher.h` & `scikit_fmm-2024.5.29/skfmm/base_marcher.h`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/distance_marcher.cpp` & `scikit_fmm-2024.5.29/skfmm/distance_marcher.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/distance_marcher.h` & `scikit_fmm-2024.5.29/skfmm/distance_marcher.h`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/extension_velocity_marcher.cpp` & `scikit_fmm-2024.5.29/skfmm/extension_velocity_marcher.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/extension_velocity_marcher.h` & `scikit_fmm-2024.5.29/skfmm/extension_velocity_marcher.h`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/fmm.cpp` & `scikit_fmm-2024.5.29/skfmm/fmm.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/heap.cpp` & `scikit_fmm-2024.5.29/skfmm/heap.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/heap.h` & `scikit_fmm-2024.5.29/skfmm/heap.h`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/heap.py` & `scikit_fmm-2024.5.29/skfmm/heap.py`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/pfmm.py` & `scikit_fmm-2024.5.29/skfmm/pfmm.py`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/pheap.pyx` & `scikit_fmm-2024.5.29/skfmm/pheap.pyx`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/travel_time_marcher.cpp` & `scikit_fmm-2024.5.29/skfmm/travel_time_marcher.cpp`

 * *Files identical despite different names*

### Comparing `scikit-fmm-2023.4.2/skfmm/travel_time_marcher.h` & `scikit_fmm-2024.5.29/skfmm/travel_time_marcher.h`

 * *Files identical despite different names*

