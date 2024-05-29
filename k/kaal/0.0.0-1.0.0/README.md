# Comparing `tmp/kaal-0.0.0.tar.gz` & `tmp/kaal-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaal-0.0.0.tar", last modified: Wed May 29 11:46:59 2024, max compression
+gzip compressed data, was "kaal-1.0.0.tar", last modified: Wed May 29 17:01:52 2024, max compression
```

## Comparing `kaal-0.0.0.tar` & `kaal-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:46:59.944820 kaal-0.0.0/
--rw-rw-rw-   0        0        0      150 2024-05-29 11:46:59.942820 kaal-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       48 2024-05-29 11:26:04.000000 kaal-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:46:59.914701 kaal-0.0.0/kaal/
--rw-rw-rw-   0        0        0       25 2024-05-29 11:36:45.000000 kaal-0.0.0/kaal/__init__.py
--rw-rw-rw-   0        0        0       38 2024-05-29 11:36:16.000000 kaal-0.0.0/kaal/hello.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:46:59.941815 kaal-0.0.0/kaal.egg-info/
--rw-rw-rw-   0        0        0      150 2024-05-29 11:46:59.000000 kaal-0.0.0/kaal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-29 11:46:59.000000 kaal-0.0.0/kaal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:46:59.000000 kaal-0.0.0/kaal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-29 11:46:59.000000 kaal-0.0.0/kaal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-05-29 11:46:56.000000 kaal-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 11:46:59.944820 kaal-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      708 2024-05-29 11:42:13.000000 kaal-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:01:52.082186 kaal-1.0.0/
+-rw-rw-rw-   0        0        0      150 2024-05-29 17:01:52.081185 kaal-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2024-05-29 11:26:04.000000 kaal-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 17:01:52.073328 kaal-1.0.0/kaal/
+-rw-rw-rw-   0        0        0       21 2024-05-29 16:58:12.000000 kaal-1.0.0/kaal/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 13:36:46.000000 kaal-1.0.0/kaal/hello.py
+-rw-rw-rw-   0        0        0       50 2024-05-29 13:53:29.000000 kaal-1.0.0/kaal/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:01:52.079332 kaal-1.0.0/kaal/utils/
+-rw-rw-rw-   0        0        0       27 2024-05-29 16:57:58.000000 kaal-1.0.0/kaal/utils/__init__.py
+-rw-rw-rw-   0        0        0      640 2024-05-29 16:55:27.000000 kaal-1.0.0/kaal/utils/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:01:52.080168 kaal-1.0.0/kaal.egg-info/
+-rw-rw-rw-   0        0        0      150 2024-05-29 17:01:51.000000 kaal-1.0.0/kaal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-29 17:01:52.000000 kaal-1.0.0/kaal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:01:51.000000 kaal-1.0.0/kaal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 17:01:51.000000 kaal-1.0.0/kaal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-05-29 17:01:02.000000 kaal-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:01:52.082932 kaal-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-29 17:01:07.000000 kaal-1.0.0/setup.py
```

### Comparing `kaal-0.0.0/setup.py` & `kaal-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.0'
+VERSION = '1.0.0'
 DESCRIPTION = 'Time series utility package'
 
 # Setting up
 setup(
     name="kaal",
     version=VERSION,
     author="Debangan Mishra",
```

