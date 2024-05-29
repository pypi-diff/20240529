# Comparing `tmp/fairbalance-0.1.6.tar.gz` & `tmp/fairbalance-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.1.6.tar", last modified: Wed May 22 09:47:00 2024, max compression
+gzip compressed data, was "fairbalance-0.1.7.tar", last modified: Wed May 29 09:52:11 2024, max compression
```

## Comparing `fairbalance-0.1.6.tar` & `fairbalance-0.1.7.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:00.370355 fairbalance-0.1.6/
--rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.6/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-22 09:47:00.349681 fairbalance-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.658218 fairbalance-0.1.6/docs/
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.765167 fairbalance-0.1.6/docs/basics/
--rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.6/docs/basics/test.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.798601 fairbalance-0.1.6/fairbalance/
--rw-rw-rw-   0        0        0       40 2024-05-22 08:39:56.000000 fairbalance-0.1.6/fairbalance/__init__.py
--rw-rw-rw-   0        0        0    12167 2024-05-21 13:36:53.000000 fairbalance-0.1.6/fairbalance/all_test.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.915259 fairbalance-0.1.6/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.6/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11937 2024-05-22 09:14:40.000000 fairbalance-0.1.6/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.931780 fairbalance-0.1.6/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.6/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.997769 fairbalance-0.1.6/fairbalance/metrics/
--rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.6/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.6/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0    12289 2024-05-22 08:34:39.000000 fairbalance-0.1.6/fairbalance/metrics/_fairness_analysis.py
--rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.6/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:00.048364 fairbalance-0.1.6/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.6/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.6/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.6/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:00.098355 fairbalance-0.1.6/fairbalance/mitigation_strategies/
--rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.6/fairbalance/mitigation_strategies/__init__.py
--rw-rw-rw-   0        0        0     8612 2024-05-22 08:34:47.000000 fairbalance-0.1.6/fairbalance/mitigation_strategies/_mitigation_strategies.py
--rw-rw-rw-   0        0        0     4763 2024-05-22 08:34:51.000000 fairbalance-0.1.6/fairbalance/mitigation_strategies/base.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:00.165232 fairbalance-0.1.6/fairbalance/processors/
--rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.6/fairbalance/processors/__init__.py
--rw-rw-rw-   0        0        0     3130 2024-05-22 09:46:00.000000 fairbalance-0.1.6/fairbalance/processors/_processors.py
--rw-rw-rw-   0        0        0     8327 2024-05-22 08:34:34.000000 fairbalance-0.1.6/fairbalance/processors/base.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:00.264757 fairbalance-0.1.6/fairbalance/tools/
--rw-rw-rw-   0        0        0      460 2024-05-22 09:45:55.000000 fairbalance-0.1.6/fairbalance/tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.6/fairbalance/tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.6/fairbalance/tools/_mitigator.py
--rw-rw-rw-   0        0        0    10334 2024-05-22 09:45:56.000000 fairbalance-0.1.6/fairbalance/tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.6/fairbalance/tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:00.331905 fairbalance-0.1.6/fairbalance/tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.6/fairbalance/tools/tests/__init__.py
--rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.6/fairbalance/tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.6/fairbalance/tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.6/fairbalance/tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.6/fairbalance/tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:59.881889 fairbalance-0.1.6/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-22 09:46:56.000000 fairbalance-0.1.6/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1329 2024-05-22 09:46:59.000000 fairbalance-0.1.6/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:46:56.000000 fairbalance-0.1.6/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-22 09:46:56.000000 fairbalance-0.1.6/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 09:46:56.000000 fairbalance-0.1.6/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 09:47:00.370355 fairbalance-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-22 09:46:36.000000 fairbalance-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.748872 fairbalance-0.1.7/
+-rw-rw-rw-   0        0        0      342 2024-05-29 09:24:59.000000 fairbalance-0.1.7/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-29 09:52:11.734310 fairbalance-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.099133 fairbalance-0.1.7/docs/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.191557 fairbalance-0.1.7/docs/basics/
+-rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.7/docs/basics/test.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.210162 fairbalance-0.1.7/fairbalance/
+-rw-rw-rw-   0        0        0       40 2024-05-29 07:36:42.000000 fairbalance-0.1.7/fairbalance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.390421 fairbalance-0.1.7/fairbalance/_tools/
+-rw-rw-rw-   0        0        0      497 2024-05-29 08:55:22.000000 fairbalance-0.1.7/fairbalance/_tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.7/fairbalance/_tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.7/fairbalance/_tools/_mitigator.py
+-rw-rw-rw-   0        0        0    10334 2024-05-22 09:45:56.000000 fairbalance-0.1.7/fairbalance/_tools/_processor.py
+-rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.7/fairbalance/_tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.451108 fairbalance-0.1.7/fairbalance/_tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.7/fairbalance/_tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.7/fairbalance/_tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.472994 fairbalance-0.1.7/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.7/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11937 2024-05-22 09:14:40.000000 fairbalance-0.1.7/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.488177 fairbalance-0.1.7/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.7/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.550106 fairbalance-0.1.7/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.7/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.7/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0    12290 2024-05-29 08:54:24.000000 fairbalance-0.1.7/fairbalance/metrics/_fairness_analysis.py
+-rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.7/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.589112 fairbalance-0.1.7/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.7/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.7/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.7/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.624795 fairbalance-0.1.7/fairbalance/mitigation_strategies/
+-rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.7/fairbalance/mitigation_strategies/__init__.py
+-rw-rw-rw-   0        0        0     8972 2024-05-29 09:21:46.000000 fairbalance-0.1.7/fairbalance/mitigation_strategies/_mitigation_strategies.py
+-rw-rw-rw-   0        0        0     4757 2024-05-29 07:38:08.000000 fairbalance-0.1.7/fairbalance/mitigation_strategies/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.671539 fairbalance-0.1.7/fairbalance/processors/
+-rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.7/fairbalance/processors/__init__.py
+-rw-rw-rw-   0        0        0     3130 2024-05-22 09:46:00.000000 fairbalance-0.1.7/fairbalance/processors/_processors.py
+-rw-rw-rw-   0        0        0     8303 2024-05-29 09:21:40.000000 fairbalance-0.1.7/fairbalance/processors/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.695841 fairbalance-0.1.7/fairbalance/utils/
+-rw-rw-rw-   0        0        0      209 2024-05-29 09:24:03.000000 fairbalance-0.1.7/fairbalance/utils/__init__.py
+-rw-rw-rw-   0        0        0     3960 2024-05-29 09:38:40.000000 fairbalance-0.1.7/fairbalance/utils/_balanced_train_test_split.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:52:11.715602 fairbalance-0.1.7/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1390 2024-05-29 09:52:11.000000 fairbalance-0.1.7/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 09:52:10.000000 fairbalance-0.1.7/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2024-05-29 08:05:51.000000 fairbalance-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:52:11.748872 fairbalance-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-29 09:51:38.000000 fairbalance-0.1.7/setup.py
```

### Comparing `fairbalance-0.1.6/PKG-INFO` & `fairbalance-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.6
+Version: 0.1.7
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.6/docs/basics/test.ipynb` & `fairbalance-0.1.7/docs/basics/test.ipynb`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.1.7/fairbalance/datasets/_datasets_loader.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/metrics/_dataset_metrics.py` & `fairbalance-0.1.7/fairbalance/metrics/_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/metrics/_fairness_analysis.py` & `fairbalance-0.1.7/fairbalance/metrics/_fairness_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 
-from ..tools._utils import binarize_columns, sanity_checker
+from .._tools._utils import binarize_columns, sanity_checker
 from ._dataset_metrics import *
 
 class FairnessAnalysis(sanity_checker) :
     """The FairnessAnalysis class gives an easy and straightforward way to assess the fairness and the biais of a dataset.
 
     Parameters
     ----------
```

### Comparing `fairbalance-0.1.6/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.1.7/fairbalance/metrics/_model_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/metrics/tests/test_dataset_metrics.py` & `fairbalance-0.1.7/fairbalance/metrics/tests/test_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/mitigation_strategies/_mitigation_strategies.py` & `fairbalance-0.1.7/fairbalance/mitigation_strategies/_mitigation_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .base import BaseMitigationStrategy
 from ..processors.base import BaseProcessor
-
+from ..processors import RandomOverSamplerProcessor
+from ..datasets import load_adult
 import pandas as pd
 
 class BalanceOutput(BaseMitigationStrategy) :
     """
     Balances the outputs of the dataset with no regards to the protected attributes.
 
     Parameters
@@ -171,15 +172,15 @@
             
                 # keep only the rows with given class
             class_df = df[df[protected_attribute] == class_]
             class_target = target[df[protected_attribute] == class_]
             
             if class_ != class_with_highest_r :  
                 # resample the target for this class
-                if len(class_target.unique()) > 1 :
+                if len(class_target.squeeze().unique()) > 1 :
                     X_processed, y_processed = self.sampler._process(class_df, class_target, cont_columns, cat_columns)
                     X_resampled, y_resampled = self.sampler.fit_resample(X_processed, y_processed)
                     X_class_final, y_class_final = self.sampler._unprocess(X_resampled, y_resampled)
                         
                 else :
                     X_class_final = class_df
                     y_class_final = class_target
@@ -193,8 +194,16 @@
                 y_final = pd.concat([y_final, class_target])
                 
         
         
         X_final = self._get_final_dataframe(X_final, protected_attributes, protected_attribute)
 
         return X_final, y_final
-      
+
+if __name__ == """__main__""" :
+    
+    balancer = BalanceOutputForAttributes(sampler = RandomOverSamplerProcessor())
+    data, target, cat, cont = load_adult()
+    
+    d, t =balancer.balance(data, target, ["sex", "race"], cont, cat)
+    
+    print(d.columns)
```

### Comparing `fairbalance-0.1.6/fairbalance/mitigation_strategies/base.py` & `fairbalance-0.1.7/fairbalance/mitigation_strategies/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -261,38 +261,38 @@
 00001040: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
 00001050: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
 00001060: 5b66 6c6f 6174 2c20 7374 725d 203a 2074  [float, str] : t
 00001070: 6865 2068 6967 6865 7374 2072 6174 696f  he highest ratio
 00001080: 2061 6e64 2074 6865 2061 7373 6f63 6961   and the associa
 00001090: 7465 6420 636c 6173 730d 0a20 2020 2020  ted class..     
 000010a0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000010b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000010c0: 2020 2020 2020 725f 6d61 7820 3d20 300d        r_max = 0.
-000010d0: 0a20 2020 2020 2020 2020 2020 2063 5f6d  .            c_m
-000010e0: 6178 203d 2063 6c61 7373 6573 5b30 5d0d  ax = classes[0].
-000010f0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001100: 6173 6574 2e6c 6f63 5b3a 2c20 2274 6172  aset.loc[:, "tar
-00001110: 6765 7422 5d20 3d20 7461 7267 6574 0d0a  get"] = target..
-00001120: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00001130: 6320 696e 2063 6c61 7373 6573 203a 0d0a  c in classes :..
-00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 7220 3d20 6461 7461 7365 745b 6461 7461  r = dataset[data
-00001160: 7365 745b 7072 6f74 6563 7465 645f 6174  set[protected_at
-00001170: 7472 6962 7574 655d 203d 3d20 635d 5b22  tribute] == c]["
-00001180: 7461 7267 6574 225d 2e76 616c 7565 5f63  target"].value_c
-00001190: 6f75 6e74 7328 295b 315d 2f64 6174 6173  ounts()[1]/datas
-000011a0: 6574 5b64 6174 6173 6574 5b70 726f 7465  et[dataset[prote
-000011b0: 6374 6564 5f61 7474 7269 6275 7465 5d20  cted_attribute] 
-000011c0: 3d3d 2063 5d5b 2274 6172 6765 7422 5d2e  == c]["target"].
-000011d0: 7661 6c75 655f 636f 756e 7473 2829 5b30  value_counts()[0
-000011e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000011f0: 2020 2069 6620 7220 3e20 3120 3a0d 0a20     if r > 1 :.. 
-00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 2020 2072 203d 2031 2f72 0d0a 2020 2020     r = 1/r..    
-00001220: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00001230: 203e 2072 5f6d 6178 203a 0d0a 2020 2020   > r_max :..    
-00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 725f 6d61 7820 3d20 720d 0a20 2020 2020  r_max = r..     
-00001260: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001270: 5f6d 6178 203d 2063 0d0a 2020 2020 2020  _max = c..      
-00001280: 2020 2020 2020 7265 7475 726e 2072 5f6d        return r_m
-00001290: 6178 2c20 635f 6d61 780d 0a              ax, c_max..
+000010b0: 2020 2020 2020 2020 6466 203d 2064 6174          df = dat
+000010c0: 6173 6574 2e63 6f70 7928 290d 0a20 2020  aset.copy()..   
+000010d0: 2020 2020 2020 2020 2072 5f6d 6178 203d           r_max =
+000010e0: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+000010f0: 635f 6d61 7820 3d20 636c 6173 7365 735b  c_max = classes[
+00001100: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00001110: 6466 2e6c 6f63 5b3a 2c20 2274 6172 6765  df.loc[:, "targe
+00001120: 7422 5d20 3d20 7461 7267 6574 0d0a 2020  t"] = target..  
+00001130: 2020 2020 2020 2020 2020 666f 7220 6320            for c 
+00001140: 696e 2063 6c61 7373 6573 203a 0d0a 2020  in classes :..  
+00001150: 2020 2020 2020 2020 2020 2020 2020 7220                r 
+00001160: 3d20 6466 5b64 665b 7072 6f74 6563 7465  = df[df[protecte
+00001170: 645f 6174 7472 6962 7574 655d 203d 3d20  d_attribute] == 
+00001180: 635d 5b22 7461 7267 6574 225d 2e76 616c  c]["target"].val
+00001190: 7565 5f63 6f75 6e74 7328 295b 315d 2f64  ue_counts()[1]/d
+000011a0: 665b 6466 5b70 726f 7465 6374 6564 5f61  f[df[protected_a
+000011b0: 7474 7269 6275 7465 5d20 3d3d 2063 5d5b  ttribute] == c][
+000011c0: 2274 6172 6765 7422 5d2e 7661 6c75 655f  "target"].value_
+000011d0: 636f 756e 7473 2829 5b30 5d0d 0a20 2020  counts()[0]..   
+000011e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000011f0: 7220 3e20 3120 3a0d 0a20 2020 2020 2020  r > 1 :..       
+00001200: 2020 2020 2020 2020 2020 2020 2072 203d               r =
+00001210: 2031 2f72 0d0a 2020 2020 2020 2020 2020   1/r..          
+00001220: 2020 2020 2020 6966 2072 203e 2072 5f6d        if r > r_m
+00001230: 6178 203a 0d0a 2020 2020 2020 2020 2020  ax :..          
+00001240: 2020 2020 2020 2020 2020 725f 6d61 7820            r_max 
+00001250: 3d20 720d 0a20 2020 2020 2020 2020 2020  = r..           
+00001260: 2020 2020 2020 2020 2063 5f6d 6178 203d           c_max =
+00001270: 2063 0d0a 2020 2020 2020 2020 2020 2020   c..            
+00001280: 7265 7475 726e 2072 5f6d 6178 2c20 635f  return r_max, c_
+00001290: 6d61 780d 0a                             max..
```

### Comparing `fairbalance-0.1.6/fairbalance/processors/_processors.py` & `fairbalance-0.1.7/fairbalance/processors/_processors.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/processors/base.py` & `fairbalance-0.1.7/fairbalance/processors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from sys import prefix
 import pandas as pd
 from sklearn.calibration import LabelEncoder
 from sklearn.preprocessing import MinMaxScaler
```

### Comparing `fairbalance-0.1.6/fairbalance/tools/_fairness_analysis.py` & `fairbalance-0.1.7/fairbalance/_tools/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/tools/_mitigator.py` & `fairbalance-0.1.7/fairbalance/_tools/_mitigator.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/tools/_processor.py` & `fairbalance-0.1.7/fairbalance/_tools/_processor.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/tools/_utils.py` & `fairbalance-0.1.7/fairbalance/_tools/_utils.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance/tools/tests/test_fairness_analysis.py` & `fairbalance-0.1.7/fairbalance/_tools/tests/test_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.6/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.1.7/fairbalance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.6
+Version: 0.1.7
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.6/fairbalance.egg-info/SOURCES.txt` & `fairbalance-0.1.7/fairbalance.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 .gitignore
 README.md
 requirements.txt
 setup.py
 docs/basics/test.ipynb
 fairbalance/__init__.py
-fairbalance/all_test.ipynb
 fairbalance.egg-info/PKG-INFO
 fairbalance.egg-info/SOURCES.txt
 fairbalance.egg-info/dependency_links.txt
 fairbalance.egg-info/requires.txt
 fairbalance.egg-info/top_level.txt
+fairbalance/_tools/__init__.py
+fairbalance/_tools/_fairness_analysis.py
+fairbalance/_tools/_mitigator.py
+fairbalance/_tools/_processor.py
+fairbalance/_tools/_utils.py
+fairbalance/_tools/tests/__init__.py
+fairbalance/_tools/tests/test_fairness_analysis.py
+fairbalance/_tools/tests/test_mitigator.py
+fairbalance/_tools/tests/test_processor.py
+fairbalance/_tools/tests/test_utils.py
 fairbalance/datasets/__init__.py
 fairbalance/datasets/_datasets_loader.py
 fairbalance/datasets/tests/test_datasets_loader.py
 fairbalance/metrics/__init__.py
 fairbalance/metrics/_dataset_metrics.py
 fairbalance/metrics/_fairness_analysis.py
 fairbalance/metrics/_model_metrics.py
@@ -22,17 +31,9 @@
 fairbalance/metrics/tests/test_model_metrics.py
 fairbalance/mitigation_strategies/__init__.py
 fairbalance/mitigation_strategies/_mitigation_strategies.py
 fairbalance/mitigation_strategies/base.py
 fairbalance/processors/__init__.py
 fairbalance/processors/_processors.py
 fairbalance/processors/base.py
-fairbalance/tools/__init__.py
-fairbalance/tools/_fairness_analysis.py
-fairbalance/tools/_mitigator.py
-fairbalance/tools/_processor.py
-fairbalance/tools/_utils.py
-fairbalance/tools/tests/__init__.py
-fairbalance/tools/tests/test_fairness_analysis.py
-fairbalance/tools/tests/test_mitigator.py
-fairbalance/tools/tests/test_processor.py
-fairbalance/tools/tests/test_utils.py
+fairbalance/utils/__init__.py
+fairbalance/utils/_balanced_train_test_split.py
```

### Comparing `fairbalance-0.1.6/setup.py` & `fairbalance-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.1.6",
+    version = "0.1.7",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
```

