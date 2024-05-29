# Comparing `tmp/fedjust-0.1.2.4.tar.gz` & `tmp/fedjust-0.1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedjust-0.1.2.4.tar", max compression
+gzip compressed data, was "fedjust-0.1.2.5.tar", max compression
```

## Comparing `fedjust-0.1.2.4.tar` & `fedjust-0.1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/aggregators/aggregator.py
--rw-r--r--   0        0        0     1442 2024-05-02 14:42:59.238594 fedjust-0.1.2.4/FedJust/aggregators/fedopt_aggregator.py
--rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2.4/FedJust/files/archive.py
--rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/files/handlers.py
--rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/files/loggers.py
--rw-r--r--   0        0        0    17171 2024-05-22 11:50:33.002404 fedjust-0.1.2.4/FedJust/model/federated_model.py
--rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2.4/FedJust/node/federated_node.py
--rw-r--r--   0        0        0     2694 2024-05-22 11:52:41.204209 fedjust-0.1.2.4/FedJust/operations/evaluations.py
--rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2.4/FedJust/operations/orchestrations.py
--rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2.4/FedJust/simulation/adaptive_optimizer_simulation.py
--rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2.4/FedJust/simulation/simulation.py
--rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2.4/FedJust/utils/computations.py
--rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2.4/README.md
--rw-r--r--   0        0        0      428 2024-05-24 12:32:49.533113 fedjust-0.1.2.4/pyproject.toml
--rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 fedjust-0.1.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2.5/FedJust/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2.5/FedJust/aggregators/aggregator.py
+-rw-r--r--   0        0        0     1442 2024-05-02 14:42:59.238594 fedjust-0.1.2.5/FedJust/aggregators/fedopt_aggregator.py
+-rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2.5/FedJust/files/archive.py
+-rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2.5/FedJust/files/handlers.py
+-rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2.5/FedJust/files/loggers.py
+-rw-r--r--   0        0        0    17202 2024-05-29 11:49:30.745392 fedjust-0.1.2.5/FedJust/model/federated_model.py
+-rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2.5/FedJust/node/federated_node.py
+-rw-r--r--   0        0        0     2742 2024-05-29 11:52:54.730464 fedjust-0.1.2.5/FedJust/operations/evaluations.py
+-rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2.5/FedJust/operations/orchestrations.py
+-rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2.5/FedJust/simulation/adaptive_optimizer_simulation.py
+-rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2.5/FedJust/simulation/simulation.py
+-rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2.5/FedJust/utils/computations.py
+-rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2.5/README.md
+-rw-r--r--   0        0        0      428 2024-05-29 11:54:00.185491 fedjust-0.1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 fedjust-0.1.2.5/PKG-INFO
```

### Comparing `fedjust-0.1.2.4/FedJust/aggregators/aggregator.py` & `fedjust-0.1.2.5/FedJust/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/aggregators/fedopt_aggregator.py` & `fedjust-0.1.2.5/FedJust/aggregators/fedopt_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/files/archive.py` & `fedjust-0.1.2.5/FedJust/files/archive.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/files/handlers.py` & `fedjust-0.1.2.5/FedJust/files/handlers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/files/loggers.py` & `fedjust-0.1.2.5/FedJust/files/loggers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/model/federated_model.py` & `fedjust-0.1.2.5/FedJust/model/federated_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,15 @@
         y_true = [item.item() for sublist in y_true for item in sublist]
         y_pred = [item.item() for sublist in y_pred for item in sublist]
 
         evaluation_results['f1score'] = f1_score(y_true, y_pred, average="macro")
         evaluation_results['precision'] = precision_score(y_true, y_pred, average="macro")
         evaluation_results['recall'] = recall_score(y_true, y_pred, average="macro")
 
-        cm = confusion_matrix(y_true, y_pred)
+        cm = confusion_matrix(y_true, y_pred, labels=[i for i in range(10)])
         cm = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
         accuracy_per_class = cm.diagonal()
         accuracy_per_class_expanded = {
             f'accuracy_per_{class_id}': value for class_id, value in enumerate(accuracy_per_class)
         }
         evaluation_results.update(accuracy_per_class_expanded)
```

### Comparing `fedjust-0.1.2.4/FedJust/node/federated_node.py` & `fedjust-0.1.2.5/FedJust/node/federated_node.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/operations/evaluations.py` & `fedjust-0.1.2.5/FedJust/operations/evaluations.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     
     Returns
     -------
         None"""
     try:
         evaluation_results = model.evaluate_model()
         evaluation_results['node_id'] = model.node_name
+        evaluation_results['epoch'] = iteration
         if log_to_screen == True:
             pass
             #logger.info(f"Evaluating model after iteration {iteration} on node {model.node_name}. Results: {metrics}")
     except Exception as e:
         logger.warning(f"Unable to compute metrics. {e}")
     path = os.path.join(save_path)
     with open(path, 'a+', newline='') as saved_file:
```

### Comparing `fedjust-0.1.2.4/FedJust/operations/orchestrations.py` & `fedjust-0.1.2.5/FedJust/operations/orchestrations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/simulation/adaptive_optimizer_simulation.py` & `fedjust-0.1.2.5/FedJust/simulation/adaptive_optimizer_simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/simulation/simulation.py` & `fedjust-0.1.2.5/FedJust/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/FedJust/utils/computations.py` & `fedjust-0.1.2.5/FedJust/utils/computations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/README.md` & `fedjust-0.1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.4/PKG-INFO` & `fedjust-0.1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedJust
-Version: 0.1.2.4
+Version: 0.1.2.5
 Summary: 
 Author: Scolpe
 Author-email: 63779111+Scolpe@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

