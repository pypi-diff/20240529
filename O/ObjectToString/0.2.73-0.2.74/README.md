# Comparing `tmp/ObjectToString-0.2.73.tar.gz` & `tmp/ObjectToString-0.2.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ObjectToString-0.2.73.tar", last modified: Mon May 27 14:16:25 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "ObjectToString-0.2.74.tar", last modified: Wed May 29 16:28:08 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `ObjectToString-0.2.73.tar` & `ObjectToString-0.2.74.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.73/
--rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.73/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.73/objecttostring/
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.73/ObjectToString.egg-info/
--rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.73/ObjectToString.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.73/ObjectToString.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.73/ObjectToString.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.73/ObjectToString.egg-info/top_level.txt
--rwxrwxrwx   0        0        0  3710464 2018-09-24 03:30:50.000000 ObjectToString-0.2.73/objecttostring/pdslib.cp312-win_amd64.pyd
--rwxrwxrwx   0        0        0    90112 2024-05-26 12:41:03.000000 ObjectToString-0.2.73/objecttostring/python.exe
--rwxrwxrwx   0        0        0    56832 2024-05-26 12:40:06.000000 ObjectToString-0.2.73/objecttostring/python3.dll
--rwxrwxrwx   0        0        0  8847872 2024-05-26 12:40:45.000000 ObjectToString-0.2.73/objecttostring/python312.dll
--rwxrwxrwx   0        0        0      100 2024-05-27 14:16:20.000000 ObjectToString-0.2.73/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.73/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.73/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.74/
+-rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.74/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.74/objecttostring/
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.74/ObjectToString.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.74/ObjectToString.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.74/ObjectToString.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.74/ObjectToString.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.74/ObjectToString.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0  3709952 2019-12-21 14:00:00.000000 ObjectToString-0.2.74/objecttostring/pdslib.cp312-win_amd64.pyd
+-rwxrwxrwx   0        0        0      100 2024-05-29 16:27:56.000000 ObjectToString-0.2.74/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.74/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.74/setup.py
```

