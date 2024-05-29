# Comparing `tmp/cerebrumscanner-0.0.1b5.tar.gz` & `tmp/cerebrumscanner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.1b5.tar", last modified: Tue May 28 06:25:36 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.2.tar", last modified: Wed May 29 12:30:54 2024, max compression
```

## Comparing `cerebrumscanner-0.0.1b5.tar` & `cerebrumscanner-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       63 2024-05-27 08:15:33.000000 cerebrumscanner-0.0.1b5/LICENSE
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       24 2024-05-27 09:23:20.000000 cerebrumscanner-0.0.1b5/MANIFEST.in
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-27 08:02:00.000000 cerebrumscanner-0.0.1b5/README.md
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      300 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        7 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/requires.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/top_level.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        6 2024-05-27 09:20:05.000000 cerebrumscanner-0.0.1b5/requirements.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/setup.cfg
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      941 2024-05-28 06:24:28.000000 cerebrumscanner-0.0.1b5/setup.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/test/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       59 2024-05-27 08:09:56.000000 cerebrumscanner-0.0.1b5/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.259007 cerebrumscanner-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    45364 2024-05-29 12:30:54.257999 cerebrumscanner-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.2/README.md
+-rw-rw-rw-   0        0        0      230 2024-05-28 10:23:21.000000 cerebrumscanner-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:30:54.260006 cerebrumscanner-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-29 12:30:00.000000 cerebrumscanner-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.221342 cerebrumscanner-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.233417 cerebrumscanner-0.0.2/src/cerebrumscanner/
+-rw-rw-rw-   0        0        0       84 2024-05-28 12:15:56.000000 cerebrumscanner-0.0.2/src/cerebrumscanner/__init__.py
+-rw-rw-rw-   0        0        0     5850 2024-05-28 12:05:08.000000 cerebrumscanner-0.0.2/src/cerebrumscanner/database_manager.py
+-rw-rw-rw-   0        0        0     1379 2024-05-28 12:11:53.000000 cerebrumscanner-0.0.2/src/cerebrumscanner/image_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:30:54.255495 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/
+-rw-rw-rw-   0        0        0    45364 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 12:29:07.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      192 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 12:30:54.000000 cerebrumscanner-0.0.2/src/cerebrumscanner.egg-info/top_level.txt
```

