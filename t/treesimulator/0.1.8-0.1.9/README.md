# Comparing `tmp/treesimulator-0.1.8.tar.gz` & `tmp/treesimulator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treesimulator-0.1.8.tar", last modified: Mon Jan 15 11:10:49 2024, max compression
+gzip compressed data, was "treesimulator-0.1.9.tar", last modified: Mon Jan 15 13:16:30 2024, max compression
```

## Comparing `treesimulator-0.1.8.tar` & `treesimulator-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2024-01-15 11:10:49.757227 treesimulator-0.1.8/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.8/LICENSE
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2024-01-15 11:10:49.757227 treesimulator-0.1.8/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.8/README.md
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2024-01-15 11:10:49.757227 treesimulator-0.1.8/setup.cfg
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2024-01-15 11:06:19.000000 treesimulator-0.1.8/setup.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2024-01-15 11:10:49.757227 treesimulator-0.1.8/treesimulator/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.8/treesimulator/__init__.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17714 2024-01-15 10:58:29.000000 treesimulator-0.1.8/treesimulator/generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10991 2024-01-15 11:06:19.000000 treesimulator-0.1.8/treesimulator/mtbd_models.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.8/treesimulator/sequence_generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5730 2024-01-15 10:57:01.000000 treesimulator-0.1.8/treesimulator/simulate_forest.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.8/treesimulator/simulate_forest_bd.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.8/treesimulator/simulate_forest_bdei.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.8/treesimulator/simulate_forest_bdss.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2024-01-15 11:10:49.757227 treesimulator-0.1.8/treesimulator.egg-info/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2024-01-15 11:10:49.000000 treesimulator-0.1.8/treesimulator.egg-info/PKG-INFO
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      513 2024-01-15 11:10:49.000000 treesimulator-0.1.8/treesimulator.egg-info/SOURCES.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2024-01-15 11:10:49.000000 treesimulator-0.1.8/treesimulator.egg-info/dependency_links.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      233 2024-01-15 11:10:49.000000 treesimulator-0.1.8/treesimulator.egg-info/entry_points.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2024-01-15 11:10:49.000000 treesimulator-0.1.8/treesimulator.egg-info/requires.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       14 2024-01-15 11:10:49.000000 treesimulator-0.1.8/treesimulator.egg-info/top_level.txt
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2024-01-15 13:16:30.921658 treesimulator-0.1.9/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.9/LICENSE
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2024-01-15 13:16:30.921658 treesimulator-0.1.9/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.9/README.md
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2024-01-15 13:16:30.921658 treesimulator-0.1.9/setup.cfg
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2024-01-15 13:15:03.000000 treesimulator-0.1.9/setup.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2024-01-15 13:16:30.921658 treesimulator-0.1.9/treesimulator/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.9/treesimulator/__init__.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17716 2024-01-15 13:14:34.000000 treesimulator-0.1.9/treesimulator/generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10991 2024-01-15 11:06:19.000000 treesimulator-0.1.9/treesimulator/mtbd_models.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.9/treesimulator/sequence_generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5730 2024-01-15 10:57:01.000000 treesimulator-0.1.9/treesimulator/simulate_forest.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.9/treesimulator/simulate_forest_bd.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.9/treesimulator/simulate_forest_bdei.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.9/treesimulator/simulate_forest_bdss.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2024-01-15 13:16:30.921658 treesimulator-0.1.9/treesimulator.egg-info/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2024-01-15 13:16:30.000000 treesimulator-0.1.9/treesimulator.egg-info/PKG-INFO
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      513 2024-01-15 13:16:30.000000 treesimulator-0.1.9/treesimulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2024-01-15 13:16:30.000000 treesimulator-0.1.9/treesimulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      233 2024-01-15 13:16:30.000000 treesimulator-0.1.9/treesimulator.egg-info/entry_points.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2024-01-15 13:16:30.000000 treesimulator-0.1.9/treesimulator.egg-info/requires.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       14 2024-01-15 13:16:30.000000 treesimulator-0.1.9/treesimulator.egg-info/top_level.txt
```

### Comparing `treesimulator-0.1.8/LICENSE` & `treesimulator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/PKG-INFO` & `treesimulator-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
 Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 Keywords: phylogenetics,tree generator,multitype birth-death model
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `treesimulator-0.1.8/README.md` & `treesimulator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/setup.py` & `treesimulator-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    version='0.1.8',
+    version='0.1.9',
     description='Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.',
     author='Anna Zhukova',
     author_email='anna.zhukova@pasteur.fr',
     url='https://github.com/evolbioinfo/treesimulator',
     keywords=['phylogenetics', 'tree generator', 'multitype birth-death model'],
     install_requires=['six', 'ete3', 'numpy'],
     entry_points={
```

### Comparing `treesimulator-0.1.8/treesimulator/__init__.py` & `treesimulator-0.1.9/treesimulator/__init__.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator/generator.py` & `treesimulator-0.1.9/treesimulator/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,29 +69,30 @@
         transition_rate_sums = model.transition_rates.sum(axis=1) * infectious_nums
         removal_rate_sums = model.removal_rates * infectious_nums
         total_transmission_rate = transmission_rate_sums.sum()
         total_transition_rate = transition_rate_sums.sum()
         total_removal_rate = removal_rate_sums.sum()
         total_rate = total_transmission_rate + total_transition_rate + total_removal_rate
 
+
         # check if we passed the time limit
         time += np.random.exponential(1 / total_rate, 1)[0]
         if time >= max_time:
             time = max_time
             break
 
         # now let us see which event will happen
         random_event = np.random.uniform(0, 1, 1)[0] * total_rate
 
         # case 1: state transition
         if random_event < total_transition_rate:
             for i in range(num_states):
                 if random_event < transition_rate_sums[i]:
-                    infectious_nums[i] -= 1
                     random_event /= infectious_nums[i]
+                    infectious_nums[i] -= 1
                     for j in range(num_states):
                         if random_event < model.transition_rates[i, j]:
                             infectious_nums[j] += 1
                             state_changing_id = random_pop(infectious_state2id[i])
                             id2state[state_changing_id[0]] = j
                             infectious_state2id[j].add(state_changing_id)
                             logging.debug('Time {}:\t{} changed state from {} to {}'.format(time, state_changing_id, model.states[i], model.states[j]))
```

### Comparing `treesimulator-0.1.8/treesimulator/mtbd_models.py` & `treesimulator-0.1.9/treesimulator/mtbd_models.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator/sequence_generator.py` & `treesimulator-0.1.9/treesimulator/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator/simulate_forest.py` & `treesimulator-0.1.9/treesimulator/simulate_forest.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator/simulate_forest_bd.py` & `treesimulator-0.1.9/treesimulator/simulate_forest_bd.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator/simulate_forest_bdei.py` & `treesimulator-0.1.9/treesimulator/simulate_forest_bdei.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator/simulate_forest_bdss.py` & `treesimulator-0.1.9/treesimulator/simulate_forest_bdss.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.8/treesimulator.egg-info/PKG-INFO` & `treesimulator-0.1.9/treesimulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
 Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 Keywords: phylogenetics,tree generator,multitype birth-death model
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `treesimulator-0.1.8/treesimulator.egg-info/SOURCES.txt` & `treesimulator-0.1.9/treesimulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

