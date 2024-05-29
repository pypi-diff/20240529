# Comparing `tmp/datacontract-0.0.1.tar.gz` & `tmp/datacontract-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\datacontract-0.0.1.tar", last modified: Wed Aug  9 11:58:14 2017, max compression
+gzip compressed data, was "datacontract-0.1.0.tar", last modified: Wed May 29 10:27:12 2024, max compression
```

## Comparing `datacontract-0.0.1.tar` & `datacontract-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2017-08-09 11:58:14.000000 datacontract-0.0.1/
-drwxrwxrwx   0        0        0        0 2017-08-09 11:58:14.000000 datacontract-0.0.1/datacontract/
--rw-rw-rw-   0        0        0        0 2017-08-09 11:52:31.000000 datacontract-0.0.1/datacontract/__init__.py
-drwxrwxrwx   0        0        0        0 2017-08-09 11:58:14.000000 datacontract-0.0.1/datacontract.egg-info/
--rw-rw-rw-   0        0        0        1 2017-08-09 11:58:13.000000 datacontract-0.0.1/datacontract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2017-08-09 11:58:13.000000 datacontract-0.0.1/datacontract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2017-08-09 11:58:14.000000 datacontract-0.0.1/datacontract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2017-08-09 11:58:13.000000 datacontract-0.0.1/datacontract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      197 2017-08-09 11:58:14.000000 datacontract-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2017-08-09 11:58:14.000000 datacontract-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      280 2017-08-09 11:52:41.000000 datacontract-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 10:27:12.265851 datacontract-0.1.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      247 2024-05-29 10:27:12.265851 datacontract-0.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      341 2024-05-29 10:26:42.000000 datacontract-0.1.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-29 10:27:12.265851 datacontract-0.1.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 10:27:12.265851 datacontract-0.1.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 10:27:12.265851 datacontract-0.1.0/src/datacontract.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      247 2024-05-29 10:27:12.000000 datacontract-0.1.0/src/datacontract.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2024-05-29 10:27:12.000000 datacontract-0.1.0/src/datacontract.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-29 10:27:12.000000 datacontract-0.1.0/src/datacontract.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-05-29 10:27:12.000000 datacontract-0.1.0/src/datacontract.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      543 2024-05-29 10:23:56.000000 datacontract-0.1.0/src/datacontract.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

