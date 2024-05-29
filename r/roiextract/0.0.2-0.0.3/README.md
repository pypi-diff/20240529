# Comparing `tmp/roiextract-0.0.2.tar.gz` & `tmp/roiextract-0.0.3.tar.gz`

## Comparing `roiextract-0.0.2.tar` & `roiextract-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 roiextract-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 roiextract-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 roiextract-0.0.2/Makefile
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 roiextract-0.0.2/make.bat
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 roiextract-0.0.2/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 roiextract-0.0.2/requirements_docs.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 roiextract-0.0.2/requirements_testing.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 roiextract-0.0.2/setup.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 roiextract-0.0.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 roiextract-0.0.2/docs/api.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 roiextract-0.0.2/docs/conf.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 roiextract-0.0.2/docs/index.rst
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 roiextract-0.0.2/docs/usage.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/__init__.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/analytic.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/filter.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/numerical.py
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/optimize.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/quantify.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 roiextract-0.0.2/src/roiextract/utils.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 roiextract-0.0.2/tests/test_filter.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 roiextract-0.0.2/tests/test_numerical.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 roiextract-0.0.2/tests/test_optimize.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 roiextract-0.0.2/tests/test_quantify.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 roiextract-0.0.2/tests/test_utils.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 roiextract-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 roiextract-0.0.2/LICENSE
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 roiextract-0.0.2/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 roiextract-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 roiextract-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 roiextract-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 roiextract-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 roiextract-0.0.3/Makefile
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 roiextract-0.0.3/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 roiextract-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 roiextract-0.0.3/requirements_docs.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 roiextract-0.0.3/requirements_testing.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 roiextract-0.0.3/setup.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 roiextract-0.0.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 roiextract-0.0.3/docs/api.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 roiextract-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 roiextract-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 roiextract-0.0.3/docs/usage.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/analytic.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/filter.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/numerical.py
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/optimize.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/quantify.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 roiextract-0.0.3/src/roiextract/utils.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 roiextract-0.0.3/tests/test_filter.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 roiextract-0.0.3/tests/test_numerical.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 roiextract-0.0.3/tests/test_optimize.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 roiextract-0.0.3/tests/test_quantify.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 roiextract-0.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 roiextract-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 roiextract-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 roiextract-0.0.3/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 roiextract-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 roiextract-0.0.3/PKG-INFO
```

### Comparing `roiextract-0.0.2/Makefile` & `roiextract-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/make.bat` & `roiextract-0.0.3/make.bat`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/.github/workflows/documentation.yml` & `roiextract-0.0.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/docs/conf.py` & `roiextract-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/docs/index.rst` & `roiextract-0.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/src/roiextract/analytic.py` & `roiextract-0.0.3/src/roiextract/analytic.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/src/roiextract/filter.py` & `roiextract-0.0.3/src/roiextract/filter.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/src/roiextract/numerical.py` & `roiextract-0.0.3/src/roiextract/numerical.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/src/roiextract/optimize.py` & `roiextract-0.0.3/src/roiextract/optimize.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/src/roiextract/quantify.py` & `roiextract-0.0.3/src/roiextract/quantify.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/src/roiextract/utils.py` & `roiextract-0.0.3/src/roiextract/utils.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/tests/test_filter.py` & `roiextract-0.0.3/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/tests/test_numerical.py` & `roiextract-0.0.3/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/tests/test_optimize.py` & `roiextract-0.0.3/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/tests/test_quantify.py` & `roiextract-0.0.3/tests/test_quantify.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/tests/test_utils.py` & `roiextract-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/LICENSE` & `roiextract-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roiextract-0.0.2/pyproject.toml` & `roiextract-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "roiextract"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Nikolai Kapralov", email="kapralov@cbs.mpg.de" }
 ]
-description = "Data-independent and data-driven optimization of extraction of ROI time series based on M/EEG"
+description = "Data-independent and data-driven optimization of spatial filters for extraction of ROI time series based on M/EEG"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

