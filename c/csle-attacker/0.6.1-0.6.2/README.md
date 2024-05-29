# Comparing `tmp/csle_attacker-0.6.1.tar.gz` & `tmp/csle_attacker-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attacker-0.6.1.tar", last modified: Thu May 23 18:35:09 2024, max compression
+gzip compressed data, was "csle_attacker-0.6.2.tar", last modified: Tue May 28 16:30:16 2024, max compression
```

## Comparing `csle_attacker-0.6.1.tar` & `csle_attacker-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.857580 csle_attacker-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      649 2024-05-23 18:35:09.857624 csle_attacker-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     3866 2024-02-13 12:24:16.000000 csle_attacker-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      673 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1734 2024-05-23 18:35:09.857851 csle_attacker-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.854454 csle_attacker-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.855324 csle_attacker-0.6.1/src/csle_attacker/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_attacker-0.6.1/src/csle_attacker/__version__.py
--rw-r--r--   0 kim        (501) staff       (20)      941 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/attacker.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.856682 csle_attacker-0.6.1/src/csle_attacker/emulation/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      994 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/attacker_stopping_middleware.py
--rw-r--r--   0 kim        (501) staff       (20)    11411 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/emulated_attacker.py
--rw-r--r--   0 kim        (501) staff       (20)    11564 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/exploit_middleware.py
--rw-r--r--   0 kim        (501) staff       (20)     4678 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/post_exploit_middleware.py
--rw-r--r--   0 kim        (501) staff       (20)     5951 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/recon_middleware.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.857339 csle_attacker-0.6.1/src/csle_attacker/emulation/util/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/util/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    45676 2023-10-10 07:21:48.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/util/exploit_util.py
--rw-r--r--   0 kim        (501) staff       (20)     7720 2023-08-15 10:44:03.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/util/nikto_util.py
--rw-r--r--   0 kim        (501) staff       (20)    34952 2024-02-13 12:24:16.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/util/nmap_util.py
--rw-r--r--   0 kim        (501) staff       (20)    30139 2023-10-10 07:21:48.000000 csle_attacker-0.6.1/src/csle_attacker/emulation/util/shell_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.856034 csle_attacker-0.6.1/src/csle_attacker.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      649 2024-05-23 18:35:09.000000 csle_attacker-0.6.1/src/csle_attacker.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      941 2024-05-23 18:35:09.000000 csle_attacker-0.6.1/src/csle_attacker.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:09.000000 csle_attacker-0.6.1/src/csle_attacker.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:41.000000 csle_attacker-0.6.1/src/csle_attacker.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      475 2024-05-23 18:35:09.000000 csle_attacker-0.6.1/src/csle_attacker.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       14 2024-05-23 18:35:09.000000 csle_attacker-0.6.1/src/csle_attacker.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:09.857479 csle_attacker-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)     1790 2023-08-17 14:41:23.000000 csle_attacker-0.6.1/tests/test_shell_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.820809 csle_attacker-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      649 2024-05-28 16:30:16.820877 csle_attacker-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3866 2024-02-13 12:24:16.000000 csle_attacker-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      673 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1734 2024-05-28 16:30:16.821175 csle_attacker-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.815028 csle_attacker-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.816400 csle_attacker-0.6.2/src/csle_attacker/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_attacker-0.6.2/src/csle_attacker/__version__.py
+-rw-r--r--   0 kim        (501) staff       (20)      941 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/attacker.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.818399 csle_attacker-0.6.2/src/csle_attacker/emulation/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      994 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/attacker_stopping_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)    11411 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/emulated_attacker.py
+-rw-r--r--   0 kim        (501) staff       (20)    11564 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/exploit_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)     4678 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/post_exploit_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)     5951 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/recon_middleware.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.820272 csle_attacker-0.6.2/src/csle_attacker/emulation/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    45676 2023-10-10 07:21:48.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/util/exploit_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     7720 2023-08-15 10:44:03.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/util/nikto_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    34952 2024-02-13 12:24:16.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/util/nmap_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    30139 2023-10-10 07:21:48.000000 csle_attacker-0.6.2/src/csle_attacker/emulation/util/shell_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.817338 csle_attacker-0.6.2/src/csle_attacker.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      649 2024-05-28 16:30:16.000000 csle_attacker-0.6.2/src/csle_attacker.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      941 2024-05-28 16:30:16.000000 csle_attacker-0.6.2/src/csle_attacker.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:16.000000 csle_attacker-0.6.2/src/csle_attacker.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:41.000000 csle_attacker-0.6.2/src/csle_attacker.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      475 2024-05-28 16:30:16.000000 csle_attacker-0.6.2/src/csle_attacker.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       14 2024-05-28 16:30:16.000000 csle_attacker-0.6.2/src/csle_attacker.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:16.820483 csle_attacker-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     1790 2023-08-17 14:41:23.000000 csle_attacker-0.6.2/tests/test_shell_util.py
```

### Comparing `csle_attacker-0.6.1/PKG-INFO` & `csle_attacker-0.6.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_attacker
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.6.1/README.md` & `csle_attacker-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/pyproject.toml` & `csle_attacker-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/setup.cfg` & `csle_attacker-0.6.2/setup.cfg`

 * *Files 6% similar despite different names*

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

### Comparing `csle_attacker-0.6.1/src/csle_attacker/attacker.py` & `csle_attacker-0.6.2/src/csle_attacker/attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/attacker_stopping_middleware.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/attacker_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/emulated_attacker.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/emulated_attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/exploit_middleware.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/post_exploit_middleware.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/post_exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/recon_middleware.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/recon_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/util/exploit_util.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/util/exploit_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/util/nikto_util.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/util/nikto_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/util/nmap_util.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/util/nmap_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker/emulation/util/shell_util.py` & `csle_attacker-0.6.2/src/csle_attacker/emulation/util/shell_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/src/csle_attacker.egg-info/PKG-INFO` & `csle_attacker-0.6.2/src/csle_attacker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-attacker
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.6.1/src/csle_attacker.egg-info/SOURCES.txt` & `csle_attacker-0.6.2/src/csle_attacker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.6.1/tests/test_shell_util.py` & `csle_attacker-0.6.2/tests/test_shell_util.py`

 * *Files identical despite different names*

