# Comparing `tmp/csle_tolerance-0.6.1.tar.gz` & `tmp/csle_tolerance-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_tolerance-0.6.1.tar", last modified: Thu May 23 18:35:48 2024, max compression
+gzip compressed data, was "csle_tolerance-0.6.2.tar", last modified: Tue May 28 16:30:57 2024, max compression
```

## Comparing `csle_tolerance-0.6.1.tar` & `csle_tolerance-0.6.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.368389 csle_tolerance-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      741 2024-05-23 18:35:48.368433 csle_tolerance-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      674 2023-09-06 08:43:30.000000 csle_tolerance-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1929 2024-05-23 18:35:48.368683 csle_tolerance-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_tolerance-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.364241 csle_tolerance-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.364982 csle_tolerance-0.6.1/src/csle_tolerance/
--rw-r--r--   0 kim        (501) staff       (20)       39 2023-09-15 16:43:44.000000 csle_tolerance-0.6.1/src/csle_tolerance/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_tolerance-0.6.1/src/csle_tolerance/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.365950 csle_tolerance-0.6.1/src/csle_tolerance/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_tolerance-0.6.1/src/csle_tolerance/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      315 2023-10-09 07:12:58.000000 csle_tolerance-0.6.1/src/csle_tolerance/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.366331 csle_tolerance-0.6.1/src/csle_tolerance/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:45:28.000000 csle_tolerance-0.6.1/src/csle_tolerance/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     5364 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/src/csle_tolerance/dao/intrusion_recovery_game_config.py
--rw-r--r--   0 kim        (501) staff       (20)     5751 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     5231 2023-09-15 15:32:19.000000 csle_tolerance-0.6.1/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.366618 csle_tolerance-0.6.1/src/csle_tolerance/envs/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:44:05.000000 csle_tolerance-0.6.1/src/csle_tolerance/envs/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    11235 2024-05-15 11:12:28.000000 csle_tolerance-0.6.1/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
--rw-r--r--   0 kim        (501) staff       (20)     8025 2024-02-13 12:24:16.000000 csle_tolerance-0.6.1/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.367133 csle_tolerance-0.6.1/src/csle_tolerance/util/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-08 12:46:59.000000 csle_tolerance-0.6.1/src/csle_tolerance/util/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2693 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/src/csle_tolerance/util/general_util.py
--rw-r--r--   0 kim        (501) staff       (20)    21542 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
--rw-r--r--   0 kim        (501) staff       (20)     5612 2024-05-23 15:58:41.000000 csle_tolerance-0.6.1/src/csle_tolerance/util/intrusion_response_cmdp_util.py
--rw-r--r--   0 kim        (501) staff       (20)     2058 2023-10-09 07:12:58.000000 csle_tolerance-0.6.1/src/csle_tolerance/util/pomdp_solve_parser.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.365730 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      741 2024-05-23 18:35:48.000000 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     1389 2024-05-23 18:35:48.000000 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:48.000000 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-09-14 11:59:31.000000 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      571 2024-05-23 18:35:48.000000 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       15 2024-05-23 18:35:48.000000 csle_tolerance-0.6.1/src/csle_tolerance.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:48.368229 csle_tolerance-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)     1977 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_general_util.py
--rw-r--r--   0 kim        (501) staff       (20)     8827 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_recovery_game_config.py
--rw-r--r--   0 kim        (501) staff       (20)     9323 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_recovery_pomdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)    10854 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_recovery_pomdp_env.py
--rw-r--r--   0 kim        (501) staff       (20)     9259 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_recovery_pomdp_util.py
--rw-r--r--   0 kim        (501) staff       (20)     9291 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_response_cmdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     4276 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_response_cmdp_util.py
--rw-r--r--   0 kim        (501) staff       (20)     9753 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_intrusion_response_pomdp_env.py
--rw-r--r--   0 kim        (501) staff       (20)     1962 2024-05-17 08:02:11.000000 csle_tolerance-0.6.1/tests/test_pomdp_solve_parser.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.017555 csle_tolerance-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      741 2024-05-28 16:30:57.017610 csle_tolerance-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      674 2023-09-06 08:43:30.000000 csle_tolerance-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1929 2024-05-28 16:30:57.017881 csle_tolerance-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_tolerance-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.011132 csle_tolerance-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.011900 csle_tolerance-0.6.2/src/csle_tolerance/
+-rw-r--r--   0 kim        (501) staff       (20)       39 2023-09-15 16:43:44.000000 csle_tolerance-0.6.2/src/csle_tolerance/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_tolerance-0.6.2/src/csle_tolerance/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.013189 csle_tolerance-0.6.2/src/csle_tolerance/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_tolerance-0.6.2/src/csle_tolerance/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      315 2023-10-09 07:12:58.000000 csle_tolerance-0.6.2/src/csle_tolerance/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.014304 csle_tolerance-0.6.2/src/csle_tolerance/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:45:28.000000 csle_tolerance-0.6.2/src/csle_tolerance/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     5364 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/src/csle_tolerance/dao/intrusion_recovery_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     5751 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     5231 2023-09-15 15:32:19.000000 csle_tolerance-0.6.2/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.015123 csle_tolerance-0.6.2/src/csle_tolerance/envs/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:44:05.000000 csle_tolerance-0.6.2/src/csle_tolerance/envs/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    11235 2024-05-15 11:12:28.000000 csle_tolerance-0.6.2/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
+-rw-r--r--   0 kim        (501) staff       (20)     8025 2024-02-13 12:24:16.000000 csle_tolerance-0.6.2/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.016002 csle_tolerance-0.6.2/src/csle_tolerance/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-08 12:46:59.000000 csle_tolerance-0.6.2/src/csle_tolerance/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2693 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/src/csle_tolerance/util/general_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    21541 2024-05-28 15:33:17.000000 csle_tolerance-0.6.2/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     5612 2024-05-23 15:58:41.000000 csle_tolerance-0.6.2/src/csle_tolerance/util/intrusion_response_cmdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     2058 2023-10-09 07:12:58.000000 csle_tolerance-0.6.2/src/csle_tolerance/util/pomdp_solve_parser.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.012941 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      741 2024-05-28 16:30:57.000000 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1389 2024-05-28 16:30:57.000000 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:57.000000 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-09-14 11:59:31.000000 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      571 2024-05-28 16:30:57.000000 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       15 2024-05-28 16:30:57.000000 csle_tolerance-0.6.2/src/csle_tolerance.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:57.017420 csle_tolerance-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     1977 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/tests/test_general_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     8797 2024-05-28 15:33:17.000000 csle_tolerance-0.6.2/tests/test_intrusion_recovery_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     9297 2024-05-28 15:36:17.000000 csle_tolerance-0.6.2/tests/test_intrusion_recovery_pomdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)    10895 2024-05-28 15:33:17.000000 csle_tolerance-0.6.2/tests/test_intrusion_recovery_pomdp_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    17000 2024-05-28 15:45:29.000000 csle_tolerance-0.6.2/tests/test_intrusion_recovery_pomdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     9291 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/tests/test_intrusion_response_cmdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     4272 2024-05-28 15:33:17.000000 csle_tolerance-0.6.2/tests/test_intrusion_response_cmdp_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     9753 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/tests/test_intrusion_response_pomdp_env.py
+-rw-r--r--   0 kim        (501) staff       (20)     1962 2024-05-17 08:02:11.000000 csle_tolerance-0.6.2/tests/test_pomdp_solve_parser.py
```

### Comparing `csle_tolerance-0.6.1/PKG-INFO` & `csle_tolerance-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_tolerance
-Version: 0.6.1
+Version: 0.6.2
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.6.1/pyproject.toml` & `csle_tolerance-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/setup.cfg` & `csle_tolerance-0.6.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
 	numpy>=1.23.5
-	csle-base>=0.6.1
-	csle-common>=0.6.1
-	csle-attacker>=0.6.1
-	csle-defender>=0.6.1
-	csle-collector>=0.6.1
+	csle-base>=0.6.2
+	csle-common>=0.6.2
+	csle-attacker>=0.6.2
+	csle-defender>=0.6.2
+	csle-collector>=0.6.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/dao/intrusion_recovery_game_config.py` & `csle_tolerance-0.6.2/src/csle_tolerance/dao/intrusion_recovery_game_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py` & `csle_tolerance-0.6.2/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/dao/intrusion_response_cmdp_config.py` & `csle_tolerance-0.6.2/src/csle_tolerance/dao/intrusion_response_cmdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py` & `csle_tolerance-0.6.2/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/envs/intrusion_response_cmdp_env.py` & `csle_tolerance-0.6.2/src/csle_tolerance/envs/intrusion_response_cmdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/util/general_util.py` & `csle_tolerance-0.6.2/src/csle_tolerance/util/general_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py` & `csle_tolerance-0.6.2/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,14 @@
                         for i, _ in enumerate(game_config.observations):
                             tr_prob = game_config.transition_tensor[a1][a2][s][s_prime]
                             obs_prob = game_config.observation_tensor[a2][i]
                             prob = tr_prob * obs_prob
                             if prob > 0:
                                 transition = f"{s} {a1} {a2} {i} {s_prime} {prob}"
                                 transitions.append(transition)
-
         return transitions
 
     @staticmethod
     def generate_rewards(game_config: IntrusionRecoveryGameConfig) -> List[str]:
         """
         Generates the reward rows of the POSG config file of HSVI
```

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/util/intrusion_response_cmdp_util.py` & `csle_tolerance-0.6.2/src/csle_tolerance/util/intrusion_response_cmdp_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance/util/pomdp_solve_parser.py` & `csle_tolerance-0.6.2/src/csle_tolerance/util/pomdp_solve_parser.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance.egg-info/PKG-INFO` & `csle_tolerance-0.6.2/src/csle_tolerance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-tolerance
-Version: 0.6.1
+Version: 0.6.2
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance.egg-info/SOURCES.txt` & `csle_tolerance-0.6.2/src/csle_tolerance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/src/csle_tolerance.egg-info/requires.txt` & `csle_tolerance-0.6.2/src/csle_tolerance.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 gymnasium>=0.27.1
 numpy>=1.23.5
-csle-base>=0.6.1
-csle-common>=0.6.1
-csle-attacker>=0.6.1
-csle-defender>=0.6.1
-csle-collector>=0.6.1
+csle-base>=0.6.2
+csle-common>=0.6.2
+csle-attacker>=0.6.2
+csle-defender>=0.6.2
+csle-collector>=0.6.2
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

### Comparing `csle_tolerance-0.6.1/tests/test_general_util.py` & `csle_tolerance-0.6.2/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/tests/test_intrusion_recovery_game_config.py` & `csle_tolerance-0.6.2/tests/test_intrusion_recovery_game_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from csle_tolerance.dao.intrusion_recovery_game_config import (
     IntrusionRecoveryGameConfig,
 )
 from csle_tolerance.util.intrusion_recovery_pomdp_util import IntrusionRecoveryPomdpUtil
 import pytest_mock
-import numpy as np
 
 
 class TestIntrusionRecoveryGameConfigSuite:
     """
     Test suite for intrusion_recovery_game_config.py
     """
 
@@ -24,15 +23,15 @@
             seed=123,
             discount_factor=0.9,
             states=[0, 1, 2],
             actions=[0, 1],
             observations=[0, 1],
             cost_tensor=[[1, 2], [3, 4]],
             observation_tensor=[[1, 2], [3, 4]],
-            transition_tensor=[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]],
+            transition_tensor=[[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]],
             b1=[0.1, 0.9],
             T=100,
             simulation_env_name="sim_env",
             gym_env_name="gym_env",
             max_horizon=1000,
         )
         assert dto.eta == 0.5
@@ -44,16 +43,15 @@
         assert dto.discount_factor == 0.9
         assert dto.states == [0, 1, 2]
         assert dto.actions == [0, 1]
         assert dto.observations == [0, 1]
         assert dto.cost_tensor == [[1, 2], [3, 4]]
         assert dto.observation_tensor == [[1, 2], [3, 4]]
         assert dto.transition_tensor == [
-            [[0.1, 0.2], [0.3, 0.4]],
-            [[0.5, 0.6], [0.7, 0.8]],
+            [[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]
         ]
         assert dto.b1 == [0.1, 0.9]
         assert dto.T == 100
         assert dto.simulation_env_name == "sim_env"
         assert dto.gym_env_name == "gym_env"
         assert dto.max_horizon == 1000
 
@@ -70,26 +68,26 @@
             seed=123,
             discount_factor=0.9,
             states=[0, 1, 2],
             actions=[0, 1],
             observations=[0, 1],
             cost_tensor=[[1, 2], [3, 4]],
             observation_tensor=[[1, 2], [3, 4]],
-            transition_tensor=[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]],
+            transition_tensor=[[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]],
             b1=[0.1, 0.9],
             T=100,
             simulation_env_name="sim_env",
             gym_env_name="gym_env",
             max_horizon=1000,
         )
         expected = (
             "eta: 0.5, p_a: 0.8, p_c_1: 0.1, BTR: 10, negate_costs: True, seed: 123, "
             "discount_factor: 0.9, states: [0, 1, 2], actions: [0, 1], observations: [[1, 2], [3, 4]], "
             "cost_tensor: [[1, 2], [3, 4]], observation_tensor: [[1, 2], [3, 4]], "
-            "transition_tensor: [[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]], b1:[0.1, 0.9], "
+            "transition_tensor: [[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]], b1:[0.1, 0.9], "
             "T: 100, simulation_env_name: sim_env, gym_env_name: gym_env, max_horizon: 1000"
         )
         assert dto.__str__() == expected
 
     def test_from_dict(self) -> None:
         """
         Tests the function of converting a dict representation to an instance
@@ -103,15 +101,15 @@
             "seed": 123,
             "discount_factor": 0.9,
             "states": [0, 1, 2],
             "actions": [0, 1],
             "observations": [0, 1],
             "cost_tensor": [[1, 2], [3, 4]],
             "observation_tensor": [[1, 2], [3, 4]],
-            "transition_tensor": [[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]],
+            "transition_tensor": [[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]],
             "b1": [0.1, 0.9],
             "T": 100,
             "simulation_env_name": "sim_env",
             "gym_env_name": "gym_env",
         }
         dto = IntrusionRecoveryGameConfig.from_dict(dto_dict)
         assert dto.eta == 0.5
@@ -123,16 +121,15 @@
         assert dto.discount_factor == 0.9
         assert dto.states == [0, 1, 2]
         assert dto.actions == [0, 1]
         assert dto.observations == [0, 1]
         assert dto.cost_tensor == [[1, 2], [3, 4]]
         assert dto.observation_tensor == [[1, 2], [3, 4]]
         assert dto.transition_tensor == [
-            [[0.1, 0.2], [0.3, 0.4]],
-            [[0.5, 0.6], [0.7, 0.8]],
+            [[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]
         ]
         assert dto.b1 == [0.1, 0.9]
         assert dto.T == 100
         assert dto.simulation_env_name == "sim_env"
         assert dto.gym_env_name == "gym_env"
 
     def test_to_dict(self) -> None:
@@ -148,15 +145,15 @@
             seed=123,
             discount_factor=0.9,
             states=[0, 1, 2],
             actions=[0, 1],
             observations=[0, 1],
             cost_tensor=[[1, 2], [3, 4]],
             observation_tensor=[[1, 2], [3, 4]],
-            transition_tensor=[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]],
+            transition_tensor=[[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]],
             b1=[0.1, 0.9],
             T=100,
             simulation_env_name="sim_env",
             gym_env_name="gym_env",
         )
         expected = {
             "eta": 0.5,
@@ -167,30 +164,30 @@
             "seed": 123,
             "discount_factor": 0.9,
             "states": [0, 1, 2],
             "actions": [0, 1],
             "observations": [0, 1],
             "cost_tensor": [[1, 2], [3, 4]],
             "observation_tensor": [[1, 2], [3, 4]],
-            "transition_tensor": [[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]],
+            "transition_tensor": [[[[0.1, 0.2], [0.3, 0.4]], [[0.5, 0.6], [0.7, 0.8]]]],
             "b1": [0.1, 0.9],
             "T": 100,
             "simulation_env_name": "sim_env",
             "gym_env_name": "gym_env",
         }
         assert dto.to_dict() == expected
 
     def test_from_json_file(self, mocker: pytest_mock.MockFixture) -> None:
         """
         tests the function of reading a json file and converting it to a DTO
         """
         eta = 2
         p_a = 0.05
         p_c_1 = 0.01
-        BTR = np.inf
+        BTR = 100
         negate_costs = False
         discount_factor = 1 - p_c_1
         num_observations = 100
         simulation_name = "csle-tolerance-intrusion-recovery-pomdp-defender-001"
         cost_tensor = IntrusionRecoveryPomdpUtil.cost_tensor(
             eta=eta,
             states=IntrusionRecoveryPomdpUtil.state_space(),
@@ -210,35 +207,35 @@
             p_a=p_a,
             p_c_1=p_c_1,
         )
         config = IntrusionRecoveryGameConfig(
             eta=eta,
             p_a=p_a,
             p_c_1=p_c_1,
-            BTR=BTR,
+            BTR=100,
             negate_costs=negate_costs,
             seed=999,
             discount_factor=discount_factor,
             states=IntrusionRecoveryPomdpUtil.state_space(),
             actions=IntrusionRecoveryPomdpUtil.action_space(),
             observations=IntrusionRecoveryPomdpUtil.observation_space(
                 num_observations=num_observations
             ),
             cost_tensor=cost_tensor,
             observation_tensor=observation_tensor,
             transition_tensor=transition_tensor,
             b1=IntrusionRecoveryPomdpUtil.initial_belief(p_a=p_a),
-            T=BTR,
+            T=int(BTR),
             simulation_env_name=simulation_name,
             gym_env_name="csle-tolerance-intrusion-recovery-pomdp-v1",
         )
         mocker.patch(
             "io.open", side_effect=mocker.mock_open(read_data=config.to_json_str())
         )
         dto = IntrusionRecoveryGameConfig.from_json_file("path")
         assert dto.eta == 2
         assert dto.p_a == 0.05
         assert dto.p_c_1 == 0.01
-        assert dto.BTR == np.inf
+        assert dto.BTR == 100
         assert dto.negate_costs is False
         assert dto.seed == 999
         assert dto.discount_factor == 1 - p_c_1
```

### Comparing `csle_tolerance-0.6.1/tests/test_intrusion_recovery_pomdp_config.py` & `csle_tolerance-0.6.2/tests/test_intrusion_recovery_pomdp_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from csle_tolerance.dao.intrusion_recovery_pomdp_config import (
     IntrusionRecoveryPomdpConfig,
 )
 from csle_tolerance.util.intrusion_recovery_pomdp_util import IntrusionRecoveryPomdpUtil
 import pytest_mock
-import numpy as np
 
 
 class TestIntrusionRecoveryPomdpConfigSuite:
     """
     Test suite for intrusion_recovery_pomdp_config.py
     """
 
@@ -198,15 +197,15 @@
         tests the function of reading a json file and converting it to a DTO
         """
         eta = 2
         p_a = 0.05
         p_c_1 = 0.01
         p_c_2 = 0.01
         p_u = 0.0
-        BTR = np.inf
+        BTR = 10
         negate_costs = False
         discount_factor = 1 - p_c_1
         num_observations = 100
         simulation_name = "csle-tolerance-intrusion-recovery-pomdp-defender-001"
         cost_tensor = IntrusionRecoveryPomdpUtil.cost_tensor(
             eta=eta,
             states=IntrusionRecoveryPomdpUtil.state_space(),
@@ -255,11 +254,11 @@
         )
         dto = IntrusionRecoveryPomdpConfig.from_json_file("path")
         assert dto.eta == 2
         assert dto.p_a == 0.05
         assert dto.p_c_1 == 0.01
         assert dto.p_c_2 == 0.01
         assert dto.p_u == 0.0
-        assert dto.BTR == np.inf
+        assert dto.BTR == BTR
         assert dto.negate_costs is False
         assert dto.seed == 999
         assert dto.discount_factor == 1 - p_c_1
```

### Comparing `csle_tolerance-0.6.1/tests/test_intrusion_recovery_pomdp_env.py` & `csle_tolerance-0.6.2/tests/test_intrusion_recovery_pomdp_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from csle_tolerance.dao.intrusion_recovery_pomdp_config import (
     IntrusionRecoveryPomdpConfig,
 )
 import csle_tolerance.constants.constants as env_constants
 import csle_common.constants.constants as constants
 import numpy as np
 import pytest
+from typing import Dict, Any
 
 
 class TestInstrusionRecoveryPomdpEnvSuite:
     """
     Test suite for intrusion_recovery_pomdp_env.py
     """
 
@@ -149,15 +150,15 @@
             transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
             b1=[1, 0],
             T=3,
             simulation_env_name="env",
             gym_env_name="gym",
             max_horizon=np.inf,
         )
-        info = {}
+        info: Dict[str, Any] = {}
         with pytest.raises(IndexError):
             assert IntrusionRecoveryPomdpEnv(config)._info(info) is not None
 
     def test_render(self) -> None:
         """
         Tests the function of rendering the environment.
 
@@ -243,15 +244,15 @@
             transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
             b1=[1, 0],
             T=3,
             simulation_env_name="env",
             gym_env_name="gym",
             max_horizon=np.inf,
         )
-        assert IntrusionRecoveryPomdpEnv(config).reset_traces() is None
+        assert not IntrusionRecoveryPomdpEnv(config).reset_traces()
 
     @patch("time.time")  # Mock the time.time function
     @patch(
         "csle_common.dao.simulation_config.simulation_trace.SimulationTrace.save_traces"
     )  # Mock the method
     def test_checkpoint_traces(self, mock_save_traces, mock_time) -> None:
         """
```

### Comparing `csle_tolerance-0.6.1/tests/test_intrusion_recovery_pomdp_util.py` & `csle_tolerance-0.6.2/tests/test_intrusion_response_pomdp_env.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,313 +1,326 @@
-from csle_tolerance.util.intrusion_recovery_pomdp_util import IntrusionRecoveryPomdpUtil
-from csle_tolerance.dao.intrusion_recovery_pomdp_config import (
-    IntrusionRecoveryPomdpConfig,
+from csle_tolerance.dao.intrusion_response_cmdp_config import (
+    IntrusionResponseCmdpConfig,
 )
-import numpy as np
+from csle_tolerance.envs.intrusion_response_cmdp_env import IntrusionResponseCmdpEnv
+from unittest.mock import patch, Mock
+import csle_tolerance.constants.constants as env_constants
+import csle_common.constants.constants as constants
 import pytest
 
 
-class TestIntrusionTolerancePomdpSuite:
+class TestInstrusionResponseCmdpEnvSuite:
     """
-    Test suite for intrusion_recovery_pomdp_util.py
+    Test suite for intrusion_response_pomdp_env.py
     """
 
-    def test__state_space(self) -> None:
+    def test__init__(self) -> None:
         """
-        Tests the state space of the POMDP
+        Tests the function of initializing the environment
 
         :return: None
         """
-        assert (
-            isinstance(item, int) for item in IntrusionRecoveryPomdpUtil.state_space()
-        )
-        assert IntrusionRecoveryPomdpUtil.state_space() is not None
-        assert IntrusionRecoveryPomdpUtil.state_space() == [0, 1, 2]
-
-    def test_initial_belief(self) -> None:
-        """
-        Tests the initial_belief function
-
-        :return: None
-        """
-        assert sum(IntrusionRecoveryPomdpUtil.initial_belief(p_a=0.5)) == 1
-
-    def test_action_space(self) -> None:
-        """
-        Tests the action space of the POMDP
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        assert IntrusionResponseCmdpEnv(env).t == 1
+        assert IntrusionResponseCmdpEnv(env).s == env.initial_state
+        assert IntrusionResponseCmdpEnv(env).traces == []
+
+    def test_step(self) -> None:
+        """
+        Tests the step function (Takes a step in the environment
+        by executing the given action)
 
         :return: None
         """
-        assert (
-            isinstance(item, int) for item in IntrusionRecoveryPomdpUtil.action_space()
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
         )
-        assert IntrusionRecoveryPomdpUtil.action_space() is not None
-        assert IntrusionRecoveryPomdpUtil.action_space() == [0, 1]
-
-    def test_observation_space(self) -> None:
-        """
-        Tests the observation space of the POMDP
-
-        :return: None
-        """
-        num_observation = 3
-        expected = [0, 1, 2]
-        assert IntrusionRecoveryPomdpUtil.observation_space(num_observation) == expected
-
-    def test_cost_function(self) -> None:
-        """
-        Tests the cost function of the POMDP
-
-        :return: None
-        """
-        s = 1
         a = 0
-        eta = 0.5
-        negate = False
-        assert IntrusionRecoveryPomdpUtil.cost_function(s, a, eta, negate) == 0.5
-
-    def test_cost_tensor(self) -> None:
-        """
-        Tests the function of creating a tensor with the costs of the POMDP
-
-        :return: None
-        """
-        eta = 0.5
-        states = [0, 1]
-        actions = [0]
-        negate = False
-        expected = [[0, 0.5]]
+        c = 0.1
+        assert IntrusionResponseCmdpEnv(env).step(a)[1] == c
+        assert not IntrusionResponseCmdpEnv(env).step(a)[2]
         assert (
-            IntrusionRecoveryPomdpUtil.cost_tensor(eta, states, actions, negate)
-            == expected
-        )
-
-    def test_observation_function(self) -> None:
-        """
-        Tests the observation function of the POMDP
-
-        :return: None
-        """
-        s = 1
-        o = 1
-        num_observations = 2
-        assert round(
-            IntrusionRecoveryPomdpUtil.observation_function(s, o, num_observations), 1
+            IntrusionResponseCmdpEnv(env).step(a)[4][
+                env_constants.ENV_METRICS.TIME_STEP
+            ]
+            == 2
         )
-
-    def test_observation_tensor(self) -> None:
-        """
-        Tests the function of creating a tensor with observation probabilities
-
-        :return: None
-        """
-        states = [0, 1]
-        observations = [0, 1]
-        expected = [[0.8, 0.2], [0.4, 0.6]]
-        obs_tensor = IntrusionRecoveryPomdpUtil.observation_tensor(states, observations)
-        for i in range(len(obs_tensor)):
-            for j in range(len(obs_tensor[i])):
-                obs_tensor[i][j] = round(obs_tensor[i][j], 1)
-            assert sum(obs_tensor[i]) == 1
-        assert obs_tensor == expected
-
-    def test_transition_function(self) -> None:
-        """
-        Tests the transition function of the POMDP
-
-        :return: None
-        """
-        s = 0
-        s_prime = 1
-        a = 0
-        p_a = 0.2
-        p_c_1 = 0.1
-        p_c_2 = 0.2
-        p_u = 0.5
         assert (
-            round(
-                IntrusionRecoveryPomdpUtil.transition_function(
-                    s, s_prime, a, p_a, p_c_1, p_c_2, p_u
-                ),
-                1,
-            )
-            == 0.2
-        )
-
-    def test_transition_tensor(self) -> None:
-        """
-        Tests the function of creating  a tensor with the transition probabilities of the POMDP
-
-        :return: None
-        """
-        states = [0, 1, 2]
-        actions = [0]
-        p_a = 0.2
-        p_c_1 = 0.1
-        p_c_2 = 0.2
-        p_u = 0.5
-        expected = [[[0.7, 0.2, 0.1], [0.4, 0.4, 0.2], [0, 0, 1.0]]]
-        transition_tensor = IntrusionRecoveryPomdpUtil.transition_tensor(
-            states, actions, p_a, p_c_1, p_c_2, p_u
-        )
-        for i in range(len(transition_tensor)):
-            for j in range(len(transition_tensor[i])):
-                for k in range(len(transition_tensor[i][j])):
-                    transition_tensor[i][j][k] = round(transition_tensor[i][j][k], 1)
-        assert transition_tensor == expected
-        states = [0, 1]
-        with pytest.raises(AssertionError):
-            transition_tensor = IntrusionRecoveryPomdpUtil.transition_tensor(
-                states, actions, p_a, p_c_1, p_c_2, p_u
-            )
-
-    def test_sample_initial_state(self) -> None:
-        """
-        Tests the function of sampling the initial state
-
-        :return: None
-        """
-        b1 = [0.2, 0.8]
-        assert isinstance(IntrusionRecoveryPomdpUtil.sample_initial_state(b1), int)
-        assert IntrusionRecoveryPomdpUtil.sample_initial_state(b1) <= len(b1)
-        assert IntrusionRecoveryPomdpUtil.sample_initial_state(b1) >= 0
-        b1 = [1.0, 0]
-        assert IntrusionRecoveryPomdpUtil.sample_initial_state(b1) == 0
-        b1 = [0.0, 1.0]
-        assert IntrusionRecoveryPomdpUtil.sample_initial_state(b1) == 1
-
-    def test_sampe_next_observation(self) -> None:
-        """
-        Tests the function of sampling the next observation
-
-        :return: None
-        """
-        observation_tensor = [[0.8, 0.2], [0.4, 0.6]]
-        s_prime = 1
-        observations = [0, 1]
-        assert isinstance(
-            IntrusionRecoveryPomdpUtil.sample_next_observation(
-                observation_tensor, s_prime, observations
-            ),
-            int,
-        )
-
-    def test_bayes_filter(self) -> None:
-        """
-        Tests the function of a bayesian filter to computer b[s_prime] of the POMDP
-
-        :return: None
-        """
-        s_prime = 1
-        o = 0
-        a = 0
-        b = [0.2, 0.8]
-        states = [0, 1]
-        observations = [0, 1]
-        observation_tensor = [[0.8, 0.2], [0.4, 0.6]]
-        transition_tensor = [[[0.6, 0.4], [0.1, 0.9]]]
-        b_prime_s_prime = 0.7
-        assert (
-            round(
-                IntrusionRecoveryPomdpUtil.bayes_filter(
-                    s_prime,
-                    o,
-                    a,
-                    b,
-                    states,
-                    observations,
-                    observation_tensor,
-                    transition_tensor,
-                ),
-                1,
-            )
-            == b_prime_s_prime
-        )
-
-    def test_p_o_given_b_a1_a2(self) -> None:
-        """
-        Tests the function of computing P[o|a,b] of the POMDP
-
-        :return: None
-        """
-        o = 0
-        b = [0.2, 0.8]
-        a = 0
-        states = [0, 1]
-        observation_tensor = [[0.8, 0.2], [0.4, 0.6]]
-        transition_tensor = [[[0.6, 0.4], [0.1, 0.9]]]
-        expected = 0.5
-        assert (
-            round(
-                IntrusionRecoveryPomdpUtil.p_o_given_b_a1_a2(
-                    o, b, a, states, transition_tensor, observation_tensor
-                ),
-                1,
-            )
-            == expected
-        )
-
-    def test_next_belief(self) -> None:
-        """
-        Tests the funtion of computing the next belief using a Bayesian filter
-
-        :return: None
-        """
-        o = 0
-        a = 0
-        b = [0.2, 0.8]
-        states = [0, 1]
-        observations = [0, 1]
-        observation_tensor = [[0.8, 0.2], [0.4, 0.6]]
-        transition_tensor = [[[0.3, 0.7], [0.6, 0.4]]]
-        assert (
-            round(
-                sum(
-                    IntrusionRecoveryPomdpUtil.next_belief(
-                        o,
-                        a,
-                        b,
-                        states,
-                        observations,
-                        observation_tensor,
-                        transition_tensor,
-                    )
-                ),
-                1,
-            )
-            == 1
-        )
-
-    def test_pomdp_solver_file(self) -> None:
-        """
-        Tests the function of getting the POMDP environment specification
-
-        :return: None
-        """
-
-        assert (
-            IntrusionRecoveryPomdpUtil.pomdp_solver_file(
-                IntrusionRecoveryPomdpConfig(
-                    eta=0.1,
-                    p_a=0.2,
-                    p_c_1=0.2,
-                    p_c_2=0.3,
-                    p_u=0.3,
-                    BTR=1,
-                    negate_costs=True,
-                    seed=1,
-                    discount_factor=0.5,
-                    states=[0, 1],
-                    actions=[0],
-                    observations=[0, 1],
-                    cost_tensor=[[0.1, 0.5], [0.5, 0.6]],
-                    observation_tensor=[[0.8, 0.2], [0.4, 0.6]],
-                    transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
-                    b1=[0.3, 0.7],
-                    T=3,
-                    simulation_env_name="env",
-                    gym_env_name="gym",
-                    max_horizon=np.inf,
-                )
-            )
-            is not None
-        )
+            IntrusionResponseCmdpEnv(env).step(a)[4][
+                env_constants.ENV_METRICS.DEFENDER_ACTION
+            ]
+            == a
+        )
+
+    def test_reset(self) -> None:
+        """
+        Tests the reset function (Resets the environment state)
+
+        :return: None
+        """
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        assert IntrusionResponseCmdpEnv(env).reset()[0] == 0
+        assert not IntrusionResponseCmdpEnv(env).reset()[1]
+
+    def test_info(self) -> None:
+        """
+        Tests the function of adding the cumulative reward and episode length to the info dict
+
+        :return: None
+        """
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        info = {}
+        assert IntrusionResponseCmdpEnv(env)._info(info) is not None
+
+    def test_render(self) -> None:
+        """
+        Tests the funtion of rendering the environment
+
+        :return: None
+        """
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        with pytest.raises(NotImplementedError):
+            IntrusionResponseCmdpEnv(env).render()
+
+    def test_get_traces(self) -> None:
+        """
+        Tests the function of getting the list of simulation traces
+
+        :return: None
+        """
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        returned_traces = IntrusionResponseCmdpEnv(env).get_traces()
+        assert not returned_traces
+
+    def test_reset_traces(self) -> None:
+        """
+        Tests the function of reseting the list of traces
+
+        :return: None
+        """
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        assert not IntrusionResponseCmdpEnv(env).reset_traces()
+
+    @patch("time.time")  # Mock the time.time function
+    @patch(
+        "csle_common.dao.simulation_config.simulation_trace.SimulationTrace.save_traces"
+    )  # Mock the method
+    def test_checkpoint_traces(self, mock_save_traces, mock_time) -> None:
+        """
+        Tests the function of checkpointing agent traces
+
+        :param mock_save_traces: _description_
+        :type mock_save_traces: _type_
+        :param mock_time: _description_
+        :type mock_time: _type_
+        """
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        mock_time.return_value = 1234567890
+        environment = IntrusionResponseCmdpEnv(env)
+        environment._IntrusionResponseCmdpEnv__checkpoint_traces()
+        mock_save_traces.assert_called_once_with(
+            traces_save_dir=constants.LOGGING.DEFAULT_LOG_DIR,
+            traces=environment.traces,
+            traces_file=f"taus{mock_time.return_value}.json",
+        )
+
+    def test_set_model(self) -> None:
+        """
+        Tests the function of setting the model
+
+        :return: None
+        """
+        mock_model = Mock()
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        environment = IntrusionResponseCmdpEnv(env)
+        environment.set_model(mock_model)
+        assert environment.model == mock_model
+
+    def test_set_state(self) -> None:
+        """
+        Tests the function of setting the state
+
+        :return: None
+        """
+        mock_state = Mock()
+        env = IntrusionResponseCmdpConfig(
+            p_a=0.2,
+            p_c=0.5,
+            p_u=0.3,
+            s_max=2,
+            transition_tensor=[[[0.8, 0.2], [0.6, 0.4]]],
+            cost_tensor=[0.1, 0.5],
+            negate_costs=True,
+            seed=1,
+            states=[0, 1],
+            actions=[0],
+            initial_state=0,
+            constraint_cost_tensor=[0.2, 0.7],
+            f=1,
+            epsilon_a=0.3,
+            simulation_env_name="env",
+            gym_env_name="gym",
+            discount_factor=0.5,
+        )
+        environment = IntrusionResponseCmdpEnv(env)
+        environment.set_state(mock_state)
+        assert environment.s == mock_state
```

### Comparing `csle_tolerance-0.6.1/tests/test_intrusion_response_cmdp_config.py` & `csle_tolerance-0.6.2/tests/test_intrusion_response_cmdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.6.1/tests/test_intrusion_response_cmdp_util.py` & `csle_tolerance-0.6.2/tests/test_intrusion_response_cmdp_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     def test_constraint_cost_function(self) -> None:
         """
         Tests the constraint cost function of the CMDP
 
         :return: None
         """
         states = [1, 2]
-        f = 0.5
-        expected = [0.0, 1.0]
+        f = 5
+        expected = [0.0, 0.0]
         assert (
             IntrusionResponseCmdpUtil.constraint_cost_function(states[0], f)
             == expected[0]
         )
         assert (
             IntrusionResponseCmdpUtil.constraint_cost_function(states[1], f)
             == expected[1]
@@ -71,16 +71,16 @@
     def test_constraint_cost_tensor(self) -> None:
         """
         Tests the function of creating a tensor with the constrained costs of the CMDP
 
         :return: None
         """
         states = [1, 2]
-        f = 0.5
-        expected = [0.0, 1.0]
+        f = 5
+        expected = [0.0, 0.0]
         assert IntrusionResponseCmdpUtil.constraint_cost_tensor(states, f) == expected
 
     def test_delta_function(self) -> None:
         """
         Tests the delta function that gives the probability of the change in the number of the healthy nodes
 
         :return: None
```

### Comparing `csle_tolerance-0.6.1/tests/test_pomdp_solve_parser.py` & `csle_tolerance-0.6.2/tests/test_pomdp_solve_parser.py`

 * *Files identical despite different names*

