# Comparing `tmp/bdup-0.0.1.tar.gz` & `tmp/bdup-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdup-0.0.1.tar", last modified: Tue May 14 08:18:20 2024, max compression
+gzip compressed data, was "bdup-0.0.2.tar", last modified: Wed May 29 05:50:44 2024, max compression
```

## Comparing `bdup-0.0.1.tar` & `bdup-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:18:20.696087 bdup-0.0.1/
--rw-rw-rw-   0        0        0      139 2024-05-14 08:18:20.695090 bdup-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        5 2024-05-09 08:09:24.000000 bdup-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 08:18:20.689105 bdup-0.0.1/bdup/
--rw-rw-rw-   0        0        0       23 2024-05-14 08:15:49.000000 bdup-0.0.1/bdup/__init__.py
--rw-rw-rw-   0        0        0     4097 2024-05-14 08:15:49.000000 bdup-0.0.1/bdup/bdup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:18:20.695090 bdup-0.0.1/bdup.egg-info/
--rw-rw-rw-   0        0        0      139 2024-05-14 08:18:20.000000 bdup-0.0.1/bdup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-05-14 08:18:20.000000 bdup-0.0.1/bdup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:18:20.000000 bdup-0.0.1/bdup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 08:18:20.000000 bdup-0.0.1/bdup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 bdup-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 08:18:20.696087 bdup-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      255 2024-05-14 08:17:39.000000 bdup-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:50:44.983200 bdup-0.0.2/
+-rw-rw-rw-   0        0        0      139 2024-05-29 05:50:44.983200 bdup-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2024-05-09 08:09:24.000000 bdup-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 05:50:44.974224 bdup-0.0.2/bdup/
+-rw-rw-rw-   0        0        0       23 2024-05-14 08:15:49.000000 bdup-0.0.2/bdup/__init__.py
+-rw-rw-rw-   0        0        0     4452 2024-05-29 05:48:17.000000 bdup-0.0.2/bdup/bdup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:50:44.982202 bdup-0.0.2/bdup.egg-info/
+-rw-rw-rw-   0        0        0      139 2024-05-29 05:50:44.000000 bdup-0.0.2/bdup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-05-29 05:50:44.000000 bdup-0.0.2/bdup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 05:50:44.000000 bdup-0.0.2/bdup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 05:50:44.000000 bdup-0.0.2/bdup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 bdup-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 05:50:44.983200 bdup-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      255 2024-05-29 05:49:33.000000 bdup-0.0.2/setup.py
```

