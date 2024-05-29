# Comparing `tmp/desgld-0.1.4.tar.gz` & `tmp/desgld-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desgld-0.1.4.tar", last modified: Fri May  3 23:52:13 2024, max compression
+gzip compressed data, was "desgld-0.1.5.tar", last modified: Wed May 29 18:00:47 2024, max compression
```

## Comparing `desgld-0.1.4.tar` & `desgld-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.322524 desgld-0.1.4/
--rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.4/LICENSE
--rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 23:52:13.321979 desgld-0.1.4/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.4/README.md
--rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.4/pyproject.toml
--rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-03 23:52:13.322618 desgld-0.1.4/setup.cfg
--rw-r--r--   0 macpc      (501) staff       (20)      708 2024-05-03 23:49:12.000000 desgld-0.1.4/setup.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.317940 desgld-0.1.4/src/
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.319769 desgld-0.1.4/src/desgld/
--rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.4/src/desgld/__init__.py
--rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-04-29 21:40:38.000000 desgld-0.1.4/src/desgld/desgld_alg.py
--rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-04-29 20:32:35.000000 desgld-0.1.4/src/desgld/evaluation.py
--rw-r--r--   0 macpc      (501) staff       (20)     8171 2024-05-03 23:50:01.000000 desgld-0.1.4/src/desgld/network.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.321160 desgld-0.1.4/src/desgld.egg-info/
--rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/SOURCES.txt
--rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/dependency_links.txt
--rw-r--r--   0 macpc      (501) staff       (20)       78 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/requires.txt
--rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/top_level.txt
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 18:00:47.077117 desgld-0.1.5/
+-rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.5/LICENSE
+-rw-r--r--   0 macpc      (501) staff       (20)      836 2024-05-29 18:00:47.076722 desgld-0.1.5/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.5/README.md
+-rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.5/pyproject.toml
+-rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-29 18:00:47.077194 desgld-0.1.5/setup.cfg
+-rw-r--r--   0 macpc      (501) staff       (20)      792 2024-05-29 16:52:36.000000 desgld-0.1.5/setup.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 18:00:47.071368 desgld-0.1.5/src/
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 18:00:47.073911 desgld-0.1.5/src/desgld/
+-rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.5/src/desgld/__init__.py
+-rw-r--r--   0 macpc      (501) staff       (20)    11643 2024-05-29 17:43:24.000000 desgld-0.1.5/src/desgld/desgld_alg.py
+-rw-r--r--   0 macpc      (501) staff       (20)     5547 2024-05-29 17:43:24.000000 desgld-0.1.5/src/desgld/evaluation.py
+-rw-r--r--   0 macpc      (501) staff       (20)     8263 2024-05-29 17:44:46.000000 desgld-0.1.5/src/desgld/network.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 18:00:47.075845 desgld-0.1.5/src/desgld.egg-info/
+-rw-r--r--   0 macpc      (501) staff       (20)      836 2024-05-29 18:00:47.000000 desgld-0.1.5/src/desgld.egg-info/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-29 18:00:47.000000 desgld-0.1.5/src/desgld.egg-info/SOURCES.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-29 18:00:47.000000 desgld-0.1.5/src/desgld.egg-info/dependency_links.txt
+-rw-r--r--   0 macpc      (501) staff       (20)       98 2024-05-29 18:00:47.000000 desgld-0.1.5/src/desgld.egg-info/requires.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-29 18:00:47.000000 desgld-0.1.5/src/desgld.egg-info/top_level.txt
```

### Comparing `desgld-0.1.4/LICENSE` & `desgld-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `desgld-0.1.4/PKG-INFO` & `desgld-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: desgld
-Version: 0.1.4
-Summary: Package for decentralized stochastic gradient descent
+Version: 0.1.5
+Summary: Decentralized stochastic gradient Langevin diffusion
 Home-page: https://github.com/mrislambd/desgld_package.git
 Author: Rafiq Islam
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: gpu
+Requires-Dist: cupy-cuda112; extra == "gpu"
 
 # Decentralized Stochastic Gradient Langevin Diffusion
 
 
 This repo is to build the package for decentralized stochastic gradient Langevin diffusion. For more details please
 visit this https://mrislambd.github.io/desgld_package/
```

### Comparing `desgld-0.1.4/setup.py` & `desgld-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,30 @@
     "numpy",
     "scipy",
     "scikit-learn",
     "matplotlib",
     "tqdm",
 ]
 
+requirements_gpu = ["cupy-cuda112"]
+
 requirements_dev = ["black", "isort", "flake8", "pre-commit"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="desgld",
-    version="0.1.4",
-    description="Package for decentralized stochastic gradient descent",
+    version="0.1.5",
+    description="Decentralized stochastic gradient Langevin diffusion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrislambd/desgld_package.git",
     author="Rafiq Islam",
     packages=["desgld"],
     package_dir={"": "src"},
     install_requires=requirements,
-    extras_require={"dev": requirements_dev},
+    extras_require={
+        "dev": requirements_dev,
+        "gpu": requirements_gpu,
+    },
 )
```

### Comparing `desgld-0.1.4/src/desgld/desgld_alg.py` & `desgld-0.1.5/src/desgld/desgld_alg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import math
 
-import numpy as np
+try:
+    import cupy as np
+
+    use_gpu = True
+except ImportError:
+    import numpy as np
+
+    use_gpu = False
 
 
 class DeSGLD:
     """Decentralized Stochastic Gradient Langevin Dynamics
 
     Args:
         size_w (int): the size of the network
@@ -53,15 +60,15 @@
             dim: the dimension of the input data
             lam: the regularization parameter
             b: the batch size
         Returns:
             gradient for the the logistic regression
         """
         f = np.zeros(dim)
-        randomList = np.random.randint(0, len(y) - 1, size=int(b))
+        randomList = np.random.randint(0, len(y), size=int(b))
         for item in randomList:
             h = 1 / (1 + np.exp(-np.dot(beta, x[item])))
             f -= np.dot((y[item] - h), x[item])
         f += (2 / lam) * beta
         return f
 
     def gradient_linreg(self, beta, x, y, dim, lam, b):
@@ -71,18 +78,18 @@
             beta: approximation at each node
             x: the input data
             y: the output data
             dim: the dimension of the input data
             lam: the regularization parameter
             b: the batch size
         Returns:
-            gradient for the the logistic regression
+            gradient for the the linear regression
         """
         f = np.zeros(dim)
-        randomList = np.random.randint(0, len(y) - 1, size=int(b))
+        randomList = np.random.randint(0, len(y), size=int(b))
         for i in randomList:
             f = f - np.dot((y[i] - np.dot(beta, x[i])), x[i])
         f += (2 / lam) * beta
         return f
 
     def vanila_desgld(self):
         """Vanila DeSGLD algorithm
@@ -127,15 +134,15 @@
                             self.y[i],
                             self.dim,
                             self.lam,
                             self.b,
                         )
                         temp = np.zeros(self.dim)
                         for j in range(len(beta[n])):
-                            temp = temp + self.w[i, j] * beta[n, j]
+                            temp += self.w[i, j] * beta[n, j]
                         noise = np.random.normal(0, self.sigma, self.dim)
                         beta[n, i] = (
                             temp - step * g + math.sqrt(2 * step) * noise
                         )
                     else:
                         g = self.gradient_linreg(
                             beta[n, i],
@@ -143,15 +150,15 @@
                             self.y[i],
                             self.dim,
                             self.lam,
                             self.b,
                         )
                         temp = np.zeros(self.dim)
                         for j in range(len(beta[n])):
-                            temp = temp + self.w[i, j] * beta[n, j]
+                            temp += self.w[i, j] * beta[n, j]
                         noise = np.random.multivariate_normal(
                             mean=np.zeros(self.dim), cov=np.eye(self.dim)
                         )
                         beta[n, i] = (
                             temp - step * g + math.sqrt(2 * step) * noise
                         )
 
@@ -219,15 +226,15 @@
                                 self.y[i],
                                 self.dim,
                                 self.lam,
                                 self.b,
                             )
                             temp = np.zeros(self.dim)
                             for j in range(len(beta[n])):
-                                temp = temp + w1[i, j] * beta[n, j]
+                                temp += w1[i, j] * beta[n, j]
                             noise = np.random.normal(0, self.sigma, self.dim)
                             beta[n, i] = (
                                 temp - step * g + math.sqrt(2 * step) * noise
                             )
                             # Extra Part
                             g = self.gradient_logreg(
                                 beta[n, i],
@@ -235,15 +242,15 @@
                                 self.y[i],
                                 self.dim,
                                 self.lam,
                                 self.b,
                             )
                             temp = np.zeros(self.dim)
                             for j in range(len(beta[n])):
-                                temp = temp + self.w[i, j] * beta[n, j]
+                                temp += self.w[i, j] * beta[n, j]
                             noise = np.random.normal(0, self.sigma, self.dim)
                             beta[n, i] = (
                                 temp - step * g + math.sqrt(2 * step) * noise
                             )
                         else:
                             # Vanila Part
                             g = self.gradient_linreg(
@@ -252,15 +259,15 @@
                                 self.y[i],
                                 self.dim,
                                 self.lam,
                                 self.b,
                             )
                             temp = np.zeros(self.dim)
                             for j in range(len(beta[n])):
-                                temp = temp + w1[i, j] * beta[n, j]
+                                temp += w1[i, j] * beta[n, j]
                             noise = np.random.multivariate_normal(
                                 mean=np.zeros(self.dim), cov=np.eye(self.dim)
                             )
                             beta[n, i] = (
                                 temp - step * g + math.sqrt(2 * step) * noise
                             )
                             # Extra Part
@@ -270,15 +277,15 @@
                                 self.y[i],
                                 self.dim,
                                 self.lam,
                                 self.b,
                             )
                             temp = np.zeros(self.dim)
                             for j in range(len(beta[n])):
-                                temp = temp + self.w[i, j] * beta[n, j]
+                                temp += self.w[i, j] * beta[n, j]
                             noise = np.random.multivariate_normal(
                                 mean=np.zeros(self.dim), cov=np.eye(self.dim)
                             )
                             beta[n, i] = (
                                 temp - step * g + math.sqrt(2 * step) * noise
                             )
```

### Comparing `desgld-0.1.4/src/desgld/evaluation.py` & `desgld-0.1.5/src/desgld/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 import math
 
-import numpy as np
+try:
+    import cupy as np
+
+    use_gpu = True
+except ImportError:
+    import numpy as np
+
+    use_gpu = False
+
 from scipy.linalg import sqrtm
 
 
 class ClassificationAccuracy:
     """Calculate the classification accuracy in Bayesian Logistic Regression
 
     Args:
```

### Comparing `desgld-0.1.4/src/desgld/network.py` & `desgld-0.1.5/src/desgld/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import random
 
-import numpy as np
+try:
+    import cupy as np
+
+    use_gpu = True
+except ImportError:
+    import numpy as np
+
+    use_gpu = False
 
 
 class NetworkArchitecture:
     """Decentralized network architecture
 
     Description:
         This class is used to generate different network
```

### Comparing `desgld-0.1.4/src/desgld.egg-info/PKG-INFO` & `desgld-0.1.5/src/desgld.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: desgld
-Version: 0.1.4
-Summary: Package for decentralized stochastic gradient descent
+Version: 0.1.5
+Summary: Decentralized stochastic gradient Langevin diffusion
 Home-page: https://github.com/mrislambd/desgld_package.git
 Author: Rafiq Islam
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: gpu
+Requires-Dist: cupy-cuda112; extra == "gpu"
 
 # Decentralized Stochastic Gradient Langevin Diffusion
 
 
 This repo is to build the package for decentralized stochastic gradient Langevin diffusion. For more details please
 visit this https://mrislambd.github.io/desgld_package/
```

