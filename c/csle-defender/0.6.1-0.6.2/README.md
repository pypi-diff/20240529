# Comparing `tmp/csle_defender-0.6.1.tar.gz` & `tmp/csle_defender-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_defender-0.6.1.tar", last modified: Thu May 23 18:35:12 2024, max compression
+gzip compressed data, was "csle_defender-0.6.2.tar", last modified: Tue May 28 16:30:19 2024, max compression
```

## Comparing `csle_defender-0.6.1.tar` & `csle_defender-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:12.726407 csle_defender-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      644 2024-05-23 18:35:12.726446 csle_defender-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     3801 2024-02-13 12:24:16.000000 csle_defender-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      673 2023-08-15 10:44:03.000000 csle_defender-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1729 2024-05-23 18:35:12.726672 csle_defender-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_defender-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:12.724464 csle_defender-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:12.725239 csle_defender-0.6.1/src/csle_defender/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_defender-0.6.1/src/csle_defender/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_defender-0.6.1/src/csle_defender/__version__.py
--rw-r--r--   0 kim        (501) staff       (20)     1197 2023-08-15 10:44:03.000000 csle_defender-0.6.1/src/csle_defender/defender.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:12.726220 csle_defender-0.6.1/src/csle_defender/emulation/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_defender-0.6.1/src/csle_defender/emulation/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     1291 2023-08-17 14:02:07.000000 csle_defender-0.6.1/src/csle_defender/emulation/defender_stopping_middleware.py
--rw-r--r--   0 kim        (501) staff       (20)     2568 2023-08-17 14:00:51.000000 csle_defender-0.6.1/src/csle_defender/emulation/emulated_defender.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:12.725924 csle_defender-0.6.1/src/csle_defender.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      644 2024-05-23 18:35:12.000000 csle_defender-0.6.1/src/csle_defender.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      572 2024-05-23 18:35:12.000000 csle_defender-0.6.1/src/csle_defender.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:12.000000 csle_defender-0.6.1/src/csle_defender.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:46.000000 csle_defender-0.6.1/src/csle_defender.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      475 2024-05-23 18:35:12.000000 csle_defender-0.6.1/src/csle_defender.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       14 2024-05-23 18:35:12.000000 csle_defender-0.6.1/src/csle_defender.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:12.726316 csle_defender-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)      774 2023-08-17 14:42:27.000000 csle_defender-0.6.1/tests/test_defender_stopping_middleware.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:19.812026 csle_defender-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      644 2024-05-28 16:30:19.812125 csle_defender-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3801 2024-02-13 12:24:16.000000 csle_defender-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      673 2023-08-15 10:44:03.000000 csle_defender-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1729 2024-05-28 16:30:19.814446 csle_defender-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_defender-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:19.803228 csle_defender-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:19.804733 csle_defender-0.6.2/src/csle_defender/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_defender-0.6.2/src/csle_defender/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_defender-0.6.2/src/csle_defender/__version__.py
+-rw-r--r--   0 kim        (501) staff       (20)     1197 2023-08-15 10:44:03.000000 csle_defender-0.6.2/src/csle_defender/defender.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:19.807254 csle_defender-0.6.2/src/csle_defender/emulation/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_defender-0.6.2/src/csle_defender/emulation/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     1291 2023-08-17 14:02:07.000000 csle_defender-0.6.2/src/csle_defender/emulation/defender_stopping_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)     2568 2023-08-17 14:00:51.000000 csle_defender-0.6.2/src/csle_defender/emulation/emulated_defender.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:19.806202 csle_defender-0.6.2/src/csle_defender.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      644 2024-05-28 16:30:19.000000 csle_defender-0.6.2/src/csle_defender.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      572 2024-05-28 16:30:19.000000 csle_defender-0.6.2/src/csle_defender.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:19.000000 csle_defender-0.6.2/src/csle_defender.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:46.000000 csle_defender-0.6.2/src/csle_defender.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      475 2024-05-28 16:30:19.000000 csle_defender-0.6.2/src/csle_defender.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       14 2024-05-28 16:30:19.000000 csle_defender-0.6.2/src/csle_defender.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:19.807540 csle_defender-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)      774 2023-08-17 14:42:27.000000 csle_defender-0.6.2/tests/test_defender_stopping_middleware.py
```

### Comparing `csle_defender-0.6.1/PKG-INFO` & `csle_defender-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_defender
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.6.1/README.md` & `csle_defender-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_defender-0.6.1/pyproject.toml` & `csle_defender-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_defender-0.6.1/setup.cfg` & `csle_defender-0.6.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.6.1
-	csle-common>=0.6.1
+	csle-base>=0.6.2
+	csle-common>=0.6.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_defender-0.6.1/src/csle_defender/defender.py` & `csle_defender-0.6.2/src/csle_defender/defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.6.1/src/csle_defender/emulation/defender_stopping_middleware.py` & `csle_defender-0.6.2/src/csle_defender/emulation/defender_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.6.1/src/csle_defender/emulation/emulated_defender.py` & `csle_defender-0.6.2/src/csle_defender/emulation/emulated_defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.6.1/src/csle_defender.egg-info/PKG-INFO` & `csle_defender-0.6.2/src/csle_defender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-defender
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.6.1/src/csle_defender.egg-info/SOURCES.txt` & `csle_defender-0.6.2/src/csle_defender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_defender-0.6.1/tests/test_defender_stopping_middleware.py` & `csle_defender-0.6.2/tests/test_defender_stopping_middleware.py`

 * *Files identical despite different names*

