# Comparing `tmp/csle_attack_profiler-0.6.1.tar.gz` & `tmp/csle_attack_profiler-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attack_profiler-0.6.1.tar", last modified: Thu May 23 18:36:07 2024, max compression
+gzip compressed data, was "csle_attack_profiler-0.6.2.tar", last modified: Tue May 28 16:31:17 2024, max compression
```

## Comparing `csle_attack_profiler-0.6.1.tar` & `csle_attack_profiler-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:36:07.836566 csle_attack_profiler-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      652 2024-05-23 18:36:07.836605 csle_attack_profiler-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     3933 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      681 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1779 2024-05-23 18:36:07.836829 csle_attack_profiler-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:36:07.834410 csle_attack_profiler-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:36:07.835241 csle_attack_profiler-0.6.1/src/csle_attack_profiler/
--rw-r--r--   0 kim        (501) staff       (20)       37 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler/__version__.py
--rw-r--r--   0 kim        (501) staff       (20)    10535 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler/attack_profiler.py
--rw-r--r--   0 kim        (501) staff       (20)    24167 2024-05-23 18:33:18.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler/hmm_profiling.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:36:07.836144 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      652 2024-05-23 18:36:07.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      572 2024-05-23 18:36:07.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:36:07.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:44:09.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      502 2024-05-23 18:36:07.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       21 2024-05-23 18:36:07.000000 csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:36:07.836470 csle_attack_profiler-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)    44600 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/tests/test_attack_profiler.py
--rw-r--r--   0 kim        (501) staff       (20)     2780 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/tests/test_hmm_profiler.py
--rw-r--r--   0 kim        (501) staff       (20)     1286 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.1/tests/test_kullback.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:31:17.287179 csle_attack_profiler-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      652 2024-05-28 16:31:17.287236 csle_attack_profiler-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3933 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      681 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1779 2024-05-28 16:31:17.287479 csle_attack_profiler-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:31:17.283770 csle_attack_profiler-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:31:17.284904 csle_attack_profiler-0.6.2/src/csle_attack_profiler/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler/__version__.py
+-rw-r--r--   0 kim        (501) staff       (20)    10535 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler/attack_profiler.py
+-rw-r--r--   0 kim        (501) staff       (20)    24167 2024-05-23 18:33:18.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler/hmm_profiling.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:31:17.286082 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      652 2024-05-28 16:31:17.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      572 2024-05-28 16:31:17.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:31:17.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:44:09.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      502 2024-05-28 16:31:17.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       21 2024-05-28 16:31:17.000000 csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:31:17.287004 csle_attack_profiler-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)    44600 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/tests/test_attack_profiler.py
+-rw-r--r--   0 kim        (501) staff       (20)     2780 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/tests/test_hmm_profiler.py
+-rw-r--r--   0 kim        (501) staff       (20)     1286 2024-05-04 07:32:30.000000 csle_attack_profiler-0.6.2/tests/test_kullback.py
```

### Comparing `csle_attack_profiler-0.6.1/PKG-INFO` & `csle_attack_profiler-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_attack_profiler
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library with MITRE attack profiler for CSLE
 Author: Bength Pappila
 Author-email: brpa@kth.se
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attack_profiler-0.6.1/README.md` & `csle_attack_profiler-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/pyproject.toml` & `csle_attack_profiler-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/setup.cfg` & `csle_attack_profiler-0.6.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 install_requires = 
 	mitreattack-python==2.0.14
-	csle-base==0.6.1
-	csle-common==0.6.1
+	csle-base==0.6.2
+	csle-common==0.6.2
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
```

### Comparing `csle_attack_profiler-0.6.1/src/csle_attack_profiler/attack_profiler.py` & `csle_attack_profiler-0.6.2/src/csle_attack_profiler/attack_profiler.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/src/csle_attack_profiler/hmm_profiling.py` & `csle_attack_profiler-0.6.2/src/csle_attack_profiler/hmm_profiling.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/PKG-INFO` & `csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-attack-profiler
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library with MITRE attack profiler for CSLE
 Author: Bength Pappila
 Author-email: brpa@kth.se
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attack_profiler-0.6.1/src/csle_attack_profiler.egg-info/SOURCES.txt` & `csle_attack_profiler-0.6.2/src/csle_attack_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/tests/test_attack_profiler.py` & `csle_attack_profiler-0.6.2/tests/test_attack_profiler.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/tests/test_hmm_profiler.py` & `csle_attack_profiler-0.6.2/tests/test_hmm_profiler.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.6.1/tests/test_kullback.py` & `csle_attack_profiler-0.6.2/tests/test_kullback.py`

 * *Files identical despite different names*

