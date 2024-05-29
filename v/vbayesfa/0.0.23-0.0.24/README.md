# Comparing `tmp/vbayesfa-0.0.23.tar.gz` & `tmp/vbayesfa-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbayesfa-0.0.23.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vbayesfa-0.0.24.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vbayesfa-0.0.23.tar` & `vbayesfa-0.0.24.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      234 2024-04-26 17:46:51.889270 vbayesfa-0.0.23/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.23/src/vbayesfa/.DS_Store
--rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.23/src/vbayesfa/__init__.py
--rw-r--r--   0        0        0    16841 2024-04-08 17:09:57.330242 vbayesfa-0.0.23/src/vbayesfa/bayes_factors.py
--rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.23/src/vbayesfa/exp_families.py
--rw-r--r--   0        0        0     7498 2024-04-26 15:44:45.654627 vbayesfa-0.0.23/src/vbayesfa/finite_lpa.py
--rw-r--r--   0        0        0     2565 2024-04-26 17:40:28.877298 vbayesfa-0.0.23/src/vbayesfa/fit_finite_lpa.py
--rw-r--r--   0        0        0     2576 2024-04-26 16:42:01.807322 vbayesfa-0.0.23/src/vbayesfa/fit_lpa.py
--rw-r--r--   0        0        0     3896 2024-04-25 20:52:37.200820 vbayesfa-0.0.23/src/vbayesfa/fit_lpa2.py
--rw-r--r--   0        0        0     3627 2024-04-26 17:26:36.489698 vbayesfa-0.0.23/src/vbayesfa/fit_mixture_model.py
--rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.23/src/vbayesfa/ibp/discrete_finite.py
--rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.23/src/vbayesfa/ibp/fit_ibp.py
--rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.23/src/vbayesfa/ibp/full_discrete_finite.py
--rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.23/src/vbayesfa/ibp/make_sim_data.py
--rw-r--r--   0        0        0    11261 2024-04-04 15:36:07.290321 vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_cont_finite.py
--rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_pos_cont_finite.py
--rw-r--r--   0        0        0    10900 2024-04-26 15:44:53.989278 vbayesfa-0.0.23/src/vbayesfa/lpa.py
--rw-r--r--   0        0        0    20925 2024-04-10 19:09:07.425525 vbayesfa-0.0.23/src/vbayesfa/lpa_outcome_analysis.py
--rw-r--r--   0        0        0    35808 2024-04-26 16:31:13.132014 vbayesfa-0.0.23/src/vbayesfa/mixture_model.py
--rw-r--r--   0        0        0    40897 2024-04-09 19:30:59.411472 vbayesfa-0.0.23/src/vbayesfa/old_lpa.py
--rw-r--r--   0        0        0    10712 2024-04-17 21:13:53.670539 vbayesfa-0.0.23/src/vbayesfa/simulate_data.py
--rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.23/src/vbayesfa/tests/.DS_Store
--rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.23/src/vbayesfa/tests/test_exp_families.py
--rw-r--r--   0        0        0     1625 2024-04-26 17:43:28.152597 vbayesfa-0.0.23/src/vbayesfa/tests/test_finite_lpa.py
--rw-r--r--   0        0        0     1595 2024-04-26 17:42:56.650573 vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa.py
--rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa_outcome_analysis.py
--rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 vbayesfa-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0      234 2024-05-29 17:31:01.463420 vbayesfa-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.24/src/vbayesfa/.DS_Store
+-rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.24/src/vbayesfa/__init__.py
+-rw-r--r--   0        0        0    16841 2024-04-08 17:09:57.330242 vbayesfa-0.0.24/src/vbayesfa/bayes_factors.py
+-rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.24/src/vbayesfa/exp_families.py
+-rw-r--r--   0        0        0     7498 2024-04-26 15:44:45.654627 vbayesfa-0.0.24/src/vbayesfa/finite_lpa.py
+-rw-r--r--   0        0        0     3998 2024-05-29 17:28:47.618282 vbayesfa-0.0.24/src/vbayesfa/fit_finite_lpa.py
+-rw-r--r--   0        0        0     4005 2024-05-29 17:27:13.141396 vbayesfa-0.0.24/src/vbayesfa/fit_lpa.py
+-rw-r--r--   0        0        0     4082 2024-05-06 14:31:28.004311 vbayesfa-0.0.24/src/vbayesfa/fit_lpa2.py
+-rw-r--r--   0        0        0     5840 2024-05-03 14:20:53.148675 vbayesfa-0.0.24/src/vbayesfa/fit_mixture_model.py
+-rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.24/src/vbayesfa/ibp/discrete_finite.py
+-rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.24/src/vbayesfa/ibp/fit_ibp.py
+-rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.24/src/vbayesfa/ibp/full_discrete_finite.py
+-rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.24/src/vbayesfa/ibp/make_sim_data.py
+-rw-r--r--   0        0        0    11261 2024-04-04 15:36:07.290321 vbayesfa-0.0.24/src/vbayesfa/ibp/sparse_cont_finite.py
+-rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.24/src/vbayesfa/ibp/sparse_pos_cont_finite.py
+-rw-r--r--   0        0        0    10811 2024-05-01 18:57:03.548251 vbayesfa-0.0.24/src/vbayesfa/lpa.py
+-rw-r--r--   0        0        0    21168 2024-05-07 21:02:29.910960 vbayesfa-0.0.24/src/vbayesfa/lpa_outcome_analysis.py
+-rw-r--r--   0        0        0    36149 2024-05-17 17:46:16.325453 vbayesfa-0.0.24/src/vbayesfa/mixture_model.py
+-rw-r--r--   0        0        0    40897 2024-04-09 19:30:59.411472 vbayesfa-0.0.24/src/vbayesfa/old_lpa.py
+-rw-r--r--   0        0        0    10802 2024-05-03 16:52:22.870053 vbayesfa-0.0.24/src/vbayesfa/simulate_data.py
+-rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.24/src/vbayesfa/tests/.DS_Store
+-rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.24/src/vbayesfa/tests/test_exp_families.py
+-rw-r--r--   0        0        0     1625 2024-04-26 17:43:28.152597 vbayesfa-0.0.24/src/vbayesfa/tests/test_finite_lpa.py
+-rw-r--r--   0        0        0     1595 2024-04-26 17:42:56.650573 vbayesfa-0.0.24/src/vbayesfa/tests/test_lpa.py
+-rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.24/src/vbayesfa/tests/test_lpa_outcome_analysis.py
+-rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 vbayesfa-0.0.24/PKG-INFO
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/.DS_Store` & `vbayesfa-0.0.24/src/vbayesfa/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/bayes_factors.py` & `vbayesfa-0.0.24/src/vbayesfa/bayes_factors.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/exp_families.py` & `vbayesfa-0.0.24/src/vbayesfa/exp_families.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/finite_lpa.py` & `vbayesfa-0.0.24/src/vbayesfa/finite_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/fit_lpa2.py` & `vbayesfa-0.0.24/src/vbayesfa/fit_lpa2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
+import pandas as pd
 import functools
 import multiprocessing
-from .fit_finite_lpa import fit_finite_lpa
 from .lpa import lpa_model
 from time import perf_counter
+from scipy.cluster.vq import kmeans2
 
 def fit_lpa2(x, n_workers = 4, restarts = 20, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 1000, min_iter = 10):
     """
     Fit a Dirichlet process latent profile analysis (DPM-LPA) model using mean field
     variational Bayes.
     
     This version of the function fits finite LPA models first to provide starting points
@@ -45,20 +46,31 @@
     min_iter: integer, optional
         Minimum number of iterations to run the optimization.
         
     Notes
     -----
     This creates multiple lpa_model objects from the lpa.py module and fits them with using parallel
     processing. See the documentation for the lpa_model object for more details.
-    """
-    finite_fits = fit_finite_lpa(x, T_range = np.arange(2, T + 1), prior_alpha_pi = 0.5, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, restarts = restarts, seed = seed)
-    phi_list = [finite_fits.loc[Tval, 'best_model'].phi for Tval in np.arange(2, T + 1)]
+    """    
+    # initialize with k-means
+    if isinstance(x, pd.DataFrame):
+        x = x.values.copy().transpose()
+    n = x.shape[1]
+    phi_list = []
+    for Tval in range(2, T + 1, 1):
+        centroid, label = kmeans2(x.T, k = Tval, minit = '++', seed = seed)
+        #phi = np.zeros([Tval, n])
+        phi = np.ones([Tval, n])*0.3/(Tval - 1)
+        for i in range(n):
+            #phi[label[i], i] = 1.0
+            phi[label[i], i] = 0.7
+        phi_list += [phi]
+    
     model_list = []
     final_elbo = []
-    
     with multiprocessing.Pool(n_workers) as pool:
         fun = functools.partial(_model_fit_wrapper, x = x, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)        
         results = pool.map(fun, phi_list)
     for result in results:
         model_list += [result]
         final_elbo += [result.elbo_list[-1]]
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/fit_mixture_model.py` & `vbayesfa-0.0.24/src/vbayesfa/fit_lpa.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,74 @@
-import numpy as np
-import functools
-import multiprocessing
-from time import perf_counter
-from vbayesfa.lpa import lpa_model
-from vbayesfa.finite_lpa import finite_lpa_model
+from .fit_mixture_model import fit_mixture_model
+from .lpa import lpa_model
 
-def fit_mixture_model(x,
-                      model_class = lpa_model,
-                      n_workers = 4, 
-                      restarts = 20, 
-                      T = 20,
-                      seed = 1234, 
-                      tolerance = 1e-05, 
-                      max_iter = 1000, 
-                      min_iter = 10,
-                      **prior_hpar):
+def fit_lpa(x, n_workers = 4, kmeans = False, restarts = 20, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 1000, min_iter = 10):
     """
-    Fit a mixture model using mean field variational Bayes.
+    Fit a Dirichlet process latent profile analysis (DPM-LPA) model using mean field
+    variational Bayes.
     
     Parameters
     ----------
     x: data frame or array
         Observed data (data frame or matrix).  If a matrix then rows are variables and columns
         are observations; if a data frame then rows are observations and columns are variables.
-    model_class: class, optional
-        Class of mixture model to fit.
     n_workers: int, optional
         Number of workers in the pool for parallel processing; should be less than
         or equal to the number of available CPUs.
+    kmeans: logical, optional
+        Should the k-means++ algorithm be used for initial starting points?
+        If so, then k-means clusterings of different sizes are produced and used.
     restarts: int, optional
         Number of random restarts.
     T: integer, optional
         Truncation level of the variational approximation.
+    prior_w1: float, optional
+        First prior hyperparameter on alpha.
+    prior_w2: float, optional
+        Second prior hyperparameter on alpha.
+    prior_lambda_mu: float, optional
+        Controls the width of the prior distribution on mu: 
+        higher values -> tighter prior around 0.
+    prior_strength_for_xi: float, optional
+        Controls the strength of the gamma prior distribution on xi.
+        This prior is assumed to have a mean of 1, with alpha = prior_strength_for_xi/2
+        and beta = prior_strength_for_xi/2.
     seed: int, optional
         Random seed (determines starting conditions of each optimization).
     tolerance: float, optional
         Relative change in the ELBO at which the optimization should stop.
     max_iter: integer, optional
         Maximum number of iterations to run the optimization.
     min_iter: integer, optional
         Minimum number of iterations to run the optimization.
-    prior_hpar:
-        Prior hyperparameters (specified with keywords).
-        
+    
     Notes
     -----
-    This creates multiple mixture model objects and fits them using parallel
-    processing. See the documentation for the lpa_model object for more details.
+    This is a wrapper for the fit_mixture_model function.
+    
+    One fits a statistical model using variational Bayes by maximizing a quantity called
+    the ELBO (evidence lower bound). The best variational Bayes approximation of the true
+    model posterior distribution is the one with the highest ELBO. The algorithm for maximizing
+    the ELBO unfortunately only finds local maxima, so to have a decent chance of finding the
+    global maximum (truly best approximation to the real model posterior distribution) we need
+    different starting points of the variational model hyperparameters. This function provides two
+    ways to choose starting points. First, the k-means++ algorithm (a simple clustering algorithm)
+    can be used to produce initial clustering of participants. Second, participants can be randomly
+    assigned (in a 'soft' way) to different mixture components/latent classes/latent profiles. These
+    two methods are not exclusive: both types of starting point will be used if 'kmeans' is set to
+    True and 'restarts' > 0. The function creates a separate mixture model object with each starting
+    point and fits them using parallel processing for speed.
     
     Output
     ------
     A dictionary with the following:
     
     final_elbo: list
         Final ELBO (evidence lower bound) values of each model.
     model_list: list
         Fitted model objects.
     best_model: mixture_model object
         Best fitted model (i.e. the one with the highest ELBO).
     fit_time: float
         Total time used to fit.
     """
-    tic = perf_counter()
-
-    model_list = []
-    final_elbo = []
-    
-    with multiprocessing.Pool(n_workers) as pool:
-        fun = functools.partial(__model_fit_wrapper__, x = x, T = T, model_class = model_class, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter, **prior_hpar)
-        
-        # generate random seeds for each model based on the seed parameter
-        seed_list = []
-        rng = np.random.default_rng(seed)
-        for i in range(restarts):
-            seed_list += [rng.integers(low = 1000, high = 9999)]
-        
-        results = pool.map(fun, seed_list)
-        for result in results:
-            model_list += [result]
-            final_elbo += [result.elbo_list[-1]]
-        
-    final_elbo = np.array(final_elbo)
-    toc = perf_counter()
-    
-    return {'final_elbo': final_elbo, 'model_list': model_list, 'best_model': model_list[final_elbo.argmax()], 'fit_time': toc - tic}
-
-def __model_fit_wrapper__(seed, x, T, model_class, tolerance, max_iter, min_iter, **prior_hpar):
-    """
-    Defines a mixture model and fits it to the data, returning the result.
-    This function is only defined in order to get the parallelization to work.
-    """
-    new_model = model_class(x = x, T = T, seed = seed, **prior_hpar)
-    new_model.fit(tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
-    return new_model
+    return fit_mixture_model(x = x, model_class = lpa_model, n_workers = n_workers, kmeans = kmeans, restarts = restarts, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, seed = seed, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/ibp/discrete_finite.py` & `vbayesfa-0.0.24/src/vbayesfa/ibp/discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/ibp/fit_ibp.py` & `vbayesfa-0.0.24/src/vbayesfa/ibp/fit_ibp.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/ibp/full_discrete_finite.py` & `vbayesfa-0.0.24/src/vbayesfa/ibp/full_discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/ibp/make_sim_data.py` & `vbayesfa-0.0.24/src/vbayesfa/ibp/make_sim_data.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_cont_finite.py` & `vbayesfa-0.0.24/src/vbayesfa/ibp/sparse_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/ibp/sparse_pos_cont_finite.py` & `vbayesfa-0.0.24/src/vbayesfa/ibp/sparse_pos_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/lpa.py` & `vbayesfa-0.0.24/src/vbayesfa/lpa.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,14 @@
         # update distribution of stick-breaking lengths (V)
         for t in range(self.T):
             self.gamma1[t] = 1 + np.sum(self.phi[t,:])
             self.gamma2[t] = self.E_alpha + np.sum(self.phi[range(t+1,self.T),:])
             self.E_log_V[t] = digamma(self.gamma1[t]) - digamma(self.gamma1[t] + self.gamma2[t])
             self.E_log_1minusV[t] = digamma(self.gamma2[t]) - digamma(self.gamma1[t] + self.gamma2[t]) 
         for t in range(self.T):
-            #self.E_log_pi[t] = self.E_log_V[t] + np.sum(self.E_log_1minusV[range(t-1)])
             self.E_log_pi[t] = self.E_log_V[t] + np.sum(self.E_log_1minusV[range(t-1+1)])
         self.E_V = self.gamma1/(self.gamma1 + self.gamma2)
         product_term = np.concatenate([np.array([1]), np.cumprod(1 - self.E_V)[range(self.T-1)]])
         self.E_pi = self.E_V*product_term
         
     def _update_q_alpha(self):
         # update distribution of the Dirichlet process concentration parameter (alpha)
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/lpa_outcome_analysis.py` & `vbayesfa-0.0.24/src/vbayesfa/lpa_outcome_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 def fit_y_normal(model,
                  y,
                  x_new = None,
                  y_new = None,
                  index = None,
                  profile_labels = None,
+                 do_post_hoc = True,
                  start_profile_labels_from1 = False,
                  prior_alpha = 1.0,
                  prior_beta = 1.0,
                  prior_m = 0.0,
                  prior_lambda = 1.0,
                  figure_size = [10, 12],
                  font_size = 11,
@@ -48,14 +49,18 @@
         New LPA model data (from participants not used to fit the LPA model).
     y_new: dataframe
         New outcome data (from participants not used to fit the LPA model).
     index: array-like, optional
         Optional individual participant/observation labels.
     profile_labels: array-like, optional
         Optional labels for latent profiles.
+    do_post_hoc: logical, optional
+        Whether or not to do post-hoc analysis to group profile means into
+        partitions. This can be computationally intensive if there are more
+        than a few profiles.
     start_profile_labels_from1: boolean, optional
         Whether to label latent profiles starting from 0 (Python style)
         or from 1 (R/Matlab/ordinary counting style). This only affects
         output labeling, not any calculations.
     prior_alpha: float, optional
         Prior alpha parameter.
     prior_beta: float, optional
@@ -117,26 +122,29 @@
     ##### SET UP DATA ETC #####
     y_names = pd.Categorical(y.columns.values, categories = y.columns.values, ordered = True)
     if index is None:
         y = y.copy()
     else:
         y = y.iloc[index].copy().transpose()
     n_y = y.shape[1] # number of dependent variables
-        
-    bayes_factor_df = pd.DataFrame(columns = ['bf10', 'log10_bf10', 'conclusion', 'post_hoc_result'],
+    col_names = ['bf10', 'log10_bf10', 'conclusion']
+    if do_post_hoc:
+        col_names += ['post_hoc_result']
+    bayes_factor_df = pd.DataFrame(columns = col_names,
                                    index = y_names) # empty dataframe for results
     
     ##### COMPUTE BAYES FACTORS (BAYESIAN ANOVAS) #####
     for j in range(n_y):
         y_j = y[y_names[j]].values
         bayes_factor_df.loc[y_names[j], 'bf10'] = bayes_factors.bf10_1way_anova(y = y_j, groups = model.z_hat, rscale = 0.5, epsrel = 1e-4, limit = 50)
         bayes_factor_df.loc[y_names[j], 'log10_bf10'] = np.log10(bayes_factor_df.loc[y_names[j], 'bf10'])
         if bayes_factor_df.loc[y_names[j], 'log10_bf10'] > 0.5:
             bayes_factor_df.loc[y_names[j], 'conclusion'] = 'profile means differ'
-            bayes_factor_df.loc[y_names[j], 'post_hoc_result'] = bayes_factors.partition_posthoc(y = y_j, groups = model.z_hat, rscale = 0.5, epsrel = 1e-4, limit = 50)['best_partition'] # post-hoc analysis (partition-based)
+            if do_post_hoc:
+                bayes_factor_df.loc[y_names[j], 'post_hoc_result'] = bayes_factors.partition_posthoc(y = y_j, groups = model.z_hat, rscale = 0.5, epsrel = 1e-4, limit = 50)['best_partition'] # post-hoc analysis (partition-based)
         elif bayes_factor_df.loc[y_names[j], 'log10_bf10'] < 0.5:
             bayes_factor_df.loc[y_names[j], 'conclusion'] = 'profile means ='
         else:
             bayes_factor_df.loc[y_names[j], 'conclusion'] = 'indecisive'
     
     ##### POSTERIOR HYPERPARAMETERS #####
     post_hpar = {'m': np.zeros([n_y, model.n_profiles]), 'lambda': np.zeros([n_y, model.n_profiles]), 'alpha': np.zeros(n_y), 'beta': np.zeros(n_y)}
@@ -162,16 +170,14 @@
     
     ##### MAKE PLOT #####
     plot_df = pd.DataFrame(product(range(n_y), range(model.n_profiles)),
                                 columns = ['j', 'profile'])
     plot_df['variable'] = y_names[plot_df['j'].values]
     plot_df['mu'] = 0.0
     plot_df['v'] = 0.0
-    hard_m_mu = np.zeros([n_y, model.n_profiles])
-    hard_v_mu = np.zeros([n_y, model.n_profiles])
     for r in range(plot_df.shape[0]):
         plot_df.loc[r, 'mu'] = post_hpar['m'][plot_df.iloc[r]['j'].astype(int), plot_df.iloc[r]['profile'].astype(int)]
         plot_df.loc[r, 'v'] = v_mu[plot_df.iloc[r]['j'].astype(int), plot_df.iloc[r]['profile'].astype(int)]
     plot_df['mu_minus'] = plot_df['mu'] - 1.96*np.sqrt(plot_df['v'])
     plot_df['mu_plus'] = plot_df['mu'] + 1.96*np.sqrt(plot_df['v'])
     if start_profile_labels_from1:
         plot_df['profile'] += 1
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/mixture_model.py` & `vbayesfa-0.0.24/src/vbayesfa/mixture_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,18 +246,14 @@
         '''
         pass
     
     def _H_q_z(self):
         '''
         Entropy of the variational distribution over z (profile membership).
         '''
-        #H = 0.0
-        #for i in range(self.n):
-        #    H += multinomial_dist.entropy(1, self.phi[:,i])
-        #return H
         return np.sum([multinomial_dist.entropy(1, self.phi[:,i]) for i in range(self.n)])
     
     def _E_log_prior_z(self):
         '''
         Variational expectation of the log-prior on profile membership (z).
         '''
         # UPDATE
@@ -294,15 +290,15 @@
     def profile_similarity(self, figure_size = (6, 5), font_size = 11, start_profile_labels_from1 = False):
         '''
         Computes pairwise distance and similarity between latent profiles.
         
         Parameters
         ----------
         figure_size: list of floats, optional
-            Size of plots.
+            Size of plot (in inches).
         font_size: integer, optional
             Font size for plots.
         start_profile_labels_from1: boolean, optional
             Whether to label latent profiles starting from 0 (Python style)
             or from 1 (R/Matlab/ordinary counting style). This only affects
             output labeling, not any calculations.
         
@@ -526,15 +522,15 @@
     def plot_residuals(self, figure_size = (6, 5), font_size = 11, ncol = 4, bins = 20):
         '''
         Plot residuals (actual observations - posterior mean predicted observations).
         
         Parameters
         ----------
         figure_size: list of floats, optional
-            Size of plots.
+            Size of plot (in inches).
         font_size: integer, optional
             Font size for plots.
         ncol: integer, optional
             Number of columns to use in plots.
         bins: integer, optional
             Number of bins for histograms.
             
@@ -617,15 +613,15 @@
         Returns
         -------
         A bar plot of estimated latent profile probabilities.
         
         Parameters
         ----------
         figure_size: list of floats, optional
-            Size of plots.
+            Size of plot (in inches).
         font_size: integer, optional
             Font size for plots.
         start_profile_labels_from1: boolean, optional
             Whether to label latent profiles starting from 0 (Python style)
             or from 1 (R/Matlab/ordinary counting style). This only affects
             output labeling, not any calculations.
         '''
@@ -642,21 +638,23 @@
     def plot_profile_means(self, figure_size = (6, 5), font_size = 11, kind = 'bar', facet_var = 'profile', ncol = 4, fancy_labels = True, start_profile_labels_from1 = False):
         '''
         Plot latent profile means.
         
         Parameters
         ----------
         figure_size: list of floats, optional
-            Size of plots.
+            Size of plot (in inches).
         font_size: integer, optional
             Font size for plots.
         kind: string, optional
             Type of plot. Options are 'bar', 'point', and 'point_and_errorbar'.
         facet_var: string, optional
-            Faceting variable for plots.
+            Faceting variable for plots. Options are 'profile', 'profile (flipped)',
+            and 'variable'. The option 'profile (flipped)' flips the x and y axes after
+            facetting by latent profile, which can sometimes make things more readable.
         ncol: integer, optional
             Number of columns to use in plots.
         fancy_labels: boolean, optional
             If True, then profile labels are formatted like "profile 2 (19%)",
             giving the percent of people/observations in that profile.
         start_profile_labels_from1: boolean, optional
             Whether to label latent profiles starting from 0 (Python style)
@@ -676,15 +674,15 @@
         plot_df['mu_minus'] = 0.0
         plot_df['mu_plus'] = 0.0
         for r in range(plot_df.shape[0]):
             plot_df.loc[r, 'mu'] = self.sorted_m_mu[plot_df.iloc[r]['j'], plot_df.iloc[r]['profile']]
             plot_df.loc[r, 'v'] = self.sorted_v_mu[plot_df.iloc[r]['j'], plot_df.iloc[r]['profile']]
         plot_df['mu_minus'] = plot_df['mu'] - 1.96*np.sqrt(plot_df['v'])
         plot_df['mu_plus'] = plot_df['mu'] + 1.96*np.sqrt(plot_df['v'])
-        if fancy_labels and facet_var == 'profile':
+        if fancy_labels and facet_var in ['profile', 'profile (flipped)']:
             # add information about pi (i.e. how many data points are in the profile) to labels
             pct_for_labels = np.round(100*self.prop_per_profile).astype(int) # pi, represented as percentages
             pct_info_list = [ ' (' + str(pct_for_labels[plot_df['profile'][r]]) + '%)' for r in range(plot_df.shape[0])]
             if start_profile_labels_from1:
                 plot_df['profile'] += 1
             plot_df['profile'] = plot_df['profile'].astype('string')
             plot_df['profile'] = plot_df['profile'].str.cat(pct_info_list) # add pi information (as percentages)
@@ -698,15 +696,15 @@
                 plot_df['profile'] += 1
             plot_df['profile'] = plot_df['profile'].astype('string')
             plot_df['profile'] = pd.Categorical(plot_df['profile'].values, 
                                                 categories = plot_df['profile'].values[range(self.n_profiles)], 
                                                 ordered = True)
         
         # make the plot
-        if facet_var == 'profile':
+        if facet_var in ['profile', 'profile (flipped)']:
             plot = p9.ggplot(plot_df, p9.aes(x = 'variable', y = 'mu', ymin = 'mu_plus', ymax = 'mu_minus'))
         elif facet_var == 'variable':
             plot = p9.ggplot(plot_df, p9.aes(x = 'profile', y = 'mu', ymin = 'mu_plus', ymax = 'mu_minus'))
         
         if kind == 'bar':
             plot += p9.geom_bar(stat = 'identity')
         elif kind == 'point':
@@ -718,11 +716,14 @@
             plot += p9.geom_hline(yintercept = 0, linetype = 'dashed')
         plot += p9.theme_classic(base_size = font_size)
         plot += p9.theme(figure_size = figure_size)
         
         if facet_var == 'profile':
             plot += p9.facet_wrap('profile', scales = 'free_x', ncol = ncol)
             plot += p9.theme(axis_text_x = p9.element_text(rotation = 90, hjust = 1))
+        elif facet_var == 'profile (flipped)':
+            plot += p9.coord_flip()
+            plot += p9.facet_wrap('profile', scales = 'free_y', ncol = ncol)
         elif facet_var == 'variable':
             plot += p9.facet_wrap('variable', scales = 'free_x', ncol = ncol)
         
         return plot
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/old_lpa.py` & `vbayesfa-0.0.24/src/vbayesfa/old_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/simulate_data.py` & `vbayesfa-0.0.24/src/vbayesfa/simulate_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,22 @@
     
     Notes
     -----
     The residual variance of simulated data (x) is set at 1.0.
     
     Because of this fact and the fact that profile means (mu) are
     drawn from a normal distribution with mean 0, the following relationship
-    hold between Mahalanobis distance and the 'separation' parameter (variance
+    holds between Mahalanobis distance and the 'separation' parameter (variance
     for drawing profile means):
     
     separation = (average squared Mahalanobis distance)/(2*m)
+    
+    Similarly,
+    
+    separation = (average squared Cohen's d between profiles)/2
     '''
     if seed is None:
         rng = np.random.default_rng()
     else:
         rng = np.random.default_rng(seed = seed)
 
     # overwrite n_profiles if pi is manually specified
```

### Comparing `vbayesfa-0.0.23/src/vbayesfa/tests/.DS_Store` & `vbayesfa-0.0.24/src/vbayesfa/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/tests/test_exp_families.py` & `vbayesfa-0.0.24/src/vbayesfa/tests/test_exp_families.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/tests/test_finite_lpa.py` & `vbayesfa-0.0.24/src/vbayesfa/tests/test_finite_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa.py` & `vbayesfa-0.0.24/src/vbayesfa/tests/test_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.23/src/vbayesfa/tests/test_lpa_outcome_analysis.py` & `vbayesfa-0.0.24/src/vbayesfa/tests/test_lpa_outcome_analysis.py`

 * *Files identical despite different names*

