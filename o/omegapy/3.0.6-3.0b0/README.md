# Comparing `tmp/omegapy-3.0.6.tar.gz` & `tmp/omegapy-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegapy-3.0.6.tar", last modified: Wed May 29 12:09:09 2024, max compression
+gzip compressed data, was "omegapy-3.0b0.tar", last modified: Thu Oct 19 05:32:58 2023, max compression
```

## Comparing `omegapy-3.0.6.tar` & `omegapy-3.0b0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:09.797691 omegapy-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 12:09:01.000000 omegapy-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-29 12:09:09.797691 omegapy-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-29 12:09:01.000000 omegapy-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:09.781691 omegapy-3.0.6/omegapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:09.797691 omegapy-3.0.6/omegapy/OMEGA_dataref/
--rw-r--r--   0 runner    (1001) docker     (127)   143760 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/boundcur.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/corrupted_obs.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1495234 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/cubindex.ref
--rw-r--r--   0 runner    (1001) docker     (127)    49152 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/flatVIS050701.bin
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/fond2.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/lambda_0403.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48007 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/linearC.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/mtf120315_25.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/mtf120315_50.dat
--rw-r--r--   0 runner    (1001) docker     (127)   108892 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/omega128_interpol.sav
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/omega_wvl_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/rapcur_25.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/rapcur_50.dat
--rw-r--r--   0 runner    (1001) docker     (127)  6723584 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/rapmtflcur.bin
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/OMEGA_dataref/specsol_0403.dat
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   139272 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/omega_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    74612 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/omega_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:09.797691 omegapy-3.0.6/omegapy/res_findcube/
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/res_findcube/cubelist
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-05-29 12:09:01.000000 omegapy-3.0.6/omegapy/useful_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:09.797691 omegapy-3.0.6/omegapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-29 12:09:09.000000 omegapy-3.0.6/omegapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-29 12:09:09.000000 omegapy-3.0.6/omegapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:09:09.000000 omegapy-3.0.6/omegapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 12:09:09.000000 omegapy-3.0.6/omegapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 12:09:09.000000 omegapy-3.0.6/omegapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:09:09.797691 omegapy-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 12:09:01.000000 omegapy-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.501486 omegapy-3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-10-19 05:32:47.000000 omegapy-3.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-19 05:32:58.497486 omegapy-3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-10-19 05:32:47.000000 omegapy-3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.477486 omegapy-3.0b0/omegapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.497486 omegapy-3.0b0/omegapy/OMEGA_dataref/
+-rw-r--r--   0 runner    (1001) docker     (127)   143760 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/boundcur.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/corrupted_obs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1495234 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/cubindex.ref
+-rw-r--r--   0 runner    (1001) docker     (127)    49152 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/flatVIS050701.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/fond2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/lambda_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48007 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/linearC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_25.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_50.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   108892 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega128_interpol.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega_wvl_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_25.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_50.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  6723584 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapmtflcur.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/specsol_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   134170 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/omega_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74027 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/omega_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.497486 omegapy-3.0b0/omegapy/res_findcube/
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/res_findcube/cubelist
+-rw-r--r--   0 runner    (1001) docker     (127)    15597 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/useful_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.481486 omegapy-3.0b0/omegapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 05:32:58.501486 omegapy-3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-10-19 05:32:47.000000 omegapy-3.0b0/setup.py
```

### Comparing `omegapy-3.0.6/LICENSE` & `omegapy-3.0b0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Aurélien Stcherbinine
+Copyright (c) 2021 Aurélien Stcherbinine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `omegapy-3.0.6/README.md` & `omegapy-3.0b0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,174 @@
-00000000: 5b21 5b76 6572 7369 6f6e 2d6a 736f 6e5d  [![version-json]
-00000010: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000020: 656c 6473 2e69 6f2f 6261 6467 652f 6479  elds.io/badge/dy
-00000030: 6e61 6d69 632f 6a73 6f6e 3f75 726c 3d68  namic/json?url=h
-00000040: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
-00000050: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000060: 6e74 2e63 6f6d 2532 4641 5374 6368 6572  nt.com%2FAStcher
-00000070: 6269 6e69 6e65 2532 466f 6d65 6761 7079  binine%2Fomegapy
-00000080: 2532 466d 6173 7465 7225 3246 6f6d 6567  %2Fmaster%2Fomeg
-00000090: 6170 7925 3246 7061 636b 6167 652e 6a73  apy%2Fpackage.js
-000000a0: 6f6e 2671 7565 7279 3d25 3234 2e76 6572  on&query=%24.ver
-000000b0: 7369 6f6e 266c 6162 656c 3d76 6572 7369  sion&label=versi
-000000c0: 6f6e 266c 6162 656c 436f 6c6f 723d 6772  on&labelColor=gr
-000000d0: 6579 2663 6f6c 6f72 3d62 6c75 6529 5d28  ey&color=blue)](
-000000e0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-000000f0: 2f70 726f 6a65 6374 2f6f 6d65 6761 7079  /project/omegapy
-00000100: 290a 215b 7079 7468 6f6e 7665 7273 696f  ).![pythonversio
-00000110: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-00000120: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000130: 6479 6e61 6d69 632f 6a73 6f6e 3f75 726c  dynamic/json?url
-00000140: 3d68 7474 7073 2533 4125 3246 2532 4672  =https%3A%2F%2Fr
-00000150: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000160: 7465 6e74 2e63 6f6d 2532 4641 5374 6368  tent.com%2FAStch
-00000170: 6572 6269 6e69 6e65 2532 466f 6d65 6761  erbinine%2Fomega
-00000180: 7079 2532 466d 6173 7465 7225 3246 6f6d  py%2Fmaster%2Fom
-00000190: 6567 6170 7925 3246 7061 636b 6167 652e  egapy%2Fpackage.
-000001a0: 6a73 6f6e 2671 7565 7279 3d25 3234 2e70  json&query=%24.p
-000001b0: 7974 686f 6e56 6572 7369 6f6e 4d69 6e26  ythonVersionMin&
-000001c0: 7375 6666 6978 3d25 3242 266c 6f67 6f3d  suffix=%2B&logo=
-000001d0: 7079 7468 6f6e 266c 6f67 6f43 6f6c 6f72  python&logoColor
-000001e0: 3d77 6869 7465 266c 6162 656c 3d70 7974  =white&label=pyt
-000001f0: 686f 6e26 6c61 6265 6c43 6f6c 6f72 3d67  hon&labelColor=g
-00000200: 7265 7926 636f 6c6f 723d 626c 7565 290a  rey&color=blue).
-00000210: 5b21 5b44 4f49 5d28 6874 7470 733a 2f2f  [![DOI](https://
-00000220: 7a65 6e6f 646f 2e6f 7267 2f62 6164 6765  zenodo.org/badge
-00000230: 2f33 3439 3736 3338 3439 2e73 7667 295d  /349763849.svg)]
-00000240: 2868 7474 7073 3a2f 2f7a 656e 6f64 6f2e  (https://zenodo.
-00000250: 6f72 672f 646f 692f 3130 2e35 3238 312f  org/doi/10.5281/
-00000260: 7a65 6e6f 646f 2e37 3831 3838 3238 290a  zenodo.7818828).
-00000270: 5b21 5b73 7461 7475 735d 2868 7474 7073  [![status](https
-00000280: 3a2f 2f6a 6f73 732e 7468 656f 6a2e 6f72  ://joss.theoj.or
-00000290: 672f 7061 7065 7273 2f31 3563 6633 3438  g/papers/15cf348
-000002a0: 6132 3964 3138 3665 3132 6634 3961 3131  a29d186e12f49a11
-000002b0: 3066 3966 3738 3766 382f 7374 6174 7573  0f9f787f8/status
-000002c0: 2e73 7667 295d 2868 7474 7073 3a2f 2f6a  .svg)](https://j
-000002d0: 6f73 732e 7468 656f 6a2e 6f72 672f 7061  oss.theoj.org/pa
-000002e0: 7065 7273 2f31 3563 6633 3438 6132 3964  pers/15cf348a29d
-000002f0: 3138 3665 3132 6634 3961 3131 3066 3966  186e12f49a110f9f
-00000300: 3738 3766 3829 0a0a 3c70 2061 6c69 676e  787f8)..<p align
-00000310: 3d22 6365 6e74 6572 223e 0a3c 696d 6720  ="center">.<img 
-00000320: 7769 6474 683d 2232 3530 2220 6865 6967  width="250" heig
-00000330: 6874 3d22 3235 3022 2073 7263 3d22 6874  ht="250" src="ht
-00000340: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000350: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000360: 4153 7463 6865 7262 696e 696e 652f 6f6d  AStcherbinine/om
-00000370: 6567 6170 792f 6d61 7374 6572 2f64 6f63  egapy/master/doc
-00000380: 732f 6c6f 676f 5f6f 6d65 6761 7079 5f73  s/logo_omegapy_s
-00000390: 6d61 6c6c 322e 706e 6722 3e0a 3c2f 703e  mall2.png">.</p>
-000003a0: 0a0a 2320 4f4d 4547 412d 5079 203a 2050  ..# OMEGA-Py : P
-000003b0: 7974 686f 6e20 746f 6f6c 7320 666f 7220  ython tools for 
-000003c0: 4f4d 4547 4120 6461 7461 0a0a 496d 706f  OMEGA data..Impo
-000003d0: 7274 6174 696f 6e20 616e 6420 6469 7370  rtation and disp
-000003e0: 6c61 7920 6f66 204f 4d45 4741 2f4d 4578  lay of OMEGA/MEx
-000003f0: 206f 6273 6572 7661 7469 6f6e 7320 696e   observations in
-00000400: 2050 7974 686f 6e20 332c 2062 6173 6564   Python 3, based
-00000410: 206f 6e20 7468 6520 4944 4c20 2a53 4f46   on the IDL *SOF
-00000420: 5431 302a 2072 6f75 7469 6e65 7320 6465  T10* routines de
-00000430: 7665 6c6f 7070 6564 2069 6e20 7468 6520  velopped in the 
-00000440: 4941 5320 706c 616e 6574 6172 7920 7465  IAS planetary te
-00000450: 616d 2e0a 0a23 2320 496e 7374 616c 6c61  am...## Installa
-00000460: 7469 6f6e 2026 2055 7064 6174 650a 2323  tion & Update.##
-00000470: 2320 4d65 7468 6f64 2031 3a20 6672 6f6d  # Method 1: from
-00000480: 2050 7950 4920 2872 6563 6f6d 6d65 6e64   PyPI (recommend
-00000490: 6564 290a 2a2a 496e 7374 616c 6c61 7469  ed).**Installati
-000004a0: 6f6e 3a2a 2a20 6070 6970 3320 696e 7374  on:** `pip3 inst
-000004b0: 616c 6c20 6f6d 6567 6170 7960 0a0a 2a2a  all omegapy`..**
-000004c0: 5570 6461 7465 3a2a 2a20 6070 6970 3320  Update:** `pip3 
-000004d0: 696e 7374 616c 6c20 6f6d 6567 6170 7920  install omegapy 
-000004e0: 2d2d 7570 6772 6164 6560 200a 0a0a 2323  --upgrade` ...##
-000004f0: 2320 4d65 7468 6f64 2032 3a20 6672 6f6d  # Method 2: from
-00000500: 2074 6865 2047 6974 4875 6220 7265 706f   the GitHub repo
-00000510: 7369 746f 7279 2028 6465 7665 6c6f 706d  sitory (developm
-00000520: 656e 7420 7665 7273 696f 6e29 0a2a 2a49  ent version).**I
-00000530: 6e73 7461 6c6c 6174 696f 6e3a 2a2a 2043  nstallation:** C
-00000540: 6c6f 6e65 2074 6865 2072 6570 6f73 6974  lone the reposit
-00000550: 6f72 7920 616e 6420 696e 7374 616c 6c20  ory and install 
-00000560: 7769 7468 2070 6970 3a0a 0a7e 7e7e 6261  with pip:..~~~ba
-00000570: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
-00000580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000590: 4153 7463 6865 7262 696e 696e 652f 6f6d  AStcherbinine/om
-000005a0: 6567 6170 792e 6769 740a 6364 206f 6d65  egapy.git.cd ome
-000005b0: 6761 7079 0a70 6970 3320 696e 7374 616c  gapy.pip3 instal
-000005c0: 6c20 2e0a 7e7e 7e0a 0a2a 2a55 7064 6174  l ..~~~..**Updat
-000005d0: 653a 2a2a 2047 6f20 746f 2074 6865 2070  e:** Go to the p
-000005e0: 7265 7669 6f75 736c 7920 636c 6f6e 6564  reviously cloned
-000005f0: 2072 6570 6f73 6974 6f72 792c 2070 756c   repository, pul
-00000600: 6c20 7468 6520 6c61 7374 2075 7064 6174  l the last updat
-00000610: 6573 2c20 616e 6420 696e 7374 616c 6c20  es, and install 
-00000620: 7468 656d 2077 6974 6820 7069 703a 0a7e  them with pip:.~
-00000630: 7e7e 6261 7368 0a63 6420 6f6d 6567 6170  ~~bash.cd omegap
-00000640: 790a 6769 7420 7075 6c6c 0a70 6970 3320  y.git pull.pip3 
-00000650: 696e 7374 616c 6c20 2e0a 7e7e 7e0a 0a23  install ..~~~..#
-00000660: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
-00000670: 4675 6c6c 2064 6f63 756d 656e 7461 7469  Full documentati
-00000680: 6f6e 206f 6620 7468 6520 4f4d 4547 412d  on of the OMEGA-
-00000690: 5079 206d 6f64 756c 6520 6973 2061 7661  Py module is ava
-000006a0: 696c 6162 6c65 2061 7420 5b61 7374 6368  ilable at [astch
-000006b0: 6572 6269 6e69 6e65 2e67 6974 6875 622e  erbinine.github.
-000006c0: 696f 2f6f 6d65 6761 7079 5d28 6874 7470  io/omegapy](http
-000006d0: 733a 2f2f 6173 7463 6865 7262 696e 696e  s://astcherbinin
-000006e0: 652e 6769 7468 7562 2e69 6f2f 6f6d 6567  e.github.io/omeg
-000006f0: 6170 792f 290a 0a50 6c61 6e65 7461 7279  apy/)..Planetary
-00000700: 2044 6174 6120 576f 726b 7368 6f70 2032   Data Workshop 2
-00000710: 3032 333a 205b 6162 7374 7261 6374 5d28  023: [abstract](
-00000720: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000730: 6f6d 2f41 5374 6368 6572 6269 6e69 6e65  om/AStcherbinine
-00000740: 2f6f 6d65 6761 7079 2f62 6c6f 622f 6d61  /omegapy/blob/ma
-00000750: 7374 6572 2f64 6f63 732f 5374 6368 6572  ster/docs/Stcher
-00000760: 6269 6e69 6e65 5f50 4457 3230 3233 5f37  binine_PDW2023_7
-00000770: 3030 375f 6f6d 6567 6170 792e 7064 6629  007_omegapy.pdf)
-00000780: 2026 205b 736c 6964 6573 5d28 6874 7470   & [slides](http
-00000790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-000007a0: 5374 6368 6572 6269 6e69 6e65 2f6f 6d65  Stcherbinine/ome
-000007b0: 6761 7079 2f62 6c6f 622f 6d61 7374 6572  gapy/blob/master
-000007c0: 2f64 6f63 732f 5044 575f 466c 6167 7374  /docs/PDW_Flagst
-000007d0: 6166 665f 5374 6368 6572 6269 6e69 6e65  aff_Stcherbinine
-000007e0: 5f6f 6d65 6761 7079 5f75 706c 6f61 642e  _omegapy_upload.
-000007f0: 7064 6629 0a0a 2323 2043 6f6d 6d75 6e69  pdf)..## Communi
-00000800: 7479 2067 7569 6465 6c69 6e65 730a 546f  ty guidelines.To
-00000810: 2063 6f6e 7472 6962 7574 6520 746f 204f   contribute to O
-00000820: 4d45 4741 2d50 792c 2072 6570 6f72 7420  MEGA-Py, report 
-00000830: 616e 2069 7373 7565 206f 7220 7365 656b  an issue or seek
-00000840: 2073 7570 706f 7274 2c20 706c 6561 7365   support, please
-00000850: 2072 6566 6572 2074 6f20 7468 6520 636f   refer to the co
-00000860: 6d6d 756e 6974 7920 6775 6964 656c 696e  mmunity guidelin
-00000870: 6573 0a70 6167 6520 6f66 2074 6865 2064  es.page of the d
-00000880: 6f63 756d 656e 7461 7469 6f6e 2061 7661  ocumentation ava
-00000890: 696c 6162 6c65 205b 6865 7265 5d28 6874  ilable [here](ht
-000008a0: 7470 733a 2f2f 6173 7463 6865 7262 696e  tps://astcherbin
-000008b0: 696e 652e 6769 7468 7562 2e69 6f2f 6f6d  ine.github.io/om
-000008c0: 6567 6170 792f 636f 6d6d 756e 6974 792f  egapy/community/
-000008d0: 292e 0a0a 2323 2043 6974 696e 6720 4f4d  )...## Citing OM
-000008e0: 4547 412d 5079 0a49 6620 796f 7520 6172  EGA-Py.If you ar
-000008f0: 6520 7573 696e 6720 4f4d 4547 412d 5079  e using OMEGA-Py
-00000900: 2069 6e20 796f 7572 2072 6573 6561 7263   in your researc
-00000910: 682c 2070 6c65 6173 6520 6369 7465 2069  h, please cite i
-00000920: 7420 6163 636f 7264 696e 6720 746f 2074  t according to t
-00000930: 6865 2067 7569 6465 6c69 6e65 7320 6176  he guidelines av
-00000940: 6169 6c61 626c 6520 5b68 6572 655d 2868  ailable [here](h
-00000950: 7474 7073 3a2f 2f61 7374 6368 6572 6269  ttps://astcherbi
-00000960: 6e69 6e65 2e67 6974 6875 622e 696f 2f6f  nine.github.io/o
-00000970: 6d65 6761 7079 2f63 7265 6469 7473 2f29  megapy/credits/)
-00000980: 2e0a 0a23 2320 4372 6564 6974 730a 0ac2  ...## Credits...
-00000990: a920 4175 72c3 a96c 6965 6e20 5374 6368  . Aur..lien Stch
-000009a0: 6572 6269 6e69 6e65 2028 3230 3230 e280  erbinine (2020..
-000009b0: 9332 3032 3429 0a0a 496e 7374 6974 7574  .2024)..Institut
-000009c0: 2064 2741 7374 726f 7068 7973 6971 7565   d'Astrophysique
-000009d0: 2053 7061 7469 616c 6520 2849 4153 292c   Spatiale (IAS),
-000009e0: 2055 6e69 7665 7273 6974 c3a9 2050 6172   Universit.. Par
-000009f0: 6973 2d53 6163 6c61 792c 2043 4e52 532c  is-Saclay, CNRS,
-00000a00: 204f 7273 6179 2c20 4672 616e 6365 0a0a   Orsay, France..
-00000a10: 4c41 544d 4f53 2f49 5053 4c2c 2055 5653  LATMOS/IPSL, UVS
-00000a20: 5120 556e 6976 6572 7369 74c3 a920 5061  Q Universit.. Pa
-00000a30: 7269 732d 5361 636c 6179 2c20 536f 7262  ris-Saclay, Sorb
-00000a40: 6f6e 6e65 2055 6e69 7665 7273 6974 c3a9  onne Universit..
-00000a50: 2c20 434e 5253 2c20 4775 7961 6e63 6f75  , CNRS, Guyancou
-00000a60: 7274 2c20 4672 616e 6365 0a0a 4465 7061  rt, France..Depa
-00000a70: 7274 6d65 6e74 206f 6620 4173 7472 6f6e  rtment of Astron
-00000a80: 6f6d 7920 616e 6420 506c 616e 6574 6172  omy and Planetar
-00000a90: 7920 5363 6965 6e63 652c 204e 6f72 7468  y Science, North
-00000aa0: 6572 6e20 4172 697a 6f6e 6120 556e 6976  ern Arizona Univ
-00000ab0: 6572 7369 7479 2c20 466c 6167 7374 6166  ersity, Flagstaf
-00000ac0: 662c 2041 5a2c 2055 5341 0a0a 496e 7374  f, AZ, USA..Inst
-00000ad0: 6974 7574 2064 6520 5265 6368 6572 6368  itut de Recherch
-00000ae0: 6520 656e 2041 7374 726f 7068 7973 6971  e en Astrophysiq
-00000af0: 7565 2065 7420 506c 616e c3a9 746f 6c6f  ue et Plan..tolo
-00000b00: 6769 6520 2849 5241 5029 2c20 434e 4553  gie (IRAP), CNES
-00000b10: 2c20 556e 6976 6572 7369 74c3 a920 546f  , Universit.. To
-00000b20: 756c 6f75 7365 2049 4949 2c0a 434e 5253  ulouse III,.CNRS
-00000b30: 2c20 546f 756c 6f75 7365 2c20 4672 616e  , Toulouse, Fran
-00000b40: 6365 0a0a 0a23 2320 4c69 6365 6e73 650a  ce...## License.
-00000b50: 5468 6973 2070 6163 6b61 6765 2069 7320  This package is 
-00000b60: 7265 6c65 6173 6564 2075 6e64 6572 2061  released under a
-00000b70: 204d 4954 206f 7065 6e20 736f 7572 6365   MIT open source
-00000b80: 206c 6963 656e 7365 2e20 5365 6520 5b60   license. See [`
-00000b90: 4c49 4345 4e53 4560 5d28 6874 7470 733a  LICENSE`](https:
-00000ba0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 5374  //github.com/ASt
-00000bb0: 6368 6572 6269 6e69 6e65 2f6f 6d65 6761  cherbinine/omega
-00000bc0: 7079 2f62 6c6f 622f 6d61 7374 6572 2f4c  py/blob/master/L
-00000bd0: 4943 454e 5345 2920 666f 7220 6d6f 7265  ICENSE) for more
-00000be0: 2064 6574 6169 6c73 2e0a                  details..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6f6d 6567  : 2.1.Name: omeg
+00000020: 6170 790a 5665 7273 696f 6e3a 2033 2e30  apy.Version: 3.0
+00000030: 6230 0a53 756d 6d61 7279 3a20 5079 7468  b0.Summary: Pyth
+00000040: 6f6e 2074 6f6f 6c73 2066 6f72 204f 4d45  on tools for OME
+00000050: 4741 2f4d 4578 206f 6273 6572 7661 7469  GA/MEx observati
+00000060: 6f6e 7320 616e 616c 7973 6973 0a48 6f6d  ons analysis.Hom
+00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000080: 6173 7463 6865 7262 696e 696e 652e 6769  astcherbinine.gi
+00000090: 7468 7562 2e69 6f2f 6f6d 6567 6170 790a  thub.io/omegapy.
+000000a0: 4175 7468 6f72 3a20 4175 72c3 a96c 6965  Author: Aur..lie
+000000b0: 6e20 5374 6368 6572 6269 6e69 6e65 0a41  n Stcherbinine.A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2061 7572  uthor-email: aur
+000000d0: 656c 6965 6e40 7374 6368 6572 6269 6e69  elien@stcherbini
+000000e0: 6e65 2e6e 6574 0a50 726f 6a65 6374 2d55  ne.net.Project-U
+000000f0: 524c 3a20 536f 7572 6365 2c20 6874 7470  RL: Source, http
+00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000110: 5374 6368 6572 6269 6e69 6e65 2f6f 6d65  Stcherbinine/ome
+00000120: 6761 7079 0a43 6c61 7373 6966 6965 723a  gapy.Classifier:
+00000130: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000140: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000150: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000160: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000170: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000180: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00000190: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+000001a0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001b0: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
+000001c0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+000001d0: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+000001e0: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
+000001f0: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
+00000200: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00000210: 7269 6e67 203a 3a20 4173 7472 6f6e 6f6d  ring :: Astronom
+00000220: 790a 5265 7175 6972 6573 2d50 7974 686f  y.Requires-Pytho
+00000230: 6e3a 203e 3d33 2e37 0a44 6573 6372 6970  n: >=3.7.Descrip
+00000240: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000250: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000260: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+00000270: 4943 454e 5345 0a0a 215b 7665 7273 696f  ICENSE..![versio
+00000280: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000290: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000002a0: 7665 7273 696f 6e2d 332e 3062 6574 612d  version-3.0beta-
+000002b0: 626c 7565 290a 215b 7079 7468 6f6e 7665  blue).![pythonve
+000002c0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+000002d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000002e0: 6467 652f 5079 7468 6f6e 2d33 2e37 2b2d  dge/Python-3.7+-
+000002f0: 626c 7565 290a 5b21 5b44 4f49 5d28 6874  blue).[![DOI](ht
+00000300: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
+00000310: 2f62 6164 6765 2f33 3439 3736 3338 3439  /badge/349763849
+00000320: 2e73 7667 295d 2868 7474 7073 3a2f 2f7a  .svg)](https://z
+00000330: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
+00000340: 6c61 7465 7374 646f 692f 3334 3937 3633  latestdoi/349763
+00000350: 3834 3929 0a0a 0a3c 7020 616c 6967 6e3d  849)...<p align=
+00000360: 2263 656e 7465 7222 3e0a 3c69 6d67 2077  "center">.<img w
+00000370: 6964 7468 3d22 3235 3022 2068 6569 6768  idth="250" heigh
+00000380: 743d 2232 3530 2220 7372 633d 2268 7474  t="250" src="htt
+00000390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000003a0: 4153 7463 6865 7262 696e 696e 652f 6f6d  AStcherbinine/om
+000003b0: 6567 6170 792f 626c 6f62 2f6d 6173 7465  egapy/blob/maste
+000003c0: 722f 646f 6373 2f6c 6f67 6f5f 6f6d 6567  r/docs/logo_omeg
+000003d0: 6170 795f 736d 616c 6c32 2e70 6e67 223e  apy_small2.png">
+000003e0: 0a3c 2f70 3e0a 0a23 204f 4d45 4741 2d50  .</p>..# OMEGA-P
+000003f0: 7920 3a20 5079 7468 6f6e 2074 6f6f 6c73  y : Python tools
+00000400: 2066 6f72 204f 4d45 4741 2064 6174 610a   for OMEGA data.
+00000410: 0a49 6d70 6f72 7461 7469 6f6e 2061 6e64  .Importation and
+00000420: 2064 6973 706c 6179 206f 6620 4f4d 4547   display of OMEG
+00000430: 412f 4d45 7820 6f62 7365 7276 6174 696f  A/MEx observatio
+00000440: 6e73 2069 6e20 5079 7468 6f6e 2033 2c20  ns in Python 3, 
+00000450: 6261 7365 6420 6f6e 2074 6865 2049 444c  based on the IDL
+00000460: 202a 534f 4654 3130 2a20 726f 7574 696e   *SOFT10* routin
+00000470: 6573 2064 6576 656c 6f70 7065 6420 696e  es developped in
+00000480: 2074 6865 2049 4153 2070 6c61 6e65 7461   the IAS planeta
+00000490: 7279 2074 6561 6d2e 0a0a 3e20 2a2a 4469  ry team...> **Di
+000004a0: 7363 6c61 696d 6572 3a2a 2a20 5468 6973  sclaimer:** This
+000004b0: 206d 6f64 756c 6520 6973 206e 6f74 2074   module is not t
+000004c0: 6865 206f 6666 6963 6961 6c20 736f 6674  he official soft
+000004d0: 7761 7265 2064 6973 7472 6962 7574 6564  ware distributed
+000004e0: 2062 7920 7468 6520 4f4d 4547 4120 7465   by the OMEGA te
+000004f0: 616d 2e0a 0a23 2320 496e 7374 616c 6c61  am...## Installa
+00000500: 7469 6f6e 2026 2055 7064 6174 650a 2323  tion & Update.##
+00000510: 2320 4d65 7468 6f64 2031 3a20 6672 6f6d  # Method 1: from
+00000520: 2050 7950 4920 2872 6563 6f6d 6d65 6e64   PyPI (recommend
+00000530: 6564 290a 2a2a 496e 7374 616c 6c61 7469  ed).**Installati
+00000540: 6f6e 3a2a 2a20 6070 6970 3320 696e 7374  on:** `pip3 inst
+00000550: 616c 6c20 6f6d 6567 6170 7960 0a0a 2a2a  all omegapy`..**
+00000560: 5570 6461 7465 3a2a 2a20 6070 6970 3320  Update:** `pip3 
+00000570: 696e 7374 616c 6c20 6f6d 6567 6170 7920  install omegapy 
+00000580: 2d2d 7570 6772 6164 6560 200a 0a0a 2323  --upgrade` ...##
+00000590: 2320 4d65 7468 6f64 2032 3a20 6672 6f6d  # Method 2: from
+000005a0: 2074 6865 2047 6974 4875 6220 7265 706f   the GitHub repo
+000005b0: 7369 746f 7279 2028 6465 7665 6c6f 706d  sitory (developm
+000005c0: 656e 7420 7665 7273 696f 6e29 0a2a 2a49  ent version).**I
+000005d0: 6e73 7461 6c6c 6174 696f 6e3a 2a2a 2043  nstallation:** C
+000005e0: 6c6f 6e65 2074 6865 2072 6570 6f73 6974  lone the reposit
+000005f0: 6f72 7920 616e 6420 696e 7374 616c 6c20  ory and install 
+00000600: 7769 7468 2070 6970 3a0a 0a7e 7e7e 6261  with pip:..~~~ba
+00000610: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
+00000620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000630: 4153 7463 6865 7262 696e 696e 652f 6f6d  AStcherbinine/om
+00000640: 6567 6170 792e 6769 740a 6364 206f 6d65  egapy.git.cd ome
+00000650: 6761 7079 0a70 6970 3320 696e 7374 616c  gapy.pip3 instal
+00000660: 6c20 2e0a 7e7e 7e0a 0a2a 2a55 7064 6174  l ..~~~..**Updat
+00000670: 653a 2a2a 2047 6f20 746f 2074 6865 2070  e:** Go to the p
+00000680: 7265 7669 6f75 736c 7920 636c 6f6e 6564  reviously cloned
+00000690: 2072 6570 6f73 6974 6f72 792c 2070 756c   repository, pul
+000006a0: 6c20 7468 6520 6c61 7374 2075 7064 6174  l the last updat
+000006b0: 6573 2c20 616e 6420 696e 7374 616c 6c20  es, and install 
+000006c0: 7468 656d 2077 6974 6820 7069 703a 0a7e  them with pip:.~
+000006d0: 7e7e 6261 7368 0a63 6420 6f6d 6567 6170  ~~bash.cd omegap
+000006e0: 790a 6769 7420 7075 6c6c 0a70 6970 3320  y.git pull.pip3 
+000006f0: 696e 7374 616c 6c20 2e0a 7e7e 7e0a 0a23  install ..~~~..#
+00000700: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
+00000710: 4675 6c6c 2064 6f63 756d 656e 7461 7469  Full documentati
+00000720: 6f6e 206f 6620 7468 6520 4f4d 4547 412d  on of the OMEGA-
+00000730: 5079 206d 6f64 756c 6520 6973 2061 7661  Py module is ava
+00000740: 696c 6162 6c65 2061 7420 5b61 7374 6368  ilable at [astch
+00000750: 6572 6269 6e69 6e65 2e67 6974 6875 622e  erbinine.github.
+00000760: 696f 2f6f 6d65 6761 7079 5d28 6874 7470  io/omegapy](http
+00000770: 733a 2f2f 6173 7463 6865 7262 696e 696e  s://astcherbinin
+00000780: 652e 6769 7468 7562 2e69 6f2f 6f6d 6567  e.github.io/omeg
+00000790: 6170 792f 290a 0a50 6c61 6e65 7461 7279  apy/)..Planetary
+000007a0: 2044 6174 6120 576f 726b 7368 6f70 2032   Data Workshop 2
+000007b0: 3032 333a 205b 6162 7374 7261 6374 5d28  023: [abstract](
+000007c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007d0: 6f6d 2f41 5374 6368 6572 6269 6e69 6e65  om/AStcherbinine
+000007e0: 2f6f 6d65 6761 7079 2f62 6c6f 622f 6d61  /omegapy/blob/ma
+000007f0: 7374 6572 2f64 6f63 732f 5374 6368 6572  ster/docs/Stcher
+00000800: 6269 6e69 6e65 5f50 4457 3230 3233 5f37  binine_PDW2023_7
+00000810: 3030 375f 6f6d 6567 6170 792e 7064 6629  007_omegapy.pdf)
+00000820: 2026 205b 736c 6964 6573 5d28 6874 7470   & [slides](http
+00000830: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000840: 5374 6368 6572 6269 6e69 6e65 2f6f 6d65  Stcherbinine/ome
+00000850: 6761 7079 2f62 6c6f 622f 6d61 7374 6572  gapy/blob/master
+00000860: 2f64 6f63 732f 5044 575f 466c 6167 7374  /docs/PDW_Flagst
+00000870: 6166 665f 5374 6368 6572 6269 6e69 6e65  aff_Stcherbinine
+00000880: 5f6f 6d65 6761 7079 5f75 706c 6f61 642e  _omegapy_upload.
+00000890: 7064 6629 0a0a 2323 2043 6974 696e 6720  pdf)..## Citing 
+000008a0: 4f4d 4547 412d 5079 0a49 6620 796f 7520  OMEGA-Py.If you 
+000008b0: 6172 6520 7573 696e 6720 4f4d 4547 412d  are using OMEGA-
+000008c0: 5079 2069 6e20 796f 7572 2072 6573 6561  Py in your resea
+000008d0: 7263 682c 2070 6c65 6173 6520 6369 7465  rch, please cite
+000008e0: 2069 7420 6163 636f 7264 696e 6720 746f   it according to
+000008f0: 2074 6865 2067 7569 6465 6c69 6e65 7320   the guidelines 
+00000900: 6176 6169 6c61 626c 6520 5b68 6572 655d  available [here]
+00000910: 2868 7474 7073 3a2f 2f61 7374 6368 6572  (https://astcher
+00000920: 6269 6e69 6e65 2e67 6974 6875 622e 696f  binine.github.io
+00000930: 2f6f 6d65 6761 7079 2f63 7265 6469 7473  /omegapy/credits
+00000940: 2f29 2e0a 0a23 2320 4372 6564 6974 730a  /)...## Credits.
+00000950: 0ac2 a920 4175 72c3 a96c 6965 6e20 5374  ... Aur..lien St
+00000960: 6368 6572 6269 6e69 6e65 2028 3230 3230  cherbinine (2020
+00000970: e280 9332 3032 3329 0a0a 496e 7374 6974  ...2023)..Instit
+00000980: 7574 2064 2741 7374 726f 7068 7973 6971  ut d'Astrophysiq
+00000990: 7565 2053 7061 7469 616c 6520 2849 4153  ue Spatiale (IAS
+000009a0: 292c 2055 6e69 7665 7273 6974 c3a9 2050  ), Universit.. P
+000009b0: 6172 6973 2d53 6163 6c61 792c 2043 4e52  aris-Saclay, CNR
+000009c0: 532c 204f 7273 6179 2c20 4672 616e 6365  S, Orsay, France
+000009d0: 0a0a 4c41 544d 4f53 2f49 5053 4c2c 2055  ..LATMOS/IPSL, U
+000009e0: 5653 5120 556e 6976 6572 7369 74c3 a920  VSQ Universit.. 
+000009f0: 5061 7269 732d 5361 636c 6179 2c20 536f  Paris-Saclay, So
+00000a00: 7262 6f6e 6e65 2055 6e69 7665 7273 6974  rbonne Universit
+00000a10: c3a9 2c20 434e 5253 2c20 4775 7961 6e63  .., CNRS, Guyanc
+00000a20: 6f75 7274 2c20 4672 616e 6365 0a0a 0a23  ourt, France...#
+00000a30: 2320 4c69 6365 6e73 650a 5468 6973 2070  # License.This p
+00000a40: 6163 6b61 6765 2069 7320 7265 6c65 6173  ackage is releas
+00000a50: 6564 2075 6e64 6572 2061 204d 4954 206f  ed under a MIT o
+00000a60: 7065 6e20 736f 7572 6365 206c 6963 656e  pen source licen
+00000a70: 7365 2e20 5365 6520 5b60 4c49 4345 4e53  se. See [`LICENS
+00000a80: 4560 5d28 6874 7470 733a 2f2f 6769 7468  E`](https://gith
+00000a90: 7562 2e63 6f6d 2f41 5374 6368 6572 6269  ub.com/AStcherbi
+00000aa0: 6e69 6e65 2f6f 6d65 6761 7079 2f62 6c6f  nine/omegapy/blo
+00000ab0: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
+00000ac0: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
+00000ad0: 6c73 2e0a                                ls..
```

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav` & `omegapy-3.0b0/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/boundcur.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/boundcur.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/corrupted_obs.csv` & `omegapy-3.0b0/omegapy/OMEGA_dataref/corrupted_obs.csv`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/cubindex.ref` & `omegapy-3.0b0/omegapy/OMEGA_dataref/cubindex.ref`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/flatVIS050701.bin` & `omegapy-3.0b0/omegapy/OMEGA_dataref/flatVIS050701.bin`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/fond2.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/fond2.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/lambda_0403.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/lambda_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/linearC.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/linearC.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/mtf120315_25.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/mtf120315_50.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/omega128_interpol.sav` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega128_interpol.sav`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/omega_atmorap_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega_atmorap_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/omega_wvl_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega_wvl_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/rapcur_25.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/rapcur_50.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/rapmtflcur.bin` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapmtflcur.bin`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/OMEGA_dataref/specsol_0403.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/specsol_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/omega_data.py` & `omegapy-3.0b0/omegapy/omega_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## omega_data.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 29/05/2024
+## Last modified by Aurélien STCHERBININE : 18/10/2023
 
 ##----------------------------------------------------------------------------------------
 """Importation and correction of OMEGA/MEx observations from binaries files.
 """
 ##----------------------------------------------------------------------------------------
 ##----------------------------------------------------------------------------------------
 ## Packages
@@ -255,55 +255,48 @@
 class CubeError(Exception):
     """Exception raised if encounter an issue when reading the OMEGA/MEx cube
     binaries data.
     """
     def __init__(self, message):
         self.message = message
 
-def _readomega(cube_id, disp=True, corrV=True, corrL=True, data_path_qub='_omega_bin_path',
-               data_path_nav='_omega_bin_path'):
+def _readomega(cube_id, disp=True, corrV=True, corrL=True, data_path='_omega_bin_path'):
     """Python implementation of the `readomega.pro` routine from the SOFT10 OMEGA pipeline.
     
     Parameters
     ----------
     cube_id : str
         The observation ID (format ORBXXXX_X).
     disp : bool, default True
         Enable or disable the display of informations during the file reading.
         | `True` --> Enable display.
     corrV : bool, default True
         If `True`, compute the correction on the visible channel (Vis).
     corrL : bool, default True
         If `True`, compute the correction on the long-IR channel (L).
-    data_path_qub : str, default _omega_bin_path
-        The path of the directory containing the data files (.QUB).
-    data_path_nav : str, default _omega_bin_path
-        The path of the directory containing the navigation files (.NAV).
+    data_path : str, default _omega_bin_path
+        The path of the directory containing the data (.QUB) and 
+        navigation (.NAV) files.
 
     Returns
     -------
     out_data : dict
         {'ldat', 'jdat', 'wvl', 'ic', 'specmars'}
     out_geom : dict
-        {'latitude', 'longitude', 'emergence', 'emergence_norm', 'incidence',
-        'incidence_norm', 'altitude', 'ut_time', 'temperature_c', 'temperature_l',
-        'saturation_c', 'saturation_vis', 'lat_grid', 'lon_grid', 'latitude_v',
-        'longitude_v', 'altitude_v', 'incidence_norm_v', 'emergence_norm_v',
-        'lat_grid_v', 'lon_grid_v'}
+        {'latitude', 'longitude', 'emergence', 'incidence', 'altitude', 'ut_time',
+         'temperature, 'saturation_C', 'saturation_vis', 'lat_grid', 'lon_grid'}
     """
     # Default path
-    if data_path_qub == "_omega_bin_path":
-        data_path_qub = _omega_bin_path
-    if data_path_nav == "_omega_bin_path":
-        data_path_nav = _omega_bin_path
+    if data_path == "_omega_bin_path":
+        data_path = _omega_bin_path
     # Filename
     nomgeo0 = cube_id + '.NAV'
     nomfic0 = cube_id + '.QUB'
-    nomfic = os.path.join(data_path_qub, nomfic0)
-    nomgeo = os.path.join(data_path_nav, nomgeo0)
+    nomfic = os.path.join(data_path, nomfic0)
+    nomgeo = os.path.join(data_path, nomgeo0)
     if disp:
         print('\n\033[1mComputing OMEGA observation {0:s}\033[0m'.format(cube_id))
     # Orbit number in base 10
     orbnum = int.from_bytes(str.encode(nomfic0[3]), byteorder='big') - 48
     if orbnum > 9:
         orbnum -= 7
     orbnum = 1000 * orbnum + int(nomfic0[4:7])
@@ -951,15 +944,15 @@
         self.atm_corr = False
         self.therm_corr_infos = {'datetime': None, 'method': None}
         self.atm_corr_infos = {'datetime': None, 'method': None}
         self.quality = 1
         self.add_infos = ''
 
         if not empty:
-            obs_name = uf.myglob(os.path.join(data_path, '**', '*' + obs + '*.QUB'), recursive=True)
+            obs_name = uf.myglob(os.path.join(data_path, '*' + obs + '*.QUB'))
             if obs_name is None:
                 print("\033[1;33mAborted\033[0m")
                 empty = True
 
         if empty:
             # Data
             self.name = ''
@@ -1023,27 +1016,21 @@
             self.max_lon = None
             self.slant = None
             self.target = None
             # Ajout pour correction position
             self.ref_C = np.array([[]])
 
         else:
-            nomfic0 = os.path.split(obs_name)[1][:-4]   # Récupération nom + décodage UTF-8
-            data_path_qub = os.path.split(obs_name)[0]  # Récupération chemin dossier (utile si récursif)
-            nomgeo = obs_name[:-4] + '.NAV'
-            if os.path.exists(nomgeo):
-                data_path_nav = data_path_qub
-            else:
-                nomgeo = uf.myglob(os.path.join(data_path, '**', '*' + obs + '*.NAV'), recursive=True)
-                if nomgeo is None:
-                    raise CubeError('No corresponding NAV cube {0:s}'.format(nomfic0 + '.NAV'))
-                else:
-                    data_path_nav = os.path.split(nomgeo)[0]
+            # obs_name = uf.myglob(os.path.join(data_path, '*' + obs + '*.QUB'))
+            # if obs_name is None:
+                # print("\033[1;33mAborted\033[0m")
+                # return None
+            nomfic0 = os.path.split(obs_name)[1][:-4]    # Récupération nom + décodage UTF-8
             data_dict, geom_dict = _readomega(nomfic0, disp=disp, corrV=corrV, corrL=corrL, 
-                                              data_path_qub=data_path_qub, data_path_nav=data_path_nav)
+                                              data_path=data_path)
 
             if disp:
                 print("\n\033[01;34mComputing data extraction and correction...\033[0m", end=' ')
             # Extract values
             ldat = data_dict['ldat']
             jdat = data_dict['jdat']
             wvl = data_dict['wvl']
@@ -1073,14 +1060,17 @@
             # Correction of OMEGA data (same as clean_spec.pro)
             ic_C= ic[(ic >= 8) & (ic <= 122)]        # IR short (voie C)
             ic_L = ic[(ic >= 137) & (ic <= 255)]     # IR long (voie L)
             ic_V = ic[(ic >= 265) & (ic <= 332)]     # visible
             ic2 = np.concatenate([ic_V, ic_C, ic_L])
             lam = wvl[ic2]
             specmars = specmars[ic2]
+            lam_mask_all = deepcopy(lam)
+            lam_mask_all[:] = True
+            lam_mask = {'all' : lam_mask_all}
             # orbit_nb = int(nomfic0[3:-2])
             orbnum = int.from_bytes(str.encode(nomfic0[3]), byteorder='big') - 48
             if orbnum > 9:
                 orbnum -= 7
             orbit_nb = 1000 * orbnum + int(nomfic0[4:7])
             # Cube in physical units (W.m-2.sr-1.µm-1)
             cube_i = jdat[:, ic2, :]
@@ -1129,14 +1119,15 @@
             self.specmars = specmars.astype(np.float64)
             self.name = nomfic0
             self.orbit = orbit_nb
             self.utc = utc_dt
             self.ic = {'V' : ic_V.astype(int), 
                        'C' : ic_C.astype(int), 
                        'L' : ic_L.astype(int)}
+            self.lam_ma = lam_mask
             self.lat_grid = lat_grid
             self.lon_grid = lon_grid
             self.sensor_temp_c = temperature_c.astype(np.float64)
             self.sensor_temp_l = temperature_l.astype(np.float64)
             self.saturation_c = saturation_c.astype(np.float64)
             self.saturation_vis = saturation_vis.astype(np.float64)
             self.lat_v = lat_V.astype(np.float64)
@@ -1168,15 +1159,15 @@
             self.focal_plane_temperatures = {'V' : T_fp_V, 'C' : T_fp_C, 'L' : T_fp_L}
             T_sp_C, T_sp_L, T_sp_V = np.array(
                 hd_qub['MEX:SPECTROMETER_TEMPERATURE'][1:-5].split(','), dtype=np.float64)
             self.spectrometer_temperatures = {'V' : T_sp_V, 'C' : T_sp_C, 'L' : T_sp_L}
             #--------------------------
             # Data from the .NAV header
             #--------------------------
-            hd_nav = _read_header(nomgeo[:-4] + '.NAV')
+            hd_nav = _read_header(obs_name[:-4] + '.NAV')
             npixel, npara, nscan = np.array(hd_nav['CORE_ITEMS'][1:-1].split(','), dtype=np.int64)
             self.lrec = np.int64(hd_nav['RECORD_BYTES'])
             self.nrec = np.int64(hd_nav['LABEL_RECORDS'])
             self.sol_dist = np.float64(hd_nav['SOLAR_DISTANCE'])
             self.sol_dist_au = np.float64(hd_nav['SOLAR_DISTANCE']) / 14960e4
             npixel, npara, nscan = np.array(hd_nav['CORE_ITEMS'][1:-1].split(','), dtype=np.int64)
             self.npixel = npixel
@@ -1262,14 +1253,15 @@
         new_omega.emer_n = self.emer_n
         new_omega.inci = self.inci
         new_omega.inci_n = self.inci_n
         new_omega.specmars = self.specmars
         new_omega.utc = self.utc
         new_omega.orbit = self.orbit
         new_omega.ic = self.ic
+        new_omega.lam_ma = self.lam_ma
         new_omega.lon_grid = self.lon_grid
         new_omega.lat_grid = self.lat_grid
         new_omega.sensor_temp_c = self.sensor_temp_c
         new_omega.sensor_temp_l = self.sensor_temp_l
         new_omega.saturation_c = self.saturation_c
         new_omega.saturation_vis = self.saturation_vis
         new_omega.surf_temp = self.surf_temp
@@ -1335,14 +1327,15 @@
         new_omega.emer_n = deepcopy(self.emer_n, memo)
         new_omega.inci = deepcopy(self.inci, memo)
         new_omega.inci_n = deepcopy(self.inci_n, memo)
         new_omega.specmars = deepcopy(self.specmars, memo)
         new_omega.utc = deepcopy(self.utc, memo)
         new_omega.orbit = deepcopy(self.orbit, memo)
         new_omega.ic = deepcopy(self.ic, memo)
+        new_omega.lam_ma = deepcopy(self.lam_ma, memo)
         new_omega.lon_grid = deepcopy(self.lon_grid, memo)
         new_omega.lat_grid = deepcopy(self.lat_grid, memo)
         new_omega.sensor_temp_c = deepcopy(self.sensor_temp_c, memo)
         new_omega.sensor_temp_l = deepcopy(self.sensor_temp_l, memo)
         new_omega.saturation_c = deepcopy(self.saturation_c, memo)
         new_omega.saturation_vis = deepcopy(self.saturation_vis, memo)
         new_omega.surf_temp = deepcopy(self.surf_temp, memo)
@@ -1411,74 +1404,62 @@
         Thermal correction : {5}
         Atmospheric correction : {6}
 
         \033[3m{7}\033[0m""".format(self.name, self.version, self.ls, self.my, self.data_quality, 
                                     self.therm_corr, self.atm_corr, self.add_infos)
         return description
     
-    def get_header_qub(self, data_path='_omega_bin_path', recursive_search=True):
+    def get_header_qub(self, data_path='_omega_bin_path'):
         """Return the data from the header of the .QUB file, as a dictionary.
 
         See the OMEGA ECAID for informations about the header entries.
         
         Parameters
         ----------
         data_path : str, default _omega_bin_path
             The path of the directory containing the data (.QUB) files.
-        recursive_search : bool, default True
-            If `True`, enable the search for the .QUB file in subdirectories
-            from `data_path`.
 
         Returns
         -------
         hd_qub : dict
             Dictionary containing the data from the ORBXXXX_X.QUB file.
         """
         # Default path
         if data_path == "_omega_bin_path":
             data_path = _omega_bin_path
-        if recursive_search:
-            qub_path = uf.myglob(os.path.join(data_path, '**', self.name+'.QUB'), recursive=True)
-        else:
-            qub_path = os.path.join(data_path, self.name+'.QUB')
+        qub_path = os.path.join(data_path, self.name+'.QUB')
         hd_qub = _read_header(qub_path)
         return hd_qub
 
-    def get_header_nav(self, data_path='_omega_bin_path', recursive_search=True):
+    def get_header_nav(self, data_path='_omega_bin_path'):
         """Return the data from the header of the .NAV file, as a dictionary.
 
         See the OMEGA ECAID for informations about the header entries.
         
         Parameters
         ----------
         data_path : str, default _omega_bin_path
             The path of the directory containing the navigation (.NAV) files.
-        recursive_search : bool, default True
-            If `True`, enable the search for the .QUB file in subdirectories
-            from `data_path`.
 
         Returns
         -------
         hd_nav : dict
             Dictionary containing the data from the ORBXXXX_X.NAV file.
         """
         # Default path
         if data_path == "_omega_bin_path":
             data_path = _omega_bin_path
-        if recursive_search:
-            nav_path = uf.myglob(os.path.join(data_path, '**', self.name+'.NAV'), recursive=True)
-        else:
-            nav_path = os.path.join(data_path, self.name+'.NAV')
+        nav_path = os.path.join(data_path, self.name+'.NAV')
         hd_nav = _read_header(nav_path)
         return hd_nav
 
 ##-----------------------------------------------------------------------------------
 ## Recherche observation
 def find_cube(lon0, lat0, cmin=0, cmax=10000, out=False, data_path='_omega_bin_path',
-              nadir_only=False, recursive_search=True):
+              nadir_only=False):
     """Display the available OMEGA/MEx cubes with observations of the target
     latitude and longitude, Python translation of the IDL procedure `findcub.pro`.
 
     Parameters
     ----------
     lon0 : float
         The target longitude (in degrees).
@@ -1491,17 +1472,14 @@
     out : bool, default False
         If `True` --> return output
     data_path : str, default _omega_bin_path
         The path of the directory containing the data (.QUB) and 
         navigation (.NAV) files.
     nadir_only : bool, default False
         If `True` --> Only cubes with nadir pointing will be returned.
-    recursive_search : bool, default True
-        If `True`, enable the search for the .NAV files in subdirectories
-        from `data_path`.
 
     Returns
     -------
     cub_list : array-like
         List of matching observations.</br>
         `Format : (orbit, x, y, dmin, altMEx, inci, emer, phas, loct, Ls, MY)`
     """
@@ -1633,26 +1611,18 @@
                 nomc.append(nomcube)
                 nhits += 1
     cubindex.close()
     # Find position & infos for each observation
     print('{0:^10s} {1:^6s}{2:^6s}{3:^8s}{4:^9s}{5:^7s}{6:^8s}{7:^8s}{8:^8s}{9:^8s}{10:^4s}'.format(
             'orbit', 'x', 'y', 'dmin', 'altMEx', 'inci', 'emer', 'phas', 'loct', 'Ls', 'MY'))
     for n in range(nhits):
-        if recursive_search:
-            testfile = glob.glob(os.path.join(data_path, '**', nomc[n]+'.NAV'), recursive=True)
-            if testfile == []:
-                print('{0:8s}{1:s}'.format(nomc[n], '\033[3m   No corresponding .NAV file\033[0m'))
-                continue
-            else:
-                testfile = testfile[0]
-        else:
-            testfile = os.path.join(data_path, nomc[n]+'.NAV')
-            if os.path.exists(testfile) == False:
-                print('{0:8s}{1:s}'.format(nomc[n], '\033[3m   No corresponding .NAV file\033[0m'))
-                continue
+        testfile = os.path.join(data_path, nomc[n]+'.NAV')
+        if os.path.exists(testfile) == False:
+            print('{0:8s}{1:s}'.format(nomc[n], '\033[3m   No corresponding .NAV file\033[0m'))
+            continue
         #--------------------------
         # Data from the geometry .NAV file
         #--------------------------
         hd_nav = _read_header(testfile)
         npixel, npara, nscan = np.array(hd_nav['CORE_ITEMS'][1:-1].split(','), dtype=np.int64)
         lrec = np.int64(hd_nav['RECORD_BYTES'])
         nrec = np.int64(hd_nav['LABEL_RECORDS'])
@@ -1874,16 +1844,15 @@
     if write:
         with open(target_path, 'wb') as output:
             pickle.dump(omega, output)
         if disp:
             print('\033[01;34mSaved as \033[0;03m' + target_path + '\033[0m')
 
 def autoload_omega(obs_name, folder='auto', version=_Version, base_folder='_omega_py_path',
-                   therm_corr=None, atm_corr=None, disp=True, bin_folder='_omega_bin_path',
-                   recursive=False):
+                   therm_corr=None, atm_corr=None, disp=True, bin_folder='_omega_bin_path'):
     """Load and return a previously saved `OMEGAdata` object using pickle (with `autosave_omega()`).
 
     Parameters
     ----------
     obs_name : str
         The observation ID.
     folder : str, default 'auto'
@@ -1904,21 +1873,14 @@
     disp : bool, default True
         Control the display.</br>
             | `True` --> Print the loading filename.</br>
             | `False` --> Nothing printed.
     bin_folder : str, default _omega_bin_path
         The path of the directory containing the data (.QUB) and 
         navigation (.NAV) files.
-    recursive : bool, default False
-        Option passed to the `uf.myglob` function.</br>
-        If recursive is True, the pattern `**` will match any files and
-        zero or more directories and subdirectories.</br>
-        Note: The recursive search option is not compatible with the default
-        automatic paths, as they do not include the `**` pattern.
-        One should add it where needed (e.g., in the `folder` argument).
 
     Returns
     -------
     omega : OMEGAdata 
         The loaded object of OMEGA/MEx observation.
     """
     # Default paths
@@ -1937,18 +1899,18 @@
         ext += '_atm'
     elif atm_corr == False:
         excl.append('atm')
     filename = '*{name}*{corr_ext}*.pkl'.format(name=obs_name, corr_ext=ext)
     if folder == 'auto':
         Mversion = int(version)
         folder = 'v' + str(Mversion)
-    filename2 = uf.myglob(os.path.join(base_folder, folder, filename), exclude=excl, recursive=recursive)
+    filename2 = uf.myglob(os.path.join(base_folder, folder, filename), exclude=excl)
     if filename2 is None:
         if (therm_corr in [None, False]) and (atm_corr in [None, False]):
-            obs_name_bin = glob.glob(os.path.join(bin_folder, '**', '*' + obs_name + '*.QUB'), recursive=True)
+            obs_name_bin = glob.glob(os.path.join(bin_folder, '*' + obs_name + '*.QUB'))
             if len(obs_name_bin) == 0 :
                 return None
             else:
                 print('\033[1mMatching binary files:\033[0m')
                 return OMEGAdata(obs_name, data_path=bin_folder)
         else:
             return None
@@ -2578,14 +2540,16 @@
                     else:
                         cube_rf_corr[nscan-1, 80:95, firsteven+32*w:firsteven+3+32*w] = (
                             cube_rf[nscan-2, 80:95, firsteven+32*w:firsteven+3+32*w] )
                 omega_corr.cube_i = cube_i_corr
                 omega_corr.cube_rf = cube_rf_corr
         else:
             print('\033[01;33;41mCube not in list\033[0m')
+        # lam_mask['mode128'] = 
+        # omega_corr.add_infos += '\nWarning: Corrupted 128 pixel cube'
     return omega_corr
     
 ##-----------------------------------------------------------------------------------
 ## Correction & sauvegarde
 def corr_save_omega(obsname, folder='auto', base_folder='_omega_py_path', security=True,
                     overwrite=True, compress=True, npool=1):
     """Correction and saving of OMEGA/MEx observations.
@@ -2886,46 +2850,39 @@
     for omega in omega_list:
         ls.append(omega.ls)
     return ls
 
 ##-----------------------------------------------------------------------------------
 ## Update cube quality
 def update_cube_quality(obs_name='ORB*.pkl', folder='auto', version=_Version, 
-                        base_folder='_omega_py_path', recursive=False):
+                        base_folder='_omega_py_path'):
     """Update the quality attribute of previously saved OMEGAdata objects.
 
     Parameters
     ----------
     obs_name : str, default 'ORB*.pkl'
         The files basename.
     folder : str, default 'auto'
         The subfolder where the data is.</br>
         | If `'auto'` --> `folder = 'vX'`, where `X` is the major release version of the used code.
     version : float, default _Version
         The version of the target file (if folder is `'auto'`).</br>
         Default is the current code version.
     base_folder : str, default _omega_py_path
         The base folder path.
-    recursive : bool, default False
-        Option passed to the `uf.myglob` function.</br>
-        If recursive is True, the pattern `**` will match any files and
-        zero or more directories and subdirectories.</br>
-        Note: The recursive search option is not compatible with the default
-        automatic paths, as they do not include the `**` pattern.
-        One should add it where needed (e.g., in the `folder` argument).
     """
     # Default path
     if base_folder == "_omega_py_path":
         base_folder = _omega_py_path
     # Initialisation
     if obs_name[-4] != '.pkl':
         obs_name += '.pkl'
     if folder == 'auto':
         folder = 'v' + str(int(version))
-    basename = uf.myglob(os.path.join(base_folder, folder, obs_name), recursive=recursive)
+    basename = uf.myglob(os.path.join(base_folder, folder, obs_name))
     # Load list corrupted obs
     OBC = readsav(os.path.join(package_path, 'OMEGA_dataref', 'OBC_OMEGA_OCT2017.sav'))
     good_orbits_OBC = np.array(OBC['good_orbits'][0], dtype=int)
     corrupted_orbits_csv = pd.read_csv(os.path.join(package_path, 'OMEGA_dataref', 'corrupted_obs.csv'), 
                                        comment='#', skipinitialspace=True)
     corrupted_orbits = np.array(corrupted_orbits_csv['corrupted_obs'], dtype=str)
     corrupted_orbits_comments = np.array(corrupted_orbits_csv['comment'], dtype=str)
@@ -3022,15 +2979,15 @@
     -------
     test_quality : bool
         | `True` --> Accepted observation.</br>
         | `False` --> Rejected observation.
     """
     # Recherhe nom de fichier
     data_path = _omega_bin_path
-    obs_name = uf.myglob(os.path.join(data_path, '**', '*' + obs + '*.QUB'), recursive=True)
+    obs_name = uf.myglob(os.path.join(data_path, '*' + obs + '*.QUB'))
     if obs_name is None:
         print("\033[1;33mAborted\033[0m")
         return False
     nomfic0 = os.path.split(obs_name)[1][:-4]    # Récupération nom + décodage UTF-8
     numCube = int(nomfic0[-1])
     # Lecture header fichier .QUB
     hd_qub = _read_header(obs_name[:-4] + '.QUB')
@@ -3359,74 +3316,10 @@
     # C-channel saturation criterion limit
     # (cf Vincendon et al. (2015) or Stcherbinine et al. (2021))
     if not (limsat_c is None):
         mask[omega.saturation_c < limsat_c] = np.nan
     # Output
     return mask
 
-##----------------------------------------------------------------------------------------
-## OMEGA spectral creteria computation
-def BD_omega(omega, lam0, lamc1, lamc2, norm=True):
-    """Compute the band depth on an OMEGA observation cube.
-    Continuum linear between lamc1 and lamc2.
-    
-    If an array is passed as argument for a wavelength value, the average is used.
-    
-    Parameters
-    ----------
-    omega : OMEGAdata
-        The OMEGA/MEx observation.
-    lam0 : float or array-like
-        The wavelength of the center of the band.
-    lamc1 : float or array-like
-        The wavelength of the bluer point for the continuum determination.
-    lamc2 : float or array-like
-        The wavelength of the redder point for the continuum determination.
-    norm : bool, default True
-        | `True` --> band_depth output is the normalized BD values.</br>
-        | `False` --> band_depth output is the BD values.
-    
-    Returns
-    -------
-    band_depth : 2D array
-        The array of the band depth values for the observation
-        (normalized or not depending on `norm`).
-    rf_c : 2D array
-        The value of the continuum used to measure the band depth.
-    """
-    if not omega.therm_corr:
-        print("\033[01;33mWarning: No thermal correction applied.\033[0m")
-    # Initialisation
-    refl_cube = omega.cube_rf
-    nx, ny, nlam = refl_cube.shape
-    # Conversion floats -> list
-    if isinstance(lam0, (int, float)):
-        lam0 = [lam0]
-    if isinstance(lamc1, (int, float)):
-        lamc1 = [lamc1]
-    if isinstance(lamc2, (int, float)):
-        lamc2 = [lamc2]
-    # Search for wavelength indexes
-    i_lam0 = uf.where_closer_array(lam0, omega.lam)
-    i_lamc1 = uf.where_closer_array(lamc1, omega.lam)
-    i_lamc2 = uf.where_closer_array(lamc2, omega.lam)
-    # Average wavelengths
-    lam0 = np.mean(omega.lam[i_lam0])
-    lamc1 = np.mean(omega.lam[i_lamc1])
-    lamc2 = np.mean(omega.lam[i_lamc2])
-    # Average reflectances
-    rf_band = np.mean(refl_cube[:, :, i_lam0], axis=2)
-    rf_c1 = np.mean(refl_cube[:, :, i_lamc1], axis=2)
-    rf_c2 = np.mean(refl_cube[:, :, i_lamc2], axis=2)
-    # Average continuum
-    rf_c = rf_c1 + (rf_c2 - rf_c1) * (lam0 - lamc1) / (lamc2 - lamc1)
-    # Compute BD over the OMEGA cube
-    if norm:
-        band_depth = (rf_c - rf_band) / rf_c
-    else:
-        band_depth = rf_c - rf_band
-    # Output
-    return band_depth
-
 ##-----------------------------------------------------------------------------------
 ## End of code
 ##-----------------------------------------------------------------------------------
```

### Comparing `omegapy-3.0.6/omegapy/omega_plots.py` & `omegapy-3.0b0/omegapy/omega_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## omega_plots.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 16/04/2024
+## Last modified by Aurélien STCHERBININE : 18/10/2023
 
 ##----------------------------------------------------------------------------------------
 """Display of `OMEGAdata` cubes.
 """
 ##----------------------------------------------------------------------------------------
 ##----------------------------------------------------------------------------------------
 ## Packages
@@ -178,15 +178,15 @@
     cmap : str, default 'Greys_r'
         The matplotlib colormap.
     vmin : float or None, default None
         The lower bound of the colorscale.
     vmax : float or None, default None
         The upper bound of the colorscale.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     title : str, default 'auto'
         The title of the figure.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
         The latitude bounds of the y-axis of the figure.
     Nfig : int or str or None, default None
@@ -619,15 +619,15 @@
     autoyscale : bool, default True
         | `True` --> Enable the auto-scaling of the spectra y-axis.</br>
         | `False` --> Force use of the (vmin, vmax) bounds for the spectra plots.
     ylim_sp : tuple of float or None, default (None, None)
         If autoyscale is False, can specify the bound values for the spectrum y-axis,
         other that `(vmin, vmax)`.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
         The latitude bounds of the y-axis of the figure.
     polar : bool, default False
         If `True` --> Use a polar projection for the plot.
     cbar : bool, default True
@@ -813,15 +813,15 @@
     cmap : str, default 'Greys_r'
         The matplotlib colormap.
     vmin : float or None, default None
         The lower bound of the colorscale.
     vmax : float or None, default None
         The upper bound of the colorscale.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     title : str, default 'auto'
         The title of the figure.
     cb_title : str, default 'data'
         The title of the colorbar.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
@@ -857,24 +857,16 @@
             negatives_longitudes = True
     if title == 'auto':
         title = ('OMEGA/MEx observation {0}'.format(omega.name))
     fig = plt.figure(Nfig)
     Nfig = fig.number   # get the actual figure number if Nfig=None
     if not (mask is None):
         data = deepcopy(data) * mask     # apply mask to remove bad pixels (turned to NaN)
-    if len(fig.get_axes()) != 0:    # If presence of axes
-        ax0 = fig.get_axes()[0]
-        is_ax0_polar = hasattr(ax0, 'set_theta_offset') # Test if ax has polar projection
-        if not polar == is_ax0_polar:
-            raise ValueError("Can not mix polar and non-polar projections in the same plot")
     if polar:
-        if len(fig.get_axes()) == 0:    # Test presence of axes in the figure
-            ax = plt.axes(polar=True)
-        else:
-            ax = fig.get_axes()[0]  # Do not create new axes instance
+        ax = plt.axes(polar=True)
         plt.pcolormesh(omega.lon_grid*np.pi/180, omega.lat_grid, data, cmap=cmap, 
                        alpha=alpha, vmin=vmin, vmax=vmax, **kwargs)
         ax.set_yticklabels([])  # remove the latitude values in the plot
         if latlim[0] is None:
             if np.max(omega.lat) > 0:
                 latlim = (90, np.min(omega.lat_grid)-1)
             else:
```

### Comparing `omegapy-3.0.6/omegapy/res_findcube/cubelist` & `omegapy-3.0b0/omegapy/res_findcube/cubelist`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.6/omegapy/useful_functions.py` & `omegapy-3.0b0/omegapy/useful_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## useful_functions.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 15/05/2024
+## Last modified by Aurélien STCHERBININE : 16/10/2023
 
 ##-----------------------------------------------------------------------------------
 """Useful generics functions.
 """
 ##-----------------------------------------------------------------------------------
 ##-----------------------------------------------------------------------------------
 ## Packages
@@ -258,42 +258,38 @@
     i_closer = []
     for val in values:
         i_closer.append(where_closer(val, array))
     return np.array(i_closer)
 
 ##-----------------------------------------------------------------------------------
 ## Filename search
-def myglob(basename, exclude=[], recursive=False):
+def myglob(basename, exclude=[]):
     """Return the absolute path according to the input `basename`.
     If multiple files corresponds to `basename`, the user will be asked
     to choose one.
 
     --------------------------------------------
-    * `int` --> Select the corresponding filename.</br>
-    * `q`/`quit`/`exit` --> Return `None`.</br>
-    * `a`/`all` --> Return the list of all filenames.</br>
-
+    | `int` --> Select the corresponding filename.</br>
+    | `q`/`quit`/`exit` --> Return `None`.</br>
+    | `a`/`all` --> Return the list of all filenames.</br>
     --------------------------------------------
 
     Parameters
     ----------
     basename : str
         The basename of the target file.
     exclude : array-like of str, default []
         List of sub-strings to exclude from the results.
-    recursive : bool, default False
-        If recursive is True, the pattern `**` will match any files and
-        zero or more directories and subdirectories.
 
     Returns
     -------
     fname : str
         The absolute path of the selected file.
     """
-    fnames = glob.glob(basename, recursive=recursive)
+    fnames = glob.glob(basename)
     if not isinstance(exclude, (list, np.ndarray)):
         raise ValueError("exclude parameter must be a list or numpy.ndarray")
     if len(exclude) > 0:
         fnames2 = []
         for name in fnames:
             test = True
             for excl in exclude:
```

### Comparing `omegapy-3.0.6/omegapy.egg-info/SOURCES.txt` & `omegapy-3.0b0/omegapy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.py
 omegapy/__init__.py
 omegapy/omega_data.py
 omegapy/omega_plots.py
-omegapy/package.json
 omegapy/useful_functions.py
 omegapy.egg-info/PKG-INFO
 omegapy.egg-info/SOURCES.txt
 omegapy.egg-info/dependency_links.txt
 omegapy.egg-info/requires.txt
 omegapy.egg-info/top_level.txt
 omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
```

### Comparing `omegapy-3.0.6/setup.py` & `omegapy-3.0b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import setuptools
-import json
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 with open('requirements.txt', 'r') as f:
     requirements = f.read().strip('\n').split('\n')
-with open('omegapy/package.json', 'r') as f:
-    data_json = json.load(f)
 
 package_data = {
-    '': ['OMEGA_dataref/*', 'res_findcube/*', 'package.json'],
+    '': ['OMEGA_dataref/*', 'res_findcube/*'],
     }
 
 setuptools.setup(
     name='omegapy',
-    version=data_json['version'],
+    version='3.0beta',
     author='Aurélien Stcherbinine',
     author_email='aurelien@stcherbinine.net',
     description='Python tools for OMEGA/MEx observations analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://astcherbinine.github.io/omegapy',
     project_urls={
         'Source' : 'https://github.com/AStcherbinine/omegapy',
     },
     packages=setuptools.find_packages(),
     package_data=package_data,
-    python_requires='>='+data_json['pythonVersionMin'],
+    python_requires='>=3.7',
     setup_requires=['wheel'],
     install_requires=requirements,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research',
```

