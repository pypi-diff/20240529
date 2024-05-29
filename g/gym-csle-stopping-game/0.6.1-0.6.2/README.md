# Comparing `tmp/gym_csle_stopping_game-0.6.1.tar.gz` & `tmp/gym_csle_stopping_game-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.6.1.tar", last modified: Thu May 23 18:35:20 2024, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.6.2.tar", last modified: Tue May 28 16:30:28 2024, max compression
```

## Comparing `gym_csle_stopping_game-0.6.1.tar` & `gym_csle_stopping_game-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.896435 gym_csle_stopping_game-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      705 2024-05-23 18:35:20.896526 gym_csle_stopping_game-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      703 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1894 2024-05-23 18:35:20.897570 gym_csle_stopping_game-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.885109 gym_csle_stopping_game-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.888424 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/
--rw-r--r--   0 kim        (501) staff       (20)      657 2023-09-15 16:41:55.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.891554 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     1030 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.893256 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     3494 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     6640 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-r--r--   0 kim        (501) staff       (20)     3753 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     2828 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.894819 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/
--rw-r--r--   0 kim        (501) staff       (20)       74 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    22753 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-r--r--   0 kim        (501) staff       (20)    10877 2024-03-05 13:14:47.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-r--r--   0 kim        (501) staff       (20)    10580 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.895423 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/util/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/util/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    11363 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.890933 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      705 2024-05-23 18:35:20.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     1195 2024-05-23 18:35:20.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:20.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:00.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      557 2024-05-23 18:35:20.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       23 2024-05-23 18:35:20.000000 gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:20.896130 gym_csle_stopping_game-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)     4825 2024-02-13 12:24:16.000000 gym_csle_stopping_game-0.6.1/tests/test_stopping_game_dao.py
--rw-r--r--   0 kim        (501) staff       (20)     8353 2024-02-13 12:24:16.000000 gym_csle_stopping_game-0.6.1/tests/test_stopping_game_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.583884 gym_csle_stopping_game-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      705 2024-05-28 16:30:28.584004 gym_csle_stopping_game-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      703 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1894 2024-05-28 16:30:28.584498 gym_csle_stopping_game-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.562649 gym_csle_stopping_game-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.565990 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/
+-rw-r--r--   0 kim        (501) staff       (20)      657 2023-09-15 16:41:55.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.572475 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     1030 2023-08-15 10:44:03.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.575462 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     3494 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     6640 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3753 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     2828 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.577943 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/
+-rw-r--r--   0 kim        (501) staff       (20)       74 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    22772 2024-05-28 16:10:23.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    10877 2024-03-05 13:14:47.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    10580 2024-05-04 07:32:27.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.578589 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:04.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    11363 2024-05-28 16:12:37.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.571604 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      705 2024-05-28 16:30:28.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     1319 2024-05-28 16:30:28.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:28.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:00.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      557 2024-05-28 16:30:28.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       23 2024-05-28 16:30:28.000000 gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:28.583539 gym_csle_stopping_game-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     4825 2024-02-13 12:24:16.000000 gym_csle_stopping_game-0.6.2/tests/test_stopping_game_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)    16008 2024-05-28 15:52:44.000000 gym_csle_stopping_game-0.6.2/tests/test_stopping_game_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    11840 2024-05-28 15:49:38.000000 gym_csle_stopping_game-0.6.2/tests/test_stopping_game_mdp_attacker_env.py
+-rw-r--r--   0 kim        (501) staff       (20)    12609 2024-05-28 16:16:15.000000 gym_csle_stopping_game-0.6.2/tests/test_stopping_game_pomdp_defender_env.py
+-rw-r--r--   0 kim        (501) staff       (20)     8353 2024-02-13 12:24:16.000000 gym_csle_stopping_game-0.6.2/tests/test_stopping_game_util.py
```

### Comparing `gym_csle_stopping_game-0.6.1/PKG-INFO` & `gym_csle_stopping_game-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_stopping_game
-Version: 0.6.1
+Version: 0.6.2
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.6.1/pyproject.toml` & `gym_csle_stopping_game-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/setup.cfg` & `gym_csle_stopping_game-0.6.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
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

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
         :param config: the environment configuration
         """
         self.config = config
 
         # Initialize environment state
         self.state = StoppingGameState(b1=self.config.b1, L=self.config.L)
-
         # Setup spaces
         self.attacker_observation_space = self.config.attacker_observation_space()
         self.defender_observation_space = self.config.defender_observation_space()
         self.attacker_action_space = self.config.attacker_action_space()
         self.defender_action_space = self.config.defender_action_space()
 
         self.action_space = self.defender_action_space
@@ -69,27 +68,26 @@
         :return: (obs, reward, terminated, truncated, info)
         """
 
         # Setup initial values
         a1, a2_profile = action_profile
         pi2, a2 = a2_profile
         assert pi2.shape[0] == len(self.config.S)
-        assert pi2.shape[1] == len(self.config.A1)
+        assert pi2.shape[1] == len(self.config.A2)
         done = False
         info: Dict[str, Any] = {}
 
         o = max(self.config.O)
         if self.state.s == 2:
             done = True
             r = 0
         else:
             # Compute r, s', b',o'
             r = self.config.R[self.state.l - 1][a1][a2][self.state.s]
-            self.state.s = StoppingGameUtil.sample_next_state(l=self.state.l, a1=a1, a2=a2,
-                                                              T=self.config.T,
+            self.state.s = StoppingGameUtil.sample_next_state(l=self.state.l, a1=a1, a2=a2, T=self.config.T,
                                                               S=self.config.S, s=self.state.s)
             o = StoppingGameUtil.sample_next_observation(Z=self.config.Z,
                                                          O=self.config.O, s_prime=self.state.s)
             if self.config.compute_beliefs:
                 self.state.b = StoppingGameUtil.next_belief(o=o, a1=a1, b=self.state.b, pi2=pi2,
                                                             config=self.config,
                                                             l=self.state.l, a2=a2)
@@ -433,14 +431,16 @@
         Utility method to get a hidden observation based on a history
 
         :param history: the history to get the observation from
         :param pi2: the attacker stage strategy
         :param l: the number of stops remaining
         :return: the observation
         """
+        if not history:
+            raise ValueError("History must not be empty")
         return [history[-1]]
 
     def generate_random_particles(self, o: int, num_particles: int) -> List[int]:
         """
         Generates a random list of state particles from a given observation
 
         :param o: the latest observation
```

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-stopping-game
-Version: 0.6.1
+Version: 0.6.2
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 src/gym_csle_stopping_game/envs/__init__.py
 src/gym_csle_stopping_game/envs/stopping_game_env.py
 src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
 src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
 src/gym_csle_stopping_game/util/__init__.py
 src/gym_csle_stopping_game/util/stopping_game_util.py
 tests/test_stopping_game_dao.py
+tests/test_stopping_game_env.py
+tests/test_stopping_game_mdp_attacker_env.py
+tests/test_stopping_game_pomdp_defender_env.py
 tests/test_stopping_game_util.py
```

### Comparing `gym_csle_stopping_game-0.6.1/src/gym_csle_stopping_game.egg-info/requires.txt` & `gym_csle_stopping_game-0.6.2/src/gym_csle_stopping_game.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gymnasium>=0.27.1
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

### Comparing `gym_csle_stopping_game-0.6.1/tests/test_stopping_game_dao.py` & `gym_csle_stopping_game-0.6.2/tests/test_stopping_game_dao.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.6.1/tests/test_stopping_game_util.py` & `gym_csle_stopping_game-0.6.2/tests/test_stopping_game_util.py`

 * *Files identical despite different names*

