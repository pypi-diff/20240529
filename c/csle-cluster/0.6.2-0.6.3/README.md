# Comparing `tmp/csle_cluster-0.6.2.tar.gz` & `tmp/csle_cluster-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.6.2.tar", last modified: Tue May 28 16:30:53 2024, max compression
+gzip compressed data, was "csle_cluster-0.6.3.tar", last modified: Wed May 29 08:58:46 2024, max compression
```

## Comparing `csle_cluster-0.6.2.tar` & `csle_cluster-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.990819 csle_cluster-0.6.2/
--rw-r--r--   0 kim        (501) staff       (20)      794 2024-05-28 16:30:53.990862 csle_cluster-0.6.2/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     4307 2024-02-13 12:24:16.000000 csle_cluster-0.6.2/README.md
--rw-r--r--   0 kim        (501) staff       (20)      672 2023-08-15 10:44:03.000000 csle_cluster-0.6.2/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     2067 2024-05-28 16:30:53.991105 csle_cluster-0.6.2/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_cluster-0.6.2/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.982146 csle_cluster-0.6.2/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.983094 csle_cluster-0.6.2/src/csle_cluster/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_cluster-0.6.2/src/csle_cluster/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_cluster-0.6.2/src/csle_cluster/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.989020 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)   240982 2024-04-10 18:29:55.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-r--r--   0 kim        (501) staff       (20)   270830 2024-04-17 08:32:22.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-r--r--   0 kim        (501) staff       (20)    94763 2023-08-26 08:04:28.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)   349493 2023-08-26 08:04:28.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)   207915 2023-08-26 08:04:28.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-r--r--   0 kim        (501) staff       (20)   204861 2023-08-23 08:52:10.000000 csle_cluster-0.6.2/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.989830 csle_cluster-0.6.2/src/csle_cluster/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_cluster-0.6.2/src/csle_cluster/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      459 2023-08-15 10:44:03.000000 csle_cluster-0.6.2/src/csle_cluster/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.983867 csle_cluster-0.6.2/src/csle_cluster.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      794 2024-05-28 16:30:53.000000 csle_cluster-0.6.2/src/csle_cluster.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      835 2024-05-28 16:30:53.000000 csle_cluster-0.6.2/src/csle_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:53.000000 csle_cluster-0.6.2/src/csle_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:37.000000 csle_cluster-0.6.2/src/csle_cluster.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      689 2024-05-28 16:30:53.000000 csle_cluster-0.6.2/src/csle_cluster.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       13 2024-05-28 16:30:53.000000 csle_cluster-0.6.2/src/csle_cluster.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:53.990062 csle_cluster-0.6.2/tests/
--rw-r--r--   0 kim        (501) staff       (20)   355781 2023-08-30 12:52:39.000000 csle_cluster-0.6.2/tests/test_cluster_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.911886 csle_cluster-0.6.3/
+-rw-r--r--   0 kim        (501) staff       (20)      794 2024-05-29 08:58:46.911931 csle_cluster-0.6.3/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     4307 2024-02-13 12:24:16.000000 csle_cluster-0.6.3/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      672 2023-08-15 10:44:03.000000 csle_cluster-0.6.3/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     2067 2024-05-29 08:58:46.912176 csle_cluster-0.6.3/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_cluster-0.6.3/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.903579 csle_cluster-0.6.3/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.904582 csle_cluster-0.6.3/src/csle_cluster/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_cluster-0.6.3/src/csle_cluster/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-29 08:57:56.000000 csle_cluster-0.6.3/src/csle_cluster/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.908834 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)   240982 2024-04-10 18:29:55.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-r--r--   0 kim        (501) staff       (20)   270830 2024-04-17 08:32:22.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    94763 2023-08-26 08:04:28.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)   349493 2023-08-26 08:04:28.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)   207915 2023-08-26 08:04:28.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)   204861 2023-08-23 08:52:10.000000 csle_cluster-0.6.3/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.909839 csle_cluster-0.6.3/src/csle_cluster/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_cluster-0.6.3/src/csle_cluster/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      459 2023-08-15 10:44:03.000000 csle_cluster-0.6.3/src/csle_cluster/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.905424 csle_cluster-0.6.3/src/csle_cluster.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      794 2024-05-29 08:58:46.000000 csle_cluster-0.6.3/src/csle_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      835 2024-05-29 08:58:46.000000 csle_cluster-0.6.3/src/csle_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-29 08:58:46.000000 csle_cluster-0.6.3/src/csle_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:37.000000 csle_cluster-0.6.3/src/csle_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      689 2024-05-29 08:58:46.000000 csle_cluster-0.6.3/src/csle_cluster.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       13 2024-05-29 08:58:46.000000 csle_cluster-0.6.3/src/csle_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:46.911605 csle_cluster-0.6.3/tests/
+-rw-r--r--   0 kim        (501) staff       (20)   355781 2023-08-30 12:52:39.000000 csle_cluster-0.6.3/tests/test_cluster_manager.py
```

### Comparing `csle_cluster-0.6.2/PKG-INFO` & `csle_cluster-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.6.2
+Version: 0.6.3
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.6.2/README.md` & `csle_cluster-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/pyproject.toml` & `csle_cluster-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/setup.cfg` & `csle_cluster-0.6.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.57.0
 	grpcio-tools>=1.57.0
-	csle-base>=0.6.2
-	csle-collector>=0.6.2
-	csle-common>=0.6.2
-	csle-ryu>=0.6.2
-	gym-csle-stopping-game>=0.6.2
-	gym-csle-intrusion-response-game>=0.6.2
-	gym-csle-apt-game>=0.6.2
-	gym-csle-cyborg>=0.6.2
-	csle-tolerance>=0.6.2
+	csle-base>=0.6.3
+	csle-collector>=0.6.3
+	csle-common>=0.6.3
+	csle-ryu>=0.6.3
+	gym-csle-stopping-game>=0.6.3
+	gym-csle-intrusion-response-game>=0.6.3
+	gym-csle-apt-game>=0.6.3
+	gym-csle-cyborg>=0.6.3
+	csle-tolerance>=0.6.3
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.6.3/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.6.3/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.6.3/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.6.2
+Version: 0.6.3
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.6.2/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.6.3/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.6.2/tests/test_cluster_manager.py` & `csle_cluster-0.6.3/tests/test_cluster_manager.py`

 * *Files identical despite different names*

