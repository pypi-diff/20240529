# Comparing `tmp/swifttools-3.0.8.tar.gz` & `tmp/swifttools-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swifttools-3.0.8.tar", last modified: Fri Sep 23 19:48:55 2022, max compression
+gzip compressed data, was "swifttools-3.0.9.tar", last modified: Wed Nov 16 10:31:25 2022, max compression
```

## Comparing `swifttools-3.0.8.tar` & `swifttools-3.0.9.tar`

### file list

```diff
@@ -1,82 +1,65 @@
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.878807 swifttools-3.0.8/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       80 2021-10-26 20:00:45.000000 swifttools-3.0.8/.gitignore
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      270 2021-12-17 14:52:54.000000 swifttools-3.0.8/ChangeLog.md
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     1123 2021-10-26 20:00:45.000000 swifttools-3.0.8/LICENSE
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     1682 2022-09-23 19:48:55.878981 swifttools-3.0.8/PKG-INFO
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      802 2021-10-26 20:00:45.000000 swifttools-3.0.8/README.md
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.836738 swifttools-3.0.8/examples/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    14083 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Query existing job example.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    38617 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift GUANO Example Notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)   182530 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift Observation Query Example Notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)   101021 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift Plan Query Example Notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    21693 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift SAA Example Notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    38742 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift TOO Requests Example Notebook.ipynb
--rwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)    35270 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift TOO submission Example.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    38535 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift_Clock Example Notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    65453 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift_Data Example Notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    13384 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Swift_Resolve example notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    27994 2022-09-23 19:44:53.000000 swifttools-3.0.8/examples/Target Visibility Calculator Example.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    10365 2022-09-23 19:45:55.000000 swifttools-3.0.8/examples/UVOT_mode example notebook.ipynb
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      104 2022-04-07 19:24:07.000000 swifttools-3.0.8/pyproject.toml
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     1030 2022-09-23 19:48:55.879895 swifttools-3.0.8/setup.cfg
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       69 2022-04-07 19:24:05.000000 swifttools-3.0.8/setup.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.838104 swifttools-3.0.8/swifttools/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      489 2022-01-18 16:54:57.000000 swifttools-3.0.8/swifttools/__init__.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.855709 swifttools-3.0.8/swifttools/swift_too/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    10310 2022-09-23 16:58:26.000000 swifttools-3.0.8/swifttools/swift_too/ChangeLog.md
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     5401 2022-03-29 14:44:26.000000 swifttools-3.0.8/swifttools/swift_too/README.md
--rwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)     8139 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/__init__.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    25822 2022-09-23 16:44:58.000000 swifttools-3.0.8/swifttools/swift_too/api_common.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     3797 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/api_daterange.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     3698 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/api_resolve.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     2737 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/api_skycoord.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     3206 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/api_status.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     2995 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/query_job.py
--rwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)     4568 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_calendar.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    10066 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_clock.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    13679 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_data.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    11459 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_guano.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     3782 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_instruments.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     2686 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_obsid.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    15011 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_obsquery.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     8821 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_planquery.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     6150 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_requests.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     3885 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_saa.py
--rwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)    23787 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_toorequest.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     9397 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_uvot.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     6168 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/swift_visquery.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       46 2022-09-23 16:40:16.000000 swifttools-3.0.8/swifttools/swift_too/version.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.859218 swifttools-3.0.8/swifttools/ukssdc/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      458 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/__init__.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.863135 swifttools-3.0.8/swifttools/ukssdc/data/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    53460 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/data/GRB.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    83753 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/data/SXPS.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      690 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/data/__init__.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    40745 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/data/download.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    34442 2022-09-06 13:59:55.000000 swifttools-3.0.8/swifttools/ukssdc/main.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.870868 swifttools-3.0.8/swifttools/ukssdc/query/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     7733 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/DBFilter.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    31555 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/GRB.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    12671 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/Jamie_BackEnd.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    51251 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/SXPS.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      488 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/__init__.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    50506 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/dataquery_base.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)      873 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/query/obsData.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       44 2022-09-06 13:59:55.000000 swifttools-3.0.8/swifttools/ukssdc/version.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.877216 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     1915 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/__init__.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)    22472 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/prod_base.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     1502 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/prod_common.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)   120821 2022-09-23 15:04:12.000000 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/prod_request.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     9529 2022-09-02 15:54:47.000000 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/productVars.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       42 2022-09-23 15:04:12.000000 swifttools-3.0.8/swifttools/ukssdc/xrt_prods/version.py
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       22 2022-09-23 19:40:22.000000 swifttools-3.0.8/swifttools/version.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.878023 swifttools-3.0.8/swifttools/xrt_prods/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       33 2022-08-31 12:45:02.000000 swifttools-3.0.8/swifttools/xrt_prods/__init__.py
-drwxr-xr-x   0 jak51    (312409163) PSU\Domain Users (357253257)        0 2022-09-23 19:48:55.841943 swifttools-3.0.8/swifttools.egg-info/
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     1682 2022-09-23 19:48:55.000000 swifttools-3.0.8/swifttools.egg-info/PKG-INFO
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)     2465 2022-09-23 19:48:55.000000 swifttools-3.0.8/swifttools.egg-info/SOURCES.txt
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)        1 2022-09-23 19:48:55.000000 swifttools-3.0.8/swifttools.egg-info/dependency_links.txt
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)        1 2022-04-07 18:42:31.000000 swifttools-3.0.8/swifttools.egg-info/not-zip-safe
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       43 2022-09-23 19:48:55.000000 swifttools-3.0.8/swifttools.egg-info/requires.txt
--rw-r--r--   0 jak51    (312409163) PSU\Domain Users (357253257)       11 2022-09-23 19:48:55.000000 swifttools-3.0.8/swifttools.egg-info/top_level.txt
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.672465 swifttools-3.0.9/
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1123 2021-09-01 07:56:42.000000 swifttools-3.0.9/LICENSE
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1682 2022-11-16 10:31:25.672465 swifttools-3.0.9/PKG-INFO
+-rw-r--r--   0 pae9      (1009) xra       (1000)      802 2022-02-22 11:50:20.000000 swifttools-3.0.9/README.md
+-rw-r--r--   0 pae9      (1009) xra       (1000)      104 2022-08-31 08:34:28.000000 swifttools-3.0.9/pyproject.toml
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1030 2022-11-16 10:31:25.672465 swifttools-3.0.9/setup.cfg
+-rw-r--r--   0 pae9      (1009) xra       (1000)       69 2022-08-31 08:34:28.000000 swifttools-3.0.9/setup.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.660465 swifttools-3.0.9/swifttools/
+-rw-r--r--   0 pae9      (1009) xra       (1000)      489 2022-02-22 11:50:20.000000 swifttools-3.0.9/swifttools/__init__.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.664466 swifttools-3.0.9/swifttools/swift_too/
+-rwxr-xr-x   0 pae9      (1009) xra       (1000)     8139 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/__init__.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    25822 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/api_common.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     3797 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/api_daterange.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     3698 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/api_resolve.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     2737 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/api_skycoord.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     3206 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/api_status.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     2995 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/query_job.py
+-rwxr-xr-x   0 pae9      (1009) xra       (1000)     4568 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_calendar.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    10066 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_clock.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    13679 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_data.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    11459 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_guano.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     3782 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_instruments.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     2686 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_obsid.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    15011 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_obsquery.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     8821 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_planquery.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     6150 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_requests.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     3885 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_saa.py
+-rwxr-xr-x   0 pae9      (1009) xra       (1000)    23787 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_toorequest.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     9397 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_uvot.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     6168 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/swift_visquery.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)       46 2022-09-30 07:07:33.000000 swifttools-3.0.9/swifttools/swift_too/version.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.668465 swifttools-3.0.9/swifttools/ukssdc/
+-rw-r--r--   0 pae9      (1009) xra       (1000)      458 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/__init__.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.668465 swifttools-3.0.9/swifttools/ukssdc/data/
+-rw-r--r--   0 pae9      (1009) xra       (1000)    54091 2022-11-16 10:28:09.000000 swifttools-3.0.9/swifttools/ukssdc/data/GRB.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    83753 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/data/SXPS.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)      690 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/data/__init__.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    40847 2022-11-16 10:28:09.000000 swifttools-3.0.9/swifttools/ukssdc/data/download.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    34442 2022-09-06 13:48:16.000000 swifttools-3.0.9/swifttools/ukssdc/main.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.672465 swifttools-3.0.9/swifttools/ukssdc/query/
+-rw-r--r--   0 pae9      (1009) xra       (1000)     7733 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/DBFilter.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    31555 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/GRB.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    12671 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/Jamie_BackEnd.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    51251 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/SXPS.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)      488 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/__init__.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    50506 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/dataquery_base.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)      873 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/query/obsData.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)       44 2022-11-16 10:28:09.000000 swifttools-3.0.9/swifttools/ukssdc/version.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.672465 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1915 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/__init__.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)    22472 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/prod_base.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1502 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/prod_common.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)   120821 2022-09-23 07:22:15.000000 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/prod_request.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)     9529 2022-08-31 08:37:54.000000 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/productVars.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)       42 2022-09-23 07:23:17.000000 swifttools-3.0.9/swifttools/ukssdc/xrt_prods/version.py
+-rw-r--r--   0 pae9      (1009) xra       (1000)       22 2022-11-16 10:28:09.000000 swifttools-3.0.9/swifttools/version.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.672465 swifttools-3.0.9/swifttools/xrt_prods/
+-rw-r--r--   0 pae9      (1009) xra       (1000)       33 2022-08-31 08:37:57.000000 swifttools-3.0.9/swifttools/xrt_prods/__init__.py
+drwxr-xr-x   0 pae9      (1009) xra       (1000)        0 2022-11-16 10:31:25.660465 swifttools-3.0.9/swifttools.egg-info/
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1682 2022-11-16 10:31:25.000000 swifttools-3.0.9/swifttools.egg-info/PKG-INFO
+-rw-r--r--   0 pae9      (1009) xra       (1000)     1821 2022-11-16 10:31:25.000000 swifttools-3.0.9/swifttools.egg-info/SOURCES.txt
+-rw-r--r--   0 pae9      (1009) xra       (1000)        1 2022-11-16 10:31:25.000000 swifttools-3.0.9/swifttools.egg-info/dependency_links.txt
+-rw-r--r--   0 pae9      (1009) xra       (1000)        1 2022-11-16 10:31:25.000000 swifttools-3.0.9/swifttools.egg-info/not-zip-safe
+-rw-r--r--   0 pae9      (1009) xra       (1000)       43 2022-11-16 10:31:25.000000 swifttools-3.0.9/swifttools.egg-info/requires.txt
+-rw-r--r--   0 pae9      (1009) xra       (1000)       11 2022-11-16 10:31:25.000000 swifttools-3.0.9/swifttools.egg-info/top_level.txt
```

### Comparing `swifttools-3.0.8/LICENSE` & `swifttools-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/PKG-INFO` & `swifttools-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swifttools
-Version: 3.0.8
+Version: 3.0.9
 Summary: Tools for users of the Swift satellite
 Home-page: https://gitlab.com/DrPhilEvans/swifttools
 Author: Phil A. Evans
 Author-email: pae9@leicester.ac.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `swifttools-3.0.8/README.md` & `swifttools-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/setup.cfg` & `swifttools-3.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = swifttools
-version = 3.0.8
+version = 3.0.9
 description = Tools for users of the Swift satellite
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Phil A. Evans
 author_email = pae9@leicester.ac.uk
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `swifttools-3.0.8/swifttools/swift_too/__init__.py` & `swifttools-3.0.9/swifttools/swift_too/__init__.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/api_common.py` & `swifttools-3.0.9/swifttools/swift_too/api_common.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/api_daterange.py` & `swifttools-3.0.9/swifttools/swift_too/api_daterange.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/api_resolve.py` & `swifttools-3.0.9/swifttools/swift_too/api_resolve.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/api_skycoord.py` & `swifttools-3.0.9/swifttools/swift_too/api_skycoord.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/api_status.py` & `swifttools-3.0.9/swifttools/swift_too/api_status.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/query_job.py` & `swifttools-3.0.9/swifttools/swift_too/query_job.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_calendar.py` & `swifttools-3.0.9/swifttools/swift_too/swift_calendar.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_clock.py` & `swifttools-3.0.9/swifttools/swift_too/swift_clock.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_data.py` & `swifttools-3.0.9/swifttools/swift_too/swift_data.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_guano.py` & `swifttools-3.0.9/swifttools/swift_too/swift_guano.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_instruments.py` & `swifttools-3.0.9/swifttools/swift_too/swift_instruments.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_obsid.py` & `swifttools-3.0.9/swifttools/swift_too/swift_obsid.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_obsquery.py` & `swifttools-3.0.9/swifttools/swift_too/swift_obsquery.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_planquery.py` & `swifttools-3.0.9/swifttools/swift_too/swift_planquery.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_requests.py` & `swifttools-3.0.9/swifttools/swift_too/swift_requests.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_saa.py` & `swifttools-3.0.9/swifttools/swift_too/swift_saa.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_toorequest.py` & `swifttools-3.0.9/swifttools/swift_too/swift_toorequest.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_uvot.py` & `swifttools-3.0.9/swifttools/swift_too/swift_uvot.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/swift_too/swift_visquery.py` & `swifttools-3.0.9/swifttools/swift_too/swift_visquery.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/data/GRB.py` & `swifttools-3.0.9/swifttools/ukssdc/data/GRB.py`

 * *Files 1% similar despite different names*

```diff
@@ -991,14 +991,16 @@
 
 
 def getBurstAnalyser(
     targetID=None,
     GRBName=None,
     returnData=False,
     instruments="all",
+    BATBinning="all",
+    bands="all",
     nosys="no",
     incbad="yes",
     saveData=True,
     downloadTar=False,
     subDirs=True,
     destDir="BurstAn",
     clobber=False,
@@ -1063,14 +1065,24 @@
         Whether to return a dict containing all of the downloaded data
         (default: ``True``).
 
     instruments : str or list, optional
         Which instrument data to retrieve. Must be 'all' or a list of
         instruments (from: BAT, XRT, UVOT) (default: 'all').
 
+    BATBinning : str or list, optional
+        Which BAT binning methods' data to retrieve. Must be 'all' or a
+        case-insensitive list of binning methods (e.g. ['snr4',
+        'timedel0.064']); (default: 'all').
+
+    bands : str or list, optional
+        Which energy band data to retrieve. Must be 'all' or a list of
+        case-insensitive bands (from 'ObservedFlux', 'Density',
+        'BATBand', 'XRTBand'); (default: 'all').
+
     nosys : str
         Whether to return the light curves from which the WT
         systematic error has been removed. Can be 'yes', 'no',
         'both' -- the latter returning datasets with and without the
         systematic error. Only used if ``returnData=True`` or
         ``saveData=True`` (default: 'no').
 
@@ -1161,15 +1173,22 @@
             # And get the tar data:
             ok = dl._saveTar(tmp["URL"], tarPath, strip=True, clobber=clobber, silent=silent, verbose=verbose, **kwargs)
             if not (ok or skipErrors):
                 raise RuntimeError(f"Failed getting tar for {key}")
 
         if saveData or returnData:
 
-            sendData = {"targetID": t, "instruments": instruments, "incbad": incbad, "nosys": nosys}
+            sendData = {
+                "targetID": t,
+                "instruments": instruments,
+                "bands": bands,
+                "BATBinning": BATBinning,
+                "incbad": incbad,
+                "nosys": nosys,
+            }
             tmp = base.submitAPICall("downloadBurstAnalyser", sendData, verbose=verbose, minKeys=("Instruments",))
 
             # If we are getting multiple light curves, and no subdirs, then the file names will need prefixes.
             prefix = ""
             if (not subDirs) and (not single):
                 prefix = key
```

### Comparing `swifttools-3.0.8/swifttools/ukssdc/data/SXPS.py` & `swifttools-3.0.9/swifttools/ukssdc/data/SXPS.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/data/__init__.py` & `swifttools-3.0.9/swifttools/ukssdc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/data/download.py` & `swifttools-3.0.9/swifttools/ukssdc/data/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,17 +499,18 @@
         if "columns" not in data[tmpKey]:
             raise RuntimeError(f"`{key}` contains no column information.")
         cols = data[tmpKey]["columns"]
         skipKeys.append(tmpKey)
 
         if len(data[tmpKey]["data"]) > 0:
             if len(cols) != len(data[tmpKey]["data"][0]):
-                print(f"ARSE - {tmpKey}")
-                print(cols)
-                print(data[tmpKey]["data"])
+                # print(f"ARSE - {tmpKey}")
+                # print(cols)
+                # print(data[tmpKey]["data"])
+                raise RuntimeError(f"Unable to handle the {tmpKey} light curve, corrupt data?")
 
         if "UL" in key and not oldCols:
             cols = ["UpperLimit" if x == "Rate" else x for x in cols]
 
         tmpDF = pd.DataFrame(data[tmpKey]["data"], columns=cols, dtype=str)
 
         types = {}
```

### Comparing `swifttools-3.0.8/swifttools/ukssdc/main.py` & `swifttools-3.0.9/swifttools/ukssdc/main.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/query/DBFilter.py` & `swifttools-3.0.9/swifttools/ukssdc/query/DBFilter.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/query/GRB.py` & `swifttools-3.0.9/swifttools/ukssdc/query/GRB.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/query/Jamie_BackEnd.py` & `swifttools-3.0.9/swifttools/ukssdc/query/Jamie_BackEnd.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/query/SXPS.py` & `swifttools-3.0.9/swifttools/ukssdc/query/SXPS.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/query/dataquery_base.py` & `swifttools-3.0.9/swifttools/ukssdc/query/dataquery_base.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/query/obsData.py` & `swifttools-3.0.9/swifttools/ukssdc/query/obsData.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/xrt_prods/__init__.py` & `swifttools-3.0.9/swifttools/ukssdc/xrt_prods/__init__.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/xrt_prods/prod_base.py` & `swifttools-3.0.9/swifttools/ukssdc/xrt_prods/prod_base.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/xrt_prods/prod_common.py` & `swifttools-3.0.9/swifttools/ukssdc/xrt_prods/prod_common.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/xrt_prods/prod_request.py` & `swifttools-3.0.9/swifttools/ukssdc/xrt_prods/prod_request.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools/ukssdc/xrt_prods/productVars.py` & `swifttools-3.0.9/swifttools/ukssdc/xrt_prods/productVars.py`

 * *Files identical despite different names*

### Comparing `swifttools-3.0.8/swifttools.egg-info/PKG-INFO` & `swifttools-3.0.9/swifttools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swifttools
-Version: 3.0.8
+Version: 3.0.9
 Summary: Tools for users of the Swift satellite
 Home-page: https://gitlab.com/DrPhilEvans/swifttools
 Author: Phil A. Evans
 Author-email: pae9@leicester.ac.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

