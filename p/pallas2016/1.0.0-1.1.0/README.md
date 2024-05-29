# Comparing `tmp/pallas2016-1.0.0.tar.gz` & `tmp/pallas2016-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pallas2016-1.0.0.tar", last modified: Fri Mar  4 08:11:47 2022, max compression
+gzip compressed data, was "pallas2016-1.1.0.tar", last modified: Wed May 29 12:40:53 2024, max compression
```

## Comparing `pallas2016-1.0.0.tar` & `pallas2016-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.921577 pallas2016-1.0.0/
--rw-rw-rw-   0        0        0      316 2022-03-04 08:06:49.000000 pallas2016-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3322 2022-03-04 08:06:49.000000 pallas2016-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-03-04 08:06:49.000000 pallas2016-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-03-04 08:06:49.000000 pallas2016-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      438 2022-03-04 08:06:49.000000 pallas2016-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2306 2022-03-04 08:11:47.922581 pallas2016-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1490 2022-03-04 08:06:49.000000 pallas2016-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.812577 pallas2016-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.832576 pallas2016-1.0.0/doc/_gallery/
--rw-rw-rw-   0        0        0     2206 2022-03-01 13:06:38.000000 pallas2016-1.0.0/doc/_gallery/index.rst
--rw-rw-rw-   0        0        0     2492 2022-03-01 13:06:36.000000 pallas2016-1.0.0/doc/_gallery/plot_eq1.rst
--rw-rw-rw-   0        0        0     2456 2022-03-01 13:06:36.000000 pallas2016-1.0.0/doc/_gallery/plot_fig4.rst
--rw-rw-rw-   0        0        0     4441 2022-03-01 13:06:37.000000 pallas2016-1.0.0/doc/_gallery/plot_fig4_eval.rst
--rw-rw-rw-   0        0        0     2489 2022-03-01 13:06:38.000000 pallas2016-1.0.0/doc/_gallery/plot_weather_daily.rst
--rw-rw-rw-   0        0        0     2379 2022-03-01 13:06:38.000000 pallas2016-1.0.0/doc/_gallery/plot_weather_hourly.rst
--rw-rw-rw-   0        0        0     1272 2022-03-01 13:06:38.000000 pallas2016-1.0.0/doc/_gallery/sg_execution_times.rst
--rw-rw-rw-   0        0        0       29 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.834585 pallas2016-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.840581 pallas2016-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5102 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      595 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      165 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1409 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.846576 pallas2016-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       83 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-03-04 08:06:49.000000 pallas2016-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      352 2022-03-04 08:06:49.000000 pallas2016-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-03-04 08:06:49.000000 pallas2016-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-03-04 08:11:47.926578 pallas2016-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1867 2022-03-04 08:06:49.000000 pallas2016-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.742577 pallas2016-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.859577 pallas2016-1.0.0/src/pallas2016/
--rw-rw-rw-   0        0        0      261 2022-03-04 08:06:49.000000 pallas2016-1.0.0/src/pallas2016/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.913586 pallas2016-1.0.0/src/pallas2016/clean/
--rw-rw-rw-   0        0        0      445 2022-03-03 18:20:46.000000 pallas2016-1.0.0/src/pallas2016/clean/fig3.csv
--rw-rw-rw-   0        0        0    10209 2022-03-02 16:02:36.000000 pallas2016-1.0.0/src/pallas2016/clean/fig4.csv
--rw-rw-rw-   0        0        0      928 2022-03-03 15:25:14.000000 pallas2016-1.0.0/src/pallas2016/clean/fig9.csv
--rw-rw-rw-   0        0        0      202 2022-03-01 14:22:01.000000 pallas2016-1.0.0/src/pallas2016/clean/info.json
--rw-rw-rw-   0        0        0      134 2022-03-04 08:06:49.000000 pallas2016-1.0.0/src/pallas2016/clean/readme.rst
--rw-rw-rw-   0        0        0      775 2022-03-03 16:55:47.000000 pallas2016-1.0.0/src/pallas2016/clean/table1.csv
--rw-rw-rw-   0        0        0      423 2022-03-04 08:05:19.000000 pallas2016-1.0.0/src/pallas2016/clean/table2.csv
--rw-rw-rw-   0        0        0     1666 2022-03-01 08:47:33.000000 pallas2016-1.0.0/src/pallas2016/clean/table_s1.csv
--rw-rw-rw-   0        0        0    21657 2022-03-01 09:55:48.000000 pallas2016-1.0.0/src/pallas2016/clean/weather_daily.csv
--rw-rw-rw-   0        0        0   477108 2022-03-01 17:04:07.000000 pallas2016-1.0.0/src/pallas2016/clean/weather_hourly.csv
--rw-rw-rw-   0        0        0      152 2022-03-04 08:06:49.000000 pallas2016-1.0.0/src/pallas2016/info.py
--rw-rw-rw-   0        0        0      912 2022-03-01 13:14:49.000000 pallas2016-1.0.0/src/pallas2016/raw.py
--rw-rw-rw-   0        0        0      367 2022-03-04 08:06:49.000000 pallas2016-1.0.0/src/pallas2016/version.py
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.885579 pallas2016-1.0.0/src/pallas2016.egg-info/
--rw-rw-rw-   0        0        0     2306 2022-03-04 08:11:47.000000 pallas2016-1.0.0/src/pallas2016.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1266 2022-03-04 08:11:47.000000 pallas2016-1.0.0/src/pallas2016.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-04 08:11:47.000000 pallas2016-1.0.0/src/pallas2016.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-25 09:40:55.000000 pallas2016-1.0.0/src/pallas2016.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2022-03-04 08:11:47.000000 pallas2016-1.0.0/src/pallas2016.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-04 08:11:47.919579 pallas2016-1.0.0/test/
--rw-rw-rw-   0        0        0      974 2022-03-04 08:06:49.000000 pallas2016-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       86 2022-03-04 08:06:49.000000 pallas2016-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.050529 pallas2016-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 12:35:19.000000 pallas2016-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3323 2024-05-29 12:35:19.000000 pallas2016-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 12:35:19.000000 pallas2016-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 12:35:19.000000 pallas2016-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2972 2024-05-29 12:40:53.048528 pallas2016-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2024-05-29 12:35:19.000000 pallas2016-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:52.999904 pallas2016-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.008905 pallas2016-1.1.0/doc/_gallery/
+-rw-rw-rw-   0        0        0     2206 2022-03-01 13:06:38.000000 pallas2016-1.1.0/doc/_gallery/index.rst
+-rw-rw-rw-   0        0        0     2492 2022-03-01 13:06:36.000000 pallas2016-1.1.0/doc/_gallery/plot_eq1.rst
+-rw-rw-rw-   0        0        0     2456 2022-03-01 13:06:36.000000 pallas2016-1.1.0/doc/_gallery/plot_fig4.rst
+-rw-rw-rw-   0        0        0     4441 2022-03-01 13:06:37.000000 pallas2016-1.1.0/doc/_gallery/plot_fig4_eval.rst
+-rw-rw-rw-   0        0        0     2489 2022-03-01 13:06:38.000000 pallas2016-1.1.0/doc/_gallery/plot_weather_daily.rst
+-rw-rw-rw-   0        0        0     2379 2022-03-01 13:06:38.000000 pallas2016-1.1.0/doc/_gallery/plot_weather_hourly.rst
+-rw-rw-rw-   0        0        0     1272 2022-03-01 13:06:38.000000 pallas2016-1.1.0/doc/_gallery/sg_execution_times.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.008905 pallas2016-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.009904 pallas2016-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5102 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1069 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.011903 pallas2016-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 12:35:19.000000 pallas2016-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2322 2024-05-29 12:35:19.000000 pallas2016-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      352 2024-05-29 12:35:19.000000 pallas2016-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 12:35:19.000000 pallas2016-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:40:53.050529 pallas2016-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:52.959392 pallas2016-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.015905 pallas2016-1.1.0/src/pallas2016/
+-rw-rw-rw-   0        0        0      253 2024-05-29 12:35:19.000000 pallas2016-1.1.0/src/pallas2016/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.039530 pallas2016-1.1.0/src/pallas2016/clean/
+-rw-rw-rw-   0        0        0      445 2024-05-29 12:34:02.000000 pallas2016-1.1.0/src/pallas2016/clean/fig3.csv
+-rw-rw-rw-   0        0        0    10209 2024-05-29 12:34:05.000000 pallas2016-1.1.0/src/pallas2016/clean/fig4.csv
+-rw-rw-rw-   0        0        0      928 2024-05-29 12:34:09.000000 pallas2016-1.1.0/src/pallas2016/clean/fig9.csv
+-rw-rw-rw-   0        0        0      202 2024-05-29 12:34:14.000000 pallas2016-1.1.0/src/pallas2016/clean/info.json
+-rw-rw-rw-   0        0        0      134 2024-05-29 12:35:19.000000 pallas2016-1.1.0/src/pallas2016/clean/readme.rst
+-rw-rw-rw-   0        0        0      775 2022-03-03 16:55:47.000000 pallas2016-1.1.0/src/pallas2016/clean/table1.csv
+-rw-rw-rw-   0        0        0      423 2022-03-04 08:05:19.000000 pallas2016-1.1.0/src/pallas2016/clean/table2.csv
+-rw-rw-rw-   0        0        0     1666 2024-05-29 12:34:18.000000 pallas2016-1.1.0/src/pallas2016/clean/table_s1.csv
+-rw-rw-rw-   0        0        0    21657 2024-05-29 12:34:23.000000 pallas2016-1.1.0/src/pallas2016/clean/weather_daily.csv
+-rw-rw-rw-   0        0        0   477108 2024-05-29 12:34:28.000000 pallas2016-1.1.0/src/pallas2016/clean/weather_hourly.csv
+-rw-rw-rw-   0        0        0      379 2024-05-29 12:35:19.000000 pallas2016-1.1.0/src/pallas2016/info.py
+-rw-rw-rw-   0        0        0      912 2022-03-01 13:14:49.000000 pallas2016-1.1.0/src/pallas2016/raw.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 12:35:19.000000 pallas2016-1.1.0/src/pallas2016/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.045529 pallas2016-1.1.0/src/pallas2016.egg-info/
+-rw-rw-rw-   0        0        0     2972 2024-05-29 12:40:52.000000 pallas2016-1.1.0/src/pallas2016.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-05-29 12:40:52.000000 pallas2016-1.1.0/src/pallas2016.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:40:52.000000 pallas2016-1.1.0/src/pallas2016.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-29 12:40:52.000000 pallas2016-1.1.0/src/pallas2016.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 12:40:52.000000 pallas2016-1.1.0/src/pallas2016.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 12:40:53.043530 pallas2016-1.1.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-29 12:35:19.000000 pallas2016-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      381 2024-05-29 12:35:19.000000 pallas2016-1.1.0/test/test_packaging.py
```

### Comparing `pallas2016-1.0.0/CONTRIBUTING.rst` & `pallas2016-1.1.0/CONTRIBUTING.rst`

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

### Comparing `pallas2016-1.0.0/LICENSE` & `pallas2016-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/README.rst` & `pallas2016-1.1.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 ========================
 pallas2016
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/pallas2016/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/pallas2016/
-
 .. image:: https://b326.gitlab.io/pallas2016/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/pallas2016/1.0.0/
+    :target: https://pypi.org/project/pallas2016/1.1.0/
 
 .. image:: https://b326.gitlab.io/pallas2016/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/pallas2016
 
+.. image:: https://b326.gitlab.io/pallas2016/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/pallas2016/
+
 .. image:: https://badge.fury.io/py/pallas2016.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/pallas2016
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/pallas2016/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/pallas2016/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/pallas2016/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/pallas2016/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/pallas2016/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/pallas2016/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/pallas2016/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/pallas2016/commits/prod
 .. #}
 
 Data and formalisms from Pallas et al. (2016)
```

### Comparing `pallas2016-1.0.0/doc/Makefile` & `pallas2016-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/index.rst` & `pallas2016-1.1.0/doc/_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/plot_eq1.rst` & `pallas2016-1.1.0/doc/_gallery/plot_eq1.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/plot_fig4.rst` & `pallas2016-1.1.0/doc/_gallery/plot_fig4.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/plot_fig4_eval.rst` & `pallas2016-1.1.0/doc/_gallery/plot_fig4_eval.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/plot_weather_daily.rst` & `pallas2016-1.1.0/doc/_gallery/plot_weather_daily.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/plot_weather_hourly.rst` & `pallas2016-1.1.0/doc/_gallery/plot_weather_hourly.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/_gallery/sg_execution_times.rst` & `pallas2016-1.1.0/doc/_gallery/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/biblio/biblio.rst` & `pallas2016-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/conf.py` & `pallas2016-1.1.0/doc/conf.py`

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

### Comparing `pallas2016-1.0.0/doc/index.rst` & `pallas2016-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/make.bat` & `pallas2016-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/doc/readme.rst` & `pallas2016-1.1.0/doc/readme.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/pallas2016/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/pallas2016/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/pallas2016/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/pallas2016/1.0.0/
+    :target: https://pypi.org/project/pallas2016/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/pallas2016/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/pallas2016
 
+
+.. image:: https://b326.gitlab.io/pallas2016/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/pallas2016/
+
+
 .. image:: https://badge.fury.io/py/pallas2016.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/pallas2016
 
 
+
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/pallas2016/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/pallas2016/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/pallas2016/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/pallas2016/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/pallas2016/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/pallas2016/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/pallas2016/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/pallas2016/commits/prod
-
 .. #}
 
 Data and formalisms from Pallas et al. (2016)
```

### Comparing `pallas2016-1.0.0/src/pallas2016/clean/fig4.csv` & `pallas2016-1.1.0/src/pallas2016/clean/fig4.csv`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016/clean/fig9.csv` & `pallas2016-1.1.0/src/pallas2016/clean/fig9.csv`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016/clean/table1.csv` & `pallas2016-1.1.0/src/pallas2016/clean/table1.csv`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016/clean/table_s1.csv` & `pallas2016-1.1.0/src/pallas2016/clean/table_s1.csv`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016/clean/weather_daily.csv` & `pallas2016-1.1.0/src/pallas2016/clean/weather_daily.csv`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016/clean/weather_hourly.csv` & `pallas2016-1.1.0/src/pallas2016/clean/weather_hourly.csv`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016/raw.py` & `pallas2016-1.1.0/src/pallas2016/raw.py`

 * *Files identical despite different names*

### Comparing `pallas2016-1.0.0/src/pallas2016.egg-info/SOURCES.txt` & `pallas2016-1.1.0/src/pallas2016.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

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
@@ -33,15 +31,15 @@
 src/pallas2016/__init__.py
 src/pallas2016/info.py
 src/pallas2016/raw.py
 src/pallas2016/version.py
 src/pallas2016.egg-info/PKG-INFO
 src/pallas2016.egg-info/SOURCES.txt
 src/pallas2016.egg-info/dependency_links.txt
-src/pallas2016.egg-info/not-zip-safe
+src/pallas2016.egg-info/requires.txt
 src/pallas2016.egg-info/top_level.txt
 src/pallas2016/clean/fig3.csv
 src/pallas2016/clean/fig4.csv
 src/pallas2016/clean/fig9.csv
 src/pallas2016/clean/info.json
 src/pallas2016/clean/readme.rst
 src/pallas2016/clean/table1.csv
```

### Comparing `pallas2016-1.0.0/test/conftest.py` & `pallas2016-1.1.0/test/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=pallas2016")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=pallas2016")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

