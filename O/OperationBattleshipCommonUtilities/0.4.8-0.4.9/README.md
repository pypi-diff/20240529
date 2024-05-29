# Comparing `tmp/OperationBattleshipCommonUtilities-0.4.8.tar.gz` & `tmp/OperationBattleshipCommonUtilities-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OperationBattleshipCommonUtilities-0.4.8.tar", last modified: Mon May 13 14:00:15 2024, max compression
+gzip compressed data, was "OperationBattleshipCommonUtilities-0.4.9.tar", last modified: Wed May 15 02:44:21 2024, max compression
```

## Comparing `OperationBattleshipCommonUtilities-0.4.8.tar` & `OperationBattleshipCommonUtilities-0.4.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:15.537356 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDaoOld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/FailureLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GeographyHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobPostingDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobSkillsDao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/NomicAICaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/OpenAICaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:44:21.140865 OperationBattleshipCommonUtilities-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:44:21.136865 OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-15 02:44:21.000000 OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-15 02:44:21.000000 OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:44:21.000000 OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 02:44:21.000000 OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:44:21.000000 OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-15 02:44:21.136865 OperationBattleshipCommonUtilities-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:44:21.136865 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/CompanyDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/CompanyDaoOld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/FailureLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/GeographyHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobPostingDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/NomicAICaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/OpenAICaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:44:21.140865 OperationBattleshipCommonUtilities-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 02:44:13.000000 OperationBattleshipCommonUtilities-0.4.9/setup.py
```

### Comparing `OperationBattleshipCommonUtilities-0.4.8/LICENSE` & `OperationBattleshipCommonUtilities-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.8
+Version: 0.4.9
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `OperationBattleshipCommonUtilities-0.4.9/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/PKG-INFO` & `OperationBattleshipCommonUtilities-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.8
+Version: 0.4.9
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.4.8/README.md` & `OperationBattleshipCommonUtilities-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/ApifyJobsCaller.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/CompanyDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDaoOld.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/CompanyDaoOld.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/FailureLogger.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/FailureLogger.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GeographyHelper.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/GeographyHelper.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobKeyWordsDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobPostingDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobPostingDao.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,17 +70,22 @@
         return self.execute_db_command(sql, data)
 
     def fetchPmJobsRequiringEnrichment(self):
         sql = "SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%') AND is_ai IS NULL ORDER BY job_posting_date DESC"
         return self.execute_db_command(sql)
 
     def fetchJobsRequiringEnrichment(self):
-        sql = "SELECT * FROM job_postings WHERE is_ai IS NULL"
+        sql = """
+        SELECT * FROM job_postings 
+        WHERE is_ai IS NULL 
+        AND date >= CURRENT_DATE - INTERVAL '30 days'
+        """
         return self.execute_db_command(sql)
 
+
     def checkIfJobExists(self, cleanedLinkedInJobURL):
         sql = "SELECT * FROM job_postings WHERE posting_url = %s"
         result = self.execute_db_command(sql, (cleanedLinkedInJobURL,))
         return len(result) > 0 if result is not None else False
 
     def insertNewJobRecord(self, jobpostingDataFrame):
         sql = """
```

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobSkillsDao.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/NomicAICaller.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/NomicAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/OpenAICaller.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/OpenAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `OperationBattleshipCommonUtilities-0.4.9/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.8/setup.py` & `OperationBattleshipCommonUtilities-0.4.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='OperationBattleshipCommonUtilities',
-    version='0.4.8',
+    version='0.4.9',
     packages=find_packages(),
     license='Apache-2.0 license',
     description='Classes and Utilities that are shared in the Operation Battleship Application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Matthew Caraway',
     author_email='matthew@CarawayLabs.com',
```

