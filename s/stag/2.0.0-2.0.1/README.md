# Comparing `tmp/stag-2.0.0.tar.gz` & `tmp/stag-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stag-2.0.0.tar", last modified: Tue May  7 10:47:59 2024, max compression
+gzip compressed data, was "stag-2.0.1.tar", last modified: Wed May 29 14:36:15 2024, max compression
```

## Comparing `stag-2.0.0.tar` & `stag-2.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 10:47:32.000000 stag-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 10:47:32.000000 stag-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 10:47:59.916824 stag-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-07 10:47:32.000000 stag-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:47:59.916824 stag-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-07 10:47:32.000000 stag-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.908824 stag-2.0.0/stag/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 10:47:32.000000 stag-2.0.0/stag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14835 2024-05-07 10:47:32.000000 stag-2.0.0/stag/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-07 10:47:32.000000 stag-2.0.0/stag/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-05-07 10:47:32.000000 stag-2.0.0/stag/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-07 10:47:32.000000 stag-2.0.0/stag/graphio.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-07 10:47:32.000000 stag-2.0.0/stag/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-07 10:47:32.000000 stag-2.0.0/stag/lsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-07 10:47:32.000000 stag-2.0.0/stag/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-07 10:47:32.000000 stag-2.0.0/stag/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-07 10:47:32.000000 stag-2.0.0/stag/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)   602218 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_internal_wrap.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_internal_wrap.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.912824 stag-2.0.0/stag/stag_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.912824 stag-2.0.0/stag/stag_lib/KMeansRex/
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.h
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/mersenneTwister2002.h
--rw-r--r--   0 runner    (1001) docker     (127)    35496 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/cluster.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/cluster.h
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/data.h
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    31852 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    23897 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graphio.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graphio.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/stag/stag_lib/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)   112777 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/indicators/indicators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26184 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/kde.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/kde.h
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/lsh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/lsh.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/stag/stag_lib/multithreading/
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/multithreading/ctpl_stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/random.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/spectrum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/spectrum.h
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/stag.h
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/stagConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/utility.h
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-05-07 10:47:32.000000 stag-2.0.0/stag/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.912824 stag-2.0.0/stag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21190 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_graphio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_lsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.656202 stag-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 14:35:47.000000 stag-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 14:35:47.000000 stag-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 14:36:15.656202 stag-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-29 14:35:47.000000 stag-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:36:15.656202 stag-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-29 14:35:47.000000 stag-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.648202 stag-2.0.1/stag/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 14:35:47.000000 stag-2.0.1/stag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14835 2024-05-29 14:35:47.000000 stag-2.0.1/stag/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-29 14:35:47.000000 stag-2.0.1/stag/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-05-29 14:35:48.000000 stag-2.0.1/stag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-29 14:35:48.000000 stag-2.0.1/stag/graphio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-29 14:35:48.000000 stag-2.0.1/stag/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-29 14:35:48.000000 stag-2.0.1/stag/lsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-29 14:35:48.000000 stag-2.0.1/stag/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-29 14:35:48.000000 stag-2.0.1/stag/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-29 14:35:48.000000 stag-2.0.1/stag/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)   602218 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_internal_wrap.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_internal_wrap.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.652202 stag-2.0.1/stag/stag_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.652202 stag-2.0.1/stag/stag_lib/KMeansRex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/KMeansRex/KMeansRexCore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/KMeansRex/KMeansRexCore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/KMeansRex/mersenneTwister2002.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35496 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/cluster.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/cluster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31852 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23897 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/graphio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/graphio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.652202 stag-2.0.1/stag/stag_lib/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)   112777 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/indicators/indicators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26184 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/kde.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/kde.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/lsh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/lsh.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.656202 stag-2.0.1/stag/stag_lib/multithreading/
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/multithreading/ctpl_stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/spectrum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/spectrum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/stag.h
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/stagConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-29 14:35:48.000000 stag-2.0.1/stag/stag_lib/utility.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-05-29 14:35:48.000000 stag-2.0.1/stag/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.648202 stag-2.0.1/stag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 14:36:15.000000 stag-2.0.1/stag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-29 14:36:15.000000 stag-2.0.1/stag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:36:15.000000 stag-2.0.1/stag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:36:15.000000 stag-2.0.1/stag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 14:36:15.000000 stag-2.0.1/stag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:15.656202 stag-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21190 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_graphio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_lsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-05-29 14:35:48.000000 stag-2.0.1/test/test_utility.py
```

### Comparing `stag-2.0.0/LICENSE` & `stag-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/PKG-INFO` & `stag-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stag
-Version: 2.0.0
+Version: 2.0.1
 Summary: STAG: Spectral Toolkit of Algorithms for Graphs
 Home-page: https://staglibrary.io
 Author: Peter Macgregor
 Author-email: <macgregor.pr@gmail.com>
 License: UNKNOWN
 Keywords: python,spectral,graph,algorithms,clustering,cheeger
 Platform: UNKNOWN
```

### Comparing `stag-2.0.0/README.md` & `stag-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/setup.py` & `stag-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 
 from setuptools import setup, find_packages
 from distutils.core import setup, Extension
 
 import numpy
 
-VERSION = '2.0.0'
+VERSION = '2.0.1'
 DESCRIPTION = 'STAG: Spectral Toolkit of Algorithms for Graphs'
 LONG_DESCRIPTION =\
     "This library provides several methods and algorithms relating to spectral graph theory in python."
 URL = "https://staglibrary.io"
 
 # Depending on the build platform, the required compiler flags are slightly
 # different.
```

### Comparing `stag-2.0.0/stag/cluster.py` & `stag-2.0.1/stag/cluster.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/data.py` & `stag-2.0.1/stag/data.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/graph.py` & `stag-2.0.1/stag/graph.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/graphio.py` & `stag-2.0.1/stag/graphio.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/kde.py` & `stag-2.0.1/stag/kde.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/lsh.py` & `stag-2.0.1/stag/lsh.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/neo4j.py` & `stag-2.0.1/stag/neo4j.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/random.py` & `stag-2.0.1/stag/random.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/spectrum.py` & `stag-2.0.1/stag/spectrum.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_internal.py` & `stag-2.0.1/stag/stag_internal.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_internal_wrap.cxx` & `stag-2.0.1/stag/stag_internal_wrap.cxx`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_internal_wrap.h` & `stag-2.0.1/stag/stag_internal_wrap.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/CHANGELOG.md` & `stag-2.0.1/stag/stag_lib/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/CMakeLists.txt` & `stag-2.0.1/stag/stag_lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.cpp` & `stag-2.0.1/stag/stag_lib/KMeansRex/KMeansRexCore.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.h` & `stag-2.0.1/stag/stag_lib/KMeansRex/KMeansRexCore.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h` & `stag-2.0.1/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/KMeansRex/mersenneTwister2002.h` & `stag-2.0.1/stag/stag_lib/KMeansRex/mersenneTwister2002.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/cluster.cpp` & `stag-2.0.1/stag/stag_lib/cluster.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/cluster.h` & `stag-2.0.1/stag/stag_lib/cluster.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/data.cpp` & `stag-2.0.1/stag/stag_lib/data.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/data.h` & `stag-2.0.1/stag/stag_lib/data.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/definitions.h` & `stag-2.0.1/stag/stag_lib/definitions.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/graph.cpp` & `stag-2.0.1/stag/stag_lib/graph.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/graph.h` & `stag-2.0.1/stag/stag_lib/graph.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/graphio.cpp` & `stag-2.0.1/stag/stag_lib/graphio.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/graphio.h` & `stag-2.0.1/stag/stag_lib/graphio.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/indicators/indicators.hpp` & `stag-2.0.1/stag/stag_lib/indicators/indicators.hpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/kde.cpp` & `stag-2.0.1/stag/stag_lib/kde.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/kde.h` & `stag-2.0.1/stag/stag_lib/kde.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/lsh.cpp` & `stag-2.0.1/stag/stag_lib/lsh.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/lsh.h` & `stag-2.0.1/stag/stag_lib/lsh.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/multithreading/ctpl_stl.h` & `stag-2.0.1/stag/stag_lib/multithreading/ctpl_stl.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/random.cpp` & `stag-2.0.1/stag/stag_lib/random.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/random.h` & `stag-2.0.1/stag/stag_lib/random.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/spectrum.cpp` & `stag-2.0.1/stag/stag_lib/spectrum.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/spectrum.h` & `stag-2.0.1/stag/stag_lib/spectrum.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/stagConfig.cmake.in` & `stag-2.0.1/stag/stag_lib/stagConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/utility.cpp` & `stag-2.0.1/stag/stag_lib/utility.cpp`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/stag_lib/utility.h` & `stag-2.0.1/stag/stag_lib/utility.h`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/stag/utility.py` & `stag-2.0.1/stag/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,18 @@
     sparse matrix, and the to_scipy() method can be used to convert back
     to a scipy matrix.
 
     If they are only used as arguments to STAG library methods, they will be very
     efficient since the data will stay on the C++ side of the library.
     """
 
+    # Prioritise this object's operator implementations over numpy
+    __array_priority__ = 1000
+
+
     def __init__(self, matrix: Union[scipy.sparse.spmatrix, List[List[float]]]):
         r"""
         Construct a STAG SprsMat.
 
         Pass either a scipy sparse matrix object or a List of Lists representing
         the dense matrix to be stored in sparse format.
 
@@ -285,20 +289,24 @@
     def __mul__(self, other):
         if isinstance(other, int):
             return SprsMat(self.internal_sprsmat.__mulint__(other))
         elif isinstance(other, float):
             return SprsMat(self.internal_sprsmat.__mulfloat__(other))
         elif isinstance(other, SprsMat):
             return SprsMat(self.internal_sprsmat * other.internal_sprsmat)
+        elif isinstance(other, np.ndarray):
+            return self.to_scipy() * other
         else:
             return NotImplemented
 
     def __rmul__(self, other):
         if isinstance(other, SprsMat):
             return SprsMat(other.internal_sprsmat * self.internal_sprsmat)
+        elif isinstance(other, np.ndarray):
+            return other * self.to_scipy()
         else:
             return self.__mul__(other)
 
     def __matmul__(self, other):
         return self.__mul__(other)
 
     def __rmatmul__(self, other):
```

### Comparing `stag-2.0.0/stag.egg-info/PKG-INFO` & `stag-2.0.1/stag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stag
-Version: 2.0.0
+Version: 2.0.1
 Summary: STAG: Spectral Toolkit of Algorithms for Graphs
 Home-page: https://staglibrary.io
 Author: Peter Macgregor
 Author-email: <macgregor.pr@gmail.com>
 License: UNKNOWN
 Keywords: python,spectral,graph,algorithms,clustering,cheeger
 Platform: UNKNOWN
```

### Comparing `stag-2.0.0/stag.egg-info/SOURCES.txt` & `stag-2.0.1/stag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_clustering.py` & `stag-2.0.1/test/test_clustering.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_graph.py` & `stag-2.0.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_graphio.py` & `stag-2.0.1/test/test_graphio.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_kde.py` & `stag-2.0.1/test/test_kde.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_lsh.py` & `stag-2.0.1/test/test_lsh.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_performance.py` & `stag-2.0.1/test/test_performance.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_random.py` & `stag-2.0.1/test/test_random.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_spectrum.py` & `stag-2.0.1/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `stag-2.0.0/test/test_utility.py` & `stag-2.0.1/test/test_utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,54 @@
     assert(np.all(mat_diff.to_dense() == pytest.approx(0)))
 
     mat2 *= mat1
     mat_diff = mat2 - expected_mat
     assert(np.all(mat_diff.to_dense() == pytest.approx(0)))
 
 
+def test_sprsmat_numpy_matmul():
+    # Multiplying by numpy dense matrix will give
+    # numpy matrix
+    mat1 = stag.utility.SprsMat([[0, 1, 0, 1],
+                                 [1, 0, 1, 0],
+                                 [0, 1, 0, 1],
+                                 [1, 0, 1, 0]])
+    mat2 = np.asarray([[0, 3, 1, 1],
+                       [0, 0, 0, 2],
+                       [3, 0, 0, 2],
+                       [1, 1, 1, 1]])
+    expected_mat = np.asarray([[1, 1, 1, 3],
+                               [3, 3, 1, 3],
+                               [1, 1, 1, 3],
+                               [3, 3, 1, 3]])
+    mat3 = mat1 * mat2
+    mat_diff = mat3 - expected_mat
+    assert(np.all(mat_diff == pytest.approx(0)))
+
+    mat3 = mat1 @ mat2
+    mat_diff = mat3 - expected_mat
+    assert(np.all(mat_diff == pytest.approx(0)))
+
+    expected_mat = np.asarray([[4, 1, 4, 1],
+                               [2, 0, 2, 0],
+                               [2, 3, 2, 3],
+                               [2, 2, 2, 2]])
+    mat3 = mat2 * mat1
+    mat_diff = mat3 - expected_mat
+    assert(np.all(mat_diff == pytest.approx(0)))
+
+    mat3 = mat2 @ mat1
+    mat_diff = mat3 - expected_mat
+    assert(np.all(mat_diff == pytest.approx(0)))
+
+    mat2 *= mat1
+    mat_diff = mat2 - expected_mat
+    assert(np.all(mat_diff == pytest.approx(0)))
+
+
 def test_sprsmat_outer_product():
     vec1 = stag.utility.SprsMat([[1, 2, 0, 1]])
     vec2 = stag.utility.SprsMat([[0, -2, 1, 0]])
 
     expected_mat = stag.utility.SprsMat([[0, -2, 1, 0],
                                          [0, -4, 2, 0],
                                          [0, 0, 0, 0],
```

