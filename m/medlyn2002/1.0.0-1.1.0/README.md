# Comparing `tmp/medlyn2002-1.0.0.tar.gz` & `tmp/medlyn2002-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medlyn2002-1.0.0.tar", last modified: Mon Jan 31 10:58:21 2022, max compression
+gzip compressed data, was "medlyn2002-1.1.0.tar", last modified: Wed May 29 09:47:15 2024, max compression
```

## Comparing `medlyn2002-1.0.0.tar` & `medlyn2002-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.570642 medlyn2002-1.0.0/
--rw-rw-rw-   0        0        0      316 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3322 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      438 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2306 2022-01-31 10:58:21.570642 medlyn2002-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1490 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.507618 medlyn2002-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.507618 medlyn2002-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.514620 medlyn2002-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5102 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      595 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      165 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1409 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.514620 medlyn2002-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       83 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      360 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-01-31 10:58:21.577652 medlyn2002-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1886 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.451618 medlyn2002-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.528619 medlyn2002-1.0.0/src/medlyn2002/
--rw-rw-rw-   0        0        0      261 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/src/medlyn2002/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.556646 medlyn2002-1.0.0/src/medlyn2002/clean/
--rw-rw-rw-   0        0        0      134 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/src/medlyn2002/clean/readme.rst
--rw-rw-rw-   0        0        0     1091 2022-01-27 15:02:11.000000 medlyn2002-1.0.0/src/medlyn2002/clean/tab2_arrhenius.csv
--rw-rw-rw-   0        0        0     1874 2022-01-27 14:56:26.000000 medlyn2002-1.0.0/src/medlyn2002/clean/tab2_peaked.csv
--rw-rw-rw-   0        0        0     1936 2022-01-27 11:40:13.000000 medlyn2002-1.0.0/src/medlyn2002/clean/tab3.csv
--rw-rw-rw-   0        0        0      656 2022-01-27 08:33:41.000000 medlyn2002-1.0.0/src/medlyn2002/external.py
--rw-rw-rw-   0        0        0      152 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/src/medlyn2002/info.py
--rw-rw-rw-   0        0        0     8577 2022-01-28 17:12:18.000000 medlyn2002-1.0.0/src/medlyn2002/raw.py
--rw-rw-rw-   0        0        0      367 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/src/medlyn2002/version.py
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.549640 medlyn2002-1.0.0/src/medlyn2002.egg-info/
--rw-rw-rw-   0        0        0     2306 2022-01-31 10:58:21.000000 medlyn2002-1.0.0/src/medlyn2002.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2022-01-31 10:58:21.000000 medlyn2002-1.0.0/src/medlyn2002.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-31 10:58:21.000000 medlyn2002-1.0.0/src/medlyn2002.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-27 08:30:35.000000 medlyn2002-1.0.0/src/medlyn2002.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2022-01-31 10:58:21.000000 medlyn2002-1.0.0/src/medlyn2002.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-01-31 10:58:21.570642 medlyn2002-1.0.0/test/
--rw-rw-rw-   0        0        0      974 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       86 2022-01-31 10:45:54.000000 medlyn2002-1.0.0/test/test_packaging.py
--rw-rw-rw-   0        0        0      481 2022-01-27 11:51:55.000000 medlyn2002-1.0.0/test/test_tab2.py
--rw-rw-rw-   0        0        0      474 2022-01-27 11:48:54.000000 medlyn2002-1.0.0/test/test_tab3.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.353586 medlyn2002-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3323 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3012 2024-05-29 09:47:15.352621 medlyn2002-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.320585 medlyn2002-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.321613 medlyn2002-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.322585 medlyn2002-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5102 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1069 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.324584 medlyn2002-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2337 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      360 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:47:15.353586 medlyn2002-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.282659 medlyn2002-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.331584 medlyn2002-1.1.0/src/medlyn2002/
+-rw-rw-rw-   0        0        0      253 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/src/medlyn2002/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.343584 medlyn2002-1.1.0/src/medlyn2002/clean/
+-rw-rw-rw-   0        0        0      134 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/src/medlyn2002/clean/readme.rst
+-rw-rw-rw-   0        0        0     1091 2024-05-29 09:40:09.000000 medlyn2002-1.1.0/src/medlyn2002/clean/tab2_arrhenius.csv
+-rw-rw-rw-   0        0        0     1874 2024-05-29 09:40:13.000000 medlyn2002-1.1.0/src/medlyn2002/clean/tab2_peaked.csv
+-rw-rw-rw-   0        0        0     1936 2024-05-29 09:40:17.000000 medlyn2002-1.1.0/src/medlyn2002/clean/tab3.csv
+-rw-rw-rw-   0        0        0      656 2022-01-27 08:33:41.000000 medlyn2002-1.1.0/src/medlyn2002/external.py
+-rw-rw-rw-   0        0        0      379 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/src/medlyn2002/info.py
+-rw-rw-rw-   0        0        0     8577 2022-01-28 17:12:18.000000 medlyn2002-1.1.0/src/medlyn2002/raw.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 09:41:13.000000 medlyn2002-1.1.0/src/medlyn2002/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.350584 medlyn2002-1.1.0/src/medlyn2002.egg-info/
+-rw-rw-rw-   0        0        0     3012 2024-05-29 09:47:15.000000 medlyn2002-1.1.0/src/medlyn2002.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      905 2024-05-29 09:47:15.000000 medlyn2002-1.1.0/src/medlyn2002.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:47:15.000000 medlyn2002-1.1.0/src/medlyn2002.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-05-29 09:47:15.000000 medlyn2002-1.1.0/src/medlyn2002.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 09:47:15.000000 medlyn2002-1.1.0/src/medlyn2002.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:47:15.348584 medlyn2002-1.1.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      381 2024-05-29 09:41:14.000000 medlyn2002-1.1.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0      481 2022-01-27 11:51:55.000000 medlyn2002-1.1.0/test/test_tab2.py
+-rw-rw-rw-   0        0        0      474 2022-01-27 11:48:54.000000 medlyn2002-1.1.0/test/test_tab3.py
```

### Comparing `medlyn2002-1.0.0/CONTRIBUTING.rst` & `medlyn2002-1.1.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

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

### Comparing `medlyn2002-1.0.0/LICENSE` & `medlyn2002-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/doc/Makefile` & `medlyn2002-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/doc/biblio/biblio.rst` & `medlyn2002-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/doc/conf.py` & `medlyn2002-1.1.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.0.0"
+version = "1.1.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.0"
+release = "1.1.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `medlyn2002-1.0.0/doc/index.rst` & `medlyn2002-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/doc/make.bat` & `medlyn2002-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/doc/readme.rst` & `medlyn2002-1.1.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,36 @@
-Overview
-========
+========================
+medlyn2002
+========================
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/medlyn2002/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/medlyn2002/
+.. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/medlyn2002/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/medlyn2002/1.0.0/
+    :target: https://pypi.org/project/medlyn2002/1.1.0/
 
 .. image:: https://b326.gitlab.io/medlyn2002/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/medlyn2002
 
+.. image:: https://b326.gitlab.io/medlyn2002/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/medlyn2002/
+
 .. image:: https://badge.fury.io/py/medlyn2002.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/medlyn2002
 
+.. #}
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/medlyn2002/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/medlyn2002/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/medlyn2002/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/medlyn2002/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/medlyn2002/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/medlyn2002/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/medlyn2002/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/medlyn2002/commits/prod
-
 .. #}
 
 Data and formalisms from Medlyn et al. (2002)
+
```

### Comparing `medlyn2002-1.0.0/src/medlyn2002/clean/tab2_arrhenius.csv` & `medlyn2002-1.1.0/src/medlyn2002/clean/tab2_arrhenius.csv`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/src/medlyn2002/clean/tab2_peaked.csv` & `medlyn2002-1.1.0/src/medlyn2002/clean/tab2_peaked.csv`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/src/medlyn2002/clean/tab3.csv` & `medlyn2002-1.1.0/src/medlyn2002/clean/tab3.csv`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/src/medlyn2002/external.py` & `medlyn2002-1.1.0/src/medlyn2002/external.py`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/src/medlyn2002/raw.py` & `medlyn2002-1.1.0/src/medlyn2002/raw.py`

 * *Files identical despite different names*

### Comparing `medlyn2002-1.0.0/src/medlyn2002.egg-info/SOURCES.txt` & `medlyn2002-1.1.0/src/medlyn2002.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

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
@@ -27,15 +25,15 @@
 src/medlyn2002/external.py
 src/medlyn2002/info.py
 src/medlyn2002/raw.py
 src/medlyn2002/version.py
 src/medlyn2002.egg-info/PKG-INFO
 src/medlyn2002.egg-info/SOURCES.txt
 src/medlyn2002.egg-info/dependency_links.txt
-src/medlyn2002.egg-info/not-zip-safe
+src/medlyn2002.egg-info/requires.txt
 src/medlyn2002.egg-info/top_level.txt
 src/medlyn2002/clean/readme.rst
 src/medlyn2002/clean/tab2_arrhenius.csv
 src/medlyn2002/clean/tab2_peaked.csv
 src/medlyn2002/clean/tab3.csv
 test/conftest.py
 test/test_packaging.py
```

### Comparing `medlyn2002-1.0.0/test/conftest.py` & `medlyn2002-1.1.0/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=medlyn2002")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=medlyn2002")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

