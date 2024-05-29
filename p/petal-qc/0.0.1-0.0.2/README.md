# Comparing `tmp/petal_qc-0.0.1.tar.gz` & `tmp/petal_qc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petal_qc-0.0.1.tar", last modified: Mon May 20 22:23:03 2024, max compression
+gzip compressed data, was "petal_qc-0.0.2.tar", last modified: Wed May 29 08:29:01 2024, max compression
```

## Comparing `petal_qc-0.0.1.tar` & `petal_qc-0.0.2.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.807062 petal_qc-0.0.1/
--rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-20 22:23:03.806849 petal_qc-0.0.1/PKG-INFO
--rw-r--r--   0 lacasta    (501) staff       (20)      179 2024-05-17 07:56:57.000000 petal_qc-0.0.1/README.md
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.798483 petal_qc-0.0.1/petal_qc/
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.799824 petal_qc-0.0.1/petal_qc/BTreport/
--rw-r--r--   0 lacasta    (501) staff       (20)     9086 2024-05-19 10:03:41.000000 petal_qc-0.0.1/petal_qc/BTreport/CheckBTtests.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:22.000000 petal_qc-0.0.1/petal_qc/BTreport/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     6895 2024-05-19 10:14:36.000000 petal_qc-0.0.1/petal_qc/BTreport/bustapeReport.py
--rw-r--r--   0 lacasta    (501) staff       (20)      337 2024-05-17 15:12:21.000000 petal_qc-0.0.1/petal_qc/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)      553 2024-05-17 15:29:20.000000 petal_qc-0.0.1/petal_qc/dashBoard.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.803030 petal_qc-0.0.1/petal_qc/metrology/
--rw-r--r--   0 lacasta    (501) staff       (20)     2105 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/metrology/Cluster.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1367 2024-05-17 08:33:02.000000 petal_qc-0.0.1/petal_qc/metrology/DataFile.py
--rw-r--r--   0 lacasta    (501) staff       (20)    11886 2024-05-17 15:09:00.000000 petal_qc-0.0.1/petal_qc/metrology/PetalMetrology.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:20.000000 petal_qc-0.0.1/petal_qc/metrology/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1569 2023-09-13 15:37:58.000000 petal_qc-0.0.1/petal_qc/metrology/all2csv.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)    20539 2024-05-17 14:35:44.000000 petal_qc-0.0.1/petal_qc/metrology/analyze_locking_points.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3106 2023-06-27 23:03:41.000000 petal_qc-0.0.1/petal_qc/metrology/cold_noise.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1743 2023-07-17 12:10:41.000000 petal_qc-0.0.1/petal_qc/metrology/comparisonTable.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5449 2024-05-13 18:45:58.000000 petal_qc-0.0.1/petal_qc/metrology/convert_mitutoyo.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3836 2024-05-17 08:33:52.000000 petal_qc-0.0.1/petal_qc/metrology/convert_smartscope.py
--rw-r--r--   0 lacasta    (501) staff       (20)    13610 2024-05-19 17:46:54.000000 petal_qc-0.0.1/petal_qc/metrology/coreMetrology.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1809 2023-08-31 06:45:26.000000 petal_qc-0.0.1/petal_qc/metrology/data2csv.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3977 2024-05-17 08:30:55.000000 petal_qc-0.0.1/petal_qc/metrology/do_Metrology.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4071 2023-09-08 15:22:08.000000 petal_qc-0.0.1/petal_qc/metrology/flatness4nigel.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3372 2024-05-14 08:23:47.000000 petal_qc-0.0.1/petal_qc/metrology/gtkutils.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)    11190 2024-05-17 08:29:23.000000 petal_qc-0.0.1/petal_qc/metrology/petal_flatness.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)     4057 2024-05-17 08:37:41.000000 petal_qc-0.0.1/petal_qc/metrology/show_data_file.py
--rw-r--r--   0 lacasta    (501) staff       (20)      994 2023-07-17 12:15:20.000000 petal_qc-0.0.1/petal_qc/metrology/testSummary.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1981 2023-06-29 09:43:18.000000 petal_qc-0.0.1/petal_qc/metrology/test_paralelism.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.805651 petal_qc-0.0.1/petal_qc/thermal/
--rw-r--r--   0 lacasta    (501) staff       (20)     2038 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/CSVImage.py
--rw-r--r--   0 lacasta    (501) staff       (20)     2119 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/DebugPlot.py
--rw-r--r--   0 lacasta    (501) staff       (20)    22225 2023-06-08 14:59:18.000000 petal_qc-0.0.1/petal_qc/thermal/IRBFile.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3029 2024-05-17 10:38:18.000000 petal_qc-0.0.1/petal_qc/thermal/IRCore.py
--rw-r--r--   0 lacasta    (501) staff       (20)     9662 2024-05-17 10:40:19.000000 petal_qc-0.0.1/petal_qc/thermal/IRDataGetter.py
--rwxr-xr-x   0 lacasta    (501) staff       (20)    38208 2024-05-17 08:53:09.000000 petal_qc-0.0.1/petal_qc/thermal/IRPetal.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3516 2024-05-20 07:51:25.000000 petal_qc-0.0.1/petal_qc/thermal/IRPetalParam.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3831 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/PetalColorMaps.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3910 2024-05-17 10:42:03.000000 petal_qc-0.0.1/petal_qc/thermal/Petal_IR_Analysis.py
--rw-r--r--   0 lacasta    (501) staff       (20)    17191 2024-05-17 10:43:12.000000 petal_qc-0.0.1/petal_qc/thermal/PipeFit.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-03-06 14:33:23.000000 petal_qc-0.0.1/petal_qc/thermal/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)    14463 2024-05-20 22:20:53.000000 petal_qc-0.0.1/petal_qc/thermal/analyze_IRCore.py
--rw-r--r--   0 lacasta    (501) staff       (20)     8244 2024-05-17 08:48:22.000000 petal_qc-0.0.1/petal_qc/thermal/contours.py
--rw-r--r--   0 lacasta    (501) staff       (20)    14428 2024-05-20 22:22:29.000000 petal_qc-0.0.1/petal_qc/thermal/coreThermal.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5638 2024-05-20 13:04:26.000000 petal_qc-0.0.1/petal_qc/thermal/create_IRCore.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3632 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/pipe_back.npz
--rw-r--r--   0 lacasta    (501) staff       (20)     3697 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/thermal/pipe_front.npz
--rwxr-xr-x   0 lacasta    (501) staff       (20)     5040 2024-05-17 10:42:44.000000 petal_qc-0.0.1/petal_qc/thermal/pipe_read.py
--rw-r--r--   0 lacasta    (501) staff       (20)    13029 2024-05-17 10:45:10.000000 petal_qc-0.0.1/petal_qc/thermal/show_IR_petal.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.806440 petal_qc-0.0.1/petal_qc/utils/
--rw-r--r--   0 lacasta    (501) staff       (20)    19765 2023-09-08 15:30:11.000000 petal_qc-0.0.1/petal_qc/utils/Geometry.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4064 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/utils/Progress.py
--rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-06-09 13:24:48.000000 petal_qc-0.0.1/petal_qc/utils/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1044 2023-10-20 08:59:51.000000 petal_qc-0.0.1/petal_qc/utils/all_files.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5805 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/utils/docx_utils.py
--rw-r--r--   0 lacasta    (501) staff       (20)     5349 2023-03-06 14:36:41.000000 petal_qc-0.0.1/petal_qc/utils/fit_utils.py
--rw-r--r--   0 lacasta    (501) staff       (20)     4035 2024-05-15 09:50:28.000000 petal_qc-0.0.1/petal_qc/utils/utils.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-20 22:23:03.806614 petal_qc-0.0.1/petal_qc.egg-info/
--rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (501) staff       (20)     1816 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (501) staff       (20)       92 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (501) staff       (20)      102 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/requires.txt
--rw-r--r--   0 lacasta    (501) staff       (20)        9 2024-05-20 22:23:03.000000 petal_qc-0.0.1/petal_qc.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (501) staff       (20)      995 2024-05-18 10:08:12.000000 petal_qc-0.0.1/pyproject.toml
--rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-05-20 22:23:03.807099 petal_qc-0.0.1/setup.cfg
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.120424 petal_qc-0.0.2/
+-rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-29 08:29:01.120225 petal_qc-0.0.2/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)      179 2024-05-17 07:56:57.000000 petal_qc-0.0.2/README.md
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.113112 petal_qc-0.0.2/petal_qc/
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.114051 petal_qc-0.0.2/petal_qc/BTreport/
+-rw-r--r--   0 lacasta    (501) staff       (20)     9086 2024-05-19 10:03:41.000000 petal_qc-0.0.2/petal_qc/BTreport/CheckBTtests.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:22.000000 petal_qc-0.0.2/petal_qc/BTreport/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     6895 2024-05-19 10:14:36.000000 petal_qc-0.0.2/petal_qc/BTreport/bustapeReport.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      337 2024-05-29 08:05:41.000000 petal_qc-0.0.2/petal_qc/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      553 2024-05-17 15:29:20.000000 petal_qc-0.0.2/petal_qc/dashBoard.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.116394 petal_qc-0.0.2/petal_qc/metrology/
+-rw-r--r--   0 lacasta    (501) staff       (20)     2105 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/metrology/Cluster.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1367 2024-05-17 08:33:02.000000 petal_qc-0.0.2/petal_qc/metrology/DataFile.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    11886 2024-05-17 15:09:00.000000 petal_qc-0.0.2/petal_qc/metrology/PetalMetrology.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2024-05-17 08:12:20.000000 petal_qc-0.0.2/petal_qc/metrology/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1569 2023-09-13 15:37:58.000000 petal_qc-0.0.2/petal_qc/metrology/all2csv.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)    20539 2024-05-17 14:35:44.000000 petal_qc-0.0.2/petal_qc/metrology/analyze_locking_points.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3106 2023-06-27 23:03:41.000000 petal_qc-0.0.2/petal_qc/metrology/cold_noise.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1743 2023-07-17 12:10:41.000000 petal_qc-0.0.2/petal_qc/metrology/comparisonTable.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5449 2024-05-13 18:45:58.000000 petal_qc-0.0.2/petal_qc/metrology/convert_mitutoyo.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3836 2024-05-17 08:33:52.000000 petal_qc-0.0.2/petal_qc/metrology/convert_smartscope.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    13610 2024-05-19 17:46:54.000000 petal_qc-0.0.2/petal_qc/metrology/coreMetrology.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1809 2023-08-31 06:45:26.000000 petal_qc-0.0.2/petal_qc/metrology/data2csv.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3977 2024-05-17 08:30:55.000000 petal_qc-0.0.2/petal_qc/metrology/do_Metrology.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4071 2023-09-08 15:22:08.000000 petal_qc-0.0.2/petal_qc/metrology/flatness4nigel.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3372 2024-05-14 08:23:47.000000 petal_qc-0.0.2/petal_qc/metrology/gtkutils.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)    11190 2024-05-17 08:29:23.000000 petal_qc-0.0.2/petal_qc/metrology/petal_flatness.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)     4057 2024-05-17 08:37:41.000000 petal_qc-0.0.2/petal_qc/metrology/show_data_file.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      994 2023-07-17 12:15:20.000000 petal_qc-0.0.2/petal_qc/metrology/testSummary.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1981 2023-06-29 09:43:18.000000 petal_qc-0.0.2/petal_qc/metrology/test_paralelism.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.118831 petal_qc-0.0.2/petal_qc/thermal/
+-rw-r--r--   0 lacasta    (501) staff       (20)     2038 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/thermal/CSVImage.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     2119 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/thermal/DebugPlot.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    22270 2024-05-24 06:51:59.000000 petal_qc-0.0.2/petal_qc/thermal/IRBFile.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3056 2024-05-28 22:21:29.000000 petal_qc-0.0.2/petal_qc/thermal/IRCore.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    10580 2024-05-28 22:33:53.000000 petal_qc-0.0.2/petal_qc/thermal/IRDataGetter.py
+-rwxr-xr-x   0 lacasta    (501) staff       (20)    38334 2024-05-23 12:28:32.000000 petal_qc-0.0.2/petal_qc/thermal/IRPetal.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3674 2024-05-28 14:55:41.000000 petal_qc-0.0.2/petal_qc/thermal/IRPetalParam.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3831 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/thermal/PetalColorMaps.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3910 2024-05-17 10:42:03.000000 petal_qc-0.0.2/petal_qc/thermal/Petal_IR_Analysis.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    17214 2024-05-28 14:53:09.000000 petal_qc-0.0.2/petal_qc/thermal/PipeFit.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-03-06 14:33:23.000000 petal_qc-0.0.2/petal_qc/thermal/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    18086 2024-05-28 21:51:46.000000 petal_qc-0.0.2/petal_qc/thermal/analyze_IRCore.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     8244 2024-05-17 08:48:22.000000 petal_qc-0.0.2/petal_qc/thermal/contours.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    12320 2024-05-28 21:50:55.000000 petal_qc-0.0.2/petal_qc/thermal/coreThermal.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     6206 2024-05-29 08:22:50.000000 petal_qc-0.0.2/petal_qc/thermal/create_IRCore.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4239 2024-05-28 21:52:22.000000 petal_qc-0.0.2/petal_qc/thermal/create_core_report.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3632 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/thermal/pipe_back.npz
+-rw-r--r--   0 lacasta    (501) staff       (20)     3697 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/thermal/pipe_front.npz
+-rwxr-xr-x   0 lacasta    (501) staff       (20)     5040 2024-05-17 10:42:44.000000 petal_qc-0.0.2/petal_qc/thermal/pipe_read.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    13159 2024-05-23 07:38:52.000000 petal_qc-0.0.2/petal_qc/thermal/show_IR_petal.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      878 2024-05-29 08:03:35.000000 petal_qc-0.0.2/petal_qc/thermal/test_Graphana.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1516 2024-05-28 21:53:06.000000 petal_qc-0.0.2/petal_qc/thermal/test_coreThermal.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.119815 petal_qc-0.0.2/petal_qc/utils/
+-rw-r--r--   0 lacasta    (501) staff       (20)    19765 2023-09-08 15:30:11.000000 petal_qc-0.0.2/petal_qc/utils/Geometry.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4064 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/utils/Progress.py
+-rw-r--r--   0 lacasta    (501) staff       (20)        0 2023-06-09 13:24:48.000000 petal_qc-0.0.2/petal_qc/utils/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1044 2023-10-20 08:59:51.000000 petal_qc-0.0.2/petal_qc/utils/all_files.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5805 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/utils/docx_utils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     5349 2023-03-06 14:36:41.000000 petal_qc-0.0.2/petal_qc/utils/fit_utils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1862 2024-05-29 07:24:26.000000 petal_qc-0.0.2/petal_qc/utils/readGraphana.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4035 2024-05-15 09:50:28.000000 petal_qc-0.0.2/petal_qc/utils/utils.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-05-29 08:29:01.120001 petal_qc-0.0.2/petal_qc.egg-info/
+-rw-r--r--   0 lacasta    (501) staff       (20)      943 2024-05-29 08:29:01.000000 petal_qc-0.0.2/petal_qc.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)     1957 2024-05-29 08:29:01.000000 petal_qc-0.0.2/petal_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-05-29 08:29:01.000000 petal_qc-0.0.2/petal_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       92 2024-05-29 08:29:01.000000 petal_qc-0.0.2/petal_qc.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      102 2024-05-29 08:29:01.000000 petal_qc-0.0.2/petal_qc.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        9 2024-05-29 08:29:01.000000 petal_qc-0.0.2/petal_qc.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      995 2024-05-29 08:05:41.000000 petal_qc-0.0.2/pyproject.toml
+-rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-05-29 08:29:01.120459 petal_qc-0.0.2/setup.cfg
```

### Comparing `petal_qc-0.0.1/PKG-INFO` & `petal_qc-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petal_qc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of scripts for Petal CORE QC.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `petal_qc-0.0.1/petal_qc/BTreport/CheckBTtests.py` & `petal_qc-0.0.2/petal_qc/BTreport/CheckBTtests.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/BTreport/bustapeReport.py` & `petal_qc-0.0.2/petal_qc/BTreport/bustapeReport.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/dashBoard.py` & `petal_qc-0.0.2/petal_qc/dashBoard.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/Cluster.py` & `petal_qc-0.0.2/petal_qc/metrology/Cluster.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/DataFile.py` & `petal_qc-0.0.2/petal_qc/metrology/DataFile.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/PetalMetrology.py` & `petal_qc-0.0.2/petal_qc/metrology/PetalMetrology.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/all2csv.py` & `petal_qc-0.0.2/petal_qc/metrology/all2csv.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/analyze_locking_points.py` & `petal_qc-0.0.2/petal_qc/metrology/analyze_locking_points.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/cold_noise.py` & `petal_qc-0.0.2/petal_qc/metrology/cold_noise.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/comparisonTable.py` & `petal_qc-0.0.2/petal_qc/metrology/comparisonTable.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/convert_mitutoyo.py` & `petal_qc-0.0.2/petal_qc/metrology/convert_mitutoyo.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/convert_smartscope.py` & `petal_qc-0.0.2/petal_qc/metrology/convert_smartscope.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/coreMetrology.py` & `petal_qc-0.0.2/petal_qc/metrology/coreMetrology.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/data2csv.py` & `petal_qc-0.0.2/petal_qc/metrology/data2csv.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/do_Metrology.py` & `petal_qc-0.0.2/petal_qc/metrology/do_Metrology.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/flatness4nigel.py` & `petal_qc-0.0.2/petal_qc/metrology/flatness4nigel.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/gtkutils.py` & `petal_qc-0.0.2/petal_qc/metrology/gtkutils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/petal_flatness.py` & `petal_qc-0.0.2/petal_qc/metrology/petal_flatness.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/show_data_file.py` & `petal_qc-0.0.2/petal_qc/metrology/show_data_file.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/testSummary.py` & `petal_qc-0.0.2/petal_qc/metrology/testSummary.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/metrology/test_paralelism.py` & `petal_qc-0.0.2/petal_qc/metrology/test_paralelism.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/CSVImage.py` & `petal_qc-0.0.2/petal_qc/thermal/CSVImage.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/DebugPlot.py` & `petal_qc-0.0.2/petal_qc/thermal/DebugPlot.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/IRBFile.py` & `petal_qc-0.0.2/petal_qc/thermal/IRBFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import bz2
 import copy
 import datetime
 import os
 import pickle
 import struct
 import sys
+from argparse import ArgumentParser
 from collections.abc import Iterable
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 OLE_TIME_ZERO = datetime.datetime(1899, 12, 30, 0, 0, 0)
@@ -715,21 +716,20 @@
             except Exception as eee:
                 print(eee)
                 irbf = None
 
     return irbf
 
 
-if __name__ == "__main__":
+def main():
     """Example of use of IRBFile.
 
-    Shows all the images in a file.
+       Shows all the images in a file.
 
     """
-    from argparse import ArgumentParser
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
     parser.add_argument("--save", action="store_true",
                         default=False,
                         help="save all figures")
     options = parser.parse_args()
     if len(options.files) == 0:
@@ -739,15 +739,16 @@
     IRfile = IRBFile(options.files)
     nimgs = IRfile.nimages
     print("Number of images: {}".format(nimgs))
 
     fig = None
     nimg = 0
     ratio = -1
-    for img in IRfile.images():
+    for ximg in IRfile.images():
+        img = ximg[0]
         tmin = np.min(img.image)
         print("Tmin {:1f} - {}x{}".format(tmin, img.width, img.height))
         if ratio < 0:
             ratio = float(img.width)/float(img.height)
 
         plt.clf()
         plt.gca().clear()
@@ -762,7 +763,10 @@
 
             fig.savefig('fig_{}.png'.format(nimg), dpi=300)
             nimg += 1
 
         plt.pause(0.00001)
 
     plt.show()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/IRCore.py` & `petal_qc-0.0.2/petal_qc/thermal/IRCore.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         self.aliasID = alias
         self.date = None
         self.institute = params.institute if params is not None else None
         self.params = params
         self.files = []
         self.results = [] if results is None else results  # list of AnalysisResults. One per side
         self.golden = []                                    # list of Golden results. One per side.
+        self.inlet = -9999
 
     def set_files(self, files):
         """Set the input files."""
         self.files = []
         for F in files:
             self.files.append(F)
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/IRDataGetter.py` & `petal_qc-0.0.2/petal_qc/thermal/IRDataGetter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 """Encapsulates different data structure at DESY and IFIC.
 """
+import sys
+from pathlib import Path
+import numpy as np
+
+try:
+    import petal_qc
+
+except ImportError:
+    cwd = Path(__file__).parent.parent.parent
+    sys.path.append(cwd.as_posix())
 
 
-import numpy as np
 from petal_qc.thermal import IRPetal
 from petal_qc.thermal import Petal_IR_Analysis
 
+HAS_GRAPHANA = False
+try:
+    from petal_qc.utils.readGraphana import ReadGraphana
+    HAS_GRAPHANA = True
+    
+except ImportError:
+    HAS_GRAPHANA = False
+    
+
 
 class IRDataGetter(object):
     """BAse class defining the interface."""
 
     def __init__(self):
         """Initialization."""
         self.factor = 1
@@ -97,21 +115,30 @@
         """
         pass
 
     def get_analysis_frame(self, irbf):
         """Get the frame where we want to perform the analysis."""
         return None
 
+    def get_inlet_temperature(self):
+        """REturn the inlet temperature."""
+        return -9999
+
 
 class IRDataIFIC(IRDataGetter):
     """Gets data for IFIC analysis."""
 
     def __init__(self) -> None:
         """Initialization."""
         super().__init__()
+        self.analysis_frame = None
+        if HAS_GRAPHANA:
+            self.DB = ReadGraphana("localhost")
+        else:
+            self.DB = None
 
     def find_reference_image(self, irbf, *args, **kargs):
         """Find first image in sequence with T < T_min.
 
         Args:
         ----
             irbf: The sequence of IR images
@@ -232,15 +259,27 @@
         """
         # Get all the temperatures
         min_T = []
         for img in irbf.images():
             min_T.append(np.min(img[0].image))
 
         indx = IRDataIFIC.find_minimum(min_T)
-        return [irbf.getImage(indx[-1])]
+        self.analysis_frame = [irbf.getImage(indx[-1])]
+        return self.analysis_frame
+
+    def get_inlet_temperature(self):
+        """REturn the inlet temperature."""
+        if self.DB:
+            img = self.analysis_frame[0]
+            val = self.DB.get_temperature(img.timestamp, 10)
+            return val
+        
+        else:
+            return -9999
+            
 
 
 class IRDataDESY(IRDataGetter):
     """Gets data for DESY."""
 
     def __init__(self) -> None:
         """Initialization."""
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/IRPetal.py` & `petal_qc-0.0.2/petal_qc/thermal/IRPetal.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.polynomial import polynomial as Polynomial
 from scipy import ndimage
 from scipy.optimize import minimize
 from skimage import measure
 
+try:
+    import petal_qc
+
+except ImportError:
+    cwd = Path(__file__).parent.parent.parent
+    sys.path.append(cwd.as_posix())
+
 from petal_qc.thermal import contours
 from petal_qc.thermal import CSVImage
 from petal_qc.thermal import DebugPlot
 from petal_qc.thermal import IRBFile
 from petal_qc.thermal import PipeFit
 from petal_qc.utils.Geometry import Line
 from petal_qc.utils.Geometry import Point
@@ -1208,15 +1215,15 @@
 
         img: the image
         i_min: the index of the image in the sequence.
 
     """
     img = None
     i_min = frame
-    if irbf.n_images() == 0:
+    if irbf.nimages == 0:
         print("Input file does not contain images.")
 
     else:
         if frame >= 0:
             img = irbf.getImage(frame)
             if img is None:
                 raise LookupError("Frame {} not found in [0, {}]".format(frame, irbf.n_images()))
@@ -1242,20 +1249,20 @@
     -------
         An image
 
     """
     ifile = Path(fnam).expanduser().resolve()
     if not ifile.exists():
         print("Input file does not exist.")
-        return None
+        return None, None
 
     suffix = ifile.suffix.lower()
-    img = None
+    img = None, None
     if suffix == ".csv":
-        img = CSVImage.CSVImage(ifile)
+        img = CSVImage.CSVImage(ifile), 0
 
     elif suffix == ".irb":
         irbf = IRBFile.IRBFile(ifile)
         img = get_image_from_irb(irbf, frame, thrs)
 
     else:
         try:
@@ -1270,31 +1277,31 @@
 
 def main(fnam, options):
     """Read data and plot edges."""
     params = IRPetalParam(options)
     params.debug = False
 
     print("Open file")
-    img = read_image(fnam, options.frame, options.thrs)
+    img, _ = read_image(fnam, options.frame, options.thrs)
     if img is None:
         sys.exit()
 
     # Show original Image
-    fig, ax = plt.subplots(1, 1, dpi=300)
+    fig, ax = plt.subplots(1, 1)
     values = get_IR_data(img, False)
     min_T = np.min(values)
     fig.suptitle("Original image - Temp. {:.1f}".format(min_T))
     pcm = ax.imshow(values, origin='lower', cmap="jet")
     fig.colorbar(pcm, ax=ax)
     fig.savefig("original-IR-img.png")
 
     # Show rotated image
     values = get_IR_data(img, True)
     min_T = np.min(values)
-    fig, ax = plt.subplots(1, 1, dpi=300)
+    fig, ax = plt.subplots(1, 1)
     fig.suptitle("Rotated image - Temp. {:.1f}".format(min_T))
     pcm = ax.imshow(values, origin='lower', cmap="jet")
     fig.colorbar(pcm, ax=ax)
     fig.savefig("rotated-IR-image.png")
 
     # Split image
     left, right = split_IR_image(values)
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/IRPetalParam.py` & `petal_qc-0.0.2/petal_qc/thermal/IRPetalParam.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
         Args:
         ----
             values: ArgParser or dict with user values-
 
         """
         self.institute = 'IFIC'   # Either IFIC or DESY to treat the different files
-        self.thrs = -20.0         # the threshold
+        self.thrs = -22.0         # the threshold
         self.tco2 = -35.0         # Inlet temperature
         self.gauss_size = 15      # Radius of gausian filtering
         self.grad_sigma = 2.5     # Sigma of grading calculation
         self.distance = 5         # Distance in contour between slices
         self.npoints = 15         # Number of points per segment
         self.min_area = 2500      # minumum area of a valid contour.
         self.contour_cut = 0.2    # Fraction of IR image range to define contour.
         self.contour_smooth = 25  # Value to smooth contour
         self.width = 2            # half widh of rectangle around point in path when getting T.
         self.do_fit = True        # True to fit the segment points.
         self.rotate = True        # Rotate to have a vertical petal in mirror image
         self.debug = False        # To debug
+        self.report = False       # 
 
         if values is not None:
             self.set_values(values)
 
     def set_values(self, values):
         """Set parameters from input values."""
         if isinstance(values, dict):
@@ -67,7 +68,8 @@
         parser.add_argument("--width", type=int, default=P.width,
                             help="width of average rectangle en get_T_along_path.")
         parser.add_argument("--contour_cut", type=float, default=P.contour_cut,
                             help="Fraction of IR image range to define contour.")
         parser.add_argument("--contour_smooth", type=float, default=P.contour_smooth,
                             help="Value to smooth contour")
         parser.add_argument("--debug", action="store_true", default=False, help="Show additional information.")
+        parser.add_argument("--report", action="store_true", default=False, help="True if figures kept for the report.")
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/PetalColorMaps.py` & `petal_qc-0.0.2/petal_qc/thermal/PetalColorMaps.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/Petal_IR_Analysis.py` & `petal_qc-0.0.2/petal_qc/thermal/Petal_IR_Analysis.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/PipeFit.py` & `petal_qc-0.0.2/petal_qc/thermal/PipeFit.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,15 @@
         else:
             out = self.data
 
         ax.plot(out[:, 0], out[:, 1], 'o', label="Data")
         ax.legend()
         plt.draw()
         plt.pause(0.0001)
+        return fig, ax
 
 
 def main(data_file, opts):
     """The main entry.
 
     Args:
     ----
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/analyze_IRCore.py` & `petal_qc-0.0.2/petal_qc/thermal/analyze_IRCore.py`

 * *Files 26% similar despite different names*

```diff
@@ -162,19 +162,110 @@
 
     return golden, result_list
 
 def golden_from_json(js_golden):
     """Converst a JSon golden into a Golden object."""
     golden = [Petal_IR_Analysis.AnalysisResult() for i in range(2)]
     for i, G in enumerate(golden):
-        G.path_length = js_golden[i]["path_length"]
-        G.path_temp = js_golden[i]["path_temp"]
-        G.path_spread = js_golden[i]["path_spread"]
-        G.sensor_avg = js_golden[i]["sensor_avg"]
-        G.sensor_std = js_golden[i]["sensor_std"]   
+        G.path_length = np.array(js_golden[i]["path_length"])
+        G.path_temp = np.array(js_golden[i]["path_temp"])
+        G.path_spread = np.array(js_golden[i]["path_spread"])
+        G.sensor_avg = np.array(js_golden[i]["sensor_avg"])
+        G.sensor_std = np.array(js_golden[i]["sensor_std"])
+
+    return golden
+
+def get_golden_axis(R, golden):
+    """Compute result on golden points."""
+    xvalues = [ [x for x in golden[i].path_length] for i in range(2) ]
+    R.golden = []
+    for iside in range(2):
+        G = Petal_IR_Analysis.AnalysisResult()
+        splnT = CubicSpline(R.results[iside].path_length, R.results[iside].path_temp)
+        splnS = CubicSpline(R.results[iside].path_length, R.results[iside].path_spread)
+        G.path_length = np.array(xvalues[iside])
+        G.path_temp = np.array([splnT(x) for x in G.path_length])
+        G.path_spread = np.array([splnS(x) for x in G.path_length])
+        G.sensor_avg = np.array(R.results[iside].sensor_avg)
+        G.sensor_std = np.array(R.results[iside].sensor_std)
+        R.golden.append(G)
+
+
+def plot_profile_and_golden(golden, core, value):
+    """Plot petal core and golden average.
+
+    Args:
+    ----
+        resuls: results from create_golden_average
+        golden: golden values (from create_golgen_average)
+        value: value to show, ej path_temp, path_spread, sensor_avg, sensor_std
+
+    """
+    tick_labels = ["R0", "R1", "R2", "R3", "R3", "R4", "R4", "R5", "R5", "EoS"]
+    figures = []
+    factor = 1.0
+    if value.find("sensor") >= 0:
+        factor = 2.0
+
+    # Get acceptance band
+    band = get_acceptance_band()
+
+    for iside in range(2):
+        fig, ax = plt.subplots(2, 1, tight_layout=True, gridspec_kw={'height_ratios': (0.66, 0.34)})
+        figures.append(fig)
+        fig.suptitle("Petal core .vs. Golden for {} - side {}.".format(value, iside))
+        for a in ax:
+            a.grid()
+
+        if value.find("path") < 0:
+            for i in range(2):
+                ax[i].set_xticks(range(10), labels=tick_labels)
+
+        RS = core.results[iside]
+        # convert to golden X
+        # TODO: get X, Y from petal core. Move golden to this X axis and draw differences.
+        # This only happens for the "_path" values, not for the sensors.
+        if value.find("path") >= 0:
+            X = RS.path_length
+            Y = getattr(RS, value)
+            spln = CubicSpline(golden[iside].path_length, getattr(golden[iside], value))
+            gY = np.array([spln(x) for x in X])
+        else:
+            X = np.array([float(x) for x in range(10)])
+            Y = getattr(RS, value)
+            gY = getattr(golden[iside], value)
+
+        delta = Y - gY
+        ax[0].plot(X, Y, '-', label=core.aliasID, linewidth=1)
+        ax[1].plot(X, delta, '-', label=core.aliasID, linewidth=1)
+
+        # Draw golden line
+        ax[0].plot(X, gY, '-', label="Golden", linewidth=4, alpha=0.4, color="black")
+
+        Tmean = np.mean(Y)
+        Tband = factor*abs(Tmean)/3
+
+        ax[0].legend(ncol=3, fontsize="x-small")
+        ax[0].set_title("T$_{prof}$ values")
+        if value.find("temp") >= 0 or value.find("_avg") >= 0:
+            ax[0].set_ylim(Tmean-Tband, Tmean+Tband)
+            ax[0].fill_between(X, gY + band, gY - band,
+                               facecolor="yellow", alpha=0.25,
+                               label="Acceptance band")
+
+            ax[1].fill_between(X, band, -band,
+                               facecolor="yellow", alpha=0.25,
+                               label="Acceptance band")
+
+        ax[1].legend(ncol=4, fontsize="x-small")
+        ax[1].set_title("T$_{prof}$ - Golden avg.")
+        if value.find("temp") >= 0 or value.find("_avg") >= 0:
+            ax[1].set_ylim(-Tband, Tband)
+
+    return figures
 
 def show_golden_average(golden, results, value):
     """Create golden average.
 
     Args:
     ----
         golden: golden values (from create_golgen_average)
@@ -280,18 +371,18 @@
 def analyze_petal_cores(files, golden, options):
     """Create golden average.
 
     Args:
         files (list): List of input files
         golden: the golden object
         options: other options.
-    
+
     Return:
         array with JSon objects corresponding to the PDB test.
-        
+
     """
     output = []
     names = get_names(files)
     for i, ifile in enumerate(files):
         ifile = find_file(options.folder, ifile)
         if not ifile.exists():
             print("+++ File {} does not exist.".format(ifile))
@@ -367,18 +458,18 @@
         # Check if we are given an output folder
         ofile = output_folder(options.folder, ofile)
         with open(ofile, 'w', encoding="UTF-8") as fp:
             print("writing {}".format(ofile))
             json.dump(dbOut, fp, indent=3, cls=IRCore.NumpyArrayEncoder)
 
         output.append(dbOut)
-        
+
     return output
 
-def analyze_IRCore(options):
+def analyze_IRCore(options, show=True):
     """Main entry."""
     output = None
     if options.create_golden:
         golden, results = create_golden_average(options.files, options)
         if options.out is None:
             options.out = "out-golden.json"
 
@@ -406,29 +497,33 @@
 
         golden = [Petal_IR_Analysis.AnalysisResult() for i in range(2)]
         for i, Jside in enumerate(J):
             golden[i].from_json(Jside)
 
         output = analyze_petal_cores(options.files, golden, options)
 
-    plt.show()
+    if show:
+        plt.show()
+
     return output
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
     # Argument parser
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
     parser.add_argument("--create-golden", action="store_true", default=False, help="Draw golden average")
     parser.add_argument("--add_attachments", action="store_true", default=False,
                         help="If true add the attachments section os DB file.")
     parser.add_argument("--golden", default=None, help="The golden to compare width")
     parser.add_argument("--prefix", default="golden", help="Prefix for figures")
     parser.add_argument("--debug", action="store_true", default=False, help="Set to debug")
+    parser.add_argument("--report", action="store_true", default=False, help="Set to produce plots for report")
+
     parser.add_argument("--out", default=None, help="File to store Golden.")
     parser.add_argument("--folder", default=None, help="Folder to store output files. Superseeds folder in --out")
 
     options = parser.parse_args()
     if len(options.files) == 0:
         print("I need an input file")
         sys.exit()
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/contours.py` & `petal_qc-0.0.2/petal_qc/thermal/contours.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/coreThermal.py` & `petal_qc-0.0.2/petal_qc/thermal/coreThermal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,37 @@
 #!/usr/bin/env python3
 """GUI for thermal QC of petal cores."""
 import sys
 from pathlib import Path
 from argparse import ArgumentParser
 import json
-import numpy as np
-from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
-from matplotlib.backends.backend_gtk3 import NavigationToolbar2GTK3 as NavigationToolbar
 import itkdb_gtk
 import itkdb_gtk.ITkDButils
 import itkdb_gtk.dbGtkUtils
 import itkdb_gtk.UploadTest
+
+
+try:
+    import petal_qc
+
+except ImportError:
+    cwd = Path(__file__).parent.parent.parent
+    sys.path.append(cwd.as_posix())
+
+
 from petal_qc.thermal.IRPetalParam import IRPetalParam
 from petal_qc.thermal.create_IRCore import create_IR_core
-from petal_qc.thermal.analyze_IRCore import analyze_IRCore, golden_from_json, show_golden_average
+from petal_qc.thermal.analyze_IRCore import analyze_IRCore, golden_from_json, get_golden_axis, plot_profile_and_golden
 from petal_qc.utils.utils import output_folder
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GObject, Gio, GLib
 
-
-def create_canvas(fig, sx=400, sy=300):
-    """Creates a canvas."""
-    sw = Gtk.ScrolledWindow()  # Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-    sw.set_border_width(10)
-    sw.set_size_request(310, 310)
-    canvas = FigureCanvas(fig)  # a Gtk.DrawingArea
-    canvas.set_size_request(sx, sy)
-    sw.add(canvas)
-    return sw
-
-class ShowThermalResults(Gtk.Window):
-    """Show thermal results."""
-    def __init__(self, golden, results):
-        """Create the window."""
-        super().__init__(title="Thermal Results")
-
-        # Create main content box
-        self.mainBox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-        self.add(self.mainBox)
-
-        # The notebook
-        self.notebook = Gtk.Notebook()
-        self.notebook.set_tab_pos(Gtk.PositionType.LEFT)
-        self.mainBox.pack_start(self.notebook, True, True, 20)
-
-        # thermal path
-        box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-        box.set_border_width(5)
-        label = Gtk.Label(label="Path Temp,")
-        self.notebook.append_page(box, label)
-
-        figs = show_golden_average(golden, results, "path_temp")
-        sw = create_canvas(figs[0])
-        box.pack_start(sw, True, True, 0)
-
-        sw = create_canvas(figs[q])
-        box.pack_start(sw, True, True, 0)
-
-        box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-        box.set_border_width(5)
-        label = Gtk.Label(label="Sensor Avg,")
-        self.notebook.append_page(box, label)
-
-        figs = show_golden_average(golden, results, "sensor_avg")
-        sw = create_canvas(figs[0])
-        box.pack_start(sw, True, True, 0)
-
-        sw = create_canvas(figs[q])
-        box.pack_start(sw, True, True, 0)
-
-
-
-        # The button box
-        btnBox = Gtk.ButtonBox(orientation=Gtk.Orientation.HORIZONTAL)
-
-        btn = Gtk.Button(label="Quit")
-        btn.connect("clicked", self.quit)
-        btnBox.add(btn)
-
-        self.mainBox.pack_start(btnBox, False, True, 0)
-
-        self.show_all()
-
-    def quit(self, *args):
-        """Close window."""
-        self.hide()
-        self.destroy()
+from petal_qc.thermal.create_core_report import create_report
 
 class CoreThermal(itkdb_gtk.dbGtkUtils.ITkDBWindow):
     """Application window."""
 
     def __init__(self, params=None, session=None, title="",  panel_size=100):
         """Initialization
 
@@ -142,15 +82,15 @@
         self.goldenData.connect("file-set", self.on_golden_set)
 
         # The Serial number
         self.SN = itkdb_gtk.dbGtkUtils.TextEntry()
         self.SN.connect("text-changed", self.on_SN_changed)
 
         self.run = Gtk.Button(label="Run")
-        self.run.connect("clicked", self.run_analysis)
+        self.run.connect("clicked", self.create_report)
 
         self.btn_state = Gtk.Button(label="Undef")
         self.btn_state.set_name("btnState")
         self.btn_state.connect("clicked", self.show_state)
         self.btn_state.set_tooltip_text("If green all good. Click to see commnets and defects.")
 
         # Put the 3 objects in a Grid
@@ -334,35 +274,32 @@
 
     def upload_test(self):
         """Uploads test and attachments."""
         if self.outDB is None:
             return
         uploadW = itkdb_gtk.UploadTest.UploadTest(self.session, payload=self.outDB)
 
-    def run_analysis(self, *args):
-        """Run analysis."""
+    def create_report(self, *args):
+        """Creates the thermal report."""
         if self.irbfile is None:
             self.write_message("Missing IRB file\n")
             return
 
         self.write_message("Start analysis\n.")
         self.param.out = "{}.json".format(self.alternativeID)
         self.param.alias = self.alternativeID
         self.param.SN = self.SN.get_text()
 
-        core = create_IR_core(self.param)
-
-        self.param.files[0] = output_folder(self.param.folder, self.param.out)
-        self.param.out = None
-        out = analyze_IRCore(self.param)
-        self.outDB = out[0] if len(out) else None
-        self.param.files = []
-        self.write_message("Done\n")
+        self.param.tco2 = float(self.entryTemp.get_text())
+        self.param.distance = int(self.entryDist.get_text())
+        self.param.thrs = float(self.entryTHrs.get_text())
+        self.param.debug = False
+        self.param.report = True
 
-        outW = ShowThermalResults(self.golden, [core, ])
+        self.outDB = create_report(self.param)
         if self.outDB:
             if len(self.outDB["defects"]) > 0:
                 itkdb_gtk.dbGtkUtils.set_button_color(self.btn_state, "red", "white")
                 self.btn_state.set_label("FAILED")
             elif len(self.outDB["comments"]) > 0:
                 itkdb_gtk.dbGtkUtils.set_button_color(self.btn_state, "orange", "white")
                 self.btn_state.set_label("PROBLEMS")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/create_IRCore.py` & `petal_qc-0.0.2/petal_qc/thermal/create_IRCore.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import dateutil
 import matplotlib.pyplot as plt
 
+try:
+    import petal_qc
+
+except ImportError:
+    cwd = Path(__file__).parent.parent.parent
+    sys.path.append(cwd.as_posix())
+
 from petal_qc.thermal import IRBFile
 from petal_qc.thermal import IRCore
 from petal_qc.thermal import IRPetal
 from petal_qc.thermal import Petal_IR_Analysis
 from petal_qc.thermal import PipeFit
 from petal_qc.thermal.IRDataGetter import IRDataGetter
 from petal_qc.thermal.IRPetalParam import IRPetalParam
@@ -46,16 +53,32 @@
             out = date2string(this_date)
         except Exception:
             out = ""
 
     return out
 
 
+__figures__ = {}
+def get_IRcore_plots():
+    """Return global list of figures."""
+    return __figures__
+
+def clean_figures():
+    global __figures__
+    for key, fig in __figures__:
+        fig.clean()
+        plt.close(fig)
+
+    __figures__ = {}
+
 def create_IR_core(options):
     """Entry point."""
+    global __figures__
+    clean_figures()
+
     # Obtain the Data getter.
     try:
         getter = IRDataGetter.factory(options.institute, options)
 
     except NotImplemented:
         print("*** Invalid institute name. ***")
         return None
@@ -72,16 +95,17 @@
     # We will use the pipe obtained from here as the reference
     # for the next
     try:
         print("Get the reference image.")
         min_T, i_min, values = getter.find_reference_image(irbf, params.thrs, nframes=10)
         print("Image size: {} x {}".format(values[0].shape[0], values[0].shape[1]))
 
-        if options.debug:
-            Petal_IR_Analysis.show_2D_image(values)
+        if options.debug or options.report:
+            fig, ax = Petal_IR_Analysis.show_2D_image(values)
+            __figures__["original"] = fig
 
     except LookupError as e:
         print(e)
         sys.exit()
 
     # Get the pipes
     print("Get the pipes.")
@@ -95,16 +119,17 @@
     ordered_pipes = [None, None]
     pipe_order = [0, 0]
     for i in range(2):
         pipe_type = PipeFit.PipeFit.guess_pipe_type(pipes[i])
         pipe_order[i] = pipe_type
         PF = PipeFit.PipeFit(pipe_type)
         R = PF.fit_ex(pipes[i], factor=getter.factor)
-        if options.debug:
-            PF.plot()
+        if options.debug or options.report:
+            fig, _ =PF.plot()
+            __figures__["fit_{}".format(i)] = fig
 
         transforms[pipe_type] = R
         fitter[pipe_type] = PF
 
         # Reorder points in pipe contour so that first point corresponds to
         # the U-shape pipe minimum.
         pipes[i] = IRPetal.reorder_pipe_points(pipes[i], pipe_type, R)
@@ -124,15 +149,15 @@
     pipes = ordered_pipes
     deltaT = 0.0
     if options.tco2 != 0:
         deltaT = -35.0 - options.tco2
 
     # get the framea from where extract the data
     # reorder if needed
-    frames = getter.get_analysis_frame(irbf)
+    frames = getter.get_analysis_frame(irbf)        
     if pipe_order[0]:
         tmp = frames[0]
         frames[0] = frames[1]
         frames[1] = tmp
 
     values = getter.get_IR_data(frames, rotate=True)
     results = getter.analyze_IR_image(values, pipes, sensors, 0, params)
@@ -155,15 +180,15 @@
     # Check if we are given an output folder
     ofile = output_folder(options.folder, options.out)
     with open(ofile, "w", encoding="utf-8") as ofile:
         core.to_json(ofile)
 
     if options.debug:
         plt.show()
-        
+
     return core
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     # Argument parser
```

### Comparing `petal_qc-0.0.1/petal_qc/thermal/pipe_back.npz` & `petal_qc-0.0.2/petal_qc/thermal/pipe_back.npz`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/pipe_front.npz` & `petal_qc-0.0.2/petal_qc/thermal/pipe_front.npz`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/pipe_read.py` & `petal_qc-0.0.2/petal_qc/thermal/pipe_read.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/thermal/show_IR_petal.py` & `petal_qc-0.0.2/petal_qc/thermal/show_IR_petal.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 from argparse import ArgumentParser
 from pathlib import Path
 from pathlib import PurePath
 
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
+
+try:
+    import petal_qc
+
+except ImportError:
+    cwd = Path(__file__).parent.parent.parent
+    sys.path.append(cwd.as_posix())
+
 from petal_qc.thermal import contours
 from petal_qc.thermal import IRBFile
 from petal_qc.thermal import IRPetal
 from petal_qc.thermal import PipeFit
 from petal_qc.thermal.Petal_IR_Analysis import AnalysisResult
 from petal_qc.thermal.Petal_IR_Analysis import show_2D_image
 from petal_qc.thermal.PetalColorMaps import HighContrast
```

### Comparing `petal_qc-0.0.1/petal_qc/utils/Geometry.py` & `petal_qc-0.0.2/petal_qc/utils/Geometry.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/utils/Progress.py` & `petal_qc-0.0.2/petal_qc/utils/Progress.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/utils/all_files.py` & `petal_qc-0.0.2/petal_qc/utils/all_files.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/utils/docx_utils.py` & `petal_qc-0.0.2/petal_qc/utils/docx_utils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/utils/fit_utils.py` & `petal_qc-0.0.2/petal_qc/utils/fit_utils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc/utils/utils.py` & `petal_qc-0.0.2/petal_qc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `petal_qc-0.0.1/petal_qc.egg-info/PKG-INFO` & `petal_qc-0.0.2/petal_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petal_qc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of scripts for Petal CORE QC.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `petal_qc-0.0.1/petal_qc.egg-info/SOURCES.txt` & `petal_qc-0.0.2/petal_qc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,18 +41,22 @@
 petal_qc/thermal/Petal_IR_Analysis.py
 petal_qc/thermal/PipeFit.py
 petal_qc/thermal/__init__.py
 petal_qc/thermal/analyze_IRCore.py
 petal_qc/thermal/contours.py
 petal_qc/thermal/coreThermal.py
 petal_qc/thermal/create_IRCore.py
+petal_qc/thermal/create_core_report.py
 petal_qc/thermal/pipe_back.npz
 petal_qc/thermal/pipe_front.npz
 petal_qc/thermal/pipe_read.py
 petal_qc/thermal/show_IR_petal.py
+petal_qc/thermal/test_Graphana.py
+petal_qc/thermal/test_coreThermal.py
 petal_qc/utils/Geometry.py
 petal_qc/utils/Progress.py
 petal_qc/utils/__init__.py
 petal_qc/utils/all_files.py
 petal_qc/utils/docx_utils.py
 petal_qc/utils/fit_utils.py
+petal_qc/utils/readGraphana.py
 petal_qc/utils/utils.py
```

### Comparing `petal_qc-0.0.1/pyproject.toml` & `petal_qc-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "petal_qc"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of scripts for Petal CORE QC."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

