# Comparing `tmp/modelagnosticsafeaipackage-0.7.0.tar.gz` & `tmp/modelagnosticsafeaipackage-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelagnosticsafeaipackage-0.7.0.tar", last modified: Wed May 29 07:29:32 2024, max compression
+gzip compressed data, was "modelagnosticsafeaipackage-0.8.0.tar", last modified: Wed May 29 10:29:36 2024, max compression
```

## Comparing `modelagnosticsafeaipackage-0.7.0.tar` & `modelagnosticsafeaipackage-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:32.316733 modelagnosticsafeaipackage-0.7.0/
--rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     2645 2024-05-29 07:29:32.314227 modelagnosticsafeaipackage-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2043 2024-05-29 07:29:05.000000 modelagnosticsafeaipackage-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:32.308523 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_accuracy.py
--rw-rw-rw-   0        0        0     1338 2024-05-28 09:45:56.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_explainability.py
--rw-rw-rw-   0        0        0     1298 2024-05-28 09:46:08.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_fairness.py
--rw-rw-rw-   0        0        0     1293 2024-05-28 09:46:15.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_privacy.py
--rw-rw-rw-   0        0        0     1532 2024-05-29 07:16:26.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_robustness.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:32.314227 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/utils/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/utils/__init__.py
--rw-rw-rw-   0        0        0     2876 2024-05-29 07:16:30.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:29:32.312492 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/
--rw-rw-rw-   0        0        0     2645 2024-05-29 07:29:32.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-29 07:29:32.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 07:29:32.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-29 07:29:32.000000 modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 07:29:32.316733 modelagnosticsafeaipackage-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1117 2024-05-29 07:17:03.000000 modelagnosticsafeaipackage-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:29:36.462733 modelagnosticsafeaipackage-0.8.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2651 2024-05-29 10:29:36.462733 modelagnosticsafeaipackage-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2049 2024-05-29 09:58:55.000000 modelagnosticsafeaipackage-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 10:29:36.459479 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/__init__.py
+-rw-rw-rw-   0        0        0     3322 2024-05-29 10:09:37.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_accuracy.py
+-rw-rw-rw-   0        0        0     1779 2024-05-29 10:09:57.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_explainability.py
+-rw-rw-rw-   0        0        0     1729 2024-05-29 10:14:21.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_fairness.py
+-rw-rw-rw-   0        0        0     1738 2024-05-29 10:10:09.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_privacy.py
+-rw-rw-rw-   0        0        0     2115 2024-05-29 09:54:23.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_robustness.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:29:36.462733 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/utils/__init__.py
+-rw-rw-rw-   0        0        0     2792 2024-05-29 09:57:05.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:29:36.462733 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/
+-rw-rw-rw-   0        0        0     2651 2024-05-29 10:29:36.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-29 10:29:36.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:29:36.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-29 10:29:36.000000 modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:29:36.462733 modelagnosticsafeaipackage-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-29 10:29:11.000000 modelagnosticsafeaipackage-0.8.0/setup.py
```

### Comparing `modelagnosticsafeaipackage-0.7.0/LICENSE` & `modelagnosticsafeaipackage-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.7.0/PKG-INFO` & `modelagnosticsafeaipackage-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.7.0
+Version: 0.8.0
 Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MODEL AGNOSTIC SAFE AI
 
-This package is based on [safeaipackage](https://pypi.org/project/safeaipackage/). The main difference between these two packages is the input required by the functions. In safeaipackage there are different function which ask for train\test data and a machine learning model. Then, all the process of the training and evaluation is done inside the function. However, in modelagnosticsafeaipackage, it is only needed to provide the actual values (y) and the predicted values by any model you are interested in. Hence, while safeaipackage only works with scikit-learn models, here you can use your model in interest to find the estimated values and then use this package to evaluate risks of your model.
+This package is based on [safeaipackage](https://pypi.org/project/safeaipackage/). The main difference between these two packages is the input required by the functions. In safeaipackage there are different function which ask for train\test data and a machine learning model. Then, all the process of the training and evaluation is done inside the function. However, in modelagnosticsafeaipackage, it is only needed to provide the actual values (y) and the predicted values by any model you are interested in. Hence, while safeaipackage only works with scikit-learn models, here you can use any kind of model to find the estimated values and then use this package to evaluate risks of your model.
 
 
 # Install
 
 Simply use:
 
 pip install modelagnosticsafeaipackage
@@ -28,15 +28,15 @@
 # GitHub
 
 https://github.com/GolnooshBabaei/safeaipackage/tree/modelagnostic
 
 
 # Example
 
-In the folder "examples", there is a notebook including an example that can help you to understand the functioanlity of this package. 
+On GitHub, in the folder "examples", there is a notebook including an example that can help you to understand the functioanlity of this package. 
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0)
```

### Comparing `modelagnosticsafeaipackage-0.7.0/README.md` & `modelagnosticsafeaipackage-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODEL AGNOSTIC SAFE AI
 
-This package is based on [safeaipackage](https://pypi.org/project/safeaipackage/). The main difference between these two packages is the input required by the functions. In safeaipackage there are different function which ask for train\test data and a machine learning model. Then, all the process of the training and evaluation is done inside the function. However, in modelagnosticsafeaipackage, it is only needed to provide the actual values (y) and the predicted values by any model you are interested in. Hence, while safeaipackage only works with scikit-learn models, here you can use your model in interest to find the estimated values and then use this package to evaluate risks of your model.
+This package is based on [safeaipackage](https://pypi.org/project/safeaipackage/). The main difference between these two packages is the input required by the functions. In safeaipackage there are different function which ask for train\test data and a machine learning model. Then, all the process of the training and evaluation is done inside the function. However, in modelagnosticsafeaipackage, it is only needed to provide the actual values (y) and the predicted values by any model you are interested in. Hence, while safeaipackage only works with scikit-learn models, here you can use any kind of model to find the estimated values and then use this package to evaluate risks of your model.
 
 
 # Install
 
 Simply use:
 
 pip install modelagnosticsafeaipackage
@@ -13,15 +13,15 @@
 # GitHub
 
 https://github.com/GolnooshBabaei/safeaipackage/tree/modelagnostic
 
 
 # Example
 
-In the folder "examples", there is a notebook including an example that can help you to understand the functioanlity of this package. 
+On GitHub, in the folder "examples", there is a notebook including an example that can help you to understand the functioanlity of this package. 
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0)
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_accuracy.py` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_accuracy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pandas as pd
 import numpy as np
 from scipy import stats
 from sklearn.dummy import DummyClassifier, DummyRegressor
 
 def rga(y, yhat):
     """
-    RANK GRADUATION ACCURACY (RGA) MEASURE
-    
+    RANK GRADUATION ACCURACY (RGA) MEASURE 
+    Function for the RGA measure computation
+
     Inputs:
-    y    : Actual values of the target variable (numpy array)
-    yhat : Predicted values generated by the model (numpy array)
+    y    : Actual values of the target variable 
+    yhat : Predicted values generated by the model 
     
     Returns:
     RGA  : Calculated RGA measure
     """
     # Calculate ranks for predicted values
     yhat_ranks = stats.rankdata(yhat, method='min')
 
@@ -23,49 +24,49 @@
     rord = list(range(len(y)))
     rord = np.where(yhat_ranks==1, y_mean_by_rank[0], y_mean_by_rank[1])
     vals = [[i, values] for i, values in enumerate(yhat)]
     ranks = [x[0] for x in sorted(vals, key= lambda item: item[1])]
     ystar = [rord[i] for i in ranks]
     I = np.arange(len(y))
     # Calculate RGA using the support dictionary
-    conc = 2*sum([I[i]*ystar[i] for i in range(len(I))])
-    dec= 2*sum([sorted(y, reverse=True)[i]*I[i] for i in range(len(I))]) 
-    inc = 2*sum([sorted(y)[i]*I[i] for i in range(len(I))]) 
+    conc = sum([I[i]*ystar[i] for i in range(len(I))])
+    dec= sum([sorted(y, reverse=True)[i]*I[i] for i in range(len(I))]) 
+    inc = sum([sorted(y)[i]*I[i] for i in range(len(I))]) 
     RGA=(conc-dec)/(inc-dec)
     
     return RGA
 
 def _delta_function(y, yhat_rm, yhat_cm):
     """
     Delta function for computing the difference between RGA measures of two models.
     
     Inputs:
-    y       : Actual values of the target variable (as a 1D array or list)
-    yhat_rm : Predicted values from the reduced model (as a 1D array or list)
-    yhat_cm : Predicted values from the complex model (as a 1D array or list)
+    y       : Actual values of the target variable 
+    yhat_rm : Predicted values from the reduced model 
+    yhat_cm : Predicted values from the full model 
     
     Returns:
     result  : Delta value (difference in RGA measures)
     """
     rga_rm = rga(y, yhat_rm)
     rga_cm = rga(y, yhat_cm)
     result = rga_cm - rga_rm
     return result
 
 def rga_statistic_test(y, yhat_rm, yhat_cm):
     """
     RGA based test for comparing the predictive accuracy of a reduced model with that of a more complex model.
     
     Inputs:
-    y       : Actual values of the target variable (as a 1D array or list)
-    yhat_rm : Predicted values from the reduced model (as a 1D array or list)
-    yhat_cm : Predicted values from the complex model (as a 1D array or list)
+    y       : Actual values of the target variable 
+    yhat_rm : Predicted values from the reduced model 
+    yhat_cm : Predicted values from the full model 
     
     Returns:
-    p_value : Two-sided p-value for the statistical test
+    p_value : p-value for the statistical test
     """
     # Convert inputs to numpy arrays
     y = np.array(y)
     yhat_rm = np.array(yhat_rm)
     yhat_cm = np.array(yhat_cm)
     
     # Compute the number of samples
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_explainability.py` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_privacy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import pandas as pd
 import numpy as np
 import scipy
-import matplotlib.pyplot as plt
 from .utils.util import _num, _den, _test_delta_function
 from .check_accuracy import rga
 
-  
-def rge(yhat, yhat_rm):
+def rgp(yhat, yhat_rm):
     """
-    ### RANK GRADUATION EXPLAINABILITY (RGE) MEASURE ###
-    Function for the RGE measure computation
-    """ 
-    rge = 1-(rga(yhat, yhat_rm))
-    return rge
+    RANK GRADUATION PRIVACY (RGP) MEASURE 
+    Function for the RGP measure computation
+
+    Inputs:
+    yhat    : Predicted values generated by the full model including all the explanatory variables 
+    yhat_rm : Predicted values generated by the model excluding the selected observation
+    
+    Returns:
+    RGP  : Calculated RGP measure
+    """      
+    rgp = rga(yhat, yhat_rm)
+    return rgp
 
 
-def rge_statistic_test(yhat, yhat_rm):
+def rgp_statistic_test(yhat, yhat_rm):
     """
-    RGE based test for comparing the ordering of the ranks related to the full model with that of the
-    reduced model without the predictor of interest
+    RGP based test for comparing the ordering of the ranks related to the full model with that of the
+    reduced model without the observation of interest
+
+    Inputs:
+    yhat    : Predicted values from the full model
+    yhat_rm : Predicted values from the reduced model 
+    
+    Returns:
+    p_value : p-value for the statistical test
     """
     yhat = np.array(yhat)
     yhat_rm = np.array(yhat_rm)
     
     # Compute the number of samples
     n = len(yhat)
     
@@ -36,9 +48,8 @@
         # Calculate delta function using optimized approach
         delta_statistic = _test_delta_function(jk_yhat, jk_yhat_rm)
         jk_results.append(delta_statistic)
     
     se = np.sqrt(((n-1)/n)*(sum([(x-np.mean(jk_results))**2 for x in jk_results])))
     z = (_den(  yhat)-_num(  yhat,yhat_rm))/se
     p_value = 2*scipy.stats.norm.cdf(-abs(z))
-    return p_value
-
+    return p_value
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_fairness.py` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_explainability.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 import pandas as pd
 import numpy as np
 import scipy
+import matplotlib.pyplot as plt
 from .utils.util import _num, _den, _test_delta_function
 from .check_accuracy import rga
 
-def rgf(yhat, yhat_rm):
+  
+def rge(yhat, yhat_rm):
     """
-    ### RANK GRADUATION FAIRNESS (RGF) MEASURE ###
-    Function for the RGF measure computation
-    """   
-    rgf = rga(yhat, yhat_rm)
-    return rgf
+    RANK GRADUATION EXPLAINABILITY (RGE) MEASURE
+    Function for the RGE measure computation
+
+    Inputs:
+    yhat    : Predicted values generated by the full model including all the explanatory variables 
+    yhat_rm : Predicted values generated by the model excluding the selected variable
+    
+    Returns:
+    RGE  : Calculated RGE measure
+    """ 
+    rge = 1-(rga(yhat, yhat_rm))
+    return rge
 
 
-def rgf_statistic_test(yhat, yhat_rm):
+def rge_statistic_test(yhat, yhat_rm):
     """
-    RGF based test for comparing the ordering of the ranks related to the full model with that of the
-    reduced model without the protected variable of interest
+    RGE based test for comparing the ordering of the ranks related to the full model with that of the
+    reduced model without the predictor of interest
+
+    Inputs:
+    yhat    : Predicted values from the full model
+    yhat_rm : Predicted values from the reduced model 
+    
+    Returns:
+    p_value : p-value for the statistical test
     """
     yhat = np.array(yhat)
     yhat_rm = np.array(yhat_rm)
     
     # Compute the number of samples
     n = len(yhat)
     
@@ -34,8 +50,9 @@
         # Calculate delta function using optimized approach
         delta_statistic = _test_delta_function(jk_yhat, jk_yhat_rm)
         jk_results.append(delta_statistic)
     
     se = np.sqrt(((n-1)/n)*(sum([(x-np.mean(jk_results))**2 for x in jk_results])))
     z = (_den(  yhat)-_num(  yhat,yhat_rm))/se
     p_value = 2*scipy.stats.norm.cdf(-abs(z))
-    return p_value
+    return p_value
+
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/check_robustness.py` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/check_robustness.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 import pandas as pd
 import numpy as np
 import scipy
 from .check_accuracy import rga
-from .utils.util import _delta_function, _rga_random
+from .utils.util import _delta_function, _rga
 
 def rgr(yhat, yhat_pert):
     """
-        ### RANK GRADUATION Robustness (RGR) MEASURE ###
-        Function for the RGR measure computation regarding perturbation of a single variable
+    RANK GRADUATION Robustness (RGR) MEASURE
+    Function for the RGR measure computation regarding perturbation of a single variable
+
+    Inputs:
+    yhat    : Predicted values generated by the full model  
+    yhat_pert : Predicted values generated by the model including the perturbed selected variable
+    
+    Returns:
+    RGR  : Calculated RGR measure
     """ 
     rgr = rga(yhat, yhat_pert)
     return rgr
 
 
 def rgr_statistic_test(yhat, yhat_mod2, yhat_pert, yhat_mode2_pert):
     """
     RGR based test for comparing the robustness of a model with that of a further model when a variable is perturbed.
+    
+    Inputs:
+    yhat    : Predicted values from the first model
+    yhat_mod2 : Predicted values from the second model 
+    yhat_pert    : Predicted values from the first model including the perturbed selected variable
+    yhat_mod2_pert : Predicted values from the second model including the perturbed selected variable
+
+    Returns:
+    p_value : p-value for the statistical test
     """
     yhat = pd.DataFrame(yhat)
     yhat_mod2 = pd.DataFrame(yhat_mod2)
     yhat_pert = pd.DataFrame(yhat_pert)
     yhat_mode2_pert = pd.DataFrame(yhat_mode2_pert)
     
     # Compute jackknife results
@@ -27,14 +43,14 @@
     jk_mat.columns = ["yhat_mod1", "yhat_mode2", "yhat_pert_mode1", "yhat_pert_mode2"]
     n = len(jk_mat)
     index = np.arange(n)
     jk_results = []
     for i in range(n):
         jk_sample = jk_mat.iloc[[x for x in index if x != i],:]
         jk_sample.reset_index(drop=True, inplace=True)
-        jk_statistic = _delta_function(jk_sample, _rga_random)
+        jk_statistic = _delta_function(jk_sample, _rga)
         jk_results.append(jk_statistic)
     se = np.sqrt(((n-1)/n)*(sum([(x-np.mean(jk_results))**2 for x in jk_results])))
-    z = (_rga_random(yhat, yhat_pert)- _rga_random(yhat_mod2, yhat_mode2_pert))/se
+    z = (_rga(yhat, yhat_pert)- _rga(yhat_mod2, yhat_mode2_pert))/se
     p_value = 2*scipy.stats.norm.cdf(-abs(z))
         
     return p_value
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage/utils/util.py` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage/utils/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def _delta_function(data, func):
         result = (func(data.iloc[:,0], data.iloc[:,2]))-(func(data.iloc[:,0], data.iloc[:,1]))
         return result
 
 def _test_delta_function(yhat, yhat_rm):
     return _den(yhat)-_num(yhat, yhat_rm)
 
-def _rga_random(y, yhat):
+def _rga(y, yhat):
     y = pd.DataFrame(y).reset_index(drop=True)
     yhat = pd.DataFrame(yhat).reset_index(drop=True)
     df = pd.concat([y,yhat], axis=1)
     df.columns = ["y", "yhat"]
     ryhat = yhat.rank(method="min")
     df["ryhat"] = ryhat
     support = df.groupby('ryhat')['y'].mean().reset_index(name='support')
@@ -23,17 +23,17 @@
         for ii in range(len(support)):
                 if df["ryhat"][jj]== support['ryhat'][ii]:
                     rord[jj] = support['support'][ii]
     vals = [[i, values] for i, values in enumerate(df["yhat"])]
     ranks = [x[0] for x in sorted(vals, key= lambda item: item[1])]
     ystar = [rord[i] for i in ranks]
     I = list(range(len(y)))
-    conc = 2*sum([I[i]*ystar[i] for i in range(len(I))])
-    dec= 2*sum([sorted(df["y"], reverse=True)[i]*I[i] for i in range(len(I))]) 
-    inc = 2*sum([sorted(df["y"])[i]*I[i] for i in range(len(I))]) 
+    conc = sum([I[i]*ystar[i] for i in range(len(I))])
+    dec= sum([sorted(df["y"], reverse=True)[i]*I[i] for i in range(len(I))]) 
+    inc = sum([sorted(df["y"])[i]*I[i] for i in range(len(I))]) 
     RGA=(conc-dec)/(inc-dec)
     return RGA
 
 def _num(yhat, yhat_xk):
     yhat = pd.DataFrame(yhat).reset_index(drop=True)
     yhat_xk = pd.DataFrame(yhat_xk).reset_index(drop=True)
     df = pd.concat([yhat,yhat_xk], axis=1)
@@ -48,15 +48,14 @@
                     rord[jj] = support['support'][ii]
     vals = [[i, values] for i, values in enumerate(df["yhat_xk"])]
     ranks = [x[0] for x in sorted(vals, key= lambda item: item[1])]
     ystar = [rord[i] for i in ranks]
     I = list(range(len(ystar)))
     conc = 2*sum([I[i]*ystar[i] for i in range(len(I))])
     dec= 2*sum([sorted(df["yhat"], reverse=True)[i]*I[i] for i in range(len(I))]) 
-    inc = 2*sum([sorted(df["yhat"])[i]*I[i] for i in range(len(I))]) 
     RGE_num=(conc-dec)
     return RGE_num
 
 
 def _den(yhat):
     yhat = pd.DataFrame(yhat)
     yhat.columns = ["yhat"]
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/PKG-INFO` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.7.0
+Version: 0.8.0
 Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MODEL AGNOSTIC SAFE AI
 
-This package is based on [safeaipackage](https://pypi.org/project/safeaipackage/). The main difference between these two packages is the input required by the functions. In safeaipackage there are different function which ask for train\test data and a machine learning model. Then, all the process of the training and evaluation is done inside the function. However, in modelagnosticsafeaipackage, it is only needed to provide the actual values (y) and the predicted values by any model you are interested in. Hence, while safeaipackage only works with scikit-learn models, here you can use your model in interest to find the estimated values and then use this package to evaluate risks of your model.
+This package is based on [safeaipackage](https://pypi.org/project/safeaipackage/). The main difference between these two packages is the input required by the functions. In safeaipackage there are different function which ask for train\test data and a machine learning model. Then, all the process of the training and evaluation is done inside the function. However, in modelagnosticsafeaipackage, it is only needed to provide the actual values (y) and the predicted values by any model you are interested in. Hence, while safeaipackage only works with scikit-learn models, here you can use any kind of model to find the estimated values and then use this package to evaluate risks of your model.
 
 
 # Install
 
 Simply use:
 
 pip install modelagnosticsafeaipackage
@@ -28,15 +28,15 @@
 # GitHub
 
 https://github.com/GolnooshBabaei/safeaipackage/tree/modelagnostic
 
 
 # Example
 
-In the folder "examples", there is a notebook including an example that can help you to understand the functioanlity of this package. 
+On GitHub, in the folder "examples", there is a notebook including an example that can help you to understand the functioanlity of this package. 
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0)
```

### Comparing `modelagnosticsafeaipackage-0.7.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt` & `modelagnosticsafeaipackage-0.8.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.7.0/setup.py` & `modelagnosticsafeaipackage-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 # Open README.md with UTF-8 encoding
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '0.7.0'
+VERSION = '0.8.0'
 DESCRIPTION = 'MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL'
 
 # Setting up
 setup(
     name="modelagnosticsafeaipackage",
     version=VERSION,
     author="Golnoosh Babaei",
```

