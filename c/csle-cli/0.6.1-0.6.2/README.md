# Comparing `tmp/csle_cli-0.6.1.tar.gz` & `tmp/csle_cli-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.6.1.tar", last modified: Thu May 23 18:35:42 2024, max compression
+gzip compressed data, was "csle_cli-0.6.2.tar", last modified: Tue May 28 16:30:51 2024, max compression
```

## Comparing `csle_cli-0.6.1.tar` & `csle_cli-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:42.845804 csle_cli-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      619 2024-05-23 18:35:42.845840 csle_cli-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)    23697 2024-02-13 12:24:16.000000 csle_cli-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      668 2023-08-15 10:44:03.000000 csle_cli-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1998 2024-05-23 18:35:42.846075 csle_cli-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_cli-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:42.843964 csle_cli-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:42.844724 csle_cli-0.6.1/src/csle_cli/
--rw-r--r--   0 kim        (501) staff       (20)       38 2023-08-15 10:44:03.000000 csle_cli-0.6.1/src/csle_cli/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_cli-0.6.1/src/csle_cli/__version__.py
--rwxr-xr-x   0 kim        (501) staff       (20)   118330 2024-03-25 12:48:05.000000 csle_cli-0.6.1/src/csle_cli/cli.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:42.845629 csle_cli-0.6.1/src/csle_cli.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      619 2024-05-23 18:35:42.000000 csle_cli-0.6.1/src/csle_cli.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      387 2024-05-23 18:35:42.000000 csle_cli-0.6.1/src/csle_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:42.000000 csle_cli-0.6.1/src/csle_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)       47 2024-05-23 18:35:42.000000 csle_cli-0.6.1/src/csle_cli.egg-info/entry_points.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:31.000000 csle_cli-0.6.1/src/csle_cli.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      699 2024-05-23 18:35:42.000000 csle_cli-0.6.1/src/csle_cli.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)        9 2024-05-23 18:35:42.000000 csle_cli-0.6.1/src/csle_cli.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:42.845723 csle_cli-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)      352 2023-08-15 10:44:03.000000 csle_cli-0.6.1/tests/test_cli.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:51.132281 csle_cli-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      619 2024-05-28 16:30:51.132322 csle_cli-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)    23697 2024-02-13 12:24:16.000000 csle_cli-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      668 2023-08-15 10:44:03.000000 csle_cli-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1998 2024-05-28 16:30:51.132580 csle_cli-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_cli-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:51.129510 csle_cli-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:51.130629 csle_cli-0.6.2/src/csle_cli/
+-rw-r--r--   0 kim        (501) staff       (20)       38 2023-08-15 10:44:03.000000 csle_cli-0.6.2/src/csle_cli/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_cli-0.6.2/src/csle_cli/__version__.py
+-rwxr-xr-x   0 kim        (501) staff       (20)   118330 2024-03-25 12:48:05.000000 csle_cli-0.6.2/src/csle_cli/cli.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:51.132039 csle_cli-0.6.2/src/csle_cli.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      619 2024-05-28 16:30:51.000000 csle_cli-0.6.2/src/csle_cli.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      387 2024-05-28 16:30:51.000000 csle_cli-0.6.2/src/csle_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:51.000000 csle_cli-0.6.2/src/csle_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)       47 2024-05-28 16:30:51.000000 csle_cli-0.6.2/src/csle_cli.egg-info/entry_points.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:31.000000 csle_cli-0.6.2/src/csle_cli.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      699 2024-05-28 16:30:51.000000 csle_cli-0.6.2/src/csle_cli.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)        9 2024-05-28 16:30:51.000000 csle_cli-0.6.2/src/csle_cli.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:51.132146 csle_cli-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)      352 2023-08-15 10:44:03.000000 csle_cli-0.6.2/tests/test_cli.py
```

### Comparing `csle_cli-0.6.1/PKG-INFO` & `csle_cli-0.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.6.1/README.md` & `csle_cli-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.6.1/pyproject.toml` & `csle_cli-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.6.1/setup.cfg` & `csle_cli-0.6.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-base>=0.6.1
-	csle-common>=0.6.1
-	csle-cluster>=0.6.1
-	csle-collector>=0.6.1
-	csle-attacker>=0.6.1
-	csle-defender>=0.6.1
-	csle-system-identification>=0.6.1
-	gym-csle-stopping-game>=0.6.1
-	gym-csle-apt-game>=0.6.1
-	gym-csle-cyborg>=0.6.1
-	gym-csle-intrusion-response-game>=0.6.1
-	csle-agents>=0.6.1
-	csle-tolerance>=0.6.1
+	csle-base>=0.6.2
+	csle-common>=0.6.2
+	csle-cluster>=0.6.2
+	csle-collector>=0.6.2
+	csle-attacker>=0.6.2
+	csle-defender>=0.6.2
+	csle-system-identification>=0.6.2
+	gym-csle-stopping-game>=0.6.2
+	gym-csle-apt-game>=0.6.2
+	gym-csle-cyborg>=0.6.2
+	gym-csle-intrusion-response-game>=0.6.2
+	csle-agents>=0.6.2
+	csle-tolerance>=0.6.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.6.1/src/csle_cli/cli.py` & `csle_cli-0.6.2/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.6.1/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.6.2/src/csle_cli.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.6.1/src/csle_cli.egg-info/requires.txt` & `csle_cli-0.6.2/src/csle_cli.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 click>=8.1.3
-csle-base>=0.6.1
-csle-common>=0.6.1
-csle-cluster>=0.6.1
-csle-collector>=0.6.1
-csle-attacker>=0.6.1
-csle-defender>=0.6.1
-csle-system-identification>=0.6.1
-gym-csle-stopping-game>=0.6.1
-gym-csle-apt-game>=0.6.1
-gym-csle-cyborg>=0.6.1
-gym-csle-intrusion-response-game>=0.6.1
-csle-agents>=0.6.1
-csle-tolerance>=0.6.1
+csle-base>=0.6.2
+csle-common>=0.6.2
+csle-cluster>=0.6.2
+csle-collector>=0.6.2
+csle-attacker>=0.6.2
+csle-defender>=0.6.2
+csle-system-identification>=0.6.2
+gym-csle-stopping-game>=0.6.2
+gym-csle-apt-game>=0.6.2
+gym-csle-cyborg>=0.6.2
+gym-csle-intrusion-response-game>=0.6.2
+csle-agents>=0.6.2
+csle-tolerance>=0.6.2
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

