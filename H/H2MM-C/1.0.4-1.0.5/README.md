# Comparing `tmp/H2MM_C-1.0.4.tar.gz` & `tmp/h2mm_c-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "H2MM_C-1.0.4.tar", last modified: Sun Mar 10 02:09:15 2024, max compression
+gzip compressed data, was "h2mm_c-1.0.5.tar", last modified: Wed May 29 04:48:13 2024, max compression
```

## Comparing `H2MM_C-1.0.4.tar` & `h2mm_c-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,76 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-03-10 02:09:15.008012 H2MM_C-1.0.4/
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-03-10 02:09:15.008012 H2MM_C-1.0.4/H2MM_C/
--rwxrwxrwx   0 paul      (1000) paul      (1000)    13757 2024-03-10 01:32:58.000000 H2MM_C-1.0.4/H2MM_C/C_H2MM.h
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-03-10 02:09:15.008012 H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)    17596 2024-03-10 02:09:15.000000 H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/PKG-INFO
--rwxrwxrwx   0 paul      (1000) paul      (1000)      508 2024-03-10 02:09:15.000000 H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/SOURCES.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)        1 2024-03-10 02:09:15.000000 H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/dependency_links.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)       22 2024-03-10 02:09:15.000000 H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/requires.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)        7 2024-03-10 02:09:15.000000 H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/top_level.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)   155285 2024-03-10 01:38:29.000000 H2MM_C-1.0.4/H2MM_C/H2MM_C.pyx
--rwxrwxrwx   0 paul      (1000) paul      (1000)     3450 2022-11-16 19:12:56.000000 H2MM_C-1.0.4/H2MM_C/burst_threads.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)     8473 2022-11-16 18:23:08.000000 H2MM_C-1.0.4/H2MM_C/fwd_back.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)    26951 2024-03-10 00:53:50.000000 H2MM_C-1.0.4/H2MM_C/h2mm_functions.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)    16791 2022-11-16 18:12:14.000000 H2MM_C-1.0.4/H2MM_C/model_array.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)    12024 2024-03-10 00:36:03.000000 H2MM_C-1.0.4/H2MM_C/model_limits_funcs.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)     4175 2022-11-16 19:15:38.000000 H2MM_C-1.0.4/H2MM_C/pathloglik.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)     4402 2022-11-16 18:12:14.000000 H2MM_C-1.0.4/H2MM_C/rho_calc.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)     4377 2022-11-16 18:12:14.000000 H2MM_C-1.0.4/H2MM_C/state_path.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)    10431 2024-03-10 01:33:30.000000 H2MM_C-1.0.4/H2MM_C/utils.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)     6523 2022-11-16 18:12:14.000000 H2MM_C-1.0.4/H2MM_C/viterbi.c
--rwxrwxrwx   0 paul      (1000) paul      (1000)     1113 2022-04-19 22:16:28.000000 H2MM_C-1.0.4/LICENSE.txt
--rwxrwxrwx   0 paul      (1000) paul      (1000)       88 2022-11-16 18:12:14.000000 H2MM_C-1.0.4/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    17596 2024-03-10 02:09:15.008012 H2MM_C-1.0.4/PKG-INFO
--rwxrwxrwx   0 paul      (1000) paul      (1000)    16723 2022-09-13 15:04:14.000000 H2MM_C-1.0.4/README.md
--rwxrwxrwx   0 paul      (1000) paul      (1000)      225 2022-11-24 14:08:58.000000 H2MM_C-1.0.4/pyproject.toml
--rwxrwxrwx   0 paul      (1000) paul      (1000)      897 2024-03-10 02:09:15.008012 H2MM_C-1.0.4/setup.cfg
--rwxrwxrwx   0 paul      (1000) paul      (1000)     1908 2024-03-10 01:11:27.000000 H2MM_C-1.0.4/setup.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-03-10 02:09:15.008012 H2MM_C-1.0.4/tests/
--rwxrwxrwx   0 paul      (1000) paul      (1000)    16909 2023-03-07 13:56:55.000000 H2MM_C-1.0.4/tests/test_H2MM.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.413848 h2mm_c-1.0.5/
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.353848 h2mm_c-1.0.5/.github/
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.353848 h2mm_c-1.0.5/.github/workflows/
+-rwxrwxr-x   0 paul      (1000) paul      (1000)      992 2024-05-28 19:12:12.000000 h2mm_c-1.0.5/.github/workflows/build_wheels.yml
+-rw-rw-r--   0 paul      (1000) paul      (1000)      863 2024-05-22 10:22:38.000000 h2mm_c-1.0.5/.github/workflows/test.yml
+-rwxrwxr-x   0 paul      (1000) paul      (1000)      122 2024-05-22 12:00:09.000000 h2mm_c-1.0.5/.gitignore
+-rwxrwxr-x   0 paul      (1000) paul      (1000)      255 2024-05-22 06:13:53.000000 h2mm_c-1.0.5/.readthedocs.yml
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.361848 h2mm_c-1.0.5/H2MM_C/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    13758 2024-05-27 10:51:41.000000 h2mm_c-1.0.5/H2MM_C/C_H2MM.h
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     7565 2022-11-16 18:12:14.000000 h2mm_c-1.0.5/H2MM_C/C_H2MM_txtread.c
+-rw-rw-r--   0 paul      (1000) paul      (1000)  4124725 2024-05-29 04:48:12.000000 h2mm_c-1.0.5/H2MM_C/H2MM_C.c
+-rwxrwxr-x   0 paul      (1000) paul      (1000)   156658 2024-05-28 09:45:07.000000 h2mm_c-1.0.5/H2MM_C/H2MM_C.pyx
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     3450 2022-11-16 19:12:56.000000 h2mm_c-1.0.5/H2MM_C/burst_threads.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     8473 2022-11-16 18:23:08.000000 h2mm_c-1.0.5/H2MM_C/fwd_back.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    26951 2024-03-10 00:53:50.000000 h2mm_c-1.0.5/H2MM_C/h2mm_functions.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    16791 2022-11-16 18:12:14.000000 h2mm_c-1.0.5/H2MM_C/model_array.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    12024 2024-03-10 00:36:03.000000 h2mm_c-1.0.5/H2MM_C/model_limits_funcs.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     4175 2022-11-16 19:15:38.000000 h2mm_c-1.0.5/H2MM_C/pathloglik.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     4402 2022-11-16 18:12:14.000000 h2mm_c-1.0.5/H2MM_C/rho_calc.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     4377 2022-11-16 18:12:14.000000 h2mm_c-1.0.5/H2MM_C/state_path.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    10427 2024-05-27 15:15:06.000000 h2mm_c-1.0.5/H2MM_C/utils.c
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     6464 2024-05-27 13:17:06.000000 h2mm_c-1.0.5/H2MM_C/viterbi.c
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.413848 h2mm_c-1.0.5/H2MM_C.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)    19294 2024-05-29 04:48:13.000000 h2mm_c-1.0.5/H2MM_C.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2179 2024-05-29 04:48:13.000000 h2mm_c-1.0.5/H2MM_C.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2024-05-29 04:48:13.000000 h2mm_c-1.0.5/H2MM_C.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       60 2024-05-29 04:48:13.000000 h2mm_c-1.0.5/H2MM_C.egg-info/requires.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        7 2024-05-29 04:48:13.000000 h2mm_c-1.0.5/H2MM_C.egg-info/top_level.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     1113 2022-04-19 22:16:28.000000 h2mm_c-1.0.5/LICENSE.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)       88 2022-11-16 18:12:14.000000 h2mm_c-1.0.5/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    19294 2024-05-29 04:48:13.413848 h2mm_c-1.0.5/PKG-INFO
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    16723 2022-09-13 15:04:14.000000 h2mm_c-1.0.5/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.365848 h2mm_c-1.0.5/docs/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      638 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/Makefile
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      804 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/make.bat
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.369848 h2mm_c-1.0.5/docs/source/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     4225 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/AboutH2MM.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    25933 2022-11-18 08:52:17.000000 h2mm_c-1.0.5/docs/source/CustomPrint.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      585 2022-11-18 15:21:50.000000 h2mm_c-1.0.5/docs/source/Documentation.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     9646 2022-11-18 08:51:35.000000 h2mm_c-1.0.5/docs/source/FBoundingTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      545 2022-11-18 08:52:09.000000 h2mm_c-1.0.5/docs/source/FFTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    20223 2022-11-18 08:54:44.000000 h2mm_c-1.0.5/docs/source/FOptimizationTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      111 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/HowTo.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     9595 2022-11-18 08:56:27.000000 h2mm_c-1.0.5/docs/source/OBoundingTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      586 2022-11-18 09:02:22.000000 h2mm_c-1.0.5/docs/source/OOTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    20161 2022-11-18 08:59:05.000000 h2mm_c-1.0.5/docs/source/OOptimizationTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     6051 2022-11-18 09:03:23.000000 h2mm_c-1.0.5/docs/source/SecondaryControl.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     8385 2022-11-18 09:04:03.000000 h2mm_c-1.0.5/docs/source/SimTutorial.rst
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      122 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/Tutorial.rst
+-rwxrwxr-x   0 paul      (1000) paul      (1000)     2290 2024-05-22 09:40:55.000000 h2mm_c-1.0.5/docs/source/conf.py
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     2113 2022-09-19 13:14:56.000000 h2mm_c-1.0.5/docs/source/index.rst
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.385848 h2mm_c-1.0.5/docs/source/notebooks/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    11760 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Bounds_Tutorial-OOP.ipynb
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     9896 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Bounds_Tutorial.ipynb
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     6874 2022-11-19 06:40:41.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Control_Optimization.ipynb
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    31257 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_DisplayProgress.ipynb
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    76780 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial-OOP.ipynb
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    77095 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial.ipynb
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.409848 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     7051 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/FOT_bic1.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     5867 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/FOT_error.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     8585 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/FOT_icl1.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    12704 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/FOT_iclbic.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     8585 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/H2MM_Optimization_Tutorial_26_1.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     7051 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/H2MM_Optimization_Tutorial_27_1.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    12704 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/H2MM_Optimization_Tutorial_30_1.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)     5867 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Optimization_Tutorial_files/H2MM_Optimization_Tutorial_42_1.png
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    11990 2022-08-28 16:35:54.000000 h2mm_c-1.0.5/docs/source/notebooks/H2MM_Simulation_Tutorial.ipynb
+-rwxrwxrwx   0 paul      (1000) paul      (1000)  3398045 2022-08-28 16:35:55.000000 h2mm_c-1.0.5/docs/source/notebooks/sample_data_2det.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)  6182873 2022-08-28 16:35:55.000000 h2mm_c-1.0.5/docs/source/notebooks/sample_data_3det.txt
+-rwxrwxrwx   0 paul      (1000) paul      (1000)      111 2022-11-19 06:52:48.000000 h2mm_c-1.0.5/docs/source/requirements.txt
+-rwxrwxr-x   0 paul      (1000) paul      (1000)     1709 2024-05-28 16:35:56.000000 h2mm_c-1.0.5/pyproject.toml
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2024-05-29 04:48:13.413848 h2mm_c-1.0.5/setup.cfg
+-rwxrwxr-x   0 paul      (1000) paul      (1000)      846 2024-05-22 07:22:49.000000 h2mm_c-1.0.5/setup.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-29 04:48:13.409848 h2mm_c-1.0.5/tests/
+-rwxrwxrwx   0 paul      (1000) paul      (1000)    20967 2024-05-28 03:47:25.000000 h2mm_c-1.0.5/tests/test_H2MM.py
```

### Comparing `H2MM_C-1.0.4/H2MM_C/C_H2MM.h` & `h2mm_c-1.0.5/H2MM_C/C_H2MM.h`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
 // structure contains all inputs for viterbi_burst thread
 
 typedef struct
 {
 	unsigned long si; // the number of states, also stride of 1st dimension of A
 	unsigned long sT; // stride of 0th dimension of A, gives power of A
-	unsigned long max_phot; // size of larges burst, used for allocating arrays
+	unsigned long max_phot; // size of largest burst, used for allocating arrays
 	double *A; // A array, the powers of the transition probability matrix
 	phstream *phot; // pointer to burst array, part of input
 	ph_path *path; // pointer to viterbi path found by viterbi algorithm
 	h2mm_mod *model; // h2mm model used in calculating the path
 	brst_mutex *burst_lock; // mutex for updating cur_burst
 } vit_vals;
```

### Comparing `H2MM_C-1.0.4/H2MM_C/H2MM_C.egg-info/PKG-INFO` & `h2mm_c-1.0.5/H2MM_C.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,58 @@
 Metadata-Version: 2.1
 Name: H2MM_C
-Version: 1.0.4
+Version: 1.0.5
 Summary: C level implementation of H2MM algorithm by Pirchi. 2016
-Home-page: https://github.com/harripd/H2MMpythonlib
-Download-URL: https://github.com/harripd/H2MMpythonlib
-Author: Paul David Harris
-Author-email: harripd@gmail.com
-Maintainer: Paul David Harris
-Maintainer-email: harripd@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/harripd/H2MMpythonlib
-Keywords: single-molecule FRET
+Author-email: Paul David Harris <harripd@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2017 harripd
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+        No changes were made to the standard MIT license
+Project-URL: Homepage, https://github.com/harripd/H2MMpythonlib
+Project-URL: Documentation, https://h2mmpythonlib.readthedocs.io/en/latest/
+Project-URL: Repositories, https://github.com/harripd/H2MMpythonlib/
+Project-URL: Issues, https://github.com/harripd/H2MMpythonlib/issues
+Keywords: single-molecule FRET,smFRET,hidden markov model
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy>=1.20.1
+Requires-Dist: numpy
 Requires-Dist: IPython
+Requires-Dist: importlib_metadata; python_version < "3.8"
 
 # H2MM_C
 
 [![Build and Test](https://github.com/harripd/H2MMpythonlib/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/harripd/H2MMpythonlib/actions)
 [![Documentation Status](https://readthedocs.org/projects/h2mmpythonlib/badge/?version=latest)](https://h2mmpythonlib.readthedocs.io/en/latest/?badge=latest)
 
 ## Project Desciption
```

### Comparing `H2MM_C-1.0.4/H2MM_C/H2MM_C.pyx` & `h2mm_c-1.0.5/H2MM_C/H2MM_C.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,24 @@
     void *txt
     void *handle
     unsigned long disp_freq
     unsigned long keep
     unsigned long max_iter
 
 #: Version string
-__version__ = '1.0.3'
+from sys import version_info as python_version
+if python_version.major > 3 or python_version.minor > 7:
+    from importlib.metadata import version, PackageNotFoundError
+else:
+    from importlib_metadata import version, PackageNotFoundError
+try:
+    __version__ = version("H2MM_C")
+except PackageNotFoundError:
+    print("cannot find package version")
+del version, PackageNotFoundError, python_version
 
 # copy data from a numpy array into an unsigned long array, and return the pointer
 cdef unsigned long* np_copy_ul(np.ndarray arr):
     cdef unsigned long* out = <unsigned long*> PyMem_Malloc(arr.shape[0]*sizeof(unsigned long))
     for i in range(arr.shape[0]):
         out[i] = <unsigned long> arr[i]
     return out
@@ -153,22 +162,30 @@
 
 # copy array into numpy
 cdef np.ndarray copy_to_np_ul(unsigned long lenp, unsigned long* arr):
     cdef np.ndarray out = np.empty(lenp, dtype=np.uint32)
     cdef i
     for i in range(lenp):
         out[i] = arr[i]
+    return out
+
+cdef np.ndarray copy_to_np_ul_and_free(unsigned long lenp, unsigned long* arr):
+    cdef np.ndarray out = copy_to_np_ul(lenp, arr)
     PyMem_Free(arr)
     return out
 
 cdef np.ndarray copy_to_np_d(unsigned long lenp, double* arr):
     cdef np.ndarray out = np.empty(lenp, dtype=np.float64)
     cdef i
     for i in range(lenp):
         out[i] = arr[i]
+    return out
+
+cdef np.ndarray copy_to_np_d_and_free(unsigned long lenp, double* arr):
+    cdef np.ndarray out = copy_to_np_d(lenp, arr)
     PyMem_Free(arr)
     return out
 
 cdef enum_arrays(model_array):
     if isinstance(model_array, (list, tuple)):
         return iter(model_array)
     elif isinstance(model_array, np.ndarray):
@@ -1949,20 +1966,20 @@
 cdef np.ndarray gen_gamma_numpy(tuple shape, unsigned long* dim1, unsigned long dim2, double** arrays):
     cdef unsigned long i
     cdef unsigned long size = 1
     for i in shape:
         size *= i
     cdef np.ndarray[object] out = np.empty(size, dtype=object)
     for i in range(size):
-        out[i] = copy_to_np_d(dim1[i] * dim2, arrays[i]).reshape((dim1[i], dim2))
+        out[i] = copy_to_np_d_and_free(dim1[i] * dim2, arrays[i]).reshape((dim1[i], dim2))
     return out.reshape(shape)
 
  # function to generate list or tuple of 2d numpy double arrays (primarily for returning gamma)
 cdef gen_gamma_py(type tp, tuple shape, unsigned long* dim1, unsigned long dim2, double** arrays):
-    return tp(copy_to_np_d(dim1[i]*dim2, arrays[i]).reshape((dim1[i], dim2)) for i in range(shape[0]))
+    return tp(copy_to_np_d_and_free(dim1[i]*dim2, arrays[i]).reshape((dim1[i], dim2)) for i in range(shape[0]))
 
 # wrapper to choose correct gamma generating function
 cdef gen_gamma(type tp, tuple shape, unsigned long* dim1, unsigned long dim2, double** gamma):
     if tp == np.ndarray:
         return gen_gamma_numpy(shape, dim1, dim2, gamma)
     elif tp in (list, tuple):
         return gen_gamma_py(tp, shape, dim1, dim2, gamma)
@@ -2013,22 +2030,17 @@
         pscale[i] = path[i].scale
     if tp == np.ndarray:
         rpath = gen_path_numpy(shape, dim1, ppath)
         rscale = gen_scale_numpy(shape, dim1, pscale)
     elif tp in (list, tuple):
         rpath = gen_path_py(tp, shape, dim1, ppath)
         rscale = gen_scale_py(tp, shape, dim1, pscale)
-    if ppath is not NULL:
-        PyMem_Free(ppath)
-        ppath = NULL
-    if pscale is not NULL:
-        PyMem_Free(pscale)
-        pscale = NULL
     return rpath, rscale
 
+
 def EM_H2MM_C(h2mm_model h_mod, indexes, times, max_iter=None, 
               print_func='iter', print_args=None, bounds_func=None, 
               bounds=None, max_time=np.inf, converged_min=None, 
               num_cores=None, reset_niter=True, gamma=False, opt_array = False):
     """
     Calculate the most likely model that explains the given set of data. The 
     input model is used as the start of the optimization.
@@ -2259,17 +2271,19 @@
         raise burst_check
     if h_mod.model.ndet > burst_check + 1:
         warnings.warn(f"Overdefined model:\nThe given data has fewer photon streams than initial model\nModel has {h_mod.model.ndet} streams, but data has only {burst_check + 1} streams.\nExtra photon streams in model will have 0 values in emission probability matrix")
     # check the bounds_func
     cdef unsigned long num_burst = indexes.size if isinstance(indexes, np.ndarray) else len(indexes)
     cdef tuple bounds_strings = ('minmax', 'revert', 'revert_old')
     cdef tuple print_strings = (None,'console','all','diff','diff_time','comp','comp_time','iter')
-    cdef object disp_txt = Pretty("Print Func validation")
-    cdef object disp_handle = DisplayHandle()
-    disp_handle.display(disp_txt)
+    cdef int ipy_disp = 0 if print_func in (None, 'console') else 1
+    cdef object disp_txt = Pretty("Print Func validation") if ipy_disp else None
+    cdef object disp_handle = DisplayHandle() if ipy_disp else None
+    if ipy_disp:
+        disp_handle.display(disp_txt)
     cdef h2mm_model h_test_new = h_mod.copy()
     cdef h2mm_model h_test_current = h_mod.copy()
     cdef h2mm_model h_test_old = h_mod.copy()
     h_test_new.model.niter, h_test_current.model.niter, h_test_old.model.niter = 3, 2, 1
     h_test_new.model.conv, h_test_current.model.conv, h_test_old.model.conv = 1, 1, 1
     h_test_new.model.nphot, h_test_current.model.nphot, h_test_old.model.nphot = 1000, 1000, 1000
     h_test_new.model.loglik, h_test_current.model.loglik, h_test_old.model.loglik = -0.0, -2e-4, -3e-4
@@ -2289,16 +2303,17 @@
         elif isinstance(print_args,int) and not isinstance(print_args,bool):
             print_args = (print_args, False)
         elif isinstance(print_args,bool):
             print_args = (1,print_args)
     elif callable(print_func):
         print_args = tuple(print_args) if isinstance(print_args, list) else print_args
         try:
-            disp_txt.data += "print_func validation\n"
-            disp_handle.update(disp_txt)
+            if ipy_disp:
+                disp_txt.data += "print_func validation\n"
+                disp_handle.update(disp_txt)
             if print_args is None:
                 print_return = print_func(1,h_test_new,h_test_current,h_test_old,0.1,0.2)
                 print_args = (disp_handle,disp_txt,1,False)
             elif isinstance(print_args, int):
                 print_return = print_func(1,h_test_new,h_test_current,h_test_old,0.1,0.2)
                 print_args = (disp_handle,disp_txt,1, print_args) if isinstance(print_args,bool) else (disp_handle,disp_txt,print_args, False)
             elif  isinstance(print_args, tuple) and len(print_args) >= 2 and isinstance(print_args[0],int) and isinstance(print_args[1],bool):
@@ -2308,41 +2323,52 @@
                     print_return = print_func(1,h_test_new,h_test_current,h_test_old,0.1,0.2,*print_args[2:])
                 print_args = ((disp_handle,disp_txt) + print_args)
             else:
                 print_return = print_func(1,h_test_new,h_test_current,h_test_old,0.1,0.2,*print_args)
                 print_args = ((disp_handle, disp_txt, 1, False) + print_args)
             if print_return is not None and not isinstance(print_return,str):
                 raise TypeError(f"print_func must either return nothing, or a str, got {type(print_return)}")
-            disp_txt.data += "print_func validated\n"
-            disp_handle.update(disp_txt)
+            if ipy_disp:
+                disp_txt.data += "print_func validated\n"
+                disp_handle.update(disp_txt)
         except Exception as e:
-            disp_txt.data += "print_func invalid function, must take (niter,new,current,old,t_iter,t_total,*print_args)\n"
-            disp_handle.update(disp_txt)
+            if ipy_disp:
+                disp_txt.data += "print_func invalid function, must take (niter,new,current,old,t_iter,t_total,*print_args)\n"
+                disp_handle.update(disp_txt)
+            else:
+                print("print_func invalid function, must take (niter,new,current,old,t_iter,t_total,*print_args)")
             raise e
+    else:
+        raise NotImplementedError("Coding error, please raise issue on github")
     # set up optimzation min/max limits
     cdef lm limits
     limits.max_iter = <unsigned long> optimization_limits._get_max_iter(max_iter)
     limits.num_cores = <unsigned long> optimization_limits._get_num_cores(num_cores)
     limits.max_time = <double> optimization_limits._get_max_time(max_time)
     limits.min_conv = <double> optimization_limits._get_converged_min(converged_min)
     # setup the printing function
     cdef int (*ptr_print_func)(unsigned long,h2mm_mod*,h2mm_mod*,h2mm_mod*,double,double,void*) noexcept
     cdef void *ptr_print_call = NULL
     cdef print_args_struct *ptr_print_args = <print_args_struct*> PyMem_Malloc(sizeof(print_args_struct))
     cdef print_struct *ptr_print_struct = <print_struct*> PyMem_Malloc(sizeof(print_struct*))
     ptr_print_args.keep = 1
     ptr_print_args.max_iter = limits.max_iter
-    disp_txt.data = ""
+    if ipy_disp:
+        disp_txt.data = ""
     if print_func in print_strings:
         ptr_print_args.txt = <void*> disp_txt
         ptr_print_args.handle = <void*> disp_handle
         ptr_print_args.keep = 1 if print_args[1] else 0
         ptr_print_args.disp_freq = <unsigned long> print_args[0]
         ptr_print_call = <void*> ptr_print_args
-        if print_func == 'console':
+        if print_func is None:
+            ptr_print_func = NULL
+            ptr_print_args.keep = 0
+        elif print_func == 'console':
+            print("console")
             ptr_print_func = baseprint
             ptr_print_args.keep = 0
         elif print_func == 'all':
             ptr_print_func = model_print_all
         elif print_func == 'diff':
             ptr_print_func = model_print_diff
         elif print_func == 'diff_time':
@@ -2355,22 +2381,21 @@
             ptr_print_func = model_print_iter
     elif callable(print_func):
         ptr_print_args.keep = 1 if print_args[3] else 0
         ptr_print_func = model_print_call_str if isinstance(print_return,str) else model_print_call
         ptr_print_struct.func = <void*> print_func
         ptr_print_struct.args = <void*> print_args
         ptr_print_call = <void*> ptr_print_struct
-    elif print_func is None:
-        ptr_print_func = NULL
-        ptr_print_args.keep = 0
-
+    else:
+        raise NotImplementedError("Coding error, please raise issue on github")
     # allocate the memory for the pointer arrays to be submitted to the C function
     # print("Allocating C bursts data")
-    disp_txt.data = "Preparing data"
-    disp_handle.update(disp_txt)
+    if ipy_disp:
+        disp_txt.data = "Preparing data"
+        disp_handle.update(disp_txt)
     cdef unsigned long **b_det = <unsigned long**> PyMem_Malloc(num_burst * sizeof(unsigned long*))
     cdef unsigned long **b_delta = <unsigned long**> PyMem_Malloc(num_burst * sizeof(unsigned long*))
     cdef unsigned long *burst_sizes = burst_convert(num_burst, indexes, times, b_det, b_delta)
     if burst_sizes is NULL:
         if ptr_print_args is not NULL: 
             PyMem_Free(ptr_print_args)
             ptr_print_args = NULL
@@ -2379,16 +2404,17 @@
             ptr_print_struct = NULL
         raise ValueError("Photon out of order")
     # print("Done Allocating C bursts data")
     # if the bounds_func is not None, then setup the bounds arrays
     cdef int (*bound_func)(h2mm_mod*, h2mm_mod*, h2mm_mod*, double, lm* ,void*) noexcept
     cdef void *b_ptr
     # cdef h2mm_minmax *bound = <h2mm_minmax*> PyMem_Malloc(sizeof(h2mm_minmax))
-    disp_txt.data = "Bounds preparation"
-    disp_handle.update(disp_txt)
+    if ipy_disp:
+        disp_txt.data = "Bounds preparation"
+        disp_handle.update(disp_txt)
     cdef _h2mm_lims bound
     cdef bound_struct *b_struct = <bound_struct*> PyMem_Malloc(sizeof(bound_struct))
     if bounds_func is None:
         bound_func = limit_check_only
         b_ptr = NULL
     elif bounds_func in ['minmax', 'revert', 'revert_old']:
         bound = bounds._make_model(h_mod)
@@ -2409,16 +2435,17 @@
     if reset_niter:
         h_mod.model.niter = 0
     # disp_handle.update(disp_txt)
     cdef int res
     cdef unsigned long i, n
     cdef h2mm_mod *out_arr
     cdef double **gamma_arr = NULL
-    disp_txt.data = "Bounds prepared"
-    disp_handle.update(disp_txt)
+    if ipy_disp:
+        disp_txt.data = "Bounds prepared"
+        disp_handle.update(disp_txt)
     # based on gamma and opt_array kwargs, choose which h2mm optimization to run
     if gamma and opt_array:
         res =  h2mm_optimize_gamma_array(num_burst,burst_sizes,b_delta,b_det, h_mod.model, &out_arr, &gamma_arr, &limits, bound_func, b_ptr, ptr_print_func, ptr_print_call)
     elif gamma:
         out_arr = allocate_models(1, h_mod.nstate, h_mod.ndet, 0)
         res =  h2mm_optimize_gamma(num_burst,burst_sizes,b_delta,b_det, h_mod.model, out_arr, &gamma_arr,&limits, bound_func, b_ptr, ptr_print_func, ptr_print_call)
     elif opt_array:
@@ -2481,19 +2508,20 @@
     elif conv == 6:
         out_text = f'An error occured on iteration {niter}, returning previous model'
     elif conv == 7:
         out_text = f'The model converged after {niter-1} iterations'
     else:
 
         raise ValueError(f'Unknown error, check C code- raise issue on GitHub, res={res}, conv={conv}, n={n}')
-    if keep == 1:
+    if keep == 1 and ipy_disp:
         disp_txt.data += out_text
-    else:
+    elif ipy_disp:
         disp_txt.data = out_text
-    disp_handle.update(disp_txt)
+    if ipy_disp:
+        disp_handle.update(disp_txt)
     if gamma:
         return out, gamma_out
     else:
         return out
 
 # function generates output numpy array of h2mm objects
 cdef h2mm_arr_gen(type mod_tp, tuple mod_shape, h2mm_mod* models):
@@ -2714,28 +2742,30 @@
     cdef unsigned long nphot = sum(burst_sizes[i] for i in range(num_burst))
     cdef ph_path *path_ret = allocate_paths(num_burst, burst_sizes, h_mod.model.nstate)
     cdef n_core = <unsigned long> optimization_limits._get_num_cores(num_cores)
     # set up the in and out h2mm_mod variables
     cdef unsigned long e_val = viterbi(num_burst, burst_sizes, b_delta, b_det, h_mod.model, path_ret, n_core)
     if e_val == 0:
         path, scale = gen_path(type(indexes), array_size(indexes), burst_sizes, path_ret) 
+    else:
+        free_paths(num_burst, path_ret)
     burst_free(num_burst, b_det, b_delta, burst_sizes)
     if e_val == 1:
         raise ValueError('Bursts photons are out of order, please check your data')
     elif e_val == 2:
         raise ValueError('Too many photon streams in data for H2MM model')
     cdef double loglik = 0.0
     cdef np.ndarray[double] ll = np.zeros(num_burst)
     for i in range(num_burst):
         loglik += path_ret[i].loglik
         ll[i] = path_ret[i].loglik
     if isinstance(indexes, np.ndarray):
         ll = ll.reshape(indexes.shape)
     cdef double icl = ((h_mod.nstate**2 + ((h_mod.ndet - 1) * h_mod.nstate) - 1) * np.log(nphot)) - 2 * loglik
-    PyMem_Free(path_ret)
+    free_paths(num_burst, path_ret)
     return path, scale, ll, icl
     
 
 def viterbi_sort(h2mm_model hmod, indexes, times, num_cores=None):
     """
     An all inclusive viterbi processing algorithm. Returns the ICL, the most likely
     state path, posterior probabilities, and a host of information sorted by
@@ -2977,15 +3007,15 @@
     cdef double *ll = <double*> PyMem_Malloc(num_burst * sizeof(double))
     cdef res = pathloglik(num_burst, burst_sizes, b_delta, b_det, state, model.model, ll, n_core)
     # process values
     cdef double sum_loglik, bic
     cdef np.ndarray loglik
     cdef list out = list()
     if res == 0:
-        loglik = copy_to_np_d(num_burst, ll).reshape(array_size(indexes))
+        loglik = copy_to_np_d_and_free(num_burst, ll).reshape(array_size(indexes))
         sum_loglik = np.sum(loglik)
         bic = (model.k * np.log(nphot)) - (2*sum_loglik)
     else:
         if ll is not NULL:
             PyMem_Free(ll)
             ll = NULL
     for i in range(num_burst):
@@ -3050,15 +3080,15 @@
     cdef unsigned int seedp = 0
     if seed is not None:
         seedp = <unsigned int> seed
     cdef int exp = statepath(hmod.model, lenp, path_n, seedp)
     if exp != 0:
         PyMem_Free(path_n)
         raise RuntimeError("Unknown error, raise issue on github")
-    cdef np.ndarray path = copy_to_np_ul(lenp, path_n)
+    cdef np.ndarray path = copy_to_np_ul_and_free(lenp, path_n)
     return path
 
 
 def sim_sparsestatepath(h2mm_model hmod, np.ndarray times, seed=None):
     """
     Generate a state path from a model and a sparse set of arrival times
 
@@ -3100,15 +3130,15 @@
         seedp = <unsigned int> seed
     cdef int exp = sparsestatepath(hmod.model, lenp, times_n, path_n, seedp)
     PyMem_Free(times_n)
     if exp == 1:
         raise ValueError("Out of order photon")
     elif exp != 0:
         raise RuntimeError("Unknown error, raise issue on github")
-    cdef np.ndarray path = copy_to_np_ul(lenp, path_n)
+    cdef np.ndarray path = copy_to_np_ul_and_free(lenp, path_n)
     return path
 
 
 def sim_phtraj_from_state(h2mm_model hmod, np.ndarray states, seed=None):
     """
     Generate a photon trajectory from a h2mm model and state trajectory
 
@@ -3147,15 +3177,15 @@
     if seed is not None:
         seedp = <unsigned int> seed
     cdef int exp = phpathgen(hmod.model, lenp, states_n, dets_n, seedp)
     PyMem_Free(states_n)
     if exp != 0:
         PyMem_Free(dets_n)
         raise RuntimeError("Unknown error, raise issue on github")
-    cdef np.ndarray dets = copy_to_np_ul(lenp, dets_n)
+    cdef np.ndarray dets = copy_to_np_ul_and_free(lenp, dets_n)
     return dets
 
 
 def sim_phtraj_from_times(h2mm_model hmod, np.ndarray times, seed=None):
     """
     Generate a state path and photon trajectory for a given set of times
 
@@ -3209,10 +3239,10 @@
     cdef unsigned long* dets_n = <unsigned long*> PyMem_Malloc(lenp * sizeof(unsigned long))
     exp = phpathgen(hmod.model, lenp, path_n, dets_n, seedp)
     PyMem_Free(times_n)
     if exp != 0:
         PyMem_Free(path_n)
         PyMem_Free(dets_n)
         raise RuntimeError("Unknown error in phtragen, raise issue on github")
-    cdef np.ndarray path = copy_to_np_ul(lenp, path_n)
-    cdef np.ndarray dets = copy_to_np_ul(lenp, dets_n)
+    cdef np.ndarray path = copy_to_np_ul_and_free(lenp, path_n)
+    cdef np.ndarray dets = copy_to_np_ul_and_free(lenp, dets_n)
     return path , dets
```

### Comparing `H2MM_C-1.0.4/H2MM_C/burst_threads.c` & `h2mm_c-1.0.5/H2MM_C/burst_threads.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/fwd_back.c` & `h2mm_c-1.0.5/H2MM_C/fwd_back.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/h2mm_functions.c` & `h2mm_c-1.0.5/H2MM_C/h2mm_functions.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/model_array.c` & `h2mm_c-1.0.5/H2MM_C/model_array.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/model_limits_funcs.c` & `h2mm_c-1.0.5/H2MM_C/model_limits_funcs.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/pathloglik.c` & `h2mm_c-1.0.5/H2MM_C/pathloglik.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/rho_calc.c` & `h2mm_c-1.0.5/H2MM_C/rho_calc.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/state_path.c` & `h2mm_c-1.0.5/H2MM_C/state_path.c`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/H2MM_C/utils.c` & `h2mm_c-1.0.5/H2MM_C/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 int free_paths(unsigned long num_burst, ph_path* paths)
 {
 	unsigned long i;
 	if (paths != NULL)
 	{
 		for (i=0; i < num_burst; i++)
 			free_path_arrs(&paths[i]);
-		//~ free(paths);
+		free(paths);
 		return 0;
 	}
 	else
 		return 1;
 }
 
 int print_model(h2mm_mod* model)
```

### Comparing `H2MM_C-1.0.4/H2MM_C/viterbi.c` & `h2mm_c-1.0.5/H2MM_C/viterbi.c`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 	pthread_mutex_init(vit_lock,NULL);
 #elif _WIN32
 	HANDLE* tid = (HANDLE*)calloc(num_cores, sizeof(HANDLE));
 	DWORD  windowsThreadId = 0;
 	HANDLE vit_lock = CreateMutex(NULL, FALSE, NULL);
 #endif
 	// alocate variables
-	phstream *b = (phstream*) calloc(num_burst,sizeof(phstream)); // remember to free all b[n]->delta to prevent memory leak
+	phstream *b = (phstream*) calloc(num_burst,sizeof(phstream));
 	// process burst arrays
 	//~ printf("Getting deltas\n");
 	unsigned long max_delta = get_max_delta(num_burst,burst_sizes,burst_deltas,burst_det,b); 
 	//~ printf("Got max delta\n");
 	if (max_delta == 0)
 	{
 		//~ printf("You have a NULL pointer on one or more of  your photon arrays\n");
```

### Comparing `H2MM_C-1.0.4/LICENSE.txt` & `h2mm_c-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `H2MM_C-1.0.4/PKG-INFO` & `h2mm_c-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,58 @@
 Metadata-Version: 2.1
 Name: H2MM_C
-Version: 1.0.4
+Version: 1.0.5
 Summary: C level implementation of H2MM algorithm by Pirchi. 2016
-Home-page: https://github.com/harripd/H2MMpythonlib
-Download-URL: https://github.com/harripd/H2MMpythonlib
-Author: Paul David Harris
-Author-email: harripd@gmail.com
-Maintainer: Paul David Harris
-Maintainer-email: harripd@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/harripd/H2MMpythonlib
-Keywords: single-molecule FRET
+Author-email: Paul David Harris <harripd@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2017 harripd
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+        No changes were made to the standard MIT license
+Project-URL: Homepage, https://github.com/harripd/H2MMpythonlib
+Project-URL: Documentation, https://h2mmpythonlib.readthedocs.io/en/latest/
+Project-URL: Repositories, https://github.com/harripd/H2MMpythonlib/
+Project-URL: Issues, https://github.com/harripd/H2MMpythonlib/issues
+Keywords: single-molecule FRET,smFRET,hidden markov model
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: numpy>=1.20.1
+Requires-Dist: numpy
 Requires-Dist: IPython
+Requires-Dist: importlib_metadata; python_version < "3.8"
 
 # H2MM_C
 
 [![Build and Test](https://github.com/harripd/H2MMpythonlib/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/harripd/H2MMpythonlib/actions)
 [![Documentation Status](https://readthedocs.org/projects/h2mmpythonlib/badge/?version=latest)](https://h2mmpythonlib.readthedocs.io/en/latest/?badge=latest)
 
 ## Project Desciption
```

### Comparing `H2MM_C-1.0.4/README.md` & `h2mm_c-1.0.5/README.md`

 * *Files identical despite different names*

