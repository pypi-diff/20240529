# Comparing `tmp/gamestorageapi-1.1.20.tar.gz` & `tmp/gamestorageapi-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamestorageapi-1.1.20.tar", last modified: Wed May 29 00:56:41 2024, max compression
+gzip compressed data, was "gamestorageapi-1.1.5.tar", last modified: Wed May 29 21:19:45 2024, max compression
```

## Comparing `gamestorageapi-1.1.20.tar` & `gamestorageapi-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:56:41.740471 gamestorageapi-1.1.20/
-drwxrwxrwx   0        0        0        0 2024-05-29 00:56:41.700782 gamestorageapi-1.1.20/GameStorageAPI/
--rw-rw-rw-   0        0        0    17273 2024-05-29 00:50:22.000000 gamestorageapi-1.1.20/GameStorageAPI/DataTypes.py
--rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-1.1.20/GameStorageAPI/__init__.py
--rw-rw-rw-   0        0        0     6916 2024-05-29 00:56:17.000000 gamestorageapi-1.1.20/GameStorageAPI/game.py
--rw-rw-rw-   0        0        0      583 2024-05-26 15:05:18.000000 gamestorageapi-1.1.20/GameStorageAPI/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:56:41.736155 gamestorageapi-1.1.20/GameStorageAPI.egg-info/
--rw-rw-rw-   0        0        0      469 2024-05-29 00:56:41.000000 gamestorageapi-1.1.20/GameStorageAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-29 00:56:41.000000 gamestorageapi-1.1.20/GameStorageAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:56:41.000000 gamestorageapi-1.1.20/GameStorageAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-29 00:56:41.000000 gamestorageapi-1.1.20/GameStorageAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 00:56:41.000000 gamestorageapi-1.1.20/GameStorageAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-1.1.20/LICENSE
--rw-rw-rw-   0        0        0      469 2024-05-29 00:56:41.737463 gamestorageapi-1.1.20/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 00:56:41.740471 gamestorageapi-1.1.20/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-05-29 00:56:09.000000 gamestorageapi-1.1.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:19:45.736205 gamestorageapi-1.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-29 21:19:45.710207 gamestorageapi-1.1.5/GameStorageAPI/
+-rw-rw-rw-   0        0        0    17273 2024-05-29 00:50:22.000000 gamestorageapi-1.1.5/GameStorageAPI/DataTypes.py
+-rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-1.1.5/GameStorageAPI/__init__.py
+-rw-rw-rw-   0        0        0     6916 2024-05-29 00:56:17.000000 gamestorageapi-1.1.5/GameStorageAPI/game.py
+-rw-rw-rw-   0        0        0      442 2024-05-29 21:17:05.000000 gamestorageapi-1.1.5/GameStorageAPI/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:19:45.731208 gamestorageapi-1.1.5/GameStorageAPI.egg-info/
+-rw-rw-rw-   0        0        0      468 2024-05-29 21:19:45.000000 gamestorageapi-1.1.5/GameStorageAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-29 21:19:45.000000 gamestorageapi-1.1.5/GameStorageAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 21:19:45.000000 gamestorageapi-1.1.5/GameStorageAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 21:19:45.000000 gamestorageapi-1.1.5/GameStorageAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 21:19:45.000000 gamestorageapi-1.1.5/GameStorageAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      468 2024-05-29 21:19:45.733206 gamestorageapi-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 21:19:45.737210 gamestorageapi-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      630 2024-05-29 21:19:41.000000 gamestorageapi-1.1.5/setup.py
```

### Comparing `gamestorageapi-1.1.20/GameStorageAPI/DataTypes.py` & `gamestorageapi-1.1.5/GameStorageAPI/DataTypes.py`

 * *Files identical despite different names*

### Comparing `gamestorageapi-1.1.20/GameStorageAPI/game.py` & `gamestorageapi-1.1.5/GameStorageAPI/game.py`

 * *Files identical despite different names*

### Comparing `gamestorageapi-1.1.20/LICENSE` & `gamestorageapi-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gamestorageapi-1.1.20/setup.py` & `gamestorageapi-1.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.20'
+VERSION = '1.1.5'
 DESCRIPTION = 'StorageAPI for games'
 
 
 setup(
     name="GameStorageAPI",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
```

