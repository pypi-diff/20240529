# Comparing `tmp/harley1992-1.0.0.tar.gz` & `tmp/harley1992-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harley1992-1.0.0.tar", last modified: Wed Dec 22 08:27:28 2021, max compression
+gzip compressed data, was "harley1992-1.1.0.tar", last modified: Wed May 29 09:11:26 2024, max compression
```

## Comparing `harley1992-1.0.0.tar` & `harley1992-1.1.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.502972 harley1992-1.0.0/
--rw-rw-rw-   0        0        0      316 2021-12-22 08:17:18.000000 harley1992-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3322 2021-12-22 08:17:18.000000 harley1992-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2021-12-22 08:17:18.000000 harley1992-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2021-12-22 08:17:18.000000 harley1992-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      438 2021-12-22 08:17:18.000000 harley1992-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2312 2021-12-22 08:27:28.502972 harley1992-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2021-12-22 08:17:18.000000 harley1992-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.386685 harley1992-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.404704 harley1992-1.0.0/doc/_gallery/
--rw-rw-rw-   0        0        0     1534 2021-12-21 15:40:01.000000 harley1992-1.0.0/doc/_gallery/index.rst
--rw-rw-rw-   0        0        0     4677 2021-12-21 15:39:59.000000 harley1992-1.0.0/doc/_gallery/plot_fig1.rst
--rw-rw-rw-   0        0        0     2931 2021-12-21 15:40:00.000000 harley1992-1.0.0/doc/_gallery/plot_fig3.rst
--rw-rw-rw-   0        0        0     6795 2021-12-21 15:43:46.000000 harley1992-1.0.0/doc/_gallery/plot_fig8.rst
--rw-rw-rw-   0        0        0      724 2021-12-21 15:43:46.000000 harley1992-1.0.0/doc/_gallery/sg_execution_times.rst
--rw-rw-rw-   0        0        0       29 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.404704 harley1992-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.408696 harley1992-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5105 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      595 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      165 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1412 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.412697 harley1992-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       83 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0      133 2021-12-22 08:17:18.000000 harley1992-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      352 2021-12-22 08:17:18.000000 harley1992-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2021-12-22 08:17:18.000000 harley1992-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2021-12-22 08:27:28.515123 harley1992-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1870 2021-12-22 08:17:18.000000 harley1992-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.308235 harley1992-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.428712 harley1992-1.0.0/src/harley1992/
--rw-rw-rw-   0        0        0      264 2021-12-22 08:17:18.000000 harley1992-1.0.0/src/harley1992/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.491483 harley1992-1.0.0/src/harley1992/clean/
--rw-rw-rw-   0        0        0      790 2021-12-21 14:39:52.000000 harley1992-1.0.0/src/harley1992/clean/fig1.csv
--rw-rw-rw-   0        0        0      439 2021-12-21 08:34:55.000000 harley1992-1.0.0/src/harley1992/clean/fig1_params.csv
--rw-rw-rw-   0        0        0     1267 2021-12-21 14:39:56.000000 harley1992-1.0.0/src/harley1992/clean/fig8.csv
--rw-rw-rw-   0        0        0      134 2021-12-22 08:17:18.000000 harley1992-1.0.0/src/harley1992/clean/readme.rst
--rw-rw-rw-   0        0        0     1539 2021-12-21 10:46:55.000000 harley1992-1.0.0/src/harley1992/clean/table1.csv
--rw-rw-rw-   0        0        0      152 2021-12-22 08:17:18.000000 harley1992-1.0.0/src/harley1992/info.py
--rw-rw-rw-   0        0        0     8050 2021-12-21 15:57:16.000000 harley1992-1.0.0/src/harley1992/raw.py
--rw-rw-rw-   0        0        0      367 2021-12-22 08:17:18.000000 harley1992-1.0.0/src/harley1992/version.py
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.476916 harley1992-1.0.0/src/harley1992.egg-info/
--rw-rw-rw-   0        0        0     2312 2021-12-22 08:27:28.000000 harley1992-1.0.0/src/harley1992.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1020 2021-12-22 08:27:28.000000 harley1992-1.0.0/src/harley1992.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-22 08:27:28.000000 harley1992-1.0.0/src/harley1992.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-17 10:19:33.000000 harley1992-1.0.0/src/harley1992.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2021-12-22 08:27:28.000000 harley1992-1.0.0/src/harley1992.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-12-22 08:27:28.498975 harley1992-1.0.0/test/
--rw-rw-rw-   0        0        0      974 2021-12-22 08:17:18.000000 harley1992-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       86 2021-12-22 08:17:18.000000 harley1992-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.799931 harley1992-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 09:03:26.000000 harley1992-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3323 2024-05-29 09:03:26.000000 harley1992-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 09:03:26.000000 harley1992-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 09:03:26.000000 harley1992-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2979 2024-05-29 09:11:26.796908 harley1992-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2024-05-29 09:03:26.000000 harley1992-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.767927 harley1992-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.772926 harley1992-1.1.0/doc/_gallery/
+-rw-rw-rw-   0        0        0     1534 2021-12-21 15:40:01.000000 harley1992-1.1.0/doc/_gallery/index.rst
+-rw-rw-rw-   0        0        0     4677 2021-12-21 15:39:59.000000 harley1992-1.1.0/doc/_gallery/plot_fig1.rst
+-rw-rw-rw-   0        0        0     2931 2021-12-21 15:40:00.000000 harley1992-1.1.0/doc/_gallery/plot_fig3.rst
+-rw-rw-rw-   0        0        0     6795 2021-12-21 15:43:46.000000 harley1992-1.1.0/doc/_gallery/plot_fig8.rst
+-rw-rw-rw-   0        0        0      724 2021-12-21 15:43:46.000000 harley1992-1.1.0/doc/_gallery/sg_execution_times.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.773926 harley1992-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.774926 harley1992-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5105 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1072 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.776926 harley1992-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 09:03:26.000000 harley1992-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2325 2024-05-29 09:03:26.000000 harley1992-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      352 2024-05-29 09:03:26.000000 harley1992-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:03:26.000000 harley1992-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:11:26.799931 harley1992-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.732418 harley1992-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.780926 harley1992-1.1.0/src/harley1992/
+-rw-rw-rw-   0        0        0      256 2024-05-29 09:03:26.000000 harley1992-1.1.0/src/harley1992/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.791926 harley1992-1.1.0/src/harley1992/clean/
+-rw-rw-rw-   0        0        0      790 2024-05-29 09:02:15.000000 harley1992-1.1.0/src/harley1992/clean/fig1.csv
+-rw-rw-rw-   0        0        0      439 2024-05-29 09:02:20.000000 harley1992-1.1.0/src/harley1992/clean/fig1_params.csv
+-rw-rw-rw-   0        0        0     1267 2024-05-29 09:02:24.000000 harley1992-1.1.0/src/harley1992/clean/fig8.csv
+-rw-rw-rw-   0        0        0      134 2024-05-29 09:03:26.000000 harley1992-1.1.0/src/harley1992/clean/readme.rst
+-rw-rw-rw-   0        0        0     1522 2024-05-29 09:02:29.000000 harley1992-1.1.0/src/harley1992/clean/table1.csv
+-rw-rw-rw-   0        0        0      379 2024-05-29 09:03:26.000000 harley1992-1.1.0/src/harley1992/info.py
+-rw-rw-rw-   0        0        0     8049 2022-01-10 16:03:28.000000 harley1992-1.1.0/src/harley1992/raw.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 09:03:26.000000 harley1992-1.1.0/src/harley1992/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.794926 harley1992-1.1.0/src/harley1992.egg-info/
+-rw-rw-rw-   0        0        0     2979 2024-05-29 09:11:26.000000 harley1992-1.1.0/src/harley1992.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-29 09:11:26.000000 harley1992-1.1.0/src/harley1992.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:11:26.000000 harley1992-1.1.0/src/harley1992.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-29 09:11:26.000000 harley1992-1.1.0/src/harley1992.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 09:11:26.000000 harley1992-1.1.0/src/harley1992.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:11:26.793926 harley1992-1.1.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-29 09:03:26.000000 harley1992-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      381 2024-05-29 09:03:26.000000 harley1992-1.1.0/test/test_packaging.py
```

### Comparing `harley1992-1.0.0/CONTRIBUTING.rst` & `harley1992-1.1.0/CONTRIBUTING.rst`

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

### Comparing `harley1992-1.0.0/LICENSE` & `harley1992-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/README.rst` & `harley1992-1.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 ========================
 harley1992
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/harley1992/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/harley1992/
-
 .. image:: https://b326.gitlab.io/harley1992/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/harley1992/1.0.0/
+    :target: https://pypi.org/project/harley1992/1.1.0/
 
 .. image:: https://b326.gitlab.io/harley1992/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/harley1992
 
+.. image:: https://b326.gitlab.io/harley1992/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/harley1992/
+
 .. image:: https://badge.fury.io/py/harley1992.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/harley1992
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/harley1992/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/harley1992/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/harley1992/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/harley1992/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/harley1992/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/harley1992/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/harley1992/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/harley1992/commits/prod
 .. #}
 
 Data and formalisms from Harley 1992 publication
```

### Comparing `harley1992-1.0.0/doc/Makefile` & `harley1992-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/_gallery/index.rst` & `harley1992-1.1.0/doc/_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/_gallery/plot_fig1.rst` & `harley1992-1.1.0/doc/_gallery/plot_fig1.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/_gallery/plot_fig3.rst` & `harley1992-1.1.0/doc/_gallery/plot_fig3.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/_gallery/plot_fig8.rst` & `harley1992-1.1.0/doc/_gallery/plot_fig8.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/_gallery/sg_execution_times.rst` & `harley1992-1.1.0/doc/_gallery/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/biblio/biblio.rst` & `harley1992-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/conf.py` & `harley1992-1.1.0/doc/conf.py`

 * *Files 5% similar despite different names*

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

### Comparing `harley1992-1.0.0/doc/index.rst` & `harley1992-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/make.bat` & `harley1992-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/doc/readme.rst` & `harley1992-1.1.0/doc/readme.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/harley1992/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/harley1992/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/harley1992/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/harley1992/1.0.0/
+    :target: https://pypi.org/project/harley1992/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/harley1992/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/harley1992
 
+
+.. image:: https://b326.gitlab.io/harley1992/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/harley1992/
+
+
 .. image:: https://badge.fury.io/py/harley1992.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/harley1992
 
 
+
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/harley1992/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/harley1992/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/harley1992/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/harley1992/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/harley1992/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/harley1992/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/harley1992/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/harley1992/commits/prod
-
 .. #}
 
 Data and formalisms from Harley 1992 publication
```

### Comparing `harley1992-1.0.0/src/harley1992/clean/fig1.csv` & `harley1992-1.1.0/src/harley1992/clean/fig1.csv`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/src/harley1992/clean/fig8.csv` & `harley1992-1.1.0/src/harley1992/clean/fig8.csv`

 * *Files identical despite different names*

### Comparing `harley1992-1.0.0/src/harley1992/clean/table1.csv` & `harley1992-1.1.0/src/harley1992/clean/table1.csv`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file has been generated by fmt_table1.py
 #
 # name: name of variable
 # unit: [none]
-# ca: [Pa CO2] growth modality, partial pressure of CO2 during growth
+# ca: [Pa CO2] partial pressure of CO2 during growth
 # value: [unit]
 #
 name;unit;ca;value
 kc_c;[-];35;35.79
 kc_c;[-];65;35.79
 kc_deltaha;[kJ.mol-1];35;80.47
 kc_deltaha;[kJ.mol-1];65;80.47
```

### Comparing `harley1992-1.0.0/src/harley1992/raw.py` & `harley1992-1.1.0/src/harley1992/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 def eq10(a, ca, gs):
     """Partial pressure of CO2 in the intercellular space.
 
     Args:
         a (float): [µmol CO2.m-2.s-1] Net carbon assimilation
         ca (float): [Pa] partial pressure of CO2 in the air outside the leaf boundary
-        gs (float): [mmmol H2O.m-2.s-1] Leaf conductance to H2O flux
+        gs (float): [mmol H2O.m-2.s-1] Leaf conductance to H2O flux
 
     Returns:
         (float): Ci [Pa]
     """
     return ca - a * 1.6 * 100 / gs  # TODO potentially 1000 instead of 100
```

### Comparing `harley1992-1.0.0/src/harley1992.egg-info/SOURCES.txt` & `harley1992-1.1.0/src/harley1992.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
@@ -31,15 +29,15 @@
 src/harley1992/__init__.py
 src/harley1992/info.py
 src/harley1992/raw.py
 src/harley1992/version.py
 src/harley1992.egg-info/PKG-INFO
 src/harley1992.egg-info/SOURCES.txt
 src/harley1992.egg-info/dependency_links.txt
-src/harley1992.egg-info/not-zip-safe
+src/harley1992.egg-info/requires.txt
 src/harley1992.egg-info/top_level.txt
 src/harley1992/clean/fig1.csv
 src/harley1992/clean/fig1_params.csv
 src/harley1992/clean/fig8.csv
 src/harley1992/clean/readme.rst
 src/harley1992/clean/table1.csv
 test/conftest.py
```

### Comparing `harley1992-1.0.0/test/conftest.py` & `harley1992-1.1.0/test/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=harley1992")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=harley1992")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

