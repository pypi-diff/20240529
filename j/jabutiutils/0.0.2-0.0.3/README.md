# Comparing `tmp/jabutiutils-0.0.2.tar.gz` & `tmp/jabutiutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jabutiutils-0.0.2.tar", last modified: Wed May 29 20:54:20 2024, max compression
+gzip compressed data, was "jabutiutils-0.0.3.tar", last modified: Wed May 29 21:00:37 2024, max compression
```

## Comparing `jabutiutils-0.0.2.tar` & `jabutiutils-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 20:54:20.851121 jabutiutils-0.0.2/
--rw-rw-rw-   0        0        0     1072 2024-05-29 20:23:25.000000 jabutiutils-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      196 2024-05-29 20:54:20.848358 jabutiutils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 20:14:42.000000 jabutiutils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 20:54:20.845595 jabutiutils-0.0.2/jabutiutils.egg-info/
--rw-rw-rw-   0        0        0      196 2024-05-29 20:54:20.000000 jabutiutils-0.0.2/jabutiutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-05-29 20:54:20.000000 jabutiutils-0.0.2/jabutiutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 20:54:20.000000 jabutiutils-0.0.2/jabutiutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 20:54:20.000000 jabutiutils-0.0.2/jabutiutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 20:54:20.000000 jabutiutils-0.0.2/jabutiutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 20:54:20.851630 jabutiutils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      237 2024-05-29 20:54:14.000000 jabutiutils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:00:37.570342 jabutiutils-0.0.3/
+-rw-rw-rw-   0        0        0     1072 2024-05-29 20:23:25.000000 jabutiutils-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      196 2024-05-29 21:00:37.567411 jabutiutils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 20:14:42.000000 jabutiutils-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 21:00:37.549341 jabutiutils-0.0.3/jabutiutils/
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:24:06.000000 jabutiutils-0.0.3/jabutiutils/JbtUtils.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:40:15.000000 jabutiutils-0.0.3/jabutiutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:00:37.564189 jabutiutils-0.0.3/jabutiutils/ms_identity_web/
+-rw-rw-rw-   0        0        0    15688 2024-05-29 20:30:56.000000 jabutiutils-0.0.3/jabutiutils/ms_identity_web/__init__.py
+-rw-rw-rw-   0        0        0     9507 2024-05-29 20:30:10.000000 jabutiutils-0.0.3/jabutiutils/ms_identity_web/adapters.py
+-rw-rw-rw-   0        0        0     3642 2024-05-29 20:27:25.000000 jabutiutils-0.0.3/jabutiutils/ms_identity_web/configuration.py
+-rw-rw-rw-   0        0        0     3173 2024-05-29 20:27:48.000000 jabutiutils-0.0.3/jabutiutils/ms_identity_web/constants.py
+-rw-rw-rw-   0        0        0     2779 2024-05-29 20:29:54.000000 jabutiutils-0.0.3/jabutiutils/ms_identity_web/context.py
+-rw-rw-rw-   0        0        0     1277 2024-05-29 20:30:31.000000 jabutiutils-0.0.3/jabutiutils/ms_identity_web/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:00:37.566372 jabutiutils-0.0.3/jabutiutils.egg-info/
+-rw-rw-rw-   0        0        0      196 2024-05-29 21:00:37.000000 jabutiutils-0.0.3/jabutiutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-05-29 21:00:37.000000 jabutiutils-0.0.3/jabutiutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 21:00:37.000000 jabutiutils-0.0.3/jabutiutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 21:00:37.000000 jabutiutils-0.0.3/jabutiutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 21:00:37.000000 jabutiutils-0.0.3/jabutiutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 21:00:37.570850 jabutiutils-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      237 2024-05-29 21:00:35.000000 jabutiutils-0.0.3/setup.py
```

### Comparing `jabutiutils-0.0.2/LICENSE` & `jabutiutils-0.0.3/LICENSE`

 * *Files identical despite different names*

