# Comparing `tmp/csmas-0.0.1.tar.gz` & `tmp/csmas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csmas-0.0.1.tar", last modified: Wed May 22 19:52:53 2024, max compression
+gzip compressed data, was "csmas-0.0.2.tar", last modified: Wed May 29 19:40:34 2024, max compression
```

## Comparing `csmas-0.0.1.tar` & `csmas-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:52:53.697641 csmas-0.0.1/
--rw-rw-rw-   0        0        0    11357 2024-05-22 19:33:15.000000 csmas-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      163 2024-05-22 19:52:53.697641 csmas-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-22 19:33:15.000000 csmas-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 19:52:53.682640 csmas-0.0.1/csmas/
--rw-rw-rw-   0        0        0     3900 2024-05-22 19:50:40.000000 csmas-0.0.1/csmas/Monitoring.py
--rw-rw-rw-   0        0        0       49 2024-05-22 19:39:25.000000 csmas-0.0.1/csmas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:52:53.696641 csmas-0.0.1/csmas.egg-info/
--rw-rw-rw-   0        0        0      163 2024-05-22 19:52:53.000000 csmas-0.0.1/csmas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-22 19:52:53.000000 csmas-0.0.1/csmas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:52:53.000000 csmas-0.0.1/csmas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-22 19:52:53.000000 csmas-0.0.1/csmas.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-22 19:52:53.000000 csmas-0.0.1/csmas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 19:52:53.697641 csmas-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      226 2024-05-22 19:39:25.000000 csmas-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:40:34.917734 csmas-0.0.2/
+-rw-rw-rw-   0        0        0    11357 2024-05-22 19:33:15.000000 csmas-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      226 2024-05-29 19:40:34.917734 csmas-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-22 19:33:15.000000 csmas-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 19:40:34.903733 csmas-0.0.2/csmas/
+-rw-rw-rw-   0        0        0     3900 2024-05-22 19:50:40.000000 csmas-0.0.2/csmas/Monitoring.py
+-rw-rw-rw-   0        0        0       49 2024-05-22 19:39:25.000000 csmas-0.0.2/csmas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:40:34.916731 csmas-0.0.2/csmas.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-29 19:40:34.000000 csmas-0.0.2/csmas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-29 19:40:34.000000 csmas-0.0.2/csmas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:40:34.000000 csmas-0.0.2/csmas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-29 19:40:34.000000 csmas-0.0.2/csmas.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 19:40:34.000000 csmas-0.0.2/csmas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:40:34.917734 csmas-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      328 2024-05-29 19:40:04.000000 csmas-0.0.2/setup.py
```

### Comparing `csmas-0.0.1/LICENSE` & `csmas-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csmas-0.0.1/csmas/Monitoring.py` & `csmas-0.0.2/csmas/Monitoring.py`

 * *Files identical despite different names*

