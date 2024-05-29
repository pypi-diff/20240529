# Comparing `tmp/poni2006-1.1.0.tar.gz` & `tmp/poni2006-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poni2006-1.1.0.tar", last modified: Fri Mar  4 14:58:23 2022, max compression
+gzip compressed data, was "poni2006-1.2.0.tar", last modified: Wed May 29 12:51:22 2024, max compression
```

## Comparing `poni2006-1.1.0.tar` & `poni2006-1.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:23.062769 poni2006-1.1.0/
--rw-rw-rw-   0        0        0      316 2022-03-04 14:54:20.000000 poni2006-1.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3302 2022-03-04 14:54:20.000000 poni2006-1.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-03-04 14:54:20.000000 poni2006-1.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-03-04 14:54:20.000000 poni2006-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      436 2022-03-04 14:54:20.000000 poni2006-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2264 2022-03-04 14:58:23.062769 poni2006-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1454 2022-03-04 14:54:20.000000 poni2006-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:22.978789 poni2006-1.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:22.982771 poni2006-1.1.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:22.982771 poni2006-1.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5080 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      591 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      163 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1375 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:22.986765 poni2006-1.1.0/doc/user/
--rw-rw-rw-   0        0        0       83 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-03-04 14:54:20.000000 poni2006-1.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      352 2022-03-04 14:54:20.000000 poni2006-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-03-04 14:54:20.000000 poni2006-1.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-03-04 14:58:23.066772 poni2006-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1857 2022-03-04 14:54:20.000000 poni2006-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:22.918771 poni2006-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:22.998766 poni2006-1.1.0/src/poni2006/
--rw-rw-rw-   0        0        0      259 2022-03-04 14:54:20.000000 poni2006-1.1.0/src/poni2006/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:23.050767 poni2006-1.1.0/src/poni2006/clean/
--rw-rw-rw-   0        0        0     3215 2022-02-23 15:19:48.000000 poni2006-1.1.0/src/poni2006/clean/fig10.csv
--rw-rw-rw-   0        0        0     3159 2022-02-23 08:53:34.000000 poni2006-1.1.0/src/poni2006/clean/fig2.csv
--rw-rw-rw-   0        0        0      273 2022-03-04 10:29:59.000000 poni2006-1.1.0/src/poni2006/clean/fig3.csv
--rw-rw-rw-   0        0        0      318 2022-03-04 10:35:58.000000 poni2006-1.1.0/src/poni2006/clean/fig4.csv
--rw-rw-rw-   0        0        0      345 2022-02-23 15:05:43.000000 poni2006-1.1.0/src/poni2006/clean/fig5.csv
--rw-rw-rw-   0        0        0     1022 2022-03-04 11:21:21.000000 poni2006-1.1.0/src/poni2006/clean/fig7.csv
--rw-rw-rw-   0        0        0      592 2022-03-04 11:21:21.000000 poni2006-1.1.0/src/poni2006/clean/fig7_legend.csv
--rw-rw-rw-   0        0        0     4823 2022-02-24 07:24:38.000000 poni2006-1.1.0/src/poni2006/clean/fig8.csv
--rw-rw-rw-   0        0        0     6819 2022-03-04 11:30:49.000000 poni2006-1.1.0/src/poni2006/clean/fig9.csv
--rw-rw-rw-   0        0        0      599 2022-03-04 14:43:09.000000 poni2006-1.1.0/src/poni2006/clean/info.json
--rw-rw-rw-   0        0        0      134 2022-03-04 14:54:20.000000 poni2006-1.1.0/src/poni2006/clean/readme.rst
--rw-rw-rw-   0        0        0   476835 2022-03-04 14:34:19.000000 poni2006-1.1.0/src/poni2006/clean/weather_hourly.csv
--rw-rw-rw-   0        0        0      152 2022-03-04 14:54:20.000000 poni2006-1.1.0/src/poni2006/info.py
--rw-rw-rw-   0        0        0      367 2022-03-04 14:54:20.000000 poni2006-1.1.0/src/poni2006/version.py
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:23.022769 poni2006-1.1.0/src/poni2006.egg-info/
--rw-rw-rw-   0        0        0     2264 2022-03-04 14:58:22.000000 poni2006-1.1.0/src/poni2006.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1038 2022-03-04 14:58:22.000000 poni2006-1.1.0/src/poni2006.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-04 14:58:22.000000 poni2006-1.1.0/src/poni2006.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-22 10:22:54.000000 poni2006-1.1.0/src/poni2006.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-03-04 14:58:22.000000 poni2006-1.1.0/src/poni2006.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-04 14:58:23.062769 poni2006-1.1.0/test/
--rw-rw-rw-   0        0        0      972 2022-03-04 14:54:20.000000 poni2006-1.1.0/test/conftest.py
--rw-rw-rw-   0        0        0       82 2022-03-04 14:54:20.000000 poni2006-1.1.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.360285 poni2006-1.2.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 12:46:48.000000 poni2006-1.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3303 2024-05-29 12:46:48.000000 poni2006-1.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 12:46:48.000000 poni2006-1.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 12:46:48.000000 poni2006-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2930 2024-05-29 12:51:22.360285 poni2006-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2024-05-29 12:46:48.000000 poni2006-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.321240 poni2006-1.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 12:46:48.000000 poni2006-1.2.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.330617 poni2006-1.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.330617 poni2006-1.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5080 2024-05-29 12:46:48.000000 poni2006-1.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      591 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      218 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 12:46:48.000000 poni2006-1.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1043 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.330617 poni2006-1.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 12:46:49.000000 poni2006-1.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2306 2024-05-29 12:46:49.000000 poni2006-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      352 2024-05-29 12:46:48.000000 poni2006-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 12:46:48.000000 poni2006-1.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:51:22.360285 poni2006-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.299044 poni2006-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.330617 poni2006-1.2.0/src/poni2006/
+-rw-rw-rw-   0        0        0      251 2024-05-29 12:46:48.000000 poni2006-1.2.0/src/poni2006/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.350630 poni2006-1.2.0/src/poni2006/clean/
+-rw-rw-rw-   0        0        0     3215 2024-05-29 12:45:49.000000 poni2006-1.2.0/src/poni2006/clean/fig10.csv
+-rw-rw-rw-   0        0        0     3159 2024-05-29 12:45:25.000000 poni2006-1.2.0/src/poni2006/clean/fig2.csv
+-rw-rw-rw-   0        0        0      273 2024-05-29 12:45:28.000000 poni2006-1.2.0/src/poni2006/clean/fig3.csv
+-rw-rw-rw-   0        0        0      318 2024-05-29 12:45:31.000000 poni2006-1.2.0/src/poni2006/clean/fig4.csv
+-rw-rw-rw-   0        0        0      345 2024-05-29 12:45:34.000000 poni2006-1.2.0/src/poni2006/clean/fig5.csv
+-rw-rw-rw-   0        0        0     1022 2024-05-29 12:45:38.000000 poni2006-1.2.0/src/poni2006/clean/fig7.csv
+-rw-rw-rw-   0        0        0      592 2024-05-29 12:45:38.000000 poni2006-1.2.0/src/poni2006/clean/fig7_legend.csv
+-rw-rw-rw-   0        0        0     4823 2024-05-29 12:45:42.000000 poni2006-1.2.0/src/poni2006/clean/fig8.csv
+-rw-rw-rw-   0        0        0     6819 2024-05-29 12:45:46.000000 poni2006-1.2.0/src/poni2006/clean/fig9.csv
+-rw-rw-rw-   0        0        0      599 2024-05-29 12:45:52.000000 poni2006-1.2.0/src/poni2006/clean/info.json
+-rw-rw-rw-   0        0        0      134 2024-05-29 12:46:49.000000 poni2006-1.2.0/src/poni2006/clean/readme.rst
+-rw-rw-rw-   0        0        0   476835 2024-05-29 12:45:56.000000 poni2006-1.2.0/src/poni2006/clean/weather_hourly.csv
+-rw-rw-rw-   0        0        0      379 2024-05-29 12:46:49.000000 poni2006-1.2.0/src/poni2006/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 12:46:48.000000 poni2006-1.2.0/src/poni2006/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.360285 poni2006-1.2.0/src/poni2006.egg-info/
+-rw-rw-rw-   0        0        0     2930 2024-05-29 12:51:22.000000 poni2006-1.2.0/src/poni2006.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1022 2024-05-29 12:51:22.000000 poni2006-1.2.0/src/poni2006.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:51:22.000000 poni2006-1.2.0/src/poni2006.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-29 12:51:22.000000 poni2006-1.2.0/src/poni2006.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 12:51:22.000000 poni2006-1.2.0/src/poni2006.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 12:51:22.360285 poni2006-1.2.0/test/
+-rw-rw-rw-   0        0        0      984 2024-05-29 12:46:49.000000 poni2006-1.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0      373 2024-05-29 12:46:49.000000 poni2006-1.2.0/test/test_packaging.py
```

### Comparing `poni2006-1.1.0/CONTRIBUTING.rst` & `poni2006-1.2.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.9.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `poni2006-1.1.0/LICENSE` & `poni2006-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/doc/Makefile` & `poni2006-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/doc/biblio/biblio.rst` & `poni2006-1.2.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/doc/conf.py` & `poni2006-1.2.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.1.0"
+version = "1.2.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.0"
+release = "1.2.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `poni2006-1.1.0/doc/index.rst` & `poni2006-1.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/doc/make.bat` & `poni2006-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/fig10.csv` & `poni2006-1.2.0/src/poni2006/clean/fig10.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/fig2.csv` & `poni2006-1.2.0/src/poni2006/clean/fig2.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/fig7.csv` & `poni2006-1.2.0/src/poni2006/clean/fig7.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/fig7_legend.csv` & `poni2006-1.2.0/src/poni2006/clean/fig7_legend.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/fig8.csv` & `poni2006-1.2.0/src/poni2006/clean/fig8.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/fig9.csv` & `poni2006-1.2.0/src/poni2006/clean/fig9.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/info.json` & `poni2006-1.2.0/src/poni2006/clean/info.json`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006/clean/weather_hourly.csv` & `poni2006-1.2.0/src/poni2006/clean/weather_hourly.csv`

 * *Files identical despite different names*

### Comparing `poni2006-1.1.0/src/poni2006.egg-info/SOURCES.txt` & `poni2006-1.2.0/src/poni2006.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
-MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 requirements_minimal.txt
-setup.cfg
-setup.py
 doc/Makefile
 doc/authors.rst
 doc/conf.py
 doc/contributing.rst
 doc/history.rst
 doc/index.rst
 doc/installation.rst
@@ -25,15 +23,15 @@
 doc/user/overview.rst
 src/poni2006/__init__.py
 src/poni2006/info.py
 src/poni2006/version.py
 src/poni2006.egg-info/PKG-INFO
 src/poni2006.egg-info/SOURCES.txt
 src/poni2006.egg-info/dependency_links.txt
-src/poni2006.egg-info/not-zip-safe
+src/poni2006.egg-info/requires.txt
 src/poni2006.egg-info/top_level.txt
 src/poni2006/clean/fig10.csv
 src/poni2006/clean/fig2.csv
 src/poni2006/clean/fig3.csv
 src/poni2006/clean/fig4.csv
 src/poni2006/clean/fig5.csv
 src/poni2006/clean/fig7.csv
```

### Comparing `poni2006-1.1.0/test/conftest.py` & `poni2006-1.2.0/test/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=poni2006")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=poni2006")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

