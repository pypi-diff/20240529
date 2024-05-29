# Comparing `tmp/checkfile-85.43.54.tar.gz` & `tmp/checkfile-85.43.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkfile-85.43.54.tar", last modified: Wed May 29 00:32:34 2024, max compression
+gzip compressed data, was "checkfile-85.43.55.tar", last modified: Wed May 29 00:40:28 2024, max compression
```

## Comparing `checkfile-85.43.54.tar` & `checkfile-85.43.55.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:32:34.081930 checkfile-85.43.54/
--rw-rw-rw-   0        0        0      211 2024-05-29 00:32:34.078713 checkfile-85.43.54/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 00:24:36.000000 checkfile-85.43.54/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 00:32:34.045698 checkfile-85.43.54/checkfile/
--rw-rw-rw-   0        0        0      608 2024-05-29 00:31:46.000000 checkfile-85.43.54/checkfile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:32:34.075176 checkfile-85.43.54/checkfile.egg-info/
--rw-rw-rw-   0        0        0      211 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 00:32:34.081930 checkfile-85.43.54/setup.cfg
--rw-rw-rw-   0        0        0      426 2024-05-29 00:32:30.000000 checkfile-85.43.54/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:40:28.166942 checkfile-85.43.55/
+-rw-rw-rw-   0        0        0      211 2024-05-29 00:40:28.164472 checkfile-85.43.55/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 00:24:36.000000 checkfile-85.43.55/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 00:40:28.139009 checkfile-85.43.55/checkfile/
+-rw-rw-rw-   0        0        0      772 2024-05-29 00:39:48.000000 checkfile-85.43.55/checkfile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:40:28.163472 checkfile-85.43.55/checkfile.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-05-29 00:40:27.000000 checkfile-85.43.55/checkfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-29 00:40:28.000000 checkfile-85.43.55/checkfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:40:27.000000 checkfile-85.43.55/checkfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 00:40:27.000000 checkfile-85.43.55/checkfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:40:28.166942 checkfile-85.43.55/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-05-29 00:40:24.000000 checkfile-85.43.55/setup.py
```

