# Comparing `tmp/safeaipackage-0.4.1.tar.gz` & `tmp/safeaipackage-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeaipackage-0.4.1.tar", last modified: Mon May 27 07:57:34 2024, max compression
+gzip compressed data, was "safeaipackage-0.5.0.tar", last modified: Wed May 29 10:32:02 2024, max compression
```

## Comparing `safeaipackage-0.4.1.tar` & `safeaipackage-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.701906 safeaipackage-0.4.1/
--rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     4907 2024-05-27 07:57:34.701906 safeaipackage-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4371 2024-05-26 14:20:44.000000 safeaipackage-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.694779 safeaipackage-0.4.1/safeaipackage/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/__init__.py
--rw-rw-rw-   0        0        0     4114 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_accuracy.py
--rw-rw-rw-   0        0        0     3165 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_explainability.py
--rw-rw-rw-   0        0        0     3181 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_fairness.py
--rw-rw-rw-   0        0        0     3042 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_privacy.py
--rw-rw-rw-   0        0        0     8219 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/check_robustness.py
-drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.699909 safeaipackage-0.4.1/safeaipackage/utils/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/utils/__init__.py
--rw-rw-rw-   0        0        0     3801 2024-05-26 18:09:20.000000 safeaipackage-0.4.1/safeaipackage/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-05-27 07:57:34.700907 safeaipackage-0.4.1/safeaipackage.egg-info/
--rw-rw-rw-   0        0        0     4907 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-27 07:57:34.000000 safeaipackage-0.4.1/safeaipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 07:57:34.702907 safeaipackage-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1051 2024-05-27 07:28:19.000000 safeaipackage-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:32:02.376246 safeaipackage-0.5.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 safeaipackage-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5204 2024-05-29 10:32:02.376246 safeaipackage-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4668 2024-05-29 09:59:31.000000 safeaipackage-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 10:32:02.361952 safeaipackage-0.5.0/safeaipackage/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:09:20.000000 safeaipackage-0.5.0/safeaipackage/__init__.py
+-rw-rw-rw-   0        0        0     4133 2024-05-29 10:07:44.000000 safeaipackage-0.5.0/safeaipackage/check_accuracy.py
+-rw-rw-rw-   0        0        0     3304 2024-05-29 10:12:49.000000 safeaipackage-0.5.0/safeaipackage/check_explainability.py
+-rw-rw-rw-   0        0        0     3310 2024-05-29 10:14:32.000000 safeaipackage-0.5.0/safeaipackage/check_fairness.py
+-rw-rw-rw-   0        0        0     3153 2024-05-29 10:15:49.000000 safeaipackage-0.5.0/safeaipackage/check_privacy.py
+-rw-rw-rw-   0        0        0     8370 2024-05-29 10:18:40.000000 safeaipackage-0.5.0/safeaipackage/check_robustness.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:32:02.374156 safeaipackage-0.5.0/safeaipackage/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:09:20.000000 safeaipackage-0.5.0/safeaipackage/utils/__init__.py
+-rw-rw-rw-   0        0        0     2866 2024-05-29 08:31:08.000000 safeaipackage-0.5.0/safeaipackage/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:32:02.361952 safeaipackage-0.5.0/safeaipackage.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-29 10:32:02.000000 safeaipackage-0.5.0/safeaipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2024-05-29 10:32:02.000000 safeaipackage-0.5.0/safeaipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:32:02.000000 safeaipackage-0.5.0/safeaipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 10:32:02.000000 safeaipackage-0.5.0/safeaipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:32:02.376246 safeaipackage-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2024-05-29 08:32:12.000000 safeaipackage-0.5.0/setup.py
```

### Comparing `safeaipackage-0.4.1/LICENSE` & `safeaipackage-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safeaipackage-0.4.1/PKG-INFO` & `safeaipackage-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: safeaipackage
-Version: 0.4.1
-Summary: SAFE AI package to measure risks of AI models
-Author: Golnoosh Babaei
-Author-email: <golnoosh.babaei93@gmail.com>
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SAFE AI
 
 The increasing widespread of Artificial Intelligence (AI) applications implies the formalisa-
 tion of an AI risk management model which needs methodological guidelines for an effec-
 tive implementation. To fill the gap, [Giudici and Raffinetti (2023)](https://www.sciencedirect.com/science/article/pii/S1544612323004609) 
 introduced a S.A.F.E.
 risk management model which derives from the proposed international regulations four main
@@ -52,18 +37,29 @@
 # Install
 
 Simply use:
 
 pip install safeaipackage
 
 
+# GitHub
+
+https://github.com/GolnooshBabaei/safeaipackage
+
+
+# Complementary package
+
+The safeaipackage works only with scikit-learn models. Therefore, if you need to evaluate other types of models you can use the following [package](https://pypi.org/project/modelagnosticsafeaipackage/):
+
+pip install modelagnosticsafeaipackage
+
+
 # Example
 
-In the folder "examples", we provide two notebooks related to a classification and a regression problem applied to the [employee dataset](https://search.r-project.org/CRAN/refmans/stima/html/employee.html).
-This dataset can also be downloaded from this folder. 
+On GitHub, in the folder "examples", we provide two notebooks related to a classification and a regression problem applied to the [employee dataset](https://search.r-project.org/CRAN/refmans/stima/html/employee.html).
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0)
```

### Comparing `safeaipackage-0.4.1/README.md` & `safeaipackage-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: safeaipackage
+Version: 0.5.0
+Summary: SAFE AI package to measure risks of AI models
+Author: Golnoosh Babaei
+Author-email: <golnoosh.babaei93@gmail.com>
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SAFE AI
 
 The increasing widespread of Artificial Intelligence (AI) applications implies the formalisa-
 tion of an AI risk management model which needs methodological guidelines for an effec-
 tive implementation. To fill the gap, [Giudici and Raffinetti (2023)](https://www.sciencedirect.com/science/article/pii/S1544612323004609) 
 introduced a S.A.F.E.
 risk management model which derives from the proposed international regulations four main
@@ -37,18 +52,29 @@
 # Install
 
 Simply use:
 
 pip install safeaipackage
 
 
+# GitHub
+
+https://github.com/GolnooshBabaei/safeaipackage
+
+
+# Complementary package
+
+The safeaipackage works only with scikit-learn models. Therefore, if you need to evaluate other types of models you can use the following [package](https://pypi.org/project/modelagnosticsafeaipackage/):
+
+pip install modelagnosticsafeaipackage
+
+
 # Example
 
-In the folder "examples", we provide two notebooks related to a classification and a regression problem applied to the [employee dataset](https://search.r-project.org/CRAN/refmans/stima/html/employee.html).
-This dataset can also be downloaded from this folder. 
+On GitHub, in the folder "examples", we provide two notebooks related to a classification and a regression problem applied to the [employee dataset](https://search.r-project.org/CRAN/refmans/stima/html/employee.html).
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0)
```

### Comparing `safeaipackage-0.4.1/safeaipackage/check_accuracy.py` & `safeaipackage-0.5.0/safeaipackage/check_accuracy.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,19 @@
         self.ytest = pd.DataFrame(ytest).reset_index(drop=True)
         self.model = model
         model_full = self.model.fit(xtrain, ytrain)
         self.yhat_cm = pd.DataFrame(model_full.predict(xtest)).reset_index(drop=True)
          
     def rga(self):
         """
-        ### RANK GRADUATION ACCURACY (RGA) MEASURE ###
-        Function for the RGE measure computation
+        RANK GRADUATION ACCURACY (RGA) MEASURE
+        Function for the RGA measure computation
+
+        Returns:
+        RGA  : Calculated RGA measure
         """ 
         df = pd.concat([self.ytest,self.yhat_cm], axis=1)
         df.columns = ["y", "yhat"]
         ryhat = self.yhat_cm.rank(method="min")
         df["ryhat"] = ryhat
         support = df.groupby('ryhat')['y'].mean().reset_index(name='support')
         rord = list(range(len(self.ytest)))
@@ -33,26 +36,28 @@
             for ii in range(len(support)):
                     if df["ryhat"][jj]== support['ryhat'][ii]:
                         rord[jj] = support['support'][ii]
         vals = [[i, values] for i, values in enumerate(df["yhat"])]
         ranks = [x[0] for x in sorted(vals, key= lambda item: item[1])]
         ystar = [rord[i] for i in ranks]
         I = list(range(len(self.ytest)))
-        conc = 2*sum([I[i]*ystar[i] for i in range(len(I))])
-        dec= 2*sum([sorted(df["y"], reverse=True)[i]*I[i] for i in range(len(I))]) 
-        inc = 2*sum([sorted(df["y"])[i]*I[i] for i in range(len(I))]) 
+        conc = sum([I[i]*ystar[i] for i in range(len(I))])
+        dec= sum([sorted(df["y"], reverse=True)[i]*I[i] for i in range(len(I))]) 
+        inc = sum([sorted(df["y"])[i]*I[i] for i in range(len(I))]) 
         RGA=(conc-dec)/(inc-dec)
         return RGA
     
     
     def rga_statistic_test(self, problemtype, variable= np.nan):
         """
-        RGA based test for comparing the predictive accuracy of the model with that of a reduced model: full model
-        without one variable, if the variable is selected by the user otherwise the predictive accuracy of the model 
-        is compared with a baseline
+        RGA based test for comparing the predictive accuracy of a reduced model with that of a more complex model Or 
+        compare the model with a random model
+        
+        Returns:
+        p_value : p-value for the statistical test
         """
         if problemtype not in ["classification", "prediction"]:
             raise ValueError("problemtype should be classification or prediction")
                              
         if variable is not np.nan: 
             xtrain_rm = self.xtrain.drop(variable, axis=1)
             xtest_rm = self.xtest.drop(variable, axis=1)
```

### Comparing `safeaipackage-0.4.1/safeaipackage/check_explainability.py` & `safeaipackage-0.5.0/safeaipackage/check_explainability.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,19 @@
         self.ytest = pd.DataFrame(ytest).reset_index(drop=True)
         self.model = model
         model_full = self.model.fit(xtrain, ytrain)
         self.yhat = pd.DataFrame(model_full.predict(xtest)).reset_index(drop=True)
          
     def rge(self):
         """
-        ### RANK GRADUATION EXPLAINABILITY (RGE) MEASURE ###
+        RANK GRADUATION EXPLAINABILITY (RGE) MEASURE
         Function for the RGE measure computation
+        
+        Returns:
+        RGE  : Calculated RGE measure
         """ 
         rge_list = []
         model_full = self.model.fit(self.xtrain, self.ytrain)
         yhat = model_full.predict(self.xtest)
         for i in self.xtrain.columns:
             xtrain_rm = self.xtrain.drop(i, axis=1)
             xtest_rm = self.xtest.drop(i, axis=1)
@@ -41,14 +44,17 @@
         plt.show()
         return rge_df
     
     def rge_statistic_test(self, variable):
         """
         RGE based test for comparing the ordering of the ranks related to the full model with that of the
         reduced model without the predictor of interest
+        
+        Returns:
+        p_value : p-value for the statistical test
         """
         if variable not in self.xtrain.columns:
             raise ValueError("protected variable is not available.")
         xtrain_rm = self.xtrain.drop(variable, axis=1)
         xtest_rm = self.xtest.drop(variable, axis=1)
         model_rm = self.model.fit(xtrain_rm, self.ytrain)
         yhat_xk = pd.DataFrame(model_rm.predict(xtest_rm)).reset_index(drop=True)
```

### Comparing `safeaipackage-0.4.1/safeaipackage/check_fairness.py` & `safeaipackage-0.5.0/safeaipackage/check_fairness.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,19 @@
         self.ytest = pd.DataFrame(ytest).reset_index(drop=True)
         self.model = model
         model_full = self.model.fit(xtrain, ytrain)
         self.yhat = pd.DataFrame(model_full.predict(xtest)).reset_index(drop=True)
          
     def rgf(self, protectedvariable):
         """
-        ### RANK GRADUATION FAIRNESS (RGF) MEASURE ###
+        RANK GRADUATION FAIRNESS (RGF) MEASURE 
         Function for the RGF measure computation
+        
+        Returns:
+        RGF  : Calculated RGF measure
         """   
         if not isinstance(protectedvariable, list):
             raise ValueError("Protectedvariables input must be a list")
         for i in range(len(list(protectedvariable))):
             if protectedvariable[i] not in self.xtrain:
                 raise ValueError(f"{protectedvariable[i]} is not in the variables")
         rgf_list = []
@@ -36,15 +39,18 @@
             rgf_list.append(_rga(self.yhat, yhat_pr))
         return pd.DataFrame(rgf_list, index=protectedvariable, columns=["RGF"]).sort_values(by="RGF", ascending=False)
 
     
     def rgf_statistic_test(self, protectedvariable):
         """
         RGF based test for comparing the ordering of the ranks related to the full model with that of the
-        reduced model without the protected variable of interest
+        reduced model without the protected variable 
+        
+        Returns:
+        p_value : p-value for the statistical test
         """
         if protectedvariable not in self.xtrain.columns:
             raise ValueError("protected variable is not available.")
         xtrain_pr = self.xtrain.drop(protectedvariable, axis=1)
         xtest_pr = self.xtest.drop(protectedvariable, axis=1)
         model_pr = self.model.fit(xtrain_pr, self.ytrain)
         yhat_pr = pd.DataFrame(model_pr.predict(xtest_pr)).reset_index(drop=True)
```

### Comparing `safeaipackage-0.4.1/safeaipackage/check_privacy.py` & `safeaipackage-0.5.0/safeaipackage/check_privacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import numpy as np
 import scipy
-from .utils.util import _delta_function, _rga_random, _rga, _num, _den, _rge_delta_function
+from .utils.util import _delta_function, _rga, _num, _den, _rge_delta_function
 
 class Privacy:
     def __init__(self, xtrain, xtest, ytrain, ytest, model):
         """
         Inputs: xtrain, xtest, ytrain, ytest -> the train and test data selected for training and testing the model; 
         model -> a classification or regression model. For example RandomForestClassifier() in ensemble module of sklearn.
         """
@@ -15,16 +15,19 @@
         self.ytest = pd.DataFrame(ytest).reset_index(drop=True)
         self.model = model
         model_full = self.model.fit(xtrain, ytrain)
         self.yhat = pd.DataFrame(model_full.predict(xtest)).reset_index(drop=True)
          
     def rgp(self, index):
         """
-        ### RANK GRADUATION PRIVACY (RGP) MEASURE ###
+        RANK GRADUATION PRIVACY (RGP) MEASURE 
         Function for the RGP measure computation
+
+        Returns:
+        RGP  : Calculated RGP measure
         """      
         if not isinstance(index, list):
             raise ValueError("Index input must be a list")
         for i in index:
             if i not in self.xtrain.index:
                 raise ValueError(f"index {i} is not available.")
         rgp_list = []
@@ -40,14 +43,17 @@
         return pd.DataFrame(rgp_list, index=index, columns=["RGP"])
 
     
     def rgp_statistic_test(self, index):
         """
         RGP based test for comparing the ordering of the ranks related to the full model with that of the
         reduced model without the observation of interest
+
+        Returns:
+        p_value : p-value for the statistical test
         """
         xtrain_rm = self.xtrain.drop(index, axis=0)
         ytrain_rm = self.ytrain.drop(index, axis=0)
         model_rm = self.model.fit(xtrain_rm, ytrain_rm)
         yhat_rm = pd.DataFrame(model_rm.predict(self.xtest)).reset_index(drop=True)
         jk_mat = pd.concat([self.yhat, yhat_rm], axis=1)
         jk_mat.columns = ["yhat", "yhat_rm"]
```

### Comparing `safeaipackage-0.4.1/safeaipackage/check_robustness.py` & `safeaipackage-0.5.0/safeaipackage/check_robustness.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import scipy
 from sklearn.dummy import DummyClassifier, DummyRegressor
-from .utils.util import _delta_function, _rga_random, _rga
+from .utils.util import _delta_function, _rga
 
 class Robustness():
     def __init__(self, xtrain, xtest, ytrain, ytest, model):
         """
         Inputs: xtrain, xtest, ytrain, ytest -> the train and test data selected for training and testing the model; 
         model -> a classification or regression model. For example RandomForestClassifier() in ensemble module of sklearn.
         """
@@ -16,16 +16,16 @@
         self.ytest = pd.DataFrame(ytest).reset_index(drop=True)
         self.model = model
         model_full = self.model.fit(xtrain, ytrain)
         self.yhat = pd.DataFrame(model_full.predict(xtest)).reset_index(drop=True)
         
     def perturb(self, data, variable, perturbation_percentage= 0.05):
         """
-         Function to perturb a single variable based on the replacement of the two percentiles selected using the
-         perturbation_percentage of the object.
+        Function to perturb a single variable based on the replacement of the two percentiles selected using the
+        perturbation_percentage of the object.
         """ 
         if perturbation_percentage > 0.5 or perturbation_percentage < 0:
             raise ValueError("The perturbation percentage should be between 0 and 0.5.")
             
         data = data.reset_index(drop=True)
         perturbed_variable = data.loc[:,variable]
         vals = [[i, values] for i, values in enumerate(perturbed_variable)]
@@ -44,16 +44,20 @@
             new_variable[lowertail_indices[j]] = perturbed_variable[uppertail_indices[j]]
             new_variable[uppertail_indices[j]] = perturbed_variable[lowertail_indices[j]]
         data.loc[:,variable] = new_variable
         return data
 
     def rgr_single(self, variable, perturbation_percentage= 0.05):
         """
-         ### RANK GRADUATION Robustness (RGR) MEASURE ###
-         Function for the RGR measure computation regarding perturbation of a single variable
+        RANK GRADUATION Robustness (RGR) MEASURE
+        Function for the RGR measure computation regarding perturbation of a single variable
+
+
+        Returns:
+        RGR  : Calculated RGR measure
         """ 
         if perturbation_percentage > 0.5 or perturbation_percentage < 0:
             raise ValueError("The perturbation percentage should be between 0 and 0.5.")
             
         if variable not in self.xtrain.columns:
             raise ValueError("The selected variable is not available.")
 
@@ -62,16 +66,19 @@
         yhat_pert = rf_perturbed.predict(self.xtest)
         rgr_val = _rga(self.yhat, yhat_pert)
         return rgr_val
     
     
     def rgr_all(self, perturbation_percentage= 0.05):
         """
-         ### RANK GRADUATION Robustness (RGR) MEASURE ###
-         Function for the RGR measure computation regarding perturbation of all variables
+        RANK GRADUATION Robustness (RGR) MEASURE 
+        Function for the RGR measure computation regarding perturbation of all variables
+
+        Returns:
+        RGR  : Calculated RGR measure
         """ 
         if perturbation_percentage > 0.5 or perturbation_percentage < 0:
             raise ValueError("The perturbation percentage should be between 0 and 0.5.")    
         perturbed_xtrain = self.xtrain.copy()
         for i in self.xtrain.columns:
             perturbed_xtrain[i] = self.perturb(self.xtrain, i, perturbation_percentage)[i]
         rf_perturbed = self.model.fit(perturbed_xtrain, self.ytrain)
@@ -81,14 +88,17 @@
     
     def rgr_statistic_test(self, problemtype, secondmodel= np.nan, variable= np.nan, perturbation_percentage= 0.05):
         """
         RGR based test for comparing the robustness of a model with that of a further model if a value is set
         for the secondmodel. In this case, variable should be set as well. If the second model and variable are
         not given by the user, this test function compares the main model of the class object with a baseline model
         depending on the type of the problem defined by the problemtype, either classification or prediction.
+
+        Returns:
+        p_value : p-value for the statistical test
         """
         if problemtype not in ["classification", "prediction"]:
             raise ValueError("problemtype should be classification or prediction")
         if secondmodel is not np.nan:
             secondmodel = secondmodel
         else:
             if problemtype == "classification":
@@ -138,10 +148,10 @@
             jk_results = []
             for i in range(n):
                 jk_sample = jk_mat.iloc[[x for x in index if x != i],:]
                 jk_sample.reset_index(drop=True, inplace=True)
                 jk_statistic = _delta_function(jk_sample, _rga)
                 jk_results.append(jk_statistic)
             se = np.sqrt(((n-1)/n)*(sum([(x-np.mean(jk_results))**2 for x in jk_results])))
-            z = (_rga(self.yhat, yhat_pert)- _rga_random(yhat_mod2, yhat_mode2_pert))/se
+            z = (_rga(self.yhat, yhat_pert)- _rga(yhat_mod2, yhat_mode2_pert))/se
             p_value = 2*scipy.stats.norm.cdf(-abs(z))
         return p_value
```

### Comparing `safeaipackage-0.4.1/safeaipackage/utils/util.py` & `safeaipackage-0.5.0/safeaipackage/utils/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import pandas as pd
 from sklearn.ensemble import RandomForestClassifier
 
 def _delta_function(data, func):
         result = (func(data.iloc[:,0], data.iloc[:,2]))-(func(data.iloc[:,0], data.iloc[:,1]))
         return result
 
+
 def _rge_delta_function(data):
     return _den(data.iloc[:,0])-_num(data.iloc[:,0], data.iloc[:,1])
 
+
 def _rga(y, yhat):
     y = pd.DataFrame(y).reset_index(drop=True)
     yhat = pd.DataFrame(yhat).reset_index(drop=True)
     df = pd.concat([y,yhat], axis=1)
     df.columns = ["y", "yhat"]
     ryhat = yhat.rank(method="min")
     df["ryhat"] = ryhat
@@ -22,41 +24,20 @@
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
 
-def _rga_random(y, yhat):
-    y = pd.DataFrame(y).reset_index(drop=True)
-    yhat = pd.DataFrame(yhat).reset_index(drop=True)
-    df = pd.concat([y,yhat], axis=1)
-    df.columns = ["y", "yhat"]
-    ryhat = yhat.rank(method="min")
-    df["ryhat"] = ryhat
-    support = df.groupby('ryhat')['y'].mean().reset_index(name='support')
-    rord = list(range(len(y)))
-    for jj in range(len(rord)):
-        for ii in range(len(support)):
-                if df["ryhat"][jj]== support['ryhat'][ii]:
-                    rord[jj] = support['support'][ii]
-    vals = [[i, values] for i, values in enumerate(df["yhat"])]
-    ranks = [x[0] for x in sorted(vals, key= lambda item: item[1])]
-    ystar = [rord[i] for i in ranks]
-    I = list(range(len(y)))
-    conc = 2*sum([I[i]*ystar[i] for i in range(len(I))])
-    dec= 2*sum([sorted(df["y"], reverse=True)[i]*I[i] for i in range(len(I))]) 
-    RGA=(conc-dec)
-    return RGA 
 
 def _num(yhat, yhat_xk):
     yhat = pd.DataFrame(yhat).reset_index(drop=True)
     yhat_xk = pd.DataFrame(yhat_xk).reset_index(drop=True)
     df = pd.concat([yhat,yhat_xk], axis=1)
     df.columns = ["yhat", "yhat_xk"]
     ryhat_xk = yhat_xk.rank(method="min")
```

### Comparing `safeaipackage-0.4.1/safeaipackage.egg-info/PKG-INFO` & `safeaipackage-0.5.0/safeaipackage.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safeaipackage
-Version: 0.4.1
+Version: 0.5.0
 Summary: SAFE AI package to measure risks of AI models
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -52,18 +52,29 @@
 # Install
 
 Simply use:
 
 pip install safeaipackage
 
 
+# GitHub
+
+https://github.com/GolnooshBabaei/safeaipackage
+
+
+# Complementary package
+
+The safeaipackage works only with scikit-learn models. Therefore, if you need to evaluate other types of models you can use the following [package](https://pypi.org/project/modelagnosticsafeaipackage/):
+
+pip install modelagnosticsafeaipackage
+
+
 # Example
 
-In the folder "examples", we provide two notebooks related to a classification and a regression problem applied to the [employee dataset](https://search.r-project.org/CRAN/refmans/stima/html/employee.html).
-This dataset can also be downloaded from this folder. 
+On GitHub, in the folder "examples", we provide two notebooks related to a classification and a regression problem applied to the [employee dataset](https://search.r-project.org/CRAN/refmans/stima/html/employee.html).
 
 
 # Citations
 
 The proposed measures in this package came primarily out of research by 
 [Paolo Giudici](https://www.linkedin.com/in/paolo-giudici-60028a/), [Emanuela Raffinetti](https://www.linkedin.com/in/emanuela-raffinetti-a3980215/), 
 and [Golnoosh Babaei](https://www.linkedin.com/in/golnoosh-babaei-990077187/) in the [Statistical laboratory](https://sites.google.com/unipv.it/statslab-pavia/home?authuser=0)
```

### Comparing `safeaipackage-0.4.1/setup.py` & `safeaipackage-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 # Open README.md with UTF-8 encoding
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '0.4.1'
+VERSION = '0.5.0'
 DESCRIPTION = 'SAFE AI package to measure risks of AI models'
 
 # Setting up
 setup(
     name="safeaipackage",
     version=VERSION,
     author="Golnoosh Babaei",
```

