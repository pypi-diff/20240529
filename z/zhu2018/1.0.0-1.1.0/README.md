# Comparing `tmp/zhu2018-1.0.0.tar.gz` & `tmp/zhu2018-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhu2018-1.0.0.tar", last modified: Tue Sep 28 18:39:04 2021, max compression
+gzip compressed data, was "zhu2018-1.1.0.tar", last modified: Wed May 29 14:14:30 2024, max compression
```

## Comparing `zhu2018-1.0.0.tar` & `zhu2018-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.610999 zhu2018-1.0.0/
--rw-rw-rw-   0        0        0      316 2021-09-28 18:29:26.000000 zhu2018-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3292 2021-09-28 18:29:26.000000 zhu2018-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2021-09-28 18:29:26.000000 zhu2018-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2021-09-28 18:29:26.000000 zhu2018-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      435 2021-09-28 18:29:26.000000 zhu2018-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2624 2021-09-28 18:39:04.610999 zhu2018-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1427 2021-09-28 18:29:26.000000 zhu2018-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.530988 zhu2018-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.541008 zhu2018-1.0.0/doc/_gallery/
--rw-rw-rw-   0        0        0     1510 2021-09-28 18:24:36.000000 zhu2018-1.0.0/doc/_gallery/index.rst
--rw-rw-rw-   0        0        0     2340 2021-09-28 18:24:36.000000 zhu2018-1.0.0/doc/_gallery/plot_fig4.rst
--rw-rw-rw-   0        0        0     2507 2021-09-28 15:04:32.000000 zhu2018-1.0.0/doc/_gallery/plot_fig5.rst
--rw-rw-rw-   0        0        0     2382 2021-09-28 15:04:33.000000 zhu2018-1.0.0/doc/_gallery/plot_figs4.rst
--rw-rw-rw-   0        0        0      738 2021-09-28 18:24:36.000000 zhu2018-1.0.0/doc/_gallery/sg_execution_times.rst
--rw-rw-rw-   0        0        0       29 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.545989 zhu2018-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.545989 zhu2018-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5060 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      589 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      162 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1349 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.550988 zhu2018-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       83 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2021-09-28 18:29:26.000000 zhu2018-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      360 2021-09-28 18:29:26.000000 zhu2018-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2021-09-28 18:29:26.000000 zhu2018-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2021-09-28 18:39:04.616005 zhu2018-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1862 2021-09-28 18:29:26.000000 zhu2018-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.475988 zhu2018-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.560998 zhu2018-1.0.0/src/zhu2018/
--rw-rw-rw-   0        0        0      249 2021-09-28 18:29:26.000000 zhu2018-1.0.0/src/zhu2018/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.595992 zhu2018-1.0.0/src/zhu2018/clean/
--rw-rw-rw-   0        0        0     5011 2021-09-28 18:13:26.000000 zhu2018-1.0.0/src/zhu2018/clean/fig4.csv
--rw-rw-rw-   0        0        0    14567 2021-09-28 09:25:29.000000 zhu2018-1.0.0/src/zhu2018/clean/fig5.csv
--rw-rw-rw-   0        0        0     4360 2021-09-28 09:42:00.000000 zhu2018-1.0.0/src/zhu2018/clean/figs4.csv
--rw-rw-rw-   0        0        0      134 2021-09-28 18:29:26.000000 zhu2018-1.0.0/src/zhu2018/clean/readme.rst
--rw-rw-rw-   0        0        0      152 2021-09-28 18:29:26.000000 zhu2018-1.0.0/src/zhu2018/info.py
--rw-rw-rw-   0        0        0      367 2021-09-28 18:29:26.000000 zhu2018-1.0.0/src/zhu2018/version.py
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.585989 zhu2018-1.0.0/src/zhu2018.egg-info/
--rw-rw-rw-   0        0        0     2624 2021-09-28 18:39:04.000000 zhu2018-1.0.0/src/zhu2018.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2021-09-28 18:39:04.000000 zhu2018-1.0.0/src/zhu2018.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-28 18:39:04.000000 zhu2018-1.0.0/src/zhu2018.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-28 07:46:46.000000 zhu2018-1.0.0/src/zhu2018.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2021-09-28 18:39:04.000000 zhu2018-1.0.0/src/zhu2018.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-09-28 18:39:04.610999 zhu2018-1.0.0/test/
--rw-rw-rw-   0        0        0      971 2021-09-28 18:29:26.000000 zhu2018-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0      462 2021-09-28 18:22:57.000000 zhu2018-1.0.0/test/test_fig4.py
--rw-rw-rw-   0        0        0      417 2021-09-28 18:22:28.000000 zhu2018-1.0.0/test/test_fig5.py
--rw-rw-rw-   0        0        0      418 2021-09-28 18:22:29.000000 zhu2018-1.0.0/test/test_figs4.py
--rw-rw-rw-   0        0        0       80 2021-09-28 18:29:26.000000 zhu2018-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.692140 zhu2018-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 14:10:34.000000 zhu2018-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3293 2024-05-29 14:10:34.000000 zhu2018-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 14:10:34.000000 zhu2018-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 14:10:34.000000 zhu2018-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2931 2024-05-29 14:14:30.691140 zhu2018-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-05-29 14:10:34.000000 zhu2018-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.654529 zhu2018-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.658518 zhu2018-1.1.0/doc/_gallery/
+-rw-rw-rw-   0        0        0     1510 2021-09-28 18:24:36.000000 zhu2018-1.1.0/doc/_gallery/index.rst
+-rw-rw-rw-   0        0        0     2340 2021-09-28 18:24:36.000000 zhu2018-1.1.0/doc/_gallery/plot_fig4.rst
+-rw-rw-rw-   0        0        0     2507 2021-09-28 15:04:32.000000 zhu2018-1.1.0/doc/_gallery/plot_fig5.rst
+-rw-rw-rw-   0        0        0     2382 2021-09-28 15:04:33.000000 zhu2018-1.1.0/doc/_gallery/plot_figs4.rst
+-rw-rw-rw-   0        0        0      738 2021-09-28 18:24:36.000000 zhu2018-1.1.0/doc/_gallery/sg_execution_times.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.659520 zhu2018-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.660519 zhu2018-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5060 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      589 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      217 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1021 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.662519 zhu2018-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 14:10:34.000000 zhu2018-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2304 2024-05-29 14:10:34.000000 zhu2018-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      360 2024-05-29 14:10:34.000000 zhu2018-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 14:10:34.000000 zhu2018-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:14:30.692140 zhu2018-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.617446 zhu2018-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.666977 zhu2018-1.1.0/src/zhu2018/
+-rw-rw-rw-   0        0        0      241 2024-05-29 14:10:34.000000 zhu2018-1.1.0/src/zhu2018/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.676991 zhu2018-1.1.0/src/zhu2018/clean/
+-rw-rw-rw-   0        0        0     5011 2024-05-29 14:09:25.000000 zhu2018-1.1.0/src/zhu2018/clean/fig4.csv
+-rw-rw-rw-   0        0        0    14567 2024-05-29 14:09:31.000000 zhu2018-1.1.0/src/zhu2018/clean/fig5.csv
+-rw-rw-rw-   0        0        0     4360 2024-05-29 14:09:48.000000 zhu2018-1.1.0/src/zhu2018/clean/figs4.csv
+-rw-rw-rw-   0        0        0      134 2024-05-29 14:10:34.000000 zhu2018-1.1.0/src/zhu2018/clean/readme.rst
+-rw-rw-rw-   0        0        0      379 2024-05-29 14:10:34.000000 zhu2018-1.1.0/src/zhu2018/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 14:10:34.000000 zhu2018-1.1.0/src/zhu2018/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.689139 zhu2018-1.1.0/src/zhu2018.egg-info/
+-rw-rw-rw-   0        0        0     2931 2024-05-29 14:14:30.000000 zhu2018-1.1.0/src/zhu2018.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2024-05-29 14:14:30.000000 zhu2018-1.1.0/src/zhu2018.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:14:30.000000 zhu2018-1.1.0/src/zhu2018.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-05-29 14:14:30.000000 zhu2018-1.1.0/src/zhu2018.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 14:14:30.000000 zhu2018-1.1.0/src/zhu2018.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 14:14:30.687139 zhu2018-1.1.0/test/
+-rw-rw-rw-   0        0        0      983 2024-05-29 14:10:34.000000 zhu2018-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      462 2021-09-28 18:22:57.000000 zhu2018-1.1.0/test/test_fig4.py
+-rw-rw-rw-   0        0        0      417 2021-09-28 18:22:28.000000 zhu2018-1.1.0/test/test_fig5.py
+-rw-rw-rw-   0        0        0      418 2021-09-28 18:22:29.000000 zhu2018-1.1.0/test/test_figs4.py
+-rw-rw-rw-   0        0        0      369 2024-05-29 14:10:34.000000 zhu2018-1.1.0/test/test_packaging.py
```

### Comparing `zhu2018-1.0.0/CONTRIBUTING.rst` & `zhu2018-1.1.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

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

### Comparing `zhu2018-1.0.0/LICENSE` & `zhu2018-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/README.rst` & `zhu2018-1.1.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 ========================
 zhu2018
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/zhu2018/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/zhu2018/
-
 .. image:: https://b326.gitlab.io/zhu2018/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/zhu2018/1.0.0/
+    :target: https://pypi.org/project/zhu2018/1.1.0/
 
 .. image:: https://b326.gitlab.io/zhu2018/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/zhu2018
 
+.. image:: https://b326.gitlab.io/zhu2018/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/zhu2018/
+
 .. image:: https://badge.fury.io/py/zhu2018.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/zhu2018
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/zhu2018/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/zhu2018/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/zhu2018/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/zhu2018/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/zhu2018/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/zhu2018/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/zhu2018/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/zhu2018/commits/prod
 .. #}
 
 Data and formalisms from Zhu 2018
```

### Comparing `zhu2018-1.0.0/doc/Makefile` & `zhu2018-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/_gallery/index.rst` & `zhu2018-1.1.0/doc/_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/_gallery/plot_fig4.rst` & `zhu2018-1.1.0/doc/_gallery/plot_fig4.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/_gallery/plot_fig5.rst` & `zhu2018-1.1.0/doc/_gallery/plot_fig5.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/_gallery/plot_figs4.rst` & `zhu2018-1.1.0/doc/_gallery/plot_figs4.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/_gallery/sg_execution_times.rst` & `zhu2018-1.1.0/doc/_gallery/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/biblio/biblio.rst` & `zhu2018-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/conf.py` & `zhu2018-1.1.0/doc/conf.py`

 * *Files 1% similar despite different names*

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

### Comparing `zhu2018-1.0.0/doc/index.rst` & `zhu2018-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/doc/make.bat` & `zhu2018-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/src/zhu2018/clean/fig4.csv` & `zhu2018-1.1.0/src/zhu2018/clean/fig4.csv`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/src/zhu2018/clean/fig5.csv` & `zhu2018-1.1.0/src/zhu2018/clean/fig5.csv`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/src/zhu2018/clean/figs4.csv` & `zhu2018-1.1.0/src/zhu2018/clean/figs4.csv`

 * *Files identical despite different names*

### Comparing `zhu2018-1.0.0/src/zhu2018.egg-info/SOURCES.txt` & `zhu2018-1.1.0/src/zhu2018.egg-info/SOURCES.txt`

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
@@ -30,15 +28,15 @@
 doc/user/overview.rst
 src/zhu2018/__init__.py
 src/zhu2018/info.py
 src/zhu2018/version.py
 src/zhu2018.egg-info/PKG-INFO
 src/zhu2018.egg-info/SOURCES.txt
 src/zhu2018.egg-info/dependency_links.txt
-src/zhu2018.egg-info/not-zip-safe
+src/zhu2018.egg-info/requires.txt
 src/zhu2018.egg-info/top_level.txt
 src/zhu2018/clean/fig4.csv
 src/zhu2018/clean/fig5.csv
 src/zhu2018/clean/figs4.csv
 src/zhu2018/clean/readme.rst
 test/conftest.py
 test/test_fig4.py
```

### Comparing `zhu2018-1.0.0/test/conftest.py` & `zhu2018-1.1.0/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=zhu2018")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=zhu2018")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

