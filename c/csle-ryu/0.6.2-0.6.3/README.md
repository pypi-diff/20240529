# Comparing `tmp/csle_ryu-0.6.2.tar.gz` & `tmp/csle_ryu-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.6.2.tar", last modified: Tue May 28 16:30:07 2024, max compression
+gzip compressed data, was "csle_ryu-0.6.3.tar", last modified: Wed May 29 08:58:01 2024, max compression
```

## Comparing `csle_ryu-0.6.2.tar` & `csle_ryu-0.6.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.577243 csle_ryu-0.6.2/
--rw-r--r--   0 kim        (501) staff       (20)      629 2024-05-28 16:30:07.577287 csle_ryu-0.6.2/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     3869 2024-02-13 12:24:16.000000 csle_ryu-0.6.2/README.md
--rw-r--r--   0 kim        (501) staff       (20)      669 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1798 2024-05-28 16:30:07.577653 csle_ryu-0.6.2/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.572923 csle_ryu-0.6.2/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.574036 csle_ryu-0.6.2/src/csle_ryu/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_ryu-0.6.2/src/csle_ryu/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.575015 csle_ryu-0.6.2/src/csle_ryu/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2484 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.575618 csle_ryu-0.6.2/src/csle_ryu/controllers/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/controllers/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     8327 2023-09-20 12:38:03.000000 csle_ryu-0.6.2/src/csle_ryu/controllers/learning_switch_controller.py
--rw-r--r--   0 kim        (501) staff       (20)    11778 2023-09-20 12:38:03.000000 csle_ryu-0.6.2/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.576654 csle_ryu-0.6.2/src/csle_ryu/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     4127 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/agg_flow_statistic.py
--rw-r--r--   0 kim        (501) staff       (20)     8185 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/avg_flow_statistic.py
--rw-r--r--   0 kim        (501) staff       (20)    14674 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/avg_port_statistic.py
--rw-r--r--   0 kim        (501) staff       (20)     6529 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/flow_statistic.py
--rw-r--r--   0 kim        (501) staff       (20)    10151 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/port_statistic.py
--rw-r--r--   0 kim        (501) staff       (20)      253 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/dao/ryu_controller_type.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.576873 csle_ryu-0.6.2/src/csle_ryu/monitor/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.2/src/csle_ryu/monitor/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    15114 2023-09-20 12:38:03.000000 csle_ryu-0.6.2/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.574841 csle_ryu-0.6.2/src/csle_ryu.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      629 2024-05-28 16:30:07.000000 csle_ryu-0.6.2/src/csle_ryu.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      914 2024-05-28 16:30:07.000000 csle_ryu-0.6.2/src/csle_ryu.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:07.000000 csle_ryu-0.6.2/src/csle_ryu.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:24.000000 csle_ryu-0.6.2/src/csle_ryu.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      565 2024-05-28 16:30:07.000000 csle_ryu-0.6.2/src/csle_ryu.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)        9 2024-05-28 16:30:07.000000 csle_ryu-0.6.2/src/csle_ryu.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:07.577006 csle_ryu-0.6.2/tests/
--rw-r--r--   0 kim        (501) staff       (20)      716 2023-08-17 14:41:40.000000 csle_ryu-0.6.2/tests/test_learning_switch_controller.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.235003 csle_ryu-0.6.3/
+-rw-r--r--   0 kim        (501) staff       (20)      629 2024-05-29 08:58:01.235068 csle_ryu-0.6.3/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3869 2024-02-13 12:24:16.000000 csle_ryu-0.6.3/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      669 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1798 2024-05-29 08:58:01.235304 csle_ryu-0.6.3/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.230804 csle_ryu-0.6.3/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.231811 csle_ryu-0.6.3/src/csle_ryu/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-29 08:57:56.000000 csle_ryu-0.6.3/src/csle_ryu/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.232750 csle_ryu-0.6.3/src/csle_ryu/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2484 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.233230 csle_ryu-0.6.3/src/csle_ryu/controllers/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/controllers/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     8327 2023-09-20 12:38:03.000000 csle_ryu-0.6.3/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-r--r--   0 kim        (501) staff       (20)    11778 2023-09-20 12:38:03.000000 csle_ryu-0.6.3/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.234328 csle_ryu-0.6.3/src/csle_ryu/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     4127 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)     8185 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)    14674 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/avg_port_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)     6529 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/flow_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)    10151 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/port_statistic.py
+-rw-r--r--   0 kim        (501) staff       (20)      253 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/dao/ryu_controller_type.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.234544 csle_ryu-0.6.3/src/csle_ryu/monitor/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_ryu-0.6.3/src/csle_ryu/monitor/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    15114 2023-09-20 12:38:03.000000 csle_ryu-0.6.3/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.232570 csle_ryu-0.6.3/src/csle_ryu.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      629 2024-05-29 08:58:01.000000 csle_ryu-0.6.3/src/csle_ryu.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      914 2024-05-29 08:58:01.000000 csle_ryu-0.6.3/src/csle_ryu.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-29 08:58:01.000000 csle_ryu-0.6.3/src/csle_ryu.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:24.000000 csle_ryu-0.6.3/src/csle_ryu.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      565 2024-05-29 08:58:01.000000 csle_ryu-0.6.3/src/csle_ryu.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)        9 2024-05-29 08:58:01.000000 csle_ryu-0.6.3/src/csle_ryu.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-29 08:58:01.234685 csle_ryu-0.6.3/tests/
+-rw-r--r--   0 kim        (501) staff       (20)      716 2023-08-17 14:41:40.000000 csle_ryu-0.6.3/tests/test_learning_switch_controller.py
```

### Comparing `csle_ryu-0.6.2/PKG-INFO` & `csle_ryu-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.6.2
+Version: 0.6.3
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.6.2/README.md` & `csle_ryu-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/pyproject.toml` & `csle_ryu-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/setup.cfg` & `csle_ryu-0.6.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.6.2
-	csle-collector>=0.6.2
+	csle-base>=0.6.3
+	csle-collector>=0.6.3
 	csle-ryu-fork>=4.37.0.dev3357
 	dnspython==2.2.1
 	eventlet>=0.33.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
```

### Comparing `csle_ryu-0.6.2/src/csle_ryu/constants/constants.py` & `csle_ryu-0.6.3/src/csle_ryu/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.6.3/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.6.3/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.6.3/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.6.3/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.6.3/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.6.3/src/csle_ryu/dao/flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.6.3/src/csle_ryu/dao/port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.6.3/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.6.3/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.6.2
+Version: 0.6.3
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.6.2/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.6.3/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.6.2/src/csle_ryu.egg-info/requires.txt` & `csle_ryu-0.6.3/src/csle_ryu.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-csle-base>=0.6.2
-csle-collector>=0.6.2
+csle-base>=0.6.3
+csle-collector>=0.6.3
 csle-ryu-fork>=4.37.0.dev3357
 dnspython==2.2.1
 eventlet>=0.33.2
 confluent-kafka>=1.9.2
 
 [testing]
 pytest>=6.0
```

### Comparing `csle_ryu-0.6.2/tests/test_learning_switch_controller.py` & `csle_ryu-0.6.3/tests/test_learning_switch_controller.py`

 * *Files identical despite different names*

