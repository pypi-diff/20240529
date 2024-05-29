# Comparing `tmp/fairbalance-0.1.7.tar.gz` & `tmp/fairbalance-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.1.7.tar", last modified: Wed May 29 09:52:11 2024, max compression
+gzip compressed data, was "fairbalance-0.1.8.tar", last modified: Wed May 29 11:24:53 2024, max compression
```

## Comparing `fairbalance-0.1.7.tar` & `fairbalance-0.1.8.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.748872 fairbalance-0.1.7/
--rw-rw-rw-   0        0        0      342 2024-05-29 09:24:59.000000 fairbalance-0.1.7/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-29 09:52:11.734310 fairbalance-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.099133 fairbalance-0.1.7/docs/
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.191557 fairbalance-0.1.7/docs/basics/
--rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.7/docs/basics/test.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.210162 fairbalance-0.1.7/fairbalance/
--rw-rw-rw-   0        0        0       40 2024-05-29 07:36:42.000000 fairbalance-0.1.7/fairbalance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.390421 fairbalance-0.1.7/fairbalance/_tools/
--rw-rw-rw-   0        0        0      497 2024-05-29 08:55:22.000000 fairbalance-0.1.7/fairbalance/_tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.7/fairbalance/_tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.7/fairbalance/_tools/_mitigator.py
--rw-rw-rw-   0        0        0    10334 2024-05-22 09:45:56.000000 fairbalance-0.1.7/fairbalance/_tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.7/fairbalance/_tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.451108 fairbalance-0.1.7/fairbalance/_tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.7/fairbalance/_tools/tests/__init__.py
--rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.472994 fairbalance-0.1.7/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.7/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11937 2024-05-22 09:14:40.000000 fairbalance-0.1.7/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.488177 fairbalance-0.1.7/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.7/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.550106 fairbalance-0.1.7/fairbalance/metrics/
--rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.7/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.7/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0    12290 2024-05-29 08:54:24.000000 fairbalance-0.1.7/fairbalance/metrics/_fairness_analysis.py
--rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.7/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.589112 fairbalance-0.1.7/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.7/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.7/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.7/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.624795 fairbalance-0.1.7/fairbalance/mitigation_strategies/
--rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.7/fairbalance/mitigation_strategies/__init__.py
--rw-rw-rw-   0        0        0     8972 2024-05-29 09:21:46.000000 fairbalance-0.1.7/fairbalance/mitigation_strategies/_mitigation_strategies.py
--rw-rw-rw-   0        0        0     4757 2024-05-29 07:38:08.000000 fairbalance-0.1.7/fairbalance/mitigation_strategies/base.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.671539 fairbalance-0.1.7/fairbalance/processors/
--rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.7/fairbalance/processors/__init__.py
--rw-rw-rw-   0        0        0     3130 2024-05-22 09:46:00.000000 fairbalance-0.1.7/fairbalance/processors/_processors.py
--rw-rw-rw-   0        0        0     8303 2024-05-29 09:21:40.000000 fairbalance-0.1.7/fairbalance/processors/base.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.695841 fairbalance-0.1.7/fairbalance/utils/
--rw-rw-rw-   0        0        0      209 2024-05-29 09:24:03.000000 fairbalance-0.1.7/fairbalance/utils/__init__.py
--rw-rw-rw-   0        0        0     3960 2024-05-29 09:38:40.000000 fairbalance-0.1.7/fairbalance/utils/_balanced_train_test_split.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.715602 fairbalance-0.1.7/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1390 2024-05-29 09:52:11.000000 fairbalance-0.1.7/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2024-05-29 08:05:51.000000 fairbalance-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 09:52:11.748872 fairbalance-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-29 09:51:38.000000 fairbalance-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.220416 fairbalance-0.1.8/
+-rw-rw-rw-   0        0        0      342 2024-05-29 09:24:59.000000 fairbalance-0.1.8/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-29 11:24:53.204126 fairbalance-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.409086 fairbalance-0.1.8/docs/
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.516879 fairbalance-0.1.8/docs/basics/
+-rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.8/docs/basics/test.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.533330 fairbalance-0.1.8/fairbalance/
+-rw-rw-rw-   0        0        0       40 2024-05-29 07:36:42.000000 fairbalance-0.1.8/fairbalance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.725018 fairbalance-0.1.8/fairbalance/_tools/
+-rw-rw-rw-   0        0        0      501 2024-05-29 11:20:19.000000 fairbalance-0.1.8/fairbalance/_tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.8/fairbalance/_tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.8/fairbalance/_tools/_mitigator.py
+-rw-rw-rw-   0        0        0    10334 2024-05-22 09:45:56.000000 fairbalance-0.1.8/fairbalance/_tools/_processor.py
+-rw-rw-rw-   0        0        0     2220 2024-05-29 11:22:30.000000 fairbalance-0.1.8/fairbalance/_tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.812602 fairbalance-0.1.8/fairbalance/_tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.8/fairbalance/_tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.8/fairbalance/_tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.8/fairbalance/_tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.8/fairbalance/_tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.8/fairbalance/_tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.845982 fairbalance-0.1.8/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.8/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11937 2024-05-22 09:14:40.000000 fairbalance-0.1.8/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.868720 fairbalance-0.1.8/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.8/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.936931 fairbalance-0.1.8/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.8/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.8/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0    12312 2024-05-29 11:23:00.000000 fairbalance-0.1.8/fairbalance/metrics/_fairness_analysis.py
+-rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.8/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:52.989446 fairbalance-0.1.8/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.8/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.8/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.8/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.038515 fairbalance-0.1.8/fairbalance/mitigation_strategies/
+-rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.8/fairbalance/mitigation_strategies/__init__.py
+-rw-rw-rw-   0        0        0     8972 2024-05-29 09:21:46.000000 fairbalance-0.1.8/fairbalance/mitigation_strategies/_mitigation_strategies.py
+-rw-rw-rw-   0        0        0     4757 2024-05-29 07:38:08.000000 fairbalance-0.1.8/fairbalance/mitigation_strategies/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.055123 fairbalance-0.1.8/fairbalance/mitigation_strategies/tests/
+-rw-rw-rw-   0        0        0     3422 2024-05-27 11:55:55.000000 fairbalance-0.1.8/fairbalance/mitigation_strategies/tests/test_mitigation_strategies.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.105479 fairbalance-0.1.8/fairbalance/processors/
+-rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.8/fairbalance/processors/__init__.py
+-rw-rw-rw-   0        0        0     3130 2024-05-22 09:46:00.000000 fairbalance-0.1.8/fairbalance/processors/_processors.py
+-rw-rw-rw-   0        0        0     8303 2024-05-29 09:21:40.000000 fairbalance-0.1.8/fairbalance/processors/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.120661 fairbalance-0.1.8/fairbalance/processors/tests/
+-rw-rw-rw-   0        0        0     1665 2024-05-27 11:51:15.000000 fairbalance-0.1.8/fairbalance/processors/tests/test_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.159579 fairbalance-0.1.8/fairbalance/utils/
+-rw-rw-rw-   0        0        0      209 2024-05-29 09:24:03.000000 fairbalance-0.1.8/fairbalance/utils/__init__.py
+-rw-rw-rw-   0        0        0     3960 2024-05-29 09:38:40.000000 fairbalance-0.1.8/fairbalance/utils/_balanced_train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:24:53.180871 fairbalance-0.1.8/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-29 11:24:51.000000 fairbalance-0.1.8/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1508 2024-05-29 11:24:52.000000 fairbalance-0.1.8/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:24:51.000000 fairbalance-0.1.8/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-29 11:24:51.000000 fairbalance-0.1.8/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 11:24:51.000000 fairbalance-0.1.8/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2024-05-29 08:05:51.000000 fairbalance-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:24:53.220416 fairbalance-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-29 11:23:55.000000 fairbalance-0.1.8/setup.py
```

### Comparing `fairbalance-0.1.7/PKG-INFO` & `fairbalance-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.7
+Version: 0.1.8
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.7/docs/basics/test.ipynb` & `fairbalance-0.1.8/docs/basics/test.ipynb`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/_tools/_fairness_analysis.py` & `fairbalance-0.1.8/fairbalance/_tools/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/_tools/_mitigator.py` & `fairbalance-0.1.8/fairbalance/_tools/_mitigator.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/_tools/_processor.py` & `fairbalance-0.1.8/fairbalance/_tools/_processor.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/_tools/_utils.py` & `fairbalance-0.1.8/fairbalance/_tools/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,19 +25,20 @@
     
     def _sanity_check(self, dataset, target = None, positive_output_target = None, protected_attributes = None, privileged_groups = None) :
         """
         Checks that are common in all classes of the package.
         """
         assert isinstance(dataset, pd.DataFrame), "Dataset should be in a pandas DataFrame format."
         
-        if target :    
-            assert target in list(dataset.columns), f""""{target}" is not a column of the dataframe."""
+        assert isinstance(target, pd.DataFrame), "Dataset should be in a pandas DataFrame format."
+        # if target :    
+        #     assert target in list(dataset.columns), f""""{target}" is not a column of the dataframe."""
         
         if positive_output_target :
-            assert positive_output_target in dataset[target].unique(), f""""{positive_output_target}" is not a value of the target"""
+            assert positive_output_target in target.squeeze().unique(), f""""{positive_output_target}" is not a value of the target"""
         
         if protected_attributes :
             assert len(protected_attributes) > 0, "Needs at least one protected attribute"
             
             if privileged_groups :
                 for protected_attribute in protected_attributes :
                     assert protected_attribute in privileged_groups.keys(), f"no privileged group defined for attribute {protected_attribute}"
```

### Comparing `fairbalance-0.1.7/fairbalance/_tools/tests/test_fairness_analysis.py` & `fairbalance-0.1.8/fairbalance/_tools/tests/test_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.1.8/fairbalance/datasets/_datasets_loader.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/metrics/_dataset_metrics.py` & `fairbalance-0.1.8/fairbalance/metrics/_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/metrics/_fairness_analysis.py` & `fairbalance-0.1.8/fairbalance/metrics/_fairness_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     
     **After self.get_fairness_score() is called:**
     attribute_fairness_score : dict
         The Composite Fairness Score (CFS) for each protected attribute.
     fairness_score : float
         The overall Composite Fairness Score (CFS) of the dataset.        
         """
-    def __init__(self, dataset: pd.DataFrame, target : str, positive_output_target, protected_attributes: list, privileged_groups: dict) :
+    def __init__(self, dataset: pd.DataFrame, target : pd.DataFrame, positive_output_target, protected_attributes: list, privileged_groups: dict) :
         super()._sanity_check(dataset, target, positive_output_target, protected_attributes, privileged_groups)
         
-        self.dataset = dataset
+        self.dataset = pd.concat([dataset, target], axis=1)
         self.protected_attributes = protected_attributes
         self.privileged_groups = privileged_groups
         
         #set target attribute
-        self.target = self.dataset[[target]]
+        self.target = target
         self.positive_output_target = positive_output_target
     
   
     def _make_binary_column(self, dataset :pd.DataFrame, protected_attribute: str, privileged_group: str) :
         """Returns a DataFrame which contains of column of the protected attribute with binary value (privileged and non_privileged)
         and a column of the output with binary value (positive output and non_positive output).
```

### Comparing `fairbalance-0.1.7/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.1.8/fairbalance/metrics/_model_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/metrics/tests/test_dataset_metrics.py` & `fairbalance-0.1.8/fairbalance/metrics/tests/test_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/mitigation_strategies/_mitigation_strategies.py` & `fairbalance-0.1.8/fairbalance/mitigation_strategies/_mitigation_strategies.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/mitigation_strategies/base.py` & `fairbalance-0.1.8/fairbalance/mitigation_strategies/base.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/processors/_processors.py` & `fairbalance-0.1.8/fairbalance/processors/_processors.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/processors/base.py` & `fairbalance-0.1.8/fairbalance/processors/base.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance/utils/_balanced_train_test_split.py` & `fairbalance-0.1.8/fairbalance/utils/_balanced_train_test_split.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.7/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.1.8/fairbalance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.7
+Version: 0.1.8
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.7/fairbalance.egg-info/SOURCES.txt` & `fairbalance-0.1.8/fairbalance.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,12 +28,14 @@
 fairbalance/metrics/_model_metrics.py
 fairbalance/metrics/tests/__init__.py
 fairbalance/metrics/tests/test_dataset_metrics.py
 fairbalance/metrics/tests/test_model_metrics.py
 fairbalance/mitigation_strategies/__init__.py
 fairbalance/mitigation_strategies/_mitigation_strategies.py
 fairbalance/mitigation_strategies/base.py
+fairbalance/mitigation_strategies/tests/test_mitigation_strategies.py
 fairbalance/processors/__init__.py
 fairbalance/processors/_processors.py
 fairbalance/processors/base.py
+fairbalance/processors/tests/test_processors.py
 fairbalance/utils/__init__.py
 fairbalance/utils/_balanced_train_test_split.py
```

### Comparing `fairbalance-0.1.7/setup.py` & `fairbalance-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.1.7",
+    version = "0.1.8",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
```

