# Comparing `tmp/colorspace-0.0.1.tar.gz` & `tmp/colorspace-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colorspace-0.0.1.tar", last modified: Thu Dec 21 17:04:10 2017, max compression
+gzip compressed data, was "colorspace-0.4.2.tar", last modified: Wed May 29 17:39:09 2024, max compression
```

## Comparing `colorspace-0.0.1.tar` & `colorspace-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,27 @@
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2017-12-21 17:04:10.000000 colorspace-0.0.1/
--rw-r--r--   0 noah      (1000) noah      (1000)      303 2017-12-21 17:02:45.000000 colorspace-0.0.1/setup.py
--rw-r--r--   0 noah      (1000) noah      (1000)      287 2017-12-21 17:04:10.000000 colorspace-0.0.1/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)       50 2017-12-13 12:05:14.000000 colorspace-0.0.1/README.md
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2017-12-21 17:04:10.000000 colorspace-0.0.1/colorspace.egg-info/
--rw-r--r--   0 noah      (1000) noah      (1000)      154 2017-12-21 17:04:10.000000 colorspace-0.0.1/colorspace.egg-info/SOURCES.txt
--rw-r--r--   0 noah      (1000) noah      (1000)        1 2017-12-21 17:04:10.000000 colorspace-0.0.1/colorspace.egg-info/dependency_links.txt
--rw-r--r--   0 noah      (1000) noah      (1000)      287 2017-12-21 17:04:10.000000 colorspace-0.0.1/colorspace.egg-info/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)        1 2017-12-21 17:04:10.000000 colorspace-0.0.1/colorspace.egg-info/top_level.txt
--rw-r--r--   0 noah      (1000) noah      (1000)       38 2017-12-21 17:04:10.000000 colorspace-0.0.1/setup.cfg
+drwxrwxr-x   0 retos     (1000) retos     (1000)        0 2024-05-29 17:39:09.444869 colorspace-0.4.2/
+-rw-rw-r--   0 retos     (1000) retos     (1000)    18432 2024-05-03 02:23:19.000000 colorspace-0.4.2/LICENSE
+-rw-rw-r--   0 retos     (1000) retos     (1000)      651 2023-08-23 19:05:10.000000 colorspace-0.4.2/MANIFEST.in
+-rw-rw-r--   0 retos     (1000) retos     (1000)     2730 2024-05-29 17:39:09.444869 colorspace-0.4.2/PKG-INFO
+-rw-rw-r--   0 retos     (1000) retos     (1000)     1932 2023-08-23 19:05:10.000000 colorspace-0.4.2/README.md
+-rw-rw-r--   0 retos     (1000) retos     (1000)       79 2024-05-29 17:39:09.444869 colorspace-0.4.2/setup.cfg
+-rw-rw-r--   0 retos     (1000) retos     (1000)     2504 2024-05-29 09:48:30.000000 colorspace-0.4.2/setup.py
+drwxrwxr-x   0 retos     (1000) retos     (1000)        0 2024-05-29 17:39:09.440873 colorspace-0.4.2/src/
+drwxrwxr-x   0 retos     (1000) retos     (1000)        0 2024-05-29 17:39:09.444869 colorspace-0.4.2/src/colorspace/
+-rw-rw-r--   0 retos     (1000) retos     (1000)    29796 2024-05-03 01:35:56.000000 colorspace-0.4.2/src/colorspace/CVD.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)     1763 2024-04-26 17:59:41.000000 colorspace-0.4.2/src/colorspace/__init__.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)    41319 2024-05-02 23:42:24.000000 colorspace-0.4.2/src/colorspace/choose_palette.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)   122412 2024-05-03 05:26:05.000000 colorspace-0.4.2/src/colorspace/colorlib.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)     6451 2024-05-03 01:53:45.000000 colorspace-0.4.2/src/colorspace/cvd_emulator.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)    24610 2024-05-03 01:25:09.000000 colorspace-0.4.2/src/colorspace/demos.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)     8673 2024-05-03 05:28:27.000000 colorspace-0.4.2/src/colorspace/hcl_palettes.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)    99016 2024-05-10 16:42:01.000000 colorspace-0.4.2/src/colorspace/palettes.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)    10624 2024-05-02 23:45:20.000000 colorspace-0.4.2/src/colorspace/specplot.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)    22679 2024-05-02 21:23:20.000000 colorspace-0.4.2/src/colorspace/swatchplot.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)    37803 2024-05-29 06:45:19.000000 colorspace-0.4.2/src/colorspace/utils.py
+-rw-rw-r--   0 retos     (1000) retos     (1000)       61 2024-05-29 17:39:09.000000 colorspace-0.4.2/src/colorspace/version.py
+drwxrwxr-x   0 retos     (1000) retos     (1000)        0 2024-05-29 17:39:09.444869 colorspace-0.4.2/src/colorspace.egg-info/
+-rw-rw-r--   0 retos     (1000) retos     (1000)     2730 2024-05-29 17:39:09.000000 colorspace-0.4.2/src/colorspace.egg-info/PKG-INFO
+-rw-rw-r--   0 retos     (1000) retos     (1000)      565 2024-05-29 17:39:09.000000 colorspace-0.4.2/src/colorspace.egg-info/SOURCES.txt
+-rw-rw-r--   0 retos     (1000) retos     (1000)        1 2024-05-29 17:39:09.000000 colorspace-0.4.2/src/colorspace.egg-info/dependency_links.txt
+-rw-rw-r--   0 retos     (1000) retos     (1000)        6 2024-05-29 17:39:09.000000 colorspace-0.4.2/src/colorspace.egg-info/requires.txt
+-rw-rw-r--   0 retos     (1000) retos     (1000)       11 2024-05-29 17:39:09.000000 colorspace-0.4.2/src/colorspace.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

