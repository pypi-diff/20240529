# Comparing `tmp/whut-0.1.0.tar.gz` & `tmp/whut-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whut-0.1.0.tar", last modified: Wed May 29 19:42:00 2024, max compression
+gzip compressed data, was "whut-0.2.0.tar", last modified: Wed May 29 19:57:18 2024, max compression
```

## Comparing `whut-0.1.0.tar` & `whut-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2024-05-29 19:42:00.136326 whut-0.1.0/
--rw-rw-r--   0 pk        (1000) pk        (1000)        0 2024-05-29 13:50:34.000000 whut-0.1.0/LICENSE
--rw-rw-r--   0 pk        (1000) pk        (1000)      615 2024-05-29 19:42:00.136326 whut-0.1.0/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)       95 2024-05-29 19:13:20.000000 whut-0.1.0/README.md
--rw-rw-r--   0 pk        (1000) pk        (1000)       38 2024-05-29 19:42:00.136326 whut-0.1.0/setup.cfg
--rw-rw-r--   0 pk        (1000) pk        (1000)      994 2024-05-29 19:24:40.000000 whut-0.1.0/setup.py
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2024-05-29 19:42:00.132326 whut-0.1.0/whut/
--rw-rw-r--   0 pk        (1000) pk        (1000)        0 2024-05-29 13:49:40.000000 whut-0.1.0/whut/__init__.py
--rw-rw-r--   0 pk        (1000) pk        (1000)      879 2024-05-29 19:09:07.000000 whut-0.1.0/whut/cli.py
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2024-05-29 19:42:00.136326 whut-0.1.0/whut.egg-info/
--rw-rw-r--   0 pk        (1000) pk        (1000)      615 2024-05-29 19:41:59.000000 whut-0.1.0/whut.egg-info/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)      225 2024-05-29 19:42:00.000000 whut-0.1.0/whut.egg-info/SOURCES.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        1 2024-05-29 19:41:59.000000 whut-0.1.0/whut.egg-info/dependency_links.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       40 2024-05-29 19:41:59.000000 whut-0.1.0/whut.egg-info/entry_points.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       20 2024-05-29 19:41:59.000000 whut-0.1.0/whut.egg-info/requires.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        5 2024-05-29 19:41:59.000000 whut-0.1.0/whut.egg-info/top_level.txt
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2024-05-29 19:57:18.235793 whut-0.2.0/
+-rw-rw-r--   0 pk        (1000) pk        (1000)     1127 2024-05-29 19:49:57.000000 whut-0.2.0/LICENSE
+-rw-rw-r--   0 pk        (1000) pk        (1000)     1297 2024-05-29 19:57:18.235793 whut-0.2.0/PKG-INFO
+-rw-rw-r--   0 pk        (1000) pk        (1000)      777 2024-05-29 19:54:51.000000 whut-0.2.0/README.md
+-rw-rw-r--   0 pk        (1000) pk        (1000)       38 2024-05-29 19:57:18.235793 whut-0.2.0/setup.cfg
+-rw-rw-r--   0 pk        (1000) pk        (1000)      994 2024-05-29 19:56:18.000000 whut-0.2.0/setup.py
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2024-05-29 19:57:18.231794 whut-0.2.0/whut/
+-rw-rw-r--   0 pk        (1000) pk        (1000)        0 2024-05-29 13:49:40.000000 whut-0.2.0/whut/__init__.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)      879 2024-05-29 19:09:07.000000 whut-0.2.0/whut/cli.py
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2024-05-29 19:57:18.235793 whut-0.2.0/whut.egg-info/
+-rw-rw-r--   0 pk        (1000) pk        (1000)     1297 2024-05-29 19:57:18.000000 whut-0.2.0/whut.egg-info/PKG-INFO
+-rw-rw-r--   0 pk        (1000) pk        (1000)      225 2024-05-29 19:57:18.000000 whut-0.2.0/whut.egg-info/SOURCES.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)        1 2024-05-29 19:57:18.000000 whut-0.2.0/whut.egg-info/dependency_links.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)       40 2024-05-29 19:57:18.000000 whut-0.2.0/whut.egg-info/entry_points.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)       20 2024-05-29 19:57:18.000000 whut-0.2.0/whut.egg-info/requires.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)        5 2024-05-29 19:57:18.000000 whut-0.2.0/whut.egg-info/top_level.txt
```

### Comparing `whut-0.1.0/setup.py` & `whut-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Function to read the requirements.txt file
 def read_requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 setup(
     name='whut',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'whut=whut.cli:main',
         ],
     },
     install_requires=[
```

### Comparing `whut-0.1.0/whut/cli.py` & `whut-0.2.0/whut/cli.py`

 * *Files identical despite different names*

