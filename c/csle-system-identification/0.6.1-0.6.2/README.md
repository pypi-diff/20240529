# Comparing `tmp/csle_system_identification-0.6.1.tar.gz` & `tmp/csle_system_identification-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_system_identification-0.6.1.tar", last modified: Thu May 23 18:35:15 2024, max compression
+gzip compressed data, was "csle_system_identification-0.6.2.tar", last modified: Tue May 28 16:30:22 2024, max compression
```

## Comparing `csle_system_identification-0.6.1.tar` & `csle_system_identification-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.472331 csle_system_identification-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      661 2024-05-23 18:35:15.472375 csle_system_identification-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     4330 2024-02-13 12:24:16.000000 csle_system_identification-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      686 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     2012 2024-05-23 18:35:15.472627 csle_system_identification-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.468331 csle_system_identification-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.469472 csle_system_identification-0.6.1/src/csle_system_identification/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_system_identification-0.6.1/src/csle_system_identification/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.470500 csle_system_identification-0.6.1/src/csle_system_identification/base/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/base/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2398 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/base/base_system_identification_algorithm.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.470694 csle_system_identification-0.6.1/src/csle_system_identification/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      984 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.470884 csle_system_identification-0.6.1/src/csle_system_identification/empirical/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/empirical/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     7360 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/empirical/empirical_algorithm.py
--rw-r--r--   0 kim        (501) staff       (20)    17176 2024-02-13 12:24:16.000000 csle_system_identification-0.6.1/src/csle_system_identification/emulator.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.471093 csle_system_identification-0.6.1/src/csle_system_identification/expectation_maximization/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/expectation_maximization/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     7604 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.471421 csle_system_identification-0.6.1/src/csle_system_identification/gp/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/gp/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     9926 2023-08-26 12:55:18.000000 csle_system_identification-0.6.1/src/csle_system_identification/gp/gp_regression_algorithm.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.471795 csle_system_identification-0.6.1/src/csle_system_identification/job_controllers/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/job_controllers/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2159 2023-08-22 07:27:08.000000 csle_system_identification-0.6.1/src/csle_system_identification/job_controllers/data_collection_job_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     2212 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/job_controllers/system_identification_job_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.472044 csle_system_identification-0.6.1/src/csle_system_identification/mcmc/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/mcmc/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     7967 2023-08-15 10:44:03.000000 csle_system_identification-0.6.1/src/csle_system_identification/mcmc/mcmc.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.470314 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      661 2024-05-23 18:35:15.000000 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     1461 2024-05-23 18:35:15.000000 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:15.000000 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:52.000000 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      604 2024-05-23 18:35:15.000000 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       27 2024-05-23 18:35:15.000000 csle_system_identification-0.6.1/src/csle_system_identification.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:15.472192 csle_system_identification-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)     2226 2023-08-17 14:55:58.000000 csle_system_identification-0.6.1/tests/test_empirical_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.786800 csle_system_identification-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      661 2024-05-28 16:30:22.786854 csle_system_identification-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     4330 2024-02-13 12:24:16.000000 csle_system_identification-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      686 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     2012 2024-05-28 16:30:22.787132 csle_system_identification-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.780922 csle_system_identification-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.782602 csle_system_identification-0.6.2/src/csle_system_identification/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.784087 csle_system_identification-0.6.2/src/csle_system_identification/base/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/base/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2398 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/base/base_system_identification_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.784452 csle_system_identification-0.6.2/src/csle_system_identification/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      984 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.784885 csle_system_identification-0.6.2/src/csle_system_identification/empirical/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/empirical/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7360 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/empirical/empirical_algorithm.py
+-rw-r--r--   0 kim        (501) staff       (20)    17176 2024-02-13 12:24:16.000000 csle_system_identification-0.6.2/src/csle_system_identification/emulator.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.785293 csle_system_identification-0.6.2/src/csle_system_identification/expectation_maximization/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/expectation_maximization/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7604 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.785586 csle_system_identification-0.6.2/src/csle_system_identification/gp/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/gp/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     9926 2023-08-26 12:55:18.000000 csle_system_identification-0.6.2/src/csle_system_identification/gp/gp_regression_algorithm.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.786178 csle_system_identification-0.6.2/src/csle_system_identification/job_controllers/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/job_controllers/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2159 2023-08-22 07:27:08.000000 csle_system_identification-0.6.2/src/csle_system_identification/job_controllers/data_collection_job_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2212 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/job_controllers/system_identification_job_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.786402 csle_system_identification-0.6.2/src/csle_system_identification/mcmc/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/mcmc/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7967 2023-08-15 10:44:03.000000 csle_system_identification-0.6.2/src/csle_system_identification/mcmc/mcmc.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.783847 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      661 2024-05-28 16:30:22.000000 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1461 2024-05-28 16:30:22.000000 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:22.000000 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:52.000000 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      604 2024-05-28 16:30:22.000000 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       27 2024-05-28 16:30:22.000000 csle_system_identification-0.6.2/src/csle_system_identification.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:22.786544 csle_system_identification-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     2226 2023-08-17 14:55:58.000000 csle_system_identification-0.6.2/tests/test_empirical_algorithm.py
```

### Comparing `csle_system_identification-0.6.1/PKG-INFO` & `csle_system_identification-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_system_identification
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.6.1/README.md` & `csle_system_identification-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/pyproject.toml` & `csle_system_identification-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/setup.cfg` & `csle_system_identification-0.6.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.6.1
-	csle-common>=0.6.1
-	csle-collector>=0.6.1
-	csle-attacker>=0.6.1
-	csle-defender>=0.6.1
+	csle-base>=0.6.2
+	csle-common>=0.6.2
+	csle-collector>=0.6.2
+	csle-attacker>=0.6.2
+	csle-defender>=0.6.2
 	gpytorch>=1.9.0
 	pymc>=5.5.0
 	pytensor>=2.12.3
 	scikit-learn>=1.3.0
 python_requires = >=3.8
 package_dir = 
 	=src
```

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/base/base_system_identification_algorithm.py` & `csle_system_identification-0.6.2/src/csle_system_identification/base/base_system_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/constants/constants.py` & `csle_system_identification-0.6.2/src/csle_system_identification/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/empirical/empirical_algorithm.py` & `csle_system_identification-0.6.2/src/csle_system_identification/empirical/empirical_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/emulator.py` & `csle_system_identification-0.6.2/src/csle_system_identification/emulator.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py` & `csle_system_identification-0.6.2/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/gp/gp_regression_algorithm.py` & `csle_system_identification-0.6.2/src/csle_system_identification/gp/gp_regression_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/job_controllers/data_collection_job_manager.py` & `csle_system_identification-0.6.2/src/csle_system_identification/job_controllers/data_collection_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/job_controllers/system_identification_job_manager.py` & `csle_system_identification-0.6.2/src/csle_system_identification/job_controllers/system_identification_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification/mcmc/mcmc.py` & `csle_system_identification-0.6.2/src/csle_system_identification/mcmc/mcmc.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification.egg-info/PKG-INFO` & `csle_system_identification-0.6.2/src/csle_system_identification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-system-identification
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification.egg-info/SOURCES.txt` & `csle_system_identification-0.6.2/src/csle_system_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.6.1/src/csle_system_identification.egg-info/requires.txt` & `csle_system_identification-0.6.2/src/csle_system_identification.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-csle-base>=0.6.1
-csle-common>=0.6.1
-csle-collector>=0.6.1
-csle-attacker>=0.6.1
-csle-defender>=0.6.1
+csle-base>=0.6.2
+csle-common>=0.6.2
+csle-collector>=0.6.2
+csle-attacker>=0.6.2
+csle-defender>=0.6.2
 gpytorch>=1.9.0
 pymc>=5.5.0
 pytensor>=2.12.3
 scikit-learn>=1.3.0
 
 [testing]
 pytest>=6.0
```

### Comparing `csle_system_identification-0.6.1/tests/test_empirical_algorithm.py` & `csle_system_identification-0.6.2/tests/test_empirical_algorithm.py`

 * *Files identical despite different names*

