# Comparing `tmp/rcsb.utils.repository-0.43.tar.gz` & `tmp/rcsb_utils_repository-0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.repository-0.43.tar", last modified: Thu Mar 21 19:30:47 2024, max compression
+gzip compressed data, was "rcsb_utils_repository-0.44.tar", last modified: Wed May 29 19:13:13 2024, max compression
```

## Comparing `rcsb.utils.repository-0.43.tar` & `rcsb_utils_repository-0.44.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 19:30:47.277513 rcsb.utils.repository-0.43/
--rw-r--r--   0 vsts      (1001) docker     (127)     3376 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2285 2024-03-21 19:30:47.277513 rcsb.utils.repository-0.43/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 19:30:47.273513 rcsb.utils.repository-0.43/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 19:30:47.273513 rcsb.utils.repository-0.43/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 19:30:47.273513 rcsb.utils.repository-0.43/rcsb/utils/repository/
--rw-r--r--   0 vsts      (1001) docker     (127)    14788 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/CurrentHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15556 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/RemovedHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    63861 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/RepositoryProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19042 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/ScanRepoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5518 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/UnreleasedHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4211 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/UpdateHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/rcsb/utils/repository/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 19:30:47.273513 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2285 2024-03-21 19:30:47.000000 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      699 2024-03-21 19:30:47.000000 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-21 19:30:47.000000 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-21 19:30:46.000000 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-03-21 19:30:47.000000 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-03-21 19:30:47.000000 rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      165 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-03-21 19:30:47.277513 rcsb.utils.repository-0.43/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2236 2024-03-21 19:18:35.000000 rcsb.utils.repository-0.43/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-29 19:13:13.137311 rcsb_utils_repository-0.44/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3410 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2285 2024-05-29 19:13:13.137311 rcsb_utils_repository-0.44/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-29 19:13:13.133311 rcsb_utils_repository-0.44/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-29 19:13:13.133311 rcsb_utils_repository-0.44/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-29 19:13:13.137311 rcsb_utils_repository-0.44/rcsb/utils/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)    14788 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/CurrentHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15556 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/RemovedHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    63861 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/RepositoryProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19058 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/ScanRepoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5518 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/UnreleasedHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4211 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/UpdateHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/rcsb/utils/repository/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-29 19:13:13.137311 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2285 2024-05-29 19:13:13.000000 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      699 2024-05-29 19:13:13.000000 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-29 19:13:13.000000 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-29 19:13:11.000000 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-05-29 19:13:13.000000 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-29 19:13:13.000000 rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      165 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-29 19:13:13.137311 rcsb_utils_repository-0.44/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2236 2024-05-29 18:59:04.000000 rcsb_utils_repository-0.44/setup.py
```

### Comparing `rcsb.utils.repository-0.43/HISTORY.txt` & `rcsb_utils_repository-0.44/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 03-Aug-2022 - V0.36 Enable retrieval of specific model files with input
 23-Dec-2022 - V0.37 Configuration changes to support tox 4
 14-Feb-2023 - V0.38 Add support for requesting specific inputIdCodeList/idCodeList for CSMs
 22-Mar-2023 - V0.39 Update references to py-rcsb_exdb_assets master branch
 19-May-2023 - V0.40 Update DNS to PDB archive
 12-Jun-2023 - V0.41 Disable useCache for holdings files to force re-download
 05-Mar-2024 - V0.42 Adjust RepositoryProvider to support BCIF loading and CSM scaling
-19-Mar-2024 - V0.43 Raise exception and return empty list if not all dataContainers are properly read from file in __mergeContainers()
+19-Mar-2024 - V0.43 Raise exception and return empty list if not all dataContainers are properly read from file in __mergeContainers()
+29-May-2024 - V0.44 Fix pylinting
```

### Comparing `rcsb.utils.repository-0.43/LICENSE` & `rcsb_utils_repository-0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/PKG-INFO` & `rcsb_utils_repository-0.44/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.repository
-Version: 0.43
+Version: 0.44
 Summary: RCSB Python Repository Data Management Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_repository
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.repository-0.43/README.md` & `rcsb_utils_repository-0.44/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/rcsb/utils/repository/CurrentHoldingsProvider.py` & `rcsb_utils_repository-0.44/rcsb/utils/repository/CurrentHoldingsProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/rcsb/utils/repository/RemovedHoldingsProvider.py` & `rcsb_utils_repository-0.44/rcsb/utils/repository/RemovedHoldingsProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/rcsb/utils/repository/RepositoryProvider.py` & `rcsb_utils_repository-0.44/rcsb/utils/repository/RepositoryProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/rcsb/utils/repository/ScanRepoUtil.py` & `rcsb_utils_repository-0.44/rcsb/utils/repository/ScanRepoUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
         except Exception as e:
             logger.exception("Failing %r with %s", contentType, str(e))
 
         return False
 
     def evalScan(self, scanDataFilePath, evalJsonFilePath, evalType="data_type"):
 
+        rD = {}
         scanDataD = self.__mU.doImport(scanDataFilePath, fmt="pickle")
         if evalType in ["data_type"]:
             rD = self.__evalScanDataType(scanDataD)
         elif evalType in ["data_coverage"]:
             rD, _ = self.__evalScanDataCoverage(scanDataD)
         else:
             logger.debug("Unknown evalType %r", evalType)
```

### Comparing `rcsb.utils.repository-0.43/rcsb/utils/repository/UnreleasedHoldingsProvider.py` & `rcsb_utils_repository-0.44/rcsb/utils/repository/UnreleasedHoldingsProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/rcsb/utils/repository/UpdateHoldingsProvider.py` & `rcsb_utils_repository-0.44/rcsb/utils/repository/UpdateHoldingsProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/PKG-INFO` & `rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.repository
-Version: 0.43
+Version: 0.44
 Summary: RCSB Python Repository Data Management Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_repository
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.repository-0.43/rcsb.utils.repository.egg-info/SOURCES.txt` & `rcsb_utils_repository-0.44/rcsb.utils.repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.43/setup.py` & `rcsb_utils_repository-0.44/setup.py`

 * *Files identical despite different names*

