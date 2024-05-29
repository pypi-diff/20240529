# Comparing `tmp/lorepy-0.3.0.tar.gz` & `tmp/lorepy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorepy-0.3.0.tar", last modified: Fri May 17 14:18:01 2024, max compression
+gzip compressed data, was "lorepy-0.4.0.tar", last modified: Wed May 29 11:01:38 2024, max compression
```

## Comparing `lorepy-0.3.0.tar` & `lorepy-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.746631 lorepy-0.3.0/
--rw-rw-rw-   0        0        0    21284 2024-02-07 13:25:48.000000 lorepy-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     8080 2024-05-17 14:18:01.744631 lorepy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7355 2024-05-17 13:56:54.000000 lorepy-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 14:18:01.746631 lorepy-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1057 2024-05-17 13:56:54.000000 lorepy-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.661728 lorepy-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.693632 lorepy-0.3.0/src/lorepy/
--rw-rw-rw-   0        0        0       30 2024-05-13 08:51:41.000000 lorepy-0.3.0/src/lorepy/__init__.py
--rw-rw-rw-   0        0        0     3453 2024-05-17 13:56:54.000000 lorepy-0.3.0/src/lorepy/lorepy.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.743631 lorepy-0.3.0/src/lorepy.egg-info/
--rw-rw-rw-   0        0        0     8080 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 14:18:01.000000 lorepy-0.3.0/src/lorepy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 14:18:01.741630 lorepy-0.3.0/tests/
--rw-rw-rw-   0        0        0     3032 2024-05-17 14:04:53.000000 lorepy-0.3.0/tests/test_plot.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:01:38.562698 lorepy-0.4.0/
+-rw-rw-rw-   0        0        0    21284 2024-05-29 06:47:25.000000 lorepy-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     8965 2024-05-29 11:01:38.562698 lorepy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8240 2024-05-29 10:58:38.000000 lorepy-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:01:38.562698 lorepy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2024-05-29 10:58:38.000000 lorepy-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:01:38.532696 lorepy-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 11:01:38.542695 lorepy-0.4.0/src/lorepy/
+-rw-rw-rw-   0        0        0       73 2024-05-29 10:58:38.000000 lorepy-0.4.0/src/lorepy/__init__.py
+-rw-rw-rw-   0        0        0     3623 2024-05-29 10:58:38.000000 lorepy-0.4.0/src/lorepy/lorepy.py
+-rw-rw-rw-   0        0        0     4691 2024-05-29 10:58:38.000000 lorepy-0.4.0/src/lorepy/uncertainty.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:01:38.561699 lorepy-0.4.0/src/lorepy.egg-info/
+-rw-rw-rw-   0        0        0     8965 2024-05-29 11:01:38.000000 lorepy-0.4.0/src/lorepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-29 11:01:38.000000 lorepy-0.4.0/src/lorepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:01:38.000000 lorepy-0.4.0/src/lorepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-29 11:01:38.000000 lorepy-0.4.0/src/lorepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 11:01:38.000000 lorepy-0.4.0/src/lorepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 11:01:38.560699 lorepy-0.4.0/tests/
+-rw-rw-rw-   0        0        0     3030 2024-05-29 10:58:38.000000 lorepy-0.4.0/tests/test_plot.py
+-rw-rw-rw-   0        0        0     1383 2024-05-29 10:58:38.000000 lorepy-0.4.0/tests/test_uncertainty.py
```

### Comparing `lorepy-0.3.0/LICENSE` & `lorepy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lorepy-0.3.0/PKG-INFO` & `lorepy-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lorepy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Draw Logistic Regression Plots in Python
 Home-page: https://github.com/raeslab/lorepy/
 Author: Sebastian Proost
 Author-email: sebastian.proost@gmail.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: Bug Tracker, https://github.com/raeslab/lorepy/issues
 Classifier: Programming Language :: Python :: 3
@@ -168,14 +168,38 @@
 )
 plt.savefig("./docs/img/loreplot_confounder.png", dpi=150)
 plt.show()
 ```
 
 ![Loreplot with a confounder](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_confounder.png)
 
+### Assess uncertainty
+
+From loreplots it isn't possible to assess how certain we are of the prevalence of each group across the range. To
+provide a view into this there is a function ```uncertainty_plot```, which can be used as shown below. This will use
+```resampling``` (or ```jackknifing```) to determine the 50% and 95% interval of predicted values and show these in a
+multi-panel plot with one plot per category.
+
+```python
+from lorepy import uncertainty_plot
+
+uncertainty_plot(
+    data=iris_df,
+    x="sepal width (cm)",
+    y="species",
+)
+plt.savefig("./docs/img/uncertainty_default.png", dpi=150)
+plt.show()
+```
+
+![Default uncertainty plot](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/uncertainty_default.png)
+
+This also supports custom colors, ranges and classifiers. More examples are available in ```example_uncertainty.py```.
+
+
 ## Development
 
 Additional [documentation for developers](./docs/dev_docs.md) is included with details on running tests, building and deploying to PyPi.
 
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
```

### Comparing `lorepy-0.3.0/README.md` & `lorepy-0.4.0/src/lorepy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: lorepy
+Version: 0.4.0
+Summary: Draw Logistic Regression Plots in Python
+Home-page: https://github.com/raeslab/lorepy/
+Author: Sebastian Proost
+Author-email: sebastian.proost@gmail.com
+License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
+Project-URL: Bug Tracker, https://github.com/raeslab/lorepy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib>=3.4.1
+Requires-Dist: numpy>=1.20.2
+Requires-Dist: pandas>=1.2.4
+Requires-Dist: scikit-learn>=0.24.1
+
 [![Run Pytest](https://github.com/raeslab/lorepy/actions/workflows/autopytest.yml/badge.svg)](https://github.com/raeslab/lorepy/actions/workflows/autopytest.yml) [![Coverage](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/coverage-badge.svg)](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/coverage-badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/686018963.svg)](https://zenodo.org/badge/latestdoi/686018963) [![PyPI version](https://badge.fury.io/py/lorepy.svg)](https://badge.fury.io/py/lorepy) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
 
 # lorepy: Logistic Regression Plots for Python
 
 Logistic Regression plots are used to plot the distribution of a categorical dependent variable in function of a 
 continuous independent variable.
 
@@ -149,14 +168,38 @@
 )
 plt.savefig("./docs/img/loreplot_confounder.png", dpi=150)
 plt.show()
 ```
 
 ![Loreplot with a confounder](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_confounder.png)
 
+### Assess uncertainty
+
+From loreplots it isn't possible to assess how certain we are of the prevalence of each group across the range. To
+provide a view into this there is a function ```uncertainty_plot```, which can be used as shown below. This will use
+```resampling``` (or ```jackknifing```) to determine the 50% and 95% interval of predicted values and show these in a
+multi-panel plot with one plot per category.
+
+```python
+from lorepy import uncertainty_plot
+
+uncertainty_plot(
+    data=iris_df,
+    x="sepal width (cm)",
+    y="species",
+)
+plt.savefig("./docs/img/uncertainty_default.png", dpi=150)
+plt.show()
+```
+
+![Default uncertainty plot](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/uncertainty_default.png)
+
+This also supports custom colors, ranges and classifiers. More examples are available in ```example_uncertainty.py```.
+
+
 ## Development
 
 Additional [documentation for developers](./docs/dev_docs.md) is included with details on running tests, building and deploying to PyPi.
 
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
```

### Comparing `lorepy-0.3.0/setup.py` & `lorepy-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="lorepy",
-    version="0.3.0",
+    version="0.4.0",
     author="Sebastian Proost",
     author_email="sebastian.proost@gmail.com",
     description="Draw Logistic Regression Plots in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raeslab/lorepy/",
     project_urls={
```

### Comparing `lorepy-0.3.0/src/lorepy/lorepy.py` & `lorepy-0.4.0/src/lorepy/lorepy.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,90 +2,98 @@
 from sklearn.linear_model import LogisticRegression
 from pandas import DataFrame
 import numpy as np
 import matplotlib.pyplot as plt
 from typing import Optional, Tuple
 
 
-def _get_area_df(lg, x_feature, x_range, deconfound=[]) -> DataFrame:
+def _prepare_data(data, x, y, confounders):
+    x_features = [x] + [i[0] for i in confounders]
+
+    tmp_df = data[x_features + [y]].dropna()
+    X_reg = np.array(tmp_df[x_features])
+    y_reg = np.array(tmp_df[y])
+
+    x_range = (X_reg[:, 0].min(), X_reg[:, 0].max())
+
+    return X_reg, y_reg, x_range
+
+
+def _get_area_df(lg, x_feature, x_range, confounders=[]) -> DataFrame:
     values = np.linspace(x_range[0], x_range[1], num=200)
 
     predict_df = pd.DataFrame({"values": values})
 
-    for k, v in deconfound:
+    for k, v in confounders:
         predict_df[k] = v
 
     proba = lg.predict_proba(predict_df.values)
     proba_df = DataFrame(proba, columns=lg.classes_)
     proba_df[x_feature] = values
     proba_df.set_index(x_feature, inplace=True)
 
     return proba_df
 
 
 def _get_dots_df(X, y, lg, y_feature, confounders=[]) -> DataFrame:
     output = []
 
-    for v, s in zip(X, y):
-        proba = lg.predict_proba([v] + [i[1] for i in confounders])
+    for x, s in zip(X, y):
+        proba = lg.predict_proba([x] + [i[1] for i in confounders])
         i = list(lg.classes_).index(s)
         min_value = sum(proba[0][:i])
         max_value = sum(proba[0][: i + 1])
         margin = (max_value - min_value) / 10
         ypos = np.random.uniform(low=min_value + margin, high=max_value - margin)
-        output.append({y_feature: s, "x": v[0], "y": ypos})
+        output.append({y_feature: s, "x": x[0], "y": ypos})
 
     return DataFrame(output)
 
 
 def loreplot(
     data: DataFrame,
     x: str,
     y: str,
     add_dots: bool = True,
     x_range: Optional[Tuple[float, float]] = None,
     scatter_kws: dict = dict({}),
     ax=None,
     clf=None,
     confounders=[],
-    **kwargs
+    **kwargs,
 ):
     """
-    Code to create a loreplot with a numerical feature on the x-axis and categorical y from a pandas dataset
+    Code to create a loreplot with a numerical feature on the v-axis and categorical y from a pandas dataset
 
     :param data: Pandas dataframe with data
     :param x: Needs to be a numerical feature
     :param y: Categorical feature
     :param add_dots: Shows where true samples are in the plot (cannot be enabled when deconfounding for additional variables)
-    :param x_range: Either None (range will be selected automatically) or a tuple with min and max value for the x-axis
+    :param x_range: Either None (range will be selected automatically) or a tuple with min and max value for the v-axis
     :param scatter_kws: Dictionary with keyword arguments to pass to the scatter function
     :param ax: subplot to draw on, in case lorepy is used in a subplot
     :param clf: provide a different scikit-learn classifier for the function. Should implement the predict_proba() and fit()
     :param confounders: list of tuples with the feature and reference value e.g. [("BMI", 25)] will confounders BMI and use a reference of 25 for plots
     :param kwargs: Additional arguments to pass to pandas' plot.area function
     """
     if ax is None:
         ax = plt.gca()
 
-    x_features = [x] + [i[0] for i in confounders]
-
-    tmp_df = data[x_features + [y]].dropna()
-    X_reg = np.array(tmp_df[x_features])
-    y_reg = np.array(tmp_df[y])
+    X_reg, y_reg, r = _prepare_data(data, x, y, confounders)
 
     if x_range is None:
-        x_range = (X_reg[:, 0].min(), X_reg[:, 0].max())
+        x_range = r
 
     lg = LogisticRegression(multi_class="multinomial") if clf is None else clf
     lg.fit(X_reg, y_reg)
 
     if "linestyle" not in kwargs.keys():
         kwargs["linestyle"] = "None"
 
-    area_df = _get_area_df(lg, x, x_range, deconfound=confounders)
+    area_df = _get_area_df(lg, x, x_range, confounders=confounders)
     area_df.plot.area(ax=ax, **kwargs)
 
     if add_dots and len(confounders) == 0:
         dot_df = _get_dots_df(X_reg, y_reg, lg, y)
         if "color" not in scatter_kws.keys():
             scatter_kws["color"] = "w"
         if "alpha" not in scatter_kws.keys():
```

### Comparing `lorepy-0.3.0/src/lorepy.egg-info/PKG-INFO` & `lorepy-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: lorepy
-Version: 0.3.0
-Summary: Draw Logistic Regression Plots in Python
-Home-page: https://github.com/raeslab/lorepy/
-Author: Sebastian Proost
-Author-email: sebastian.proost@gmail.com
-License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
-Project-URL: Bug Tracker, https://github.com/raeslab/lorepy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib>=3.4.1
-Requires-Dist: numpy>=1.20.2
-Requires-Dist: pandas>=1.2.4
-Requires-Dist: scikit-learn>=0.24.1
-
 [![Run Pytest](https://github.com/raeslab/lorepy/actions/workflows/autopytest.yml/badge.svg)](https://github.com/raeslab/lorepy/actions/workflows/autopytest.yml) [![Coverage](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/coverage-badge.svg)](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/coverage-badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/686018963.svg)](https://zenodo.org/badge/latestdoi/686018963) [![PyPI version](https://badge.fury.io/py/lorepy.svg)](https://badge.fury.io/py/lorepy) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
 
 # lorepy: Logistic Regression Plots for Python
 
 Logistic Regression plots are used to plot the distribution of a categorical dependent variable in function of a 
 continuous independent variable.
 
@@ -168,14 +149,38 @@
 )
 plt.savefig("./docs/img/loreplot_confounder.png", dpi=150)
 plt.show()
 ```
 
 ![Loreplot with a confounder](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/loreplot_confounder.png)
 
+### Assess uncertainty
+
+From loreplots it isn't possible to assess how certain we are of the prevalence of each group across the range. To
+provide a view into this there is a function ```uncertainty_plot```, which can be used as shown below. This will use
+```resampling``` (or ```jackknifing```) to determine the 50% and 95% interval of predicted values and show these in a
+multi-panel plot with one plot per category.
+
+```python
+from lorepy import uncertainty_plot
+
+uncertainty_plot(
+    data=iris_df,
+    x="sepal width (cm)",
+    y="species",
+)
+plt.savefig("./docs/img/uncertainty_default.png", dpi=150)
+plt.show()
+```
+
+![Default uncertainty plot](https://raw.githubusercontent.com/raeslab/lorepy/main/docs/img/uncertainty_default.png)
+
+This also supports custom colors, ranges and classifiers. More examples are available in ```example_uncertainty.py```.
+
+
 ## Development
 
 Additional [documentation for developers](./docs/dev_docs.md) is included with details on running tests, building and deploying to PyPi.
 
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
```

### Comparing `lorepy-0.3.0/tests/test_plot.py` & `lorepy-0.4.0/tests/test_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 z = X
 
 df = pd.DataFrame({"x": X, "y": y, "z": z})
 
 
 # Test case for loreplot with default parameters
 def test_loreplot_default():
-    loreplot(df, "x", "y")  ## first test without specifying the axis
+    loreplot(df, "x", "y")  # first test without specifying the axis
 
     fig, ax = plt.subplots()
     loreplot(df, "x", "y", ax=ax)
     assert ax.get_title() == ""
     assert ax.get_xlabel() == "x"
     assert ax.get_ylabel() == ""
 
 
 # Test case for loreplot with confounder
 def test_loreplot_default():
     loreplot(
         df, "x", "y", confounders=[("z", 1)]
-    )  ## first test without specifying the axis
+    )  # first test without specifying the axis
 
     fig, ax = plt.subplots()
     loreplot(df, "x", "y", ax=ax)
     assert ax.get_title() == ""
     assert ax.get_xlabel() == "x"
     assert ax.get_ylabel() == ""
```

