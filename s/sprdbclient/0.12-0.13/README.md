# Comparing `tmp/sprdbclient-0.12.tar.gz` & `tmp/sprdbclient-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprdbclient-0.12.tar", last modified: Mon May 27 12:04:36 2024, max compression
+gzip compressed data, was "sprdbclient-0.13.tar", last modified: Wed May 29 11:03:02 2024, max compression
```

## Comparing `sprdbclient-0.12.tar` & `sprdbclient-0.13.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 12:04:36.276740 sprdbclient-0.12/
--rw-rw-rw-   0        0        0    35821 2024-05-24 05:35:49.000000 sprdbclient-0.12/LICENSE
--rw-rw-rw-   0        0        0      196 2024-05-27 12:04:36.275740 sprdbclient-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-27 12:04:36.276740 sprdbclient-0.12/setup.cfg
--rw-rw-rw-   0        0        0      252 2024-05-27 12:04:34.000000 sprdbclient-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:04:36.274742 sprdbclient-0.12/sprdbclient.egg-info/
--rw-rw-rw-   0        0        0      196 2024-05-27 12:04:36.000000 sprdbclient-0.12/sprdbclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2024-05-27 12:04:36.000000 sprdbclient-0.12/sprdbclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:04:36.000000 sprdbclient-0.12/sprdbclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:04:36.000000 sprdbclient-0.12/sprdbclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 11:03:02.510471 sprdbclient-0.13/
+-rw-rw-rw-   0        0        0    35821 2024-05-24 05:35:49.000000 sprdbclient-0.13/LICENSE
+-rw-rw-rw-   0        0        0      226 2024-05-29 11:03:02.509472 sprdbclient-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:03:02.510471 sprdbclient-0.13/setup.cfg
+-rw-rw-rw-   0        0        0      308 2024-05-29 10:58:07.000000 sprdbclient-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:03:02.500471 sprdbclient-0.13/sprdbclient/
+-rw-rw-rw-   0        0        0      140 2024-05-27 11:09:30.000000 sprdbclient-0.13/sprdbclient/__init__.py
+-rw-rw-rw-   0        0        0      993 2024-05-28 13:06:27.000000 sprdbclient-0.13/sprdbclient/client.py
+-rw-rw-rw-   0        0        0      145 2024-05-24 05:40:02.000000 sprdbclient-0.13/sprdbclient/config.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:03:02.508471 sprdbclient-0.13/sprdbclient.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-29 11:03:02.000000 sprdbclient-0.13/sprdbclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-05-29 11:03:02.000000 sprdbclient-0.13/sprdbclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:03:02.000000 sprdbclient-0.13/sprdbclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 11:03:02.000000 sprdbclient-0.13/sprdbclient.egg-info/top_level.txt
```

### Comparing `sprdbclient-0.12/LICENSE` & `sprdbclient-0.13/LICENSE`

 * *Files identical despite different names*

