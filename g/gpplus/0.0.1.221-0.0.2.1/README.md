# Comparing `tmp/gpplus-0.0.1.221.tar.gz` & `tmp/gpplus-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpplus-0.0.1.221.tar", last modified: Thu Feb 15 23:05:59 2024, max compression
+gzip compressed data, was "gpplus-0.0.2.1.tar", last modified: Tue May 28 17:45:08 2024, max compression
```

## Comparing `gpplus-0.0.1.221.tar` & `gpplus-0.0.2.1.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.128751 gpplus-0.0.1.221/
--rw-rw-rw-   0        0        0      528 2024-02-15 23:05:59.126768 gpplus-0.0.1.221/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:58.911706 gpplus-0.0.1.221/gpplus/
--rw-rw-rw-   0        0        0       45 2024-02-15 20:55:49.000000 gpplus-0.0.1.221/gpplus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:58.963285 gpplus-0.0.1.221/gpplus/bayesian_optimizations/
--rw-rw-rw-   0        0        0     4815 2024-02-15 20:55:50.000000 gpplus-0.0.1.221/gpplus/bayesian_optimizations/AFs.py
--rw-rw-rw-   0        0        0     8488 2024-02-15 20:55:50.000000 gpplus-0.0.1.221/gpplus/bayesian_optimizations/BO_GP_plus.py
--rw-rw-rw-   0        0        0       43 2024-02-15 20:55:50.000000 gpplus-0.0.1.221/gpplus/bayesian_optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:58.972812 gpplus-0.0.1.221/gpplus/datasets/
--rw-rw-rw-   0        0        0      156 2024-02-15 20:55:50.000000 gpplus-0.0.1.221/gpplus/datasets/HOIP_noisy.py
--rw-rw-rw-   0        0        0      114 2024-02-15 20:55:50.000000 gpplus-0.0.1.221/gpplus/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:58.996981 gpplus-0.0.1.221/gpplus/kernels/
--rw-rw-rw-   0        0        0     1308 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/kernels/Rough_RBF.py
--rw-rw-rw-   0        0        0      273 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/kernels/__init__.py
--rw-rw-rw-   0        0        0      269 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/kernels/matern.py
--rw-rw-rw-   0        0        0     1581 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/kernels/wighted_RBF.py
--rw-rw-rw-   0        0        0     4983 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/kernels/wighted_RBF_Z.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.007996 gpplus-0.0.1.221/gpplus/likelihoods_noise/
--rw-rw-rw-   0        0        0       46 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/likelihoods_noise/__init__.py
--rw-rw-rw-   0        0        0     5203 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/likelihoods_noise/multifidelity.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.021322 gpplus-0.0.1.221/gpplus/models/
--rw-rw-rw-   0        0        0       58 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/models/__init__.py
--rw-rw-rw-   0        0        0    69416 2024-02-15 20:55:51.000000 gpplus-0.0.1.221/gpplus/models/gp_plus.py
--rw-rw-rw-   0        0        0    10025 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/models/gpregression.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.048760 gpplus-0.0.1.221/gpplus/optim/
--rw-rw-rw-   0        0        0      210 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/optim/__init__.py
--rw-rw-rw-   0        0        0     8375 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/optim/mll_noise_tune.py
--rw-rw-rw-   0        0        0    10701 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/optim/mll_noise_tune2.py
--rw-rw-rw-   0        0        0    11011 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/optim/mll_noise_tune3.py
--rw-rw-rw-   0        0        0    13396 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/optim/mll_scipy.py
--rw-rw-rw-   0        0        0    10351 2024-02-15 20:55:52.000000 gpplus-0.0.1.221/gpplus/optim/mll_torch.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.069073 gpplus-0.0.1.221/gpplus/preprocessing/
--rw-rw-rw-   0        0        0      543 2024-02-15 20:55:53.000000 gpplus-0.0.1.221/gpplus/preprocessing/Data_reader.py
--rw-rw-rw-   0        0        0      158 2024-02-15 20:55:53.000000 gpplus-0.0.1.221/gpplus/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-02-15 20:55:53.000000 gpplus-0.0.1.221/gpplus/preprocessing/normalizeX.py
--rw-rw-rw-   0        0        0     2433 2024-02-15 20:55:53.000000 gpplus-0.0.1.221/gpplus/preprocessing/numericlevels.py
--rw-rw-rw-   0        0        0      742 2024-02-15 20:55:53.000000 gpplus-0.0.1.221/gpplus/preprocessing/one_hot_encoding.py
--rw-rw-rw-   0        0        0     1816 2024-02-15 20:55:53.000000 gpplus-0.0.1.221/gpplus/preprocessing/split.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.077467 gpplus-0.0.1.221/gpplus/priors/
--rw-rw-rw-   0        0        0      120 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/priors/__init__.py
--rw-rw-rw-   0        0        0     3848 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/priors/horseshoe.py
--rw-rw-rw-   0        0        0     3985 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/priors/mollified_uniform.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.091988 gpplus-0.0.1.221/gpplus/test_functions/
--rw-rw-rw-   0        0        0        1 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/test_functions/__init__.py
--rw-rw-rw-   0        0        0     8220 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/test_functions/analytical.py
--rw-rw-rw-   0        0        0    30443 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/test_functions/calibration_multi_fidelity.py
--rw-rw-rw-   0        0        0     8907 2024-02-15 20:55:54.000000 gpplus-0.0.1.221/gpplus/test_functions/multi_fidelity.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.110808 gpplus-0.0.1.221/gpplus/utils/
--rw-rw-rw-   0        0        0       30 2024-02-15 20:55:55.000000 gpplus-0.0.1.221/gpplus/utils/__init__.py
--rw-rw-rw-   0        0        0    10533 2024-02-15 20:55:55.000000 gpplus-0.0.1.221/gpplus/utils/input_space.py
--rw-rw-rw-   0        0        0      352 2024-02-15 20:55:55.000000 gpplus-0.0.1.221/gpplus/utils/interval_score.py
--rw-rw-rw-   0        0        0      437 2024-02-15 20:55:55.000000 gpplus-0.0.1.221/gpplus/utils/set_seed.py
--rw-rw-rw-   0        0        0     1097 2024-02-15 20:55:55.000000 gpplus-0.0.1.221/gpplus/utils/transforms.py
--rw-rw-rw-   0        0        0     7988 2024-02-15 20:55:55.000000 gpplus-0.0.1.221/gpplus/utils/variables.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:59.122761 gpplus-0.0.1.221/gpplus/visual/
--rw-rw-rw-   0        0        0       39 2024-02-15 20:55:56.000000 gpplus-0.0.1.221/gpplus/visual/__init__.py
--rw-rw-rw-   0        0        0     1996 2024-02-15 20:55:56.000000 gpplus-0.0.1.221/gpplus/visual/plot_latent.py
--rw-rw-rw-   0        0        0     5549 2024-02-15 22:55:20.000000 gpplus-0.0.1.221/gpplus/visual/plot_latenth.py
--rw-rw-rw-   0        0        0     2539 2024-02-15 20:55:56.000000 gpplus-0.0.1.221/gpplus/visual/plot_latenth_position.py
-drwxrwxrwx   0        0        0        0 2024-02-15 23:05:58.948281 gpplus-0.0.1.221/gpplus.egg-info/
--rw-rw-rw-   0        0        0      528 2024-02-15 23:05:58.000000 gpplus-0.0.1.221/gpplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2024-02-15 23:05:58.000000 gpplus-0.0.1.221/gpplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 23:05:58.000000 gpplus-0.0.1.221/gpplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2024-02-15 23:05:58.000000 gpplus-0.0.1.221/gpplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-15 23:05:58.000000 gpplus-0.0.1.221/gpplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-15 23:05:59.129789 gpplus-0.0.1.221/setup.cfg
--rw-rw-rw-   0        0        0      952 2024-02-15 23:02:42.000000 gpplus-0.0.1.221/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.905475 gpplus-0.0.2.1/
+-rw-rw-rw-   0        0        0      526 2024-05-28 17:45:08.904466 gpplus-0.0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.804824 gpplus-0.0.2.1/gpplus/
+-rw-rw-rw-   0        0        0       45 2024-05-26 17:25:11.000000 gpplus-0.0.2.1/gpplus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.820380 gpplus-0.0.2.1/gpplus/bayesian_optimizations/
+-rw-rw-rw-   0        0        0     4815 2024-05-26 17:25:12.000000 gpplus-0.0.2.1/gpplus/bayesian_optimizations/AFs.py
+-rw-rw-rw-   0        0        0     8488 2024-05-26 17:25:12.000000 gpplus-0.0.2.1/gpplus/bayesian_optimizations/BO_GP_plus.py
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:25:11.000000 gpplus-0.0.2.1/gpplus/bayesian_optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.823083 gpplus-0.0.2.1/gpplus/datasets/
+-rw-rw-rw-   0        0        0      156 2024-05-26 17:25:13.000000 gpplus-0.0.2.1/gpplus/datasets/HOIP_noisy.py
+-rw-rw-rw-   0        0        0      114 2024-05-26 17:25:13.000000 gpplus-0.0.2.1/gpplus/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.835501 gpplus-0.0.2.1/gpplus/kernels/
+-rw-rw-rw-   0        0        0     1308 2024-05-26 17:25:13.000000 gpplus-0.0.2.1/gpplus/kernels/Rough_RBF.py
+-rw-rw-rw-   0        0        0      273 2024-05-26 17:25:13.000000 gpplus-0.0.2.1/gpplus/kernels/__init__.py
+-rw-rw-rw-   0        0        0      269 2024-05-26 17:25:13.000000 gpplus-0.0.2.1/gpplus/kernels/matern.py
+-rw-rw-rw-   0        0        0     1581 2024-05-26 17:25:13.000000 gpplus-0.0.2.1/gpplus/kernels/wighted_RBF.py
+-rw-rw-rw-   0        0        0     4983 2024-05-26 17:25:14.000000 gpplus-0.0.2.1/gpplus/kernels/wighted_RBF_Z.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.838500 gpplus-0.0.2.1/gpplus/likelihoods_noise/
+-rw-rw-rw-   0        0        0       46 2024-05-26 17:25:14.000000 gpplus-0.0.2.1/gpplus/likelihoods_noise/__init__.py
+-rw-rw-rw-   0        0        0     6470 2024-05-26 17:25:14.000000 gpplus-0.0.2.1/gpplus/likelihoods_noise/multifidelity.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.843503 gpplus-0.0.2.1/gpplus/models/
+-rw-rw-rw-   0        0        0       58 2024-05-26 17:25:15.000000 gpplus-0.0.2.1/gpplus/models/__init__.py
+-rw-rw-rw-   0        0        0    73909 2024-05-28 16:36:23.000000 gpplus-0.0.2.1/gpplus/models/gp_plus.py
+-rw-rw-rw-   0        0        0    10396 2024-05-26 17:25:15.000000 gpplus-0.0.2.1/gpplus/models/gpregression.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.851151 gpplus-0.0.2.1/gpplus/optim/
+-rw-rw-rw-   0        0        0      137 2024-05-26 17:25:16.000000 gpplus-0.0.2.1/gpplus/optim/__init__.py
+-rw-rw-rw-   0        0        0    10973 2024-05-26 17:25:16.000000 gpplus-0.0.2.1/gpplus/optim/mll_noise_continuation.py
+-rw-rw-rw-   0        0        0    13476 2024-05-26 17:25:16.000000 gpplus-0.0.2.1/gpplus/optim/mll_scipy.py
+-rw-rw-rw-   0        0        0     6631 2024-05-26 17:25:17.000000 gpplus-0.0.2.1/gpplus/optim/mll_torch.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.863195 gpplus-0.0.2.1/gpplus/preprocessing/
+-rw-rw-rw-   0        0        0      543 2024-05-26 17:25:18.000000 gpplus-0.0.2.1/gpplus/preprocessing/Data_reader.py
+-rw-rw-rw-   0        0        0      158 2024-05-26 17:25:18.000000 gpplus-0.0.2.1/gpplus/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-05-26 17:25:18.000000 gpplus-0.0.2.1/gpplus/preprocessing/normalizeX.py
+-rw-rw-rw-   0        0        0     1671 2024-05-26 17:25:18.000000 gpplus-0.0.2.1/gpplus/preprocessing/numericlevels.py
+-rw-rw-rw-   0        0        0      742 2024-05-26 17:25:18.000000 gpplus-0.0.2.1/gpplus/preprocessing/one_hot_encoding.py
+-rw-rw-rw-   0        0        0     1816 2024-05-26 17:25:18.000000 gpplus-0.0.2.1/gpplus/preprocessing/split.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.871713 gpplus-0.0.2.1/gpplus/priors/
+-rw-rw-rw-   0        0        0      120 2024-05-26 17:25:19.000000 gpplus-0.0.2.1/gpplus/priors/__init__.py
+-rw-rw-rw-   0        0        0     3848 2024-05-26 17:25:19.000000 gpplus-0.0.2.1/gpplus/priors/horseshoe.py
+-rw-rw-rw-   0        0        0     3985 2024-05-26 17:25:19.000000 gpplus-0.0.2.1/gpplus/priors/mollified_uniform.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.880800 gpplus-0.0.2.1/gpplus/test_functions/
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:25:20.000000 gpplus-0.0.2.1/gpplus/test_functions/__init__.py
+-rw-rw-rw-   0        0        0     8205 2024-05-26 17:25:20.000000 gpplus-0.0.2.1/gpplus/test_functions/analytical.py
+-rw-rw-rw-   0        0        0    30443 2024-05-26 17:25:20.000000 gpplus-0.0.2.1/gpplus/test_functions/calibration_multi_fidelity.py
+-rw-rw-rw-   0        0        0     8907 2024-05-26 17:25:20.000000 gpplus-0.0.2.1/gpplus/test_functions/multi_fidelity.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.894472 gpplus-0.0.2.1/gpplus/utils/
+-rw-rw-rw-   0        0        0       76 2024-05-26 17:25:21.000000 gpplus-0.0.2.1/gpplus/utils/__init__.py
+-rw-rw-rw-   0        0        0      461 2024-05-26 17:25:21.000000 gpplus-0.0.2.1/gpplus/utils/data_type_check.py
+-rw-rw-rw-   0        0        0    10533 2024-05-26 17:25:21.000000 gpplus-0.0.2.1/gpplus/utils/input_space.py
+-rw-rw-rw-   0        0        0      361 2024-05-26 17:25:21.000000 gpplus-0.0.2.1/gpplus/utils/interval_score.py
+-rw-rw-rw-   0        0        0      437 2024-05-26 17:25:22.000000 gpplus-0.0.2.1/gpplus/utils/set_seed.py
+-rw-rw-rw-   0        0        0     1097 2024-05-26 17:25:22.000000 gpplus-0.0.2.1/gpplus/utils/transforms.py
+-rw-rw-rw-   0        0        0     7988 2024-05-26 17:25:22.000000 gpplus-0.0.2.1/gpplus/utils/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.903465 gpplus-0.0.2.1/gpplus/visual/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:25:23.000000 gpplus-0.0.2.1/gpplus/visual/__init__.py
+-rw-rw-rw-   0        0        0     1996 2024-05-26 17:25:23.000000 gpplus-0.0.2.1/gpplus/visual/plot_latent.py
+-rw-rw-rw-   0        0        0     5549 2024-05-26 17:25:23.000000 gpplus-0.0.2.1/gpplus/visual/plot_latenth.py
+-rw-rw-rw-   0        0        0     2539 2024-05-26 17:25:23.000000 gpplus-0.0.2.1/gpplus/visual/plot_latenth_position.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:08.816375 gpplus-0.0.2.1/gpplus.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-05-28 17:45:08.000000 gpplus-0.0.2.1/gpplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1556 2024-05-28 17:45:08.000000 gpplus-0.0.2.1/gpplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 17:45:08.000000 gpplus-0.0.2.1/gpplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2024-05-28 17:45:08.000000 gpplus-0.0.2.1/gpplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 17:45:08.000000 gpplus-0.0.2.1/gpplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 17:45:08.906474 gpplus-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      949 2024-05-28 17:42:14.000000 gpplus-0.0.2.1/setup.py
```

### Comparing `gpplus-0.0.1.221/PKG-INFO` & `gpplus-0.0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gpplus
-Version: 0.0.1.221
+Version: 0.0.2.1
 Summary: Python Library for Generalized Gaussian Process Modeling
 Home-page: https://github.com/Bostanabad-Research-Group/GP-Plus
 Author: Amin Yousefpour, Ramin Bostanabad
 Author-email: yousefpo@uci.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 UNKNOWN
```

### Comparing `gpplus-0.0.1.221/gpplus/bayesian_optimizations/AFs.py` & `gpplus-0.0.2.1/gpplus/bayesian_optimizations/AFs.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/bayesian_optimizations/BO_GP_plus.py` & `gpplus-0.0.2.1/gpplus/bayesian_optimizations/BO_GP_plus.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/kernels/Rough_RBF.py` & `gpplus-0.0.2.1/gpplus/kernels/Rough_RBF.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/kernels/wighted_RBF.py` & `gpplus-0.0.2.1/gpplus/kernels/wighted_RBF.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/kernels/wighted_RBF_Z.py` & `gpplus-0.0.2.1/gpplus/kernels/wighted_RBF_Z.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/likelihoods_noise/multifidelity.py` & `gpplus-0.0.2.1/gpplus/likelihoods_noise/multifidelity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright © 2023, Dr. Bostanabad's research group at the University of California, Irvine.
+# 
+# GP+ Intellectual Property Notice:
+# 
+# The software known as GP+ is the proprietary material of Dr. Bostanabad's research group at the University of California, Irvine. 
+# Non-profit academic institutions and U.S. government agencies may utilize this software exclusively for educational and research endeavors. 
+# All other entities are granted permission for evaluation purposes solely; any additional utilization demands prior written consent from the appropriate authority. 
+# The direct sale or redistribution of this software, in any form, without explicit written authorization is strictly prohibited. 
+# Users are permitted to make duplicate copies of the software, contingent upon the assurance that no copies are sold or redistributed and they adhere to the stipulated terms herein.
+# 
+# Being academic research software, GP+ is provided on an "as is" m_gp, devoid of warranties, whether explicit or implicit. 
+# The act of downloading or executing any segment of this software inherently signifies compliance with these terms. 
+# The developers reserve the right to modify these terms and conditions without prior intimation at any juncture.
+
 from distutils.log import error
 from turtle import forward
 from gpytorch.likelihoods import _GaussianLikelihoodBase
 from gpytorch.likelihoods.noise_models import _HomoskedasticNoiseBase
 from sklearn.covariance import log_likelihood
 import torch
 from typing import Any, Optional
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpplus-0.0.1.221/gpplus/models/gp_plus.py` & `gpplus-0.0.2.1/gpplus/models/gp_plus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,395 +1,398 @@
-# Copyright © 2023, University of California, Irvine.
+# Copyright © 2023, Dr. Bostanabad's research group at the University of California, Irvine.
 # 
 # GP+ Intellectual Property Notice:
 # 
-# The software known as GP+ is the proprietary material of the University of California, Irvine. 
+# The software known as GP+ is the proprietary material of Dr. Bostanabad's research group at the University of California, Irvine. 
 # Non-profit academic institutions and U.S. government agencies may utilize this software exclusively for educational and research endeavors. 
 # All other entities are granted permission for evaluation purposes solely; any additional utilization demands prior written consent from the appropriate authority. 
 # The direct sale or redistribution of this software, in any form, without explicit written authorization is strictly prohibited. 
 # Users are permitted to make duplicate copies of the software, contingent upon the assurance that no copies are sold or redistributed and they adhere to the stipulated terms herein.
 # 
-# Being academic research software, GP+ is provided on an "as is" base, devoid of warranties, whether explicit or implicit. 
+# Being academic research software, GP+ is provided on an "as is" m_gp, devoid of warranties, whether explicit or implicit. 
 # The act of downloading or executing any segment of this software inherently signifies compliance with these terms. 
-# The University of California, Irvine reserves the right to modify these terms and conditions without prior intimation at any juncture.
+# The developers reserve the right to modify these terms and conditions without prior intimation at any juncture.
+import numpy as np
+from typing import Dict,List,Optional
+import math
+from scipy.stats import norm
+import matplotlib.pyplot as plt
+from tabulate import tabulate
+import sobol_seq
+import warnings
 
 import torch
-import math
+from torch import nn
+from torch import Tensor 
+from torch.nn.parameter import Parameter
+from torch.nn import init
+import torch.nn.functional as F 
+
 import gpytorch
-from typing import Dict,List,Optional
 from gpytorch.constraints import Positive
+from gpytorch.means import Mean
 from gpytorch.priors import NormalPrior
 from gpytorch.distributions import MultivariateNormal
-from ..priors import MollifiedUniformPrior
+
 from gpplus.visual.plot_latenth import plot_sep
 from gpplus.models.gpregression import GPR
 from gpplus import kernels
 from gpplus.priors import MollifiedUniformPrior
-import numpy as np
 from gpplus.preprocessing import setlevels
-import matplotlib.pyplot as plt
-import torch
-from gpytorch.means import Mean
-import torch
-from tabulate import tabulate
-from gpplus.utils import set_seed
-from gpplus.optim import fit_model_scipy, noise_tune2, fit_model_torch
-import torch
-import numpy as np
-import sobol_seq
-import warnings
-from torch import Tensor
-from gpytorch.means import Mean
-from torch.nn.parameter import Parameter
-from torch.nn import init
-from torch import nn
-import torch.nn.functional as F 
-from scipy.stats import norm
+from gpplus.utils import set_seed, data_type_check
+from gpplus.optim import fit_model_scipy, fit_model_continuation, fit_model_torch
 
 
 class GP_Plus(GPR):
-    """The GP_Plus which extends GPs to learn nonlinear and probabilistic nmanifold, handle categorical inputs, and  ... ...
+    """The GP_Plus class extends Gaussian Processes (GPs) to learn nonlinear and probabilistic manifolds, handle categorical inputs, and more.
 
     :note: Binary categorical variables should not be treated as qualitative inputs. There is no 
         benefit from applying a latent variable treatment for such variables. Instead, treat them
         as numerical inputs.
-
-    :param train_x: The training inputs (size N x d). Qualitative inputs needed to be encoded as 
-        integers 0,...,L-1 where L is the number of levels. For best performance, scale the 
-        numerical variables to the unit hypercube.
+    
+    :param train_x: The training inputs. This represents the input data.
+    :param train_y: The training outputs. This represents the output data.
+    :param dtype: The data type of the model and data, which could be float32 or float64 torch tensor.
+    :param device: Specifies whether the model will be built on CPU or CUDA if available. Otherwise, it should always be CPU.
+    :param qual_index: A dictionary that indicates categorical inputs. The keys represent the number of columns that are categorical, starting from 0, and the values indicate the number of levels for each specific categorical input.
+    :param multiple_noise: Used in cases where there are multiple sources of data (multiple fidelity emulation), allowing for different noise estimation for each fidelity data source.
+    :param lb_noise: The lower bound for noise estimation.
+    :param fix_noise: Determines whether to fix noise to a specific value. It can be True or False. If True, it indicates that noise should be fixed.
+    :param fix_noise_val: The value to which noise is fixed when `fix_noise` is True.
+    :param quant_correlation_class: The class of correlation used in the model.
+    :param fixed_length_scale: Indicates whether the length scale should be fixed. It can be True or False. If True, the length scale will be fixed.
+    :param fixed_length_scale_val: The value of the length scale in fixed scenarios.
+    :param encoding_type: The type of encoding used for categorical inputs.
+    :param embedding_dim: The dimension of the encoding (dimension of embedding).
+    :param separate_embedding: Specifies the layers in the embedding used for mapping.
+    :param embedding_type: The type of embedding, could be 'deterministic' or 'probabilistic'.
+    :param NN_layers_embedding: A list that shows the architecture of neural network layers for the embedding.
+    :param m_gp: Specifies the type of mean function considered for the GP model.
+    :param m_gp_ref: The mean function for the reference source, which has an ID equal to 0.
+    :param NN_layers_m_gp: A list that shows the architecture of the neural network used in the GP model for cases where a neural network is used as the mean function.
+    :param calibration_type: The type of calibration used, could be 'deterministic' or 'probabilistic'.
+    :param calibration_id: A list that indicates the inputs that have calibration parameters.
+    :param mean_prior_cal: The mean prior used for calibration, which should have the same length as `calibration_id`.
+    :param std_prior_cal: The standard deviation prior used for calibration, which should have the same length as `calibration_id`.
+    :param interval_score: Indicates whether to add interval scoring during optimization.It can be True or False. If True, it is added by default with a coefficient of 0.08.
+    :param seed_number: The seed number for random number generation to ensure reproducible results.
     """
     def __init__(
         self,
         train_x:torch.Tensor,
         train_y:torch.Tensor,
-        qual_ind_lev = {},
+        dtype= torch.float,
+        device="cpu",
+        qual_index = {},
         multiple_noise = False,
-        lv_dim:int=2,
-        quant_correlation_class:str='Rough_RBF',
-        noise:float=1e-4,
+        lb_noise:float=1e-8,
         fix_noise:bool=False,
+        fix_noise_val:float=1e-5,
+        quant_correlation_class:str='Rough_RBF',
         fixed_length_scale:bool=False,
-        fixed_omega=torch.tensor([1.0]),
-        lb_noise:float=1e-8,
-        NN_layers:list = [],
+        fixed_length_scale_val=torch.tensor([1.0]),
         encoding_type = 'one-hot',
-        manifold_type='deterministic',
-        uniform_encoding_columns = 2,
-        lv_columns = [] ,
-        base='single_constant',
-        base_hf='zero',
-        NN_layers_base=[],
-        base_function_size=None,
-        calibration_id=[],
-        seed_number=1,
-        mean_prior_cal=0,
-        std_prior_cal=1,
+        embedding_dim:int=2,
+        separate_embedding = [] , #max=2
+        embedding_type='deterministic',
+        NN_layers_embedding:list = [],
+        m_gp='single_constant',
+        m_gp_ref='zero',
+        NN_layers_m_gp=[],
         calibration_type='deterministic',
-        device="cpu",
-        dtype= torch.float,
-        IS=False
+        calibration_id=[],
+        mean_prior_cal=None,  
+        std_prior_cal=None,  
+        interval_score=False,
+        num_pass_train=1,
+        num_pass_pred=1,
+        seed_number=1
     ) -> None:
+        if calibration_type=='probabelistic' or  calibration_type=='probabelistic':
+            num_pass_train=20
+            num_pass_pred=30
+        
+        if mean_prior_cal is None:
+            mean_prior_cal = [0 for _ in calibration_id]
+        if std_prior_cal is None:
+            std_prior_cal = [1 for _ in calibration_id]
+        
+        self.mean_prior_cal=mean_prior_cal
+        self.std_prior_cal=std_prior_cal
         
-        self.IS=IS
+        self.interval_score=interval_score
         tkwargs = {}  # or dict()
         tkwargs['dtype'] = dtype
         tkwargs['device'] =torch.device(device)
         self.tkwargs=tkwargs
 
 
         self.mean_prior_cal=mean_prior_cal
         self.std_prior_cal=std_prior_cal
         if fixed_length_scale:
-            self.fixed_omega=fixed_omega.to(**self.tkwargs)
+            self.fixed_length_scale_val=fixed_length_scale_val.to(**self.tkwargs)
         else:
-            self.fixed_omega=None
+            self.fixed_length_scale_val=None
             
-        ## The checks lists:
-        if not isinstance(train_x, torch.Tensor):
-            original_type = type(train_x).__name__
-            warnings.warn(f"'train_x' was not a torch.Tensor (type: {original_type}). It is converted to torch.Tensor to proceed with the emulation.")
-            train_x = torch.tensor(train_x)
-
-        if not isinstance(train_y, torch.Tensor):
-            original_type = type(train_y).__name__
-            warnings.warn(f"'train_y' was not a torch.Tensor (type: {original_type}). It is converted to torch.Tensor to proceed with the emulation.")
-            train_y = torch.tensor(train_y)
+        # Checking inputs & output
+        train_x=data_type_check(train_x)
+        train_y=data_type_check(train_y)
 
-        if not isinstance(qual_ind_lev, dict):
-            raise ValueError("qual_ind_lev should be a dictionary")
+        if not isinstance(qual_index, dict):
+            raise ValueError("qual_index should be a dictionary.") 
 
         if multiple_noise not in [True, False]:
-            raise ValueError("multiple_noise should be either True or False")
+            raise ValueError("multiple_noise should be either True or False.")
 
-        if not isinstance(lv_dim, int):
-            raise ValueError("lv_dim should be an integer")
+        if not isinstance(embedding_dim, int):
+            raise ValueError("embedding_dim should be an integer.")
 
         if quant_correlation_class not in ['Rough_RBF', 'RBFKernel', 'Matern32Kernel', 'Matern12Kernel','Matern52Kernel']:
-            raise ValueError("quant_correlation_class should be 'Rough_RBF', 'RBFKernel', 'Matern32Kernel', 'Matern12Kernel','Matern52Kernel'")
+            raise ValueError("quant_correlation_class should be 'Rough_RBF', 'RBFKernel', 'Matern32Kernel', 'Matern12Kernel','Matern52Kernel'.")
 
         if fix_noise not in [True, False]:
-            raise ValueError("fix_noise should be either True or False")
+            raise ValueError("fix_noise should be either True or False.")
 
-        if not isinstance(NN_layers, list) or not all(isinstance(i, int) for i in NN_layers):
-            raise ValueError("NN_layers should be a list with integers representing the number of neurons in each layer for mapping the manifold")
+        if not isinstance(NN_layers_embedding, list) or not all(isinstance(i, int) for i in NN_layers_embedding):
+            raise ValueError("NN_layers_embedding should be a list of integers representing the number of neurons in each layer.")
 
         if encoding_type != 'one-hot':
-            raise ValueError("encoding_type should be 'one-hot'")
+            raise ValueError("encoding_type should be 'one-hot'.")
 
-        if manifold_type not in ['deterministic', 'probabilistic']:
-            raise ValueError("manifold_type should be either 'deterministic' or 'probabilistic'")
+        if embedding_type not in ['deterministic', 'probabilistic']:
+            raise ValueError("embedding_type should be either 'deterministic' or 'probabilistic'.")
 
-        if not isinstance(lv_columns, list) or not all(isinstance(i, int) for i in lv_columns):
-            raise ValueError("lv_columns should be a list with integers showing the number of categorical inputs to be considered in a separate manifold in each layer")
+        if not isinstance(separate_embedding, list) or not all(isinstance(i, int) for i in separate_embedding):
+            raise ValueError("separate_embedding should be a list with integers showing the number of categorical inputs to be considered in a separate manifold in each layer.")
 
     
         supported_singl_functions = ['single_sin', 'single_cos', 'single_exp', 'single_log', 'single_tan', 'single_asin', 'single_acos', 'single_atan', 
                                     'single_sinh', 'single_cosh', 'single_tanh', 'single_asinh', 'single_acosh', 'single_atanh', 'single_sqrt', 
-                                    'single_abs', 'single_ceil', 'single_floor', 'single_round']
+                                    'single_abs', 'single_ceil', 'single_floor', 'single_round'] ########## single_functions!!!!
 
-        self.supported_singl_base_functions=supported_singl_functions
+        self.supported_singl_m_gp_functions=supported_singl_functions
         
-        supported_multi_base_functions=['single_zero', 'single_polynomial', 'single_constant', 'multiple_polynomial_2d', 'multiple_constant', 'neural_network']
+        supported_multi_m_gp_functions=['single_zero', 'single_polynomial', 'single_constant', 'multiple_polynomial_2d', 'multiple_constant', 'neural_network']
 
-        #if base not in supported_multi_base_functions and base not in supported_singl_functions:
-        #     raise ValueError("base is not valied'")
 
-        if not isinstance(NN_layers_base, list) or not all(isinstance(i, int) for i in NN_layers_base):
-            raise ValueError("NN_layers_base should be a list with integers representing the number of neurons in each layer for the mean function")
+        if not isinstance(NN_layers_m_gp, list) or not all(isinstance(i, int) for i in NN_layers_m_gp):
+            raise ValueError("NN_layers_m_gp should be a list with integers representing the number of neurons in each layer for the mean function.")
 
         if not isinstance(calibration_id, list) or not all(isinstance(i, int) for i in calibration_id):
-            raise ValueError("calibration_id should be a list where each entry shows the column number in the dataset that the calibration parameters are assigned to")
+            raise ValueError("calibration_id should be a list where each entry shows the column number in the dataset that the calibration parameters are assigned to.")
         
         train_x=self.fill_nan_with_mean(train_x,calibration_id)
         ###############################################################################################
         ###############################################################################################
         self.seed=seed_number
         self.calibration_id=calibration_id
         self.calibration_source_index=0    ## It is supposed the calibration parameter is for high fidelity needs
-        qual_index = list(qual_ind_lev.keys())
+        qual_index_list = list(qual_index.keys())
         all_index = set(range(train_x.shape[-1]))
-        quant_index = list(all_index.difference(qual_index))
-        num_levels_per_var = list(qual_ind_lev.values())
+        quant_index = list(all_index.difference(qual_index_list))
+        num_levels_per_var = list(qual_index.values())
         #------------------- lm columns --------------------------
-        lm_columns = list(set(qual_index).difference(lv_columns))
+        lm_columns = list(set(qual_index_list).difference(separate_embedding))
         if len(lm_columns) > 0:
-            qual_kernel_columns = [*lv_columns, lm_columns]
+            qual_kernel_columns = [*separate_embedding, lm_columns]
         else:
-            qual_kernel_columns = lv_columns
+            qual_kernel_columns = separate_embedding
         #########################
-        if len(qual_index) > 0:
-            train_x = torch.tensor(setlevels(train_x, qual_index=qual_index))#.to(**self.tkwargs)
-        #
-        # train_x=train_x.to(**self.tkwargs)
-        train_y=train_y.reshape(-1)#.to(**self.tkwargs)
+        train_y=train_y.reshape(-1)
         if multiple_noise:
             noise_indices = list(range(0,num_levels_per_var[-1]))
         else:
             noise_indices = []
 
-        if len(qual_index) == 1 and num_levels_per_var[0] < 2:
+        if len(qual_index_list) == 1 and num_levels_per_var[0] < 2:
             temp = quant_index.copy()
-            temp.append(qual_index[0])
+            temp.append(qual_index_list[0])
             quant_index = temp.copy()
-            qual_index = []
-            lv_dim = 0
-        elif len(qual_index) == 0:
-            lv_dim = 0
-
-        quant_correlation_class_name = quant_correlation_class
-
-        if len(qual_index) == 0:
-            lv_dim = 0
-        if quant_correlation_class_name == 'Rough_RBF':
-            quant_correlation_class = 'RBFKernel'
-
-        if quant_correlation_class_name == 'Matern32Kernel':
-            quant_correlation_class = 'Matern32Kernel'
-        
-        if quant_correlation_class_name == 'Matern52Kernel':
-            quant_correlation_class = 'Matern52Kernel'
+            qual_index_list = []
+            embedding_dim = 0
+        elif len(qual_index_list) == 0:
+            embedding_dim = 0
 
-        if quant_correlation_class_name == 'Matern12Kernel':
-            quant_correlation_class = 'Matern12Kernel'
+        if len(qual_index_list) == 0:
+            embedding_dim = 0
 
-        if len(qual_index) > 0:
+        if len(qual_index_list) > 0:
             ####################### Defined multiple kernels for seperate variables ###################
             qual_kernels = []
             for i in range(len(qual_kernel_columns)):
                 qual_kernels.append(kernels.RBFKernel(
-                    active_dims=torch.arange(lv_dim) + lv_dim * i) )
+                    active_dims=torch.arange(embedding_dim) + embedding_dim * i) )
                 qual_kernels[i].initialize(**{'lengthscale':1.0})
                 qual_kernels[i].raw_lengthscale.requires_grad_(False)
                 
-
+        quant_correlation_class_name = quant_correlation_class  
+        if quant_correlation_class_name == 'Rough_RBF':
+            quant_correlation_class = 'RBFKernel'
         if len(quant_index) == 0:
             correlation_kernel = qual_kernels[0]
             for i in range(1, len(qual_kernels)):
                 correlation_kernel *= qual_kernels[i]
         else:
             try:
                 quant_correlation_class = getattr(kernels,quant_correlation_class)
             except:
                 raise RuntimeError(
                     "%s not an allowed kernel" % quant_correlation_class
                 )
             if quant_correlation_class_name == 'RBFKernel':
                 quant_kernel = quant_correlation_class(
                     ard_num_dims=len(quant_index),
-                    active_dims=len(qual_kernel_columns) * lv_dim+torch.arange(len(quant_index)),
+                    active_dims=len(qual_kernel_columns) * embedding_dim+torch.arange(len(quant_index)),
                     lengthscale_constraint= Positive(transform= torch.exp,inv_transform= torch.log)
                 )
             elif quant_correlation_class_name == 'Rough_RBF':
                 quant_kernel = quant_correlation_class(
                     ard_num_dims=len(quant_index),
-                    active_dims=len(qual_kernel_columns)*lv_dim+torch.arange(len(quant_index)),
+                    active_dims=len(qual_kernel_columns)*embedding_dim+torch.arange(len(quant_index)),
                     lengthscale_constraint= Positive(transform= lambda x: 2.0**(-0.5) * torch.pow(10,-x/2),inv_transform= lambda x: -2.0*torch.log10(x/2.0))
                 )
             elif quant_correlation_class_name == 'Matern12Kernel':
                 quant_kernel = quant_correlation_class(
                     ard_num_dims=len(quant_index),
-                    active_dims=len(qual_kernel_columns)*lv_dim+torch.arange(len(quant_index)),
+                    active_dims=len(qual_kernel_columns)*embedding_dim+torch.arange(len(quant_index)),
                     lengthscale_constraint= Positive(transform= lambda x: 2.0**(-0.5) * torch.pow(10,-x/2),inv_transform= lambda x: -2.0*torch.log10(x/2.0))
                 )
             
             elif quant_correlation_class_name == 'Matern32Kernel':
                 quant_kernel = quant_correlation_class(
                     ard_num_dims=len(quant_index),
-                    active_dims=len(qual_kernel_columns)*lv_dim+torch.arange(len(quant_index)),
-                    #lengthscale_constraint= Positive(transform= torch.exp,inv_transform= torch.log)
+                    active_dims=len(qual_kernel_columns)*embedding_dim+torch.arange(len(quant_index)),
                     lengthscale_constraint= Positive(transform= lambda x: 2.0**(-0.5) * torch.pow(10,-x/2),inv_transform= lambda x: -2.0*torch.log10(x/2.0))             
                 )
             elif quant_correlation_class_name == 'Matern52Kernel':
                 quant_kernel = quant_correlation_class(
                     ard_num_dims=len(quant_index),
-                    active_dims=len(qual_kernel_columns)*lv_dim+torch.arange(len(quant_index)),
-                    #lengthscale_constraint= Positive(transform= torch.exp,inv_transform= torch.log)  
+                    active_dims=len(qual_kernel_columns)*embedding_dim+torch.arange(len(quant_index)),
                     lengthscale_constraint= Positive(transform= lambda x: 2.0**(-0.5) * torch.pow(10,-x/2),inv_transform= lambda x: -2.0*torch.log10(x/2.0))       
                 )
                 #####################
             if quant_correlation_class_name == 'RBFKernel':
                 quant_kernel.register_prior(
                     'lengthscale_prior', MollifiedUniformPrior(math.log(0.1),math.log(10)),'raw_lengthscale'
                 )
                 
             elif quant_correlation_class_name == 'Rough_RBF':
                 quant_kernel.register_prior(
                     'lengthscale_prior',NormalPrior(-3.0,3.0),'raw_lengthscale'
                 )
             elif quant_correlation_class_name == 'Matern12Kernel':
                 quant_kernel.register_prior(
-                    #'lengthscale_prior', MollifiedUniformPrior(math.log(0.1),math.log(10)),'raw_lengthscale'
                     'lengthscale_prior',NormalPrior(-3.0,3.0),'raw_lengthscale'
                 )
 
             elif quant_correlation_class_name == 'Matern32Kernel':
                 quant_kernel.register_prior(
-                    #'lengthscale_prior', MollifiedUniformPrior(math.log(0.1),math.log(10)),'raw_lengthscale'
                     'lengthscale_prior',NormalPrior(-3.0,3.0),'raw_lengthscale'
                 )
 
             elif quant_correlation_class_name == 'Matern52Kernel':
                 quant_kernel.register_prior(
-                    #'lengthscale_prior', MollifiedUniformPrior(math.log(0.1),math.log(10)),'raw_lengthscale'
                     'lengthscale_prior',NormalPrior(-3.0,3.0),'raw_lengthscale'
                 )
-            if len(qual_index) > 0:
+            if len(qual_index_list) > 0:
                 temp = qual_kernels[0]
                 for i in range(1, len(qual_kernels)):
                     temp *= qual_kernels[i]
                 correlation_kernel = temp*quant_kernel #+ qual_kernel + quant_kernel
             else:
                 correlation_kernel = quant_kernel
-
+            #####################
         super(GP_Plus,self).__init__(
             train_x=train_x,train_y=train_y,noise_indices=noise_indices,
             correlation_kernel=correlation_kernel,
-            noise=noise,fix_noise=fix_noise,lb_noise=lb_noise
+            fix_noise=fix_noise,fix_noise_val=fix_noise_val,lb_noise=lb_noise
         )
 
         self.calibration_type=calibration_type
-        for n in self.calibration_id:
-            if self.calibration_type=='probabilistic':
-                setattr(self,'Theta_'+str(n), LinearVariational(batch_shape=torch.Size([]),mean_prior=self.mean_prior_cal,std_prior=0*self.std_prior_cal).to(**tkwargs)) 
-                setattr(self,'calibration_element'+str(n), torch.where(train_x[:, -1]==self.calibration_source_index)[0]) 
+        for n, mean_prior, std_prior in zip(self.calibration_id, self.mean_prior_cal, self.std_prior_cal):
+            if self.calibration_type == 'probabilistic':
+                setattr(self, 'Theta_' + str(n), LinearVariational(batch_shape=torch.Size([]), mean_prior=mean_prior, std_prior=0*std_prior).to(**tkwargs))
+                setattr(self, 'calibration_element' + str(n), torch.where(train_x[:, -1] == self.calibration_source_index)[0])
             else:
-                setattr(self,'Theta_'+str(n), gpytorch.means.ConstantMean(prior=NormalPrior(self.mean_prior_cal,self.std_prior_cal))) 
-                setattr(self,'calibration_element'+str(n), torch.where(train_x[:, -1]==self.calibration_source_index)[0]) 
-            train_x[getattr(self,'calibration_element'+str(n)),n]=torch.zeros_like(train_x[getattr(self,'calibration_element'+str(n)),n])
-        
+                setattr(self, 'Theta_' + str(n), gpytorch.means.ConstantMean(prior=NormalPrior(mean_prior, std_prior)))
+                setattr(self, 'calibration_element' + str(n), torch.where(train_x[:, -1] == self.calibration_source_index)[0])
+
+            train_x[getattr(self, 'calibration_element' + str(n)), n] = torch.zeros_like(train_x[getattr(self, 'calibration_element' + str(n)), n])
+
         # register index and transforms
         self.register_buffer('quant_index',torch.tensor(quant_index))
-        self.register_buffer('qual_index',torch.tensor(qual_index))
+        self.register_buffer('qual_index_list',torch.tensor(qual_index_list))
 
         self.qual_kernel_columns = qual_kernel_columns
         # latent variable mapping
         self.num_levels_per_var = num_levels_per_var
-        self.lv_dim = lv_dim
-        self.uniform_encoding_columns = uniform_encoding_columns
+        self.embedding_dim = embedding_dim
         self.encoding_type = encoding_type
-        self.manifold_type=manifold_type
+        self.embedding_type=embedding_type
         self.perm =[]
         self.zeta = []
         self.random_zeta=[]
         self.perm_dict = []
         self.A_matrix = []
         self.epsilon=None
         self.epsilon_f=None
         self.embeddings_Dtrain=[]
         self.count=train_x.size()[0]
+        self.num_pass_train=num_pass_train
+        self.num_pass_pred=num_pass_pred
         if len(qual_kernel_columns) > 0:
             for i in range(len(qual_kernel_columns)):
                 if type(qual_kernel_columns[i]) == int:
-                    num = self.num_levels_per_var[qual_index.index(qual_kernel_columns[i])]
+                    num = self.num_levels_per_var[qual_index_list.index(qual_kernel_columns[i])]
                     cat = [num]
                 else:
-                    cat = [self.num_levels_per_var[qual_index.index(k)] for k in qual_kernel_columns[i]]
+                    cat = [self.num_levels_per_var[qual_index_list.index(k)] for k in qual_kernel_columns[i]]
                     num = sum(cat)
 
-                zeta, perm, perm_dict = self.zeta_matrix(num_levels=cat, lv_dim = self.lv_dim)
+                zeta, perm, perm_dict = self.zeta_matrix(num_levels=cat, embedding_dim = self.embedding_dim)
                 self.zeta.append(zeta)
                 self.perm.append(perm)
                 self.perm_dict.append(perm_dict)       
                 ###################################  latent map (manifold) #################################   
-                if self.manifold_type=='probabilistic':
+                if self.embedding_type=='probabilistic':
                     setattr(self,'A_matrix', Variational_Encoder(self, input_size= num, num_classes=5, 
-                        layers =NN_layers, name = str(qual_kernel_columns[i])).to(**tkwargs))
+                        layers =NN_layers_embedding, name = str(qual_kernel_columns[i])).to(**tkwargs))
                 else:
-                    model_temp = FFNN(self, input_size= num, num_classes=lv_dim, 
-                        layers = NN_layers, name ='latent'+ str(qual_kernel_columns[i])).to(**self.tkwargs)
+                    model_temp = FFNN(self, input_size= num, num_classes=embedding_dim, 
+                        layers = NN_layers_embedding, name ='latent'+ str(qual_kernel_columns[i])).to(**self.tkwargs)
                     self.A_matrix.append(model_temp)
 
         ##################################################################################
         if fixed_length_scale == True:
-            self.covar_module.base_kernel.raw_lengthscale.data = self.fixed_omega #torch.tensor([self.omega, self.omega])  # Set the desired value
-            self.covar_module.base_kernel.raw_lengthscale.requires_grad = False  # Fix the hyperparameter
+            self.covar_module.m_gp_kernel.raw_lengthscale.data = self.fixed_length_scale_val 
+            self.covar_module.m_gp_kernel.raw_lengthscale.requires_grad = False  
         ###################################  Mean Function #################################   
         i=0
-        self.base=base
-        self.base_hf=base_hf
+        self.m_gp=m_gp
+        self.m_gp_ref=m_gp_ref
         self.num_sources=int(torch.max(train_x[:,-1]))
         size=train_x.shape[1]
-        if self.base.startswith('single'):
-            self.single_base_register(size,base_type=self.base,wm='mean_module')
-        elif self.base.startswith('multi'):
-            self.multi_base_register (train_x,supported_multi_base_functions,self.base_hf)
-        elif self.base=='neural_network': ###### One NN for ALL 
-            setattr(self,'mean_module_NN_All', FFNN_as_Mean(self, input_size= train_x.shape[1]+2*len(qual_index)-len(qual_index), num_classes=1,layers =NN_layers_base, name = str('mean_module_'+str(i)+'_')).to(**tkwargs)) 
+        if self.m_gp.startswith('single'):
+            self.single_m_gp_register(size,m_gp_type=self.m_gp,wm='mean_module')
+        elif self.m_gp.startswith('multi'):
+            self.multi_m_gp_register (train_x,supported_multi_m_gp_functions,self.m_gp_ref)
+        elif self.m_gp=='neural_network': 
+            setattr(self,'mean_module_NN_All', FFNN_as_Mean(self, input_size= train_x.shape[1]+2*len(qual_index_list)-len(qual_index_list), num_classes=1,layers =NN_layers_m_gp, name = str('mean_module_'+str(i)+'_')).to(**tkwargs)) 
         else: 
-            raise ValueError('The "base" argument must start with "multi", "single", or "neural_network".')
+            raise ValueError('The "m_gp" argument must start with "multi", "single", or "neural_network".')
 
 
 
     def forward(self,x:torch.Tensor) -> MultivariateNormal:
-        if self.manifold_type=='probabilistic' or self.calibration_type=='probabilistic':
+        if self.embedding_type=='probabilistic' or self.calibration_type=='probabilistic':
             set_seed(self.seed)
             if self.training:
-                Numper_of_pass=5 #20
+                Numper_of_pass=self.num_pass_train#5 
             else:
-                Numper_of_pass=10 #30
+                Numper_of_pass=self.num_pass_pred#10 
         else:
             Numper_of_pass=1
         
         Sigma_sum=torch.zeros(x.size(0),x.size(0), dtype=torch.float64).to(self.tkwargs['device'])
         mean_x_sum=torch.zeros(x.size(0), dtype=torch.float64).to(self.tkwargs['device'])
 
         for NP in range(Numper_of_pass):
@@ -403,23 +406,23 @@
             x_new= x
             if len(self.qual_kernel_columns) > 0:
                 embeddings = []
                 for i in range(len(self.qual_kernel_columns)):
                     temp= self.transform_categorical(x=x[:,self.qual_kernel_columns[i]].clone().type(torch.int64).to(self.tkwargs['device']), 
                         perm_dict = self.perm_dict[i], zeta = self.zeta[i])
                 dimm=x_forward_raw.size()[0]
-                if self.manifold_type=='probabilistic': 
+                if self.embedding_type=='probabilistic': 
                     # Convert to list of tuples
                     x_raw=torch.zeros(temp.size(0),2)
                     # Find unique rows
                     unique_rows, indices = torch.unique(temp, dim=0, return_inverse=True)
                     temp= unique_rows
                     dimm=unique_rows.size()[0]
                     if self.training:
-                        epsilon=torch.normal(mean=0,std=1,size=[dimm,2])## use np instead of torch 
+                        epsilon=torch.normal(mean=0,std=1,size=[dimm,2])
                         embeddings.append(getattr(self,'A_matrix')(x=temp.float().to(**self.tkwargs),epsilon=epsilon))
                     else:
                         if x.size()[0]==self.count:
                             epsilon=torch.normal(mean=0,std=1,size=[dimm,2])
                             embeddings.append(getattr(self,'A_matrix')(x=temp.float().to(**self.tkwargs),epsilon=epsilon))
                             self.embeddings_Dtrain.append(embeddings[0])
                         else:
@@ -454,17 +457,17 @@
                             else:
                                 calibration_element=torch.where(x[:, -1]==self.calibration_source_index)[0]
                                 x_new[calibration_element,embeddings[0].size(1)+n]=\
                                     torch.ones_like(x_new[calibration_element,embeddings[0].size(1)+n])*(getattr(self,'Theta_'+str(n))(x[i,-1].clone().reshape(-1,1)))               
             if nd_flag == 1:
                 x_new = x_new.reshape(*xsize[:-1], -1)
         #################### Multiple baises (General Case) ####################################  
-            if self.base.startswith('multi'):
+            if self.m_gp.startswith('multi'):
                 mean_x = self.multi_mean(x_new,x_forward_raw).to(**self.tkwargs) 
-            elif self.base.startswith('neural_network'):
+            elif self.m_gp.startswith('neural_network'):
                 mean_x = getattr(self, 'mean_module_NN_All')(x_new.clone().detach()).reshape(-1)
             else:
                 mean_x = self.single_mean(x_new).to(**self.tkwargs) 
 
             covar_x = self.covar_module(x_new).to(**self.tkwargs)
             mean_x_sum+=mean_x
             Sigma_sum += covar_x.evaluate()+ torch.outer(mean_x, mean_x)
@@ -477,69 +480,69 @@
         ensemble_covar -= torch.outer(ensemble_mean, ensemble_mean)
         ensemble_covar=gpytorch.lazy.NonLazyTensor(ensemble_covar)
         Sigma_sum=0
         return MultivariateNormal(ensemble_mean,ensemble_covar)
     
     ################################################################ Mean Functions #####################################################################################
     
-    def single_base_register (self,size=1,base_type='single_zero',wm='mean_module'):
-        if base_type in self.supported_singl_base_functions:
+    def single_m_gp_register (self,size=1,m_gp_type='single_zero',wm='mean_module'):
+        if m_gp_type in self.supported_singl_m_gp_functions:
             setattr(self,wm, LinearMean_with_prior(input_size=size, batch_shape=torch.Size([]), bias=False)) 
-        elif base_type.startswith('single_polynomial'):
-            degree = int(base_type.split('d')[-1])
+        elif m_gp_type.startswith('single_polynomial'):
+            degree = int(m_gp_type.split('d')[-1])
             setattr(self,wm, LinearMean_with_prior(input_size=degree*(size), batch_shape=torch.Size([]), bias=True)) 
-        elif base_type=='single_constant':
+        elif m_gp_type=='single_constant':
             setattr(self,wm, gpytorch.means.ConstantMean(prior=NormalPrior(0.,1)) )
-        elif base_type=='single_zero':
+        elif m_gp_type=='single_zero':
             setattr(self,wm, gpytorch.means.ZeroMean())  
     
-    def multi_base_register(self,train_x,supported_multi_base_functions,base_hf):
+    def multi_m_gp_register(self,train_x,supported_multi_m_gp_functions,m_gp_ref):
         size=train_x.shape[1]
-        if self.base in supported_multi_base_functions:
+        if self.m_gp in supported_multi_m_gp_functions:
             for i in range(self.num_sources +1):
                 if i==0:
-                    base_type= 'single_'+base_hf
+                    m_gp_type= 'single_'+m_gp_ref
                 else:
-                    base_type='single'+self.base[8:]
-                self.single_base_register(size,base_type=base_type,wm='mean_module_'+str(i))
+                    m_gp_type='single'+self.m_gp[8:]
+                self.single_m_gp_register(size,m_gp_type=m_gp_type,wm='mean_module_'+str(i))
 
     def single_mean(self, x):
-        base_type=self.base
+        m_gp_type=self.m_gp
         supported_functions = ['sin', 'cos', 'exp', 'log', 'tan', 'asin', 'acos', 'atan', 
                                'sinh', 'cosh', 'tanh', 'asinh', 'acosh', 'atanh', 'sqrt', 
                                'abs', 'ceil', 'floor', 'round']
         
-        if base_type in supported_functions:
-            # Dynamically call the PyTorch function based on base_type
-            transformed_x = getattr(torch, base_type)(x.clone()).float()
-        elif base_type.startswith('polynomial-d'):
-            degree = int(base_type.split('d')[-1])
+        if m_gp_type in supported_functions:
+            # Dynamically call the PyTorch function m_gpd on m_gp_type
+            transformed_x = getattr(torch, m_gp_type)(x.clone()).float()
+        elif m_gp_type.startswith('polynomial-d'):
+            degree = int(m_gp_type.split('d')[-1])
             transformed_x = x.clone().double()
             polynomial_terms = [transformed_x.pow(n).float() for n in range(1, degree + 1)]
             transformed_x = torch.cat(polynomial_terms, dim=1)
         else:
             # Default case
             transformed_x = x.float().clone()
         mean_x = getattr(self, 'mean_module')(transformed_x)
         return mean_x
 
     def multi_mean(self,x,x_forward_raw):
         mean_x=torch.zeros_like(x[:,-1])
-        if self.base=='multiple_constant':
+        if self.m_gp=='multiple_constant':
             for i in range(len(mean_x)):
                 qq=int(x_forward_raw[i,-1])                        
                 mean_x[i] = getattr(self, 'mean_module_' + str(qq))(x_forward_raw[i,:].clone().float().reshape(1,-1))
-        elif self.base=='multiple_polynomial':
+        elif self.m_gp=='multiple_polynomial':
             for i in range(len(mean_x)):
                 qq=int(x_forward_raw[i,-1])
                 # mean_x[i]=getattr(self,'mean_module_'+str(qq))(torch.cat((torch.tensor((x[i,-1].clone().double().reshape(-1,1).float())**2),torch.tensor(x[i,-1].clone().double()).reshape(-1,1).float()),1))
                 mean_x[i] = getattr(self, 'mean_module_' + str(qq))(torch.cat((x_forward_raw.clone().detach().double().reshape(-1, 1).float() ** 2,
                         x[i, -1].clone().detach().double().reshape(-1, 1).float()),1))
         
-        elif self.base=='neural_network':
+        elif self.m_gp=='neural_network':
             mean_x = getattr(self, 'mean_module_NN_All')(x.clone()).reshape(-1)
         return mean_x 
 
     ################################################################ Fit #####################################################################################
     def fit(self,add_prior:bool=True,num_restarts:int=64,theta0_list:Optional[List[np.ndarray]]=None,jac:bool=True,
             options:Dict={},n_jobs:int=-1,method = 'L-BFGS-B',constraint=False,bounds=False,regularization_parameter:List[int]=[0,0],optim_type='scipy'):
         print("## Learning the model's parameters has started ##")
@@ -561,15 +564,15 @@
                                 num_iter=100,
                                 num_restarts=4,
                                 break_steps=50)
         else:
             if optim_type=='scipy':
                 fit_model_scipy (self,add_prior,num_restarts,theta0_list,jac, options,n_jobs,method ,constraint,bounds,regularization_parameter)
             elif optim_type=='continuation':
-                noise_tune2(model=self,add_prior=add_prior,
+                fit_model_continuation(model=self,add_prior=add_prior,
                 num_restarts=num_restarts,criterion='NLL',
                 initial_noise_var=1,
                 red_factor=math.sqrt(10),
                 options=options,
                 n_jobs= n_jobs,
                 accuracy = 1e-2,
                 method = method,
@@ -584,17 +587,17 @@
                     num_iter=100,
                     num_restarts=num_restarts,
                     break_steps= 50)
             else:
                 raise ValueError(
                     'Invalid optim_type. You must choose one of the following: '
                     '"scipy" (default), "continuation", or "adam_torch".\n'
-                    '- "scipy": Uses the SciPy library for optimization, suitable for most CPU-based computations.\n'
+                    '- "scipy": Uses the SciPy library for optimization, suitable for most CPU-m_gpd computations.\n'
                     '- "continuation": A method designed for more complex optimization scenarios, potentially offering better results in most cases with higher computational cost.\n'
-                    '- "adam_torch": Employs the Adam optimizer from the PyTorch library, optimized for GPU-based computations and large datasets.'
+                    '- "adam_torch": Employs the Adam optimizer from the PyTorch library, optimized for GPU-m_gpd computations and large datasets.'
                 )
         print("## Learning the model's parameters is successfully finished ##")
 
 
 
 
     def fill_nan_with_mean(self,train_x,cal_ID):
@@ -611,33 +614,36 @@
             # Replace NaNs with the corresponding column-wise mean
             train_x[nan_indices] = col_means.repeat(train_x.shape[0], 1)[nan_indices]
 
         return train_x
     ############################  Prediction and Visualization  ###############################
     
     def predict(self, Xtest,return_std=True, include_noise = True):
+        Xtest=data_type_check(Xtest)
         with torch.no_grad():
             return super().predict(Xtest, return_std = return_std, include_noise= include_noise)
     
     def predict_with_grad(self, Xtest,return_std=True, include_noise = True):
+        Xtest=data_type_check(Xtest)
         return super().predict(Xtest, return_std = return_std, include_noise= include_noise)
     
     def noise_value(self):
         noise = self.likelihood.noise_covar.noise.detach() * self.y_std**2
         return noise
 
     def score(self, Xtest, ytest, plot_MSE = True, title = None, seperate_levels = False):
+        Xtest=data_type_check(Xtest)
+        ytest=data_type_check(ytest)
         ytest=ytest.reshape(-1).to(self.tkwargs['device'])
         Xtest=Xtest.to(self.tkwargs['device'])
         plt.rcParams.update({'font.size': 14})
         ypred = self.predict(Xtest, return_std=False)
         mse = ((ytest.reshape(-1)-ypred)**2).mean()
         print('################MSE######################')
         print(f'MSE = {mse:.5f}')
-        print('#########################################')
         print('################Noise####################')
         noise = self.likelihood.noise_covar.noise.detach() * self.y_std**2
         
         print(f'The estimated noise parameter (varaince) is {noise}')
         print(f'The estimated noise std is {np.sqrt(noise.cpu())}')
         print('#########################################')
 
@@ -647,54 +653,99 @@
             _ = plt.plot(ytest.cpu().numpy(), ytest.cpu().numpy(), 'b', label = 'MSE = ' + str(np.round(mse.detach().item(),3)))
             _ = plt.xlabel(r'Y_True')
             _ = plt.ylabel(r'Y_predict')
             _ = plt.legend()
             if title is not None:
                 _ = plt.title(title)
 
-        if seperate_levels and len(self.qual_index) > 0:
+        if seperate_levels and len(self.qual_index_list) > 0:
             for i in range(self.num_levels_per_var[0]):
-                index = torch.where(Xtest[:,self.qual_index] == i)[0]
+                index = torch.where(Xtest[:,self.qual_index_list] == i)[0]
                 _ = self.score(Xtest[index,...], ytest[index], 
                     plot_MSE=True, title = 'results' + ' Only Source ' + str(i), seperate_levels=False)
         return ypred
 
     def plot_xy(self, Xtest, ytest, input_column):
+        Xtest=data_type_check(Xtest)
+        ytest=data_type_check(ytest)
+        
         ytest=ytest.reshape(-1).to(**self.tkwargs)
         Xtest=Xtest.to(**self.tkwargs)
         if len(input_column) > 2:
             raise ValueError("Visualization can only be done for one or two input versions.")
 
         plt.rcParams.update({'font.size': 14})
         ypred = self.predict(Xtest, return_std=False)
-        mse = ((ytest.reshape(-1) - ypred) ** 2).mean()
 
         if len(input_column) == 1:
-            # 2D Plotting for one input
-            plt.scatter(Xtest[input_column[0]].cpu().numpy(), ytest.cpu().numpy(), '*r', label='Ground Truth')
-            plt.scatter(Xtest[input_column[0]].cpu().numpy(), ypred.cpu().numpy(), 'ob', label='Prediction')
+            plt.scatter(Xtest[:,input_column[0]].cpu().numpy(), ypred.cpu().numpy(),marker= 'o', label='Prediction')
             plt.xlabel('Input: ' + str(input_column[0]))
             plt.ylabel('Output')
-
         elif len(input_column) == 2:
-            # 3D Plotting for two inputs
             fig = plt.figure()
             ax = fig.add_subplot(111, projection='3d')
-            ax.scatter(Xtest[input_column[0]].cpu().numpy(), Xtest[input_column[1]].cpu().numpy(), ytest.cpu().numpy(), c='r', marker='o', label='Ground Truth')
-            ax.scatter(Xtest[input_column[0]].cpu().numpy(), Xtest[input_column[1]].cpu().numpy(), ypred.cpu().numpy(), c='b', marker='^', label='Prediction')
+            ax.scatter(Xtest[:,input_column[0]].cpu().numpy(), Xtest[input_column[1]].cpu().numpy(), ytest.cpu().numpy(), c='r', marker='o', label='Ground Truth')
+            ax.scatter(Xtest[:,input_column[0]].cpu().numpy(), Xtest[input_column[1]].cpu().numpy(), ypred.cpu().numpy(), c='b', marker='^', label='Prediction')
             ax.set_xlabel('Input: ' + str(input_column[0]))
             ax.set_ylabel('Input: ' + str(input_column[1]))
             ax.set_zlabel('Output')
 
         plt.title('Input(s): ' + str(input_column) + ' versus Output')
         plt.legend()
         plt.show()
 
 
+
+    def plot_predict_xy(self, var_input, value_range, val_fixed_inputs, num_points=100):
+        """
+        Plots the prediction of the model for a specified input variable while keeping other inputs fixed.
+
+        Parameters:
+        - var_input (int): The index of the input variable to vary.
+        - value_range (list or tuple): The range [min, max] over which to vary var_input.
+        - val_fixed_inputs (dict): Dictionary with column indices as keys and fixed values as values for all input variables except var_input.
+        - num_points (int): The number of points in the linspace for var_input. Default is 100.
+
+        Raises:
+        - ValueError: If var_input is not a valid index for the input variables.
+        """
+
+        # Check if var_input is a valid index
+        if not (0 <= var_input < len(val_fixed_inputs)+1):
+            raise ValueError("var_input must be a valid index of the input variables.")
+
+        # Define the number of points in the linspace
+        var_input_values = np.linspace(value_range[0], value_range[1], num_points)
+        
+        # Initialize Xtest with the appropriate shape
+        Xtest = np.zeros((num_points, len(val_fixed_inputs)+1))
+
+        # Fill Xtest with fixed values
+        for i in range(Xtest.shape[1]):
+            if i == var_input:
+                Xtest[:, i] = var_input_values
+            elif i in val_fixed_inputs:
+                Xtest[:, i] = val_fixed_inputs[i]
+            else:
+                raise ValueError(f"Column index {i} is not specified in val_fixed_inputs and is not the variable input index.")
+
+        Xtest=torch.tensor(Xtest)        
+        # Make predictions
+        ypred = self.predict(Xtest, return_std=False)
+        # Plotting
+        plt.plot(Xtest[:, var_input].cpu().numpy(), ypred.cpu().numpy(), label='Prediction')
+        plt.xlabel('Input ' + str(var_input))
+        plt.ylabel('Output')
+        plt.title('Input: ' + str(var_input) + ' versus Output')
+        plt.legend()
+        plt.show()
+
     def plot_xy_print_params(self, Xtest, ytest, Xtrain, ytrain, model):
+            Xtest=data_type_check(Xtest)
+            ytest=data_type_check(ytest)
             ytest=ytest.reshape(-1).to(self.tkwargs['device'])
             Xtest=Xtest.to(self.tkwargs['device'])
             Xtest, indices = torch.sort(Xtest, dim = 0)
             ytest = ytest[indices]
 
             mean_pred, std_pred = model.predict(Xtest.to(**self.tkwargs), return_std=True)
             confidence_interval = 1.96 * std_pred
@@ -703,28 +754,31 @@
             plt.scatter(Xtrain, ytrain, marker='x', color='red')
             plt.plot(Xtest, ytest,color='black', linewidth=4.0, label='Exact')
             plt.plot(Xtest, mean_pred.cpu(), color='green', linestyle='dashed', linewidth=4.0, label = 'Predicted')
             plt.fill_between(Xtest.squeeze(), mean_pred.cpu() - confidence_interval.cpu(), mean_pred.cpu() + confidence_interval.cpu(), color='lightblue', alpha=0.7, label='95% CI')
             plt.scatter(Xtrain, ytrain, s=100, marker='x', color='red', label='Training data')
             plt.xlabel(r'$x$')
             plt.ylabel(r'$y$')
-            title = r"$\hat{\beta}$ = " + f"{model.mean_module.constant.item():.3f}" + r", $\hat{\omega}$ = " + f"{model.covar_module.base_kernel.raw_lengthscale.data.item():.3e}"+ r", $\hat{\delta}$ = " + f"{model.noise_value().item():.3e}"
+            title = r"$\hat{\beta}$ = " + f"{model.mean_module.constant.item():.3f}" + r", $\hat{\omega}$ = " + f"{model.covar_module.m_gp_kernel.raw_lengthscale.data.item():.3e}"+ r", $\hat{\delta}$ = " + f"{model.noise_value().item():.3e}"
             plt.title(title, fontsize = 15, loc="center")
             plt.legend()
             plt.show()
             
     def evaluation_2(self,Xtest,ytest,n_FP=1):
+        Xtest=data_type_check(Xtest)
+        ytest=data_type_check(ytest)
+        
         ytest=ytest.reshape(-1).to(self.tkwargs['device'])
         Xtest=Xtest.to(self.tkwargs['device'])
         self.eval()
         likelihood=self.likelihood
         likelihood.fidel_indices=self.train_inputs[0][:,-1]
         output=self(Xtest)
         likelihood.fidel_indices=Xtest[:,-1]
-        ytest_sc = (ytest-self.y_mean)/self.y_std
+        ytest_sc = (ytest-self.y_min)/self.y_std
         mean_temp=[]
         var_temp=[]
         for i in range (n_FP):
             with torch.no_grad():
                 trained_pred_dist = likelihood(output)
                 mean_temp.append(trained_pred_dist.mean)
                 var_temp.append(trained_pred_dist.variance)
@@ -755,34 +809,34 @@
 
 
     def rearrange_one_hot(self,tensor):
         # Find the indices that sort each row
         sorted_indices = torch.argsort(tensor, dim=1, descending=True)
         # Generate a new tensor of zeros with the same shape
         new_tensor = torch.zeros_like(tensor)
-        # Place '1's in the appropriate positions based on the sorted indices
+        # Place '1's in the appropriate positions m_gpd on the sorted indices
         for i in range(tensor.size(0)):
             new_tensor[i, sorted_indices[i, 0]] = 1
 
         return torch.flip(new_tensor, dims=[0])
     def visualize_latent(self,type='cat',rpearts=500):
-        if self.manifold_type=='deterministic':
+        if self.embedding_type=='deterministic':
             if len(self.qual_kernel_columns) > 0:
                 for i in range(len(self.qual_kernel_columns)):
                     zeta = self.zeta[i]
                     dimm=zeta.size()[0]
                     zeta_epsilon=torch.normal(mean=0,std=1,size=[dimm,2])
 
                     A = getattr(self,'A_matrix')
                     positions = A[i](x=zeta.float().to(**self.tkwargs))
                     level = torch.max(self.perm[i]+1, axis = 0)[0].tolist()
 
                     perm = self.perm[i]
                     plot_sep(type=type,positions = positions, levels = level, perm = perm, constraints_flag=False)
-        elif self.manifold_type=='probabilistic':
+        elif self.embedding_type=='probabilistic':
             for i in range(len(self.qual_kernel_columns)):
                 temp= self.transform_categorical(x=self.train_inputs[0][:,self.qual_kernel_columns[i]].clone().type(torch.int64).to(self.tkwargs['device']), perm_dict = self.perm_dict[i], zeta = self.zeta[i])
             unique_rows, indices = torch.unique(temp, dim=0, return_inverse=True)
             xp=self.rearrange_one_hot(unique_rows)
             z_p_list =[]
             label=[]
             epsilon=torch.normal(mean=0,std=1,size=[rpearts,2])
@@ -822,21 +876,23 @@
             plt.xlabel(r'$z_1$',labelpad=0,rotation=0,usetex=True)
             plt.ylabel(r'$z_2$',labelpad=14,rotation=0,usetex=True)
             plt.tight_layout()
             plt.show()
 
     
     def evaluation(self,Xtest,ytest):
+        Xtest=data_type_check(Xtest)
+        ytest=data_type_check(ytest)
         self.eval()
         ytest=ytest.reshape(-1).to(self.tkwargs['device'])
         Xtest=Xtest.to(self.tkwargs['device'])
         ytest=ytest.reshape(-1)
         Xtest=Xtest
         likelihood=self.likelihood
-        ytest_sc = (ytest-self.y_mean)/self.y_std
+        ytest_sc = (ytest-self.y_min)/self.y_std
 
         with torch.no_grad():
             trained_pred_dist = likelihood(self(Xtest))
         # Negative Log Predictive Density (NLPD)
         final_nlpd = gpytorch.metrics.negative_log_predictive_density(trained_pred_dist,ytest_sc)
         
         # Mean Squared Error (MSE)
@@ -931,53 +987,53 @@
             _ = plt.figure(figsize=(12,6))
             _ = plt.scatter(list(range(len(X))), out.loc.detach().numpy()[index], color = 'red', s = 20, marker = 'o')
             _ = plt.scatter(np.repeat(np.arange(len(X)).reshape(1,-1), size, axis = 0), 
                 draws.detach().numpy()[:,index], color = 'blue', s = 1, alpha = 0.5, marker = '.')
         return draws
 
     def get_latent_space(self):
-        if len(self.qual_index) > 0:
+        if len(self.qual_index_list) > 0:
             zeta = torch.tensor(self.zeta, dtype = torch.float64).to(**self.tkwargs)
             positions = self.nn_model(zeta)
             return positions.detach()
         else:
             print('No categorical Variable, No latent positions')
             return None
 
 
 
-    def LMMAPPING(self, num_features:int, type = 'Linear',lv_dim = 2):
+    def LMMAPPING(self, num_features:int, type = 'Linear',embedding_dim = 2):
 
         if type == 'Linear':
             in_feature = num_features
-            out_feature = lv_dim
+            out_feature = embedding_dim
             lm = torch.nn.Linear(in_feature, out_feature, bias = False)
             return lm
 
         else:
             raise ValueError('Only Linear type for now')    
 
     def zeta_matrix(self,
         num_levels:int,
-        lv_dim:int,
+        embedding_dim:int,
         batch_shape=torch.Size()
     ) -> None:
 
         if any([i == 1 for i in num_levels]):
             raise ValueError('Categorical variable has only one level!')
 
-        if lv_dim == 1:
+        if embedding_dim == 1:
             raise RuntimeWarning('1D latent variables are difficult to optimize!')
         
         for level in num_levels:
-            if lv_dim > level - 0:
-                lv_dim = min(lv_dim, level-1)
+            if embedding_dim > level - 0:
+                embedding_dim = min(embedding_dim, level-1)
                 raise RuntimeWarning(
                     'The LV dimension can atmost be num_levels-1. '
-                    'Setting it to %s in place of %s' %(level-1,lv_dim)
+                    'Setting it to %s in place of %s' %(level-1,embedding_dim)
                 )
     
         from itertools import product
         levels = []
         for l in num_levels:
             levels.append(torch.arange(l))
 
@@ -1009,16 +1065,22 @@
     def transform_categorical(self, x:torch.Tensor,perm_dict = [], zeta = []) -> None:
         if x.dim() == 1:
             x = x.reshape(-1,1)
         # categorical should start from 0
         if self.training == False:
             x = torch.tensor(setlevels(x))
         if self.encoding_type == 'one-hot':
-            index = [perm_dict[str(row.tolist())] for row in x]
-
+            try:
+                index = [perm_dict[str(row.tolist())] for row in x]
+            except KeyError:
+                raise ValueError(
+                    "The categorical input (or source indices) are not defined properly. "
+                    "They should be integer values starting from zero. To solve the issue, "
+                    "you can use the 'setlevels' function, which is a preprocessing function."
+                )
             if x.dim() == 1:
                 x = x.reshape(len(x),)
 
             return zeta[index,:]  
 
     def transform_categorical_random_varible_for_latent(self,x_raw, x:torch.Tensor,perm_dict = [], zeta = []) -> None:
         
@@ -1086,15 +1148,15 @@
         """
         if N<1e5:
             warnings.warn('Increase N for accuracy!')
 
         p = self.train_inputs[0].shape[1] 
         dy = 1# self.train_targets.shape[1] 
 
-        self.qual_index
+        self.qual_index_list
         self.num_levels_per_var
         # sequence = torch.from_numpy( sobol_seq.i4_sobol_generate(2*p, N)).to(**self.tkwargs)
         sequence = torch.from_numpy( sobol_seq.i4_sobol_generate(2*p, N))
         def normalize_sobol_sequence(sequence, train_inputs,p):
             
             temp_1 = sequence[:,p:]
             temp_2 = sequence[:,:p]
@@ -1103,15 +1165,15 @@
             mins = train_inputs.min(dim=0)[0]
             maxs = train_inputs.max(dim=0)[0]
 
             sequence_1= mins + (maxs - mins) * temp_1
             sequence_2= mins + (maxs - mins) * temp_2
             # Take care of categotrical inputes
             j=0
-            for i in self.qual_index:
+            for i in self.qual_index_list:
                 temp_1[:,i]= temp_1[:,i]*(self.num_levels_per_var[j]-1)
                 temp_2[:,i]=temp_2[:,i]*(self.num_levels_per_var[j]-1)
                 sequence_1[:,i]=temp_1[:,i].round()
                 sequence_2[:,i]=temp_2[:,i].round()
                 j+=1
                 return sequence_1,sequence_2
         A,B = normalize_sobol_sequence(sequence, self.train_inputs[0],p)
```

### Comparing `gpplus-0.0.1.221/gpplus/models/gpregression.py` & `gpplus-0.0.2.1/gpplus/models/gpregression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# Copyright © 2023, University of California, Irvine.
-#
-# GP_Plus is a proprietary software of the University of California, Irvine. This software
-# is available for use free of charge for educational and research purposes by non-profit
-# institutions and US government agencies. Other organizations are permitted to use 
-# GP_Plus solely for evaluation purposes. Any further utilization requires explicit, prior
-# written consent. Sale or unauthorized redistribution of this software is strictly 
-# prohibited. Users may create copies for personal use, provided that these copies are 
-# not sold or distributed and are subject to the same terms and conditions as outlined 
-# herein.
-#
-# This software is provided as research software. As such, it is made available "as is" 
-# without any warranty of any kind, either express or implied. By downloading or using 
-# any part of this software, the user implicitly agrees to these terms. Please note that
-# these terms and conditions are subject to modification at any time without prior notice.
+# Copyright © 2023, Dr. Bostanabad's research group at the University of California, Irvine.
+# 
+# GP+ Intellectual Property Notice:
+# 
+# The software known as GP+ is the proprietary material of Dr. Bostanabad's research group at the University of California, Irvine. 
+# Non-profit academic institutions and U.S. government agencies may utilize this software exclusively for educational and research endeavors. 
+# All other entities are granted permission for evaluation purposes solely; any additional utilization demands prior written consent from the appropriate authority. 
+# The direct sale or redistribution of this software, in any form, without explicit written authorization is strictly prohibited. 
+# Users are permitted to make duplicate copies of the software, contingent upon the assurance that no copies are sold or redistributed and they adhere to the stipulated terms herein.
+# 
+# Being academic research software, GP+ is provided on an "as is" m_gp, devoid of warranties, whether explicit or implicit. 
+# The act of downloading or executing any segment of this software inherently signifies compliance with these terms. 
+# The developers reserve the right to modify these terms and conditions without prior intimation at any juncture.
 
 import torch
 import gpytorch
 import math
 from gpytorch.models import ExactGP
 from gpytorch import settings as gptsettings
 from gpytorch.priors import NormalPrior,LogNormalPrior
@@ -40,16 +38,16 @@
 class GPR(ExactGP, GPyTorchModel):
     def __init__(
         self,
         train_x:torch.Tensor,
         train_y:torch.Tensor,
         correlation_kernel,
         noise_indices:List[int],
-        noise:float=1e-4,
         fix_noise:bool=False,
+        fix_noise_val:float=1e-5,
         lb_noise:float=1e-12,
     ) -> None:
         # check inputs
         if not torch.is_tensor(train_x):
             raise RuntimeError("'train_x' must be a tensor")
         if not torch.is_tensor(train_y):
             raise RuntimeError("'train_y' must be a tensor")
@@ -62,35 +60,35 @@
         
         if len(noise_indices) == 0:
 
             likelihood = gpytorch.likelihoods.GaussianLikelihood(noise_constraint=noise_constraint)
         else:
 
             likelihood = Multifidelity_likelihood(noise_constraint=noise_constraint, noise_indices=noise_indices, fidel_indices=train_x[:,-1])
-        y_mean= train_y.min()
-        y_std=train_y.max()-train_y.min()
-        train_y_sc = (train_y-y_mean)/y_std
+        y_min= train_y.min()
+        y_std= train_y.max()-train_y.min()
+        train_y_sc = (train_y-y_min)/y_std
 
         ExactGP.__init__(self, train_x,train_y_sc, likelihood)
         
         # registering mean and std of the raw response
-        self.register_buffer('y_mean',y_mean)
+        self.register_buffer('y_min',y_min)
         self.register_buffer('y_std',y_std)
         self.register_buffer('y_scaled',train_y_sc)
 
         self._num_outputs = 1
 
         # initializing and fixing noise
-        if noise is not None:
-            self.likelihood.initialize(noise=noise)
+        # if noise is not None:
+        #     self.likelihood.initialize(noise=noise)
         
         self.likelihood.register_prior('noise_prior',LogHalfHorseshoePrior(0.01,lb_noise),'raw_noise')
         if fix_noise:
             self.likelihood.raw_noise.requires_grad_(False)
-            self.likelihood.noise_covar.noise =torch.tensor(4.9901e-05)
+            self.likelihood.noise_covar.noise =torch.tensor(fix_noise_val)
 
         if isinstance(correlation_kernel,str):
             try:
                 correlation_kernel_class = getattr(kernels,correlation_kernel)
                 correlation_kernel = correlation_kernel_class(
                     ard_num_dims = self.train_inputs[0].size(1),
                     lengthscale_constraint=Positive(transform=torch.exp,inv_transform=torch.log),
@@ -133,18 +131,19 @@
                 output = self(x)
             else:
                 # for batched GPs 
                 num_samples = self.train_targets.shape[0]
                 output = self(x.unsqueeze(0).repeat(num_samples,1,1))
             self.fidel_indices=x[:,-1]
             if return_std and include_noise:
-                # x=self.likelihood(x)
+                # x=self.fidel_indices
+                self.likelihood.fidel_indices=x[:,-1]   ### the fidelity indaces are alrrady set for training data, here we update them test data since 
                 output = self.likelihood(output)
 
-            out_mean = self.y_mean + self.y_std*output.mean
+            out_mean = self.y_min + self.y_std*output.mean
             
             # standard deviation may not always be needed
             if return_std:
                 out_std = output.variance.sqrt()*self.y_std
                 return out_mean,out_std
 
             return out_mean
```

### Comparing `gpplus-0.0.1.221/gpplus/optim/mll_noise_tune2.py` & `gpplus-0.0.2.1/gpplus/optim/mll_noise_continuation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Copyright © 2021 by Northwestern University.
+# Copyright © 2023, Dr. Bostanabad's research group at the University of California, Irvine.
 # 
-# LVGP-PyTorch is copyrighted by Northwestern University. It may be freely used 
-# for educational and research purposes by  non-profit institutions and US government 
-# agencies only. All other organizations may use LVGP-PyTorch for evaluation purposes 
-# only, and any further uses will require prior written approval. This software may 
-# not be sold or redistributed without prior written approval. Copies of the software 
-# may be made by a user provided that copies are not sold or distributed, and provided 
-# that copies are used under the same terms and conditions as agreed to in this 
-# paragraph.
+# GP+ Intellectual Property Notice:
 # 
-# As research software, this code is provided on an "as is'' basis without warranty of 
-# any kind, either expressed or implied. The downloading, or executing any part of this 
-# software constitutes an implicit agreement to these terms. These terms and conditions 
-# are subject to change at any time without prior notice.
+# The software known as GP+ is the proprietary material of Dr. Bostanabad's research group at the University of California, Irvine. 
+# Non-profit academic institutions and U.S. government agencies may utilize this software exclusively for educational and research endeavors. 
+# All other entities are granted permission for evaluation purposes solely; any additional utilization demands prior written consent from the appropriate authority. 
+# The direct sale or redistribution of this software, in any form, without explicit written authorization is strictly prohibited. 
+# Users are permitted to make duplicate copies of the software, contingent upon the assurance that no copies are sold or redistributed and they adhere to the stipulated terms herein.
+# 
+# Being academic research software, GP+ is provided on an "as is" m_gp, devoid of warranties, whether explicit or implicit. 
+# The act of downloading or executing any segment of this software inherently signifies compliance with these terms. 
+# The developers reserve the right to modify these terms and conditions without prior intimation at any juncture.
+
 
 import math
 import numpy as np
 import torch
 from warnings import simplefilter,catch_warnings
 from gpytorch import settings as gptsettings
 from gpytorch.utils.warnings import GPInputWarning
@@ -39,15 +38,15 @@
     Rinv = model.prediction_strategy.covar_cache # RinvRinv^T= Kinv
     Kinv_diag = (Rinv**2).sum(dim=-1)
 
     loo_error = Kinv_y/Kinv_diag
     return (loo_error**2).mean().sqrt().item()
 
 # NLL is negative loglikelihood
-def noise_tune2(
+def fit_model_continuation(
     model:GPR,add_prior:bool=True,
     num_restarts:int=32,criterion:str='NLL',
     initial_noise_var:float=1,
     red_factor:float=math.sqrt(10),
     options:Dict={},
     n_jobs:int= -1,
     accuracy = 1e-2,
@@ -227,15 +226,15 @@
         'loocv_history':loocv_list,
         'optimization_history':reslist_list
         }
 
         index = np.argmin(history['nll_history'])
 
 
-        print('Finished the for loop')
+        print('Finished for loop')
 
 
         print(history['nll_history'])
 
         if np.abs(initial_noise_var_new - history['noise_history'][index]) < accuracy:
             model.load_state_dict(old_state_dict[index])
             break
```

### Comparing `gpplus-0.0.1.221/gpplus/optim/mll_scipy.py` & `gpplus-0.0.2.1/gpplus/optim/mll_scipy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright © 2023, University of California, Irvine.
+# Copyright © 2023, Dr. Bostanabad's research group at the University of California, Irvine.
 # 
 # GP+ Intellectual Property Notice:
 # 
-# The software known as GP+ is the proprietary material of the University of California, Irvine. 
+# The software known as GP+ is the proprietary material of Dr. Bostanabad's research group at the University of California, Irvine. 
 # Non-profit academic institutions and U.S. government agencies may utilize this software exclusively for educational and research endeavors. 
 # All other entities are granted permission for evaluation purposes solely; any additional utilization demands prior written consent from the appropriate authority. 
 # The direct sale or redistribution of this software, in any form, without explicit written authorization is strictly prohibited. 
 # Users are permitted to make duplicate copies of the software, contingent upon the assurance that no copies are sold or redistributed and they adhere to the stipulated terms herein.
 # 
-# Being academic research software, GP+ is provided on an "as is" basis, devoid of warranties, whether explicit or implicit. 
+# Being academic research software, GP+ is provided on an "as is" m_gp, devoid of warranties, whether explicit or implicit. 
 # The act of downloading or executing any segment of this software inherently signifies compliance with these terms. 
-# The University of California, Irvine reserves the right to modify these terms and conditions without prior intimation at any juncture.
+# The developers reserve the right to modify these terms and conditions without prior intimation at any juncture.
 
 import torch
 import numpy as np
 from gpytorch import settings as gptsettings
 from gpytorch.utils.errors import NanError,NotPSDError
 from scipy.optimize import minimize,OptimizeResult
 from collections import OrderedDict
@@ -24,15 +24,15 @@
 from typing import Dict,List,Tuple,Optional,Union
 from copy import deepcopy
 from scipy.optimize import Bounds
 from scipy.optimize import NonlinearConstraint
 from scipy.optimize import BFGS
 #######################################################
 
-from gpplus.utils.interval_score import interval_score
+from gpplus.utils.interval_score import interval_score_function
 tkwargs = {
     "dtype": torch.float,
     "device": torch.device("cpu" if torch.cuda.is_available() else "cpu"),
 }
 
 def marginal_log_likelihood(model,add_prior:bool,regularization_parameter=[0,0]):
     output = model(*model.train_inputs)
@@ -50,16 +50,16 @@
             temp_1 += torch.sum(torch.abs(param))
         elif name in ['nn_model.' + str + '.bias' for str in string_list]:
             temp += torch.norm(param)
             temp_1 += torch.sum(torch.abs(param))
 
     out -= regularization_parameter[0]*temp_1 + regularization_parameter[1]* temp    
     ## Interval Score if neede for BO
-    if model.IS is True:
-        score, accuracy = interval_score(output.mean + 1.96 * output.variance.sqrt(), output.mean - 1.96 * output.variance.sqrt(), model.y_scaled)
+    if model.interval_score is True:
+        score, accuracy = interval_score_function(output.mean + 1.96 * output.variance.sqrt(), output.mean - 1.96 * output.variance.sqrt(), model.y_scaled)
         return out - 0.08*torch.abs(out) * score#- torch.exp(model.interval_alpha) * score
     return out 
 
 
 class MLLObjective:
 
     def __init__(self,model,add_prior,regularization_parameter):
```

### Comparing `gpplus-0.0.1.221/gpplus/preprocessing/Data_reader.py` & `gpplus-0.0.2.1/gpplus/preprocessing/Data_reader.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/preprocessing/normalizeX.py` & `gpplus-0.0.2.1/gpplus/preprocessing/normalizeX.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/preprocessing/numericlevels.py` & `gpplus-0.0.2.1/gpplus/preprocessing/numericlevels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,25 @@
 import torch
 import numpy as np
-
-# def setlevels(X, qual_index = None):
-#     if qual_index is None:
-#         qual_index = list(range(X.shape[-1]))
-#     if type(X) == torch.Tensor:
-#         temp = X.clone()
-#     if X.ndim > 1:
-#         for j in qual_index:
-#             a = X[..., j]
-#             X[..., j] = torch.tensor([*map(lambda m: list(sorted(set(a.tolist()))).index(m), a)])
-#     else:
-#         X = torch.tensor([*map(lambda m: list(set(sorted(X.tolist()))).index(m), X)])
-    
-#     if X.dtype == object:
-#         X = X.astype(float)
-
-#     if type(X) == np.ndarray:
-#         X = torch.from_numpy(X)
-#         return X
-#     else:
-#         return X.to(temp)
-
-
+from gpplus.utils import data_type_check
 
 def setlevels(X, qual_index = None, return_label = False):
     labels = []
     if qual_index == []:
         return X
     if qual_index is None:
         qual_index = list(range(X.shape[-1]))
-    # if type(X) == np.ndarray:
-    #     temp = torch.from_numpy(X).detach().clone()
-    
+    X=data_type_check(X)
     # Check if X is a PyTorch tensor
     if isinstance(X, torch.Tensor):
         # Move X to CPU if it's on CUDA
         if X.is_cuda:
             X = X.cpu()
         temp = X.clone()
     # Check if X is a NumPy array
-    elif isinstance(X, np.ndarray):
-        temp = np.copy(X)
     else:
         # Handle other types or raise an error
         raise TypeError("X must be a PyTorch tensor or a NumPy array.")
 
     # Convert PyTorch tensor to NumPy array if needed
     if isinstance(temp, torch.Tensor):
         temp = temp.numpy()
```

### Comparing `gpplus-0.0.1.221/gpplus/preprocessing/one_hot_encoding.py` & `gpplus-0.0.2.1/gpplus/preprocessing/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/preprocessing/split.py` & `gpplus-0.0.2.1/gpplus/preprocessing/split.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/priors/horseshoe.py` & `gpplus-0.0.2.1/gpplus/priors/horseshoe.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/priors/mollified_uniform.py` & `gpplus-0.0.2.1/gpplus/priors/mollified_uniform.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/test_functions/analytical.py` & `gpplus-0.0.2.1/gpplus/test_functions/analytical.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,30 +102,30 @@
         if out_flag == 1:
             return X, y
         else:
             return y
 
 ####################################Borehole Function################################################
 
-def borehole_mixed_variables(n=100, X = None, qual_ind_val = {0:5, 6:3}, 
+def borehole_mixed_variables(n=100, X = None, qual_dict = {0:5, 6:3}, 
     noise_std = 0.0, random_state = None, shuffle = True):
 
     labels = {'rw':0, 'r':1, 'Tu':2, 'Hu':3, "Tl":4, 'Hl':5, 'L':6, 'Kw':7}
 
     dx = 8
     l_bound = [0.05, 100, 63070, 990, 63.1, 700, 1120, 9855]
     u_bound = [0.15, 50000, 115600, 1110, 116, 820, 1680, 12045]
     out_flag = 0
     data = {}
     if X is None:
         sobolset = Sobol(d=dx, seed = random_state)
         X = sobolset.random(2 ** (np.log2(n) + 1).astype(int))[:n, :]
         X = scale(X, l_bounds=l_bound, u_bounds=u_bound)
         # for categorical variables we select t1 levels from the boundary
-        for key, value in qual_ind_val.items():
+        for key, value in qual_dict.items():
             levels = np.random.uniform(l_bound[key], u_bound[key], size = value)
             X[...,key] = np.random.choice(levels, size = len(X), replace=True)
 
         out_flag = 1
     if type(X) != np.ndarray:
         X = np.array(X)
     data['rw'] = X[..., 0]
@@ -147,45 +147,45 @@
 
     if shuffle:
         index = np.random.randint(0, len(y), size = len(y))
         X = X[index,...]
         y = y[index]
 
     # This will assign levels to categorical evenif the levels are strings
-    X = setlevels(X, qual_index = list(qual_ind_val.keys()))
+    X = setlevels(X, qual_index = list(qual_dict.keys()))
 
     if noise_std > 0.0:
         if out_flag == 1:
             return X, y + np.random.randn(*y.shape) * noise_std
         else:
             return y       
     else:
         if out_flag == 1:
             return X, y
         else:
             return y
 
 
 ####################################### Wing_mixed #######################################
-def wing_mixed_variables(n=100, X = None, qual_ind_val = {0:5, 6:3}, noise_std = 0.0, random_state = None, shuffle = True):
+def wing_mixed_variables(n=100, X = None, qual_dict = {0:5, 6:3}, noise_std = 0.0, random_state = None, shuffle = True):
 
     if random_state is not None:
         np.random.seed(random_state)
 
     labels = {'Sw':0, 'Wfw':1, 'A':2, 'Gama':3, "q":4, 'lamb':5, 'tc':6, 'Nz':7, 'Wdg':8, 'Wp':9}
 
     dx = 10
     l_bound = [150, 220, 6, -10, 16, 0.5, 0.08, 2.5, 1700, 0.025]
     u_bound = [200, 300, 10, 10, 45, 1, 0.18, 6, 2500, 0.08]
     out_flag = 0
     if X is None:
         sobolset = Sobol(d=dx, seed = random_state)
         X = sobolset.random(2 ** (np.log2(n) + 1).astype(int))[:n, :]
         X = scale(X, l_bounds=l_bound, u_bounds=u_bound)
-        for key, value in qual_ind_val.items():
+        for key, value in qual_dict.items():
             levels = np.random.uniform(l_bound[key], u_bound[key], size = value)
             X[...,key] = np.random.choice(levels, size = len(X), replace=True)
             
         out_flag = 1
     if type(X) != np.ndarray:
         X = np.array(X)
     Sw = X[..., 0]
```

### Comparing `gpplus-0.0.1.221/gpplus/test_functions/calibration_multi_fidelity.py` & `gpplus-0.0.2.1/gpplus/test_functions/calibration_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/test_functions/multi_fidelity.py` & `gpplus-0.0.2.1/gpplus/test_functions/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/utils/input_space.py` & `gpplus-0.0.2.1/gpplus/utils/input_space.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/utils/transforms.py` & `gpplus-0.0.2.1/gpplus/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/utils/variables.py` & `gpplus-0.0.2.1/gpplus/utils/variables.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/visual/plot_latent.py` & `gpplus-0.0.2.1/gpplus/visual/plot_latent.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/visual/plot_latenth.py` & `gpplus-0.0.2.1/gpplus/visual/plot_latenth.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus/visual/plot_latenth_position.py` & `gpplus-0.0.2.1/gpplus/visual/plot_latenth_position.py`

 * *Files identical despite different names*

### Comparing `gpplus-0.0.1.221/gpplus.egg-info/PKG-INFO` & `gpplus-0.0.2.1/gpplus.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gpplus
-Version: 0.0.1.221
+Version: 0.0.2.1
 Summary: Python Library for Generalized Gaussian Process Modeling
 Home-page: https://github.com/Bostanabad-Research-Group/GP-Plus
 Author: Amin Yousefpour, Ramin Bostanabad
 Author-email: yousefpo@uci.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 UNKNOWN
```

### Comparing `gpplus-0.0.1.221/gpplus.egg-info/SOURCES.txt` & `gpplus-0.0.2.1/gpplus.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 gpplus/kernels/wighted_RBF_Z.py
 gpplus/likelihoods_noise/__init__.py
 gpplus/likelihoods_noise/multifidelity.py
 gpplus/models/__init__.py
 gpplus/models/gp_plus.py
 gpplus/models/gpregression.py
 gpplus/optim/__init__.py
-gpplus/optim/mll_noise_tune.py
-gpplus/optim/mll_noise_tune2.py
-gpplus/optim/mll_noise_tune3.py
+gpplus/optim/mll_noise_continuation.py
 gpplus/optim/mll_scipy.py
 gpplus/optim/mll_torch.py
 gpplus/preprocessing/Data_reader.py
 gpplus/preprocessing/__init__.py
 gpplus/preprocessing/normalizeX.py
 gpplus/preprocessing/numericlevels.py
 gpplus/preprocessing/one_hot_encoding.py
@@ -36,14 +34,15 @@
 gpplus/priors/horseshoe.py
 gpplus/priors/mollified_uniform.py
 gpplus/test_functions/__init__.py
 gpplus/test_functions/analytical.py
 gpplus/test_functions/calibration_multi_fidelity.py
 gpplus/test_functions/multi_fidelity.py
 gpplus/utils/__init__.py
+gpplus/utils/data_type_check.py
 gpplus/utils/input_space.py
 gpplus/utils/interval_score.py
 gpplus/utils/set_seed.py
 gpplus/utils/transforms.py
 gpplus/utils/variables.py
 gpplus/visual/__init__.py
 gpplus/visual/plot_latent.py
```

### Comparing `gpplus-0.0.1.221/setup.py` & `gpplus-0.0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='gpplus',
-    version='0.0.1.221',
+    version='0.0.2.1',
     author='Amin Yousefpour, Ramin Bostanabad',
     author_email='yousefpo@uci.edu',
     description='Python Library for Generalized Gaussian Process Modeling',
     # long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Bostanabad-Research-Group/GP-Plus',
     packages=find_packages(),
@@ -13,19 +13,19 @@
         'numpy==1.24.2',
         'scipy==1.11.1',
         'gpytorch==1.7.0',
         'matplotlib==3.7.1',
         'sobol_seq', 
         'tabulate==0.9.0',
         'pandas==1.5.2',
-        'dill ==0.3.7',
+        'dill==0.3.7',
         'pyro-ppl==1.8.0',
         'pyDOE',
         'botorch==0.6.4',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.9',
 )
```

