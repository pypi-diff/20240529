# Comparing `tmp/tuzet2003-1.0.0.tar.gz` & `tmp/tuzet2003-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuzet2003-1.0.0.tar", last modified: Mon Jun 13 12:14:39 2022, max compression
+gzip compressed data, was "tuzet2003-1.1.0.tar", last modified: Wed May 29 13:42:28 2024, max compression
```

## Comparing `tuzet2003-1.0.0.tar` & `tuzet2003-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.322459 tuzet2003-1.0.0/
--rw-rw-rw-   0        0        0      316 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3312 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      437 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2287 2022-06-13 12:14:39.322459 tuzet2003-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.199212 tuzet2003-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.231210 tuzet2003-1.0.0/doc/_gallery/
--rw-rw-rw-   0        0        0     4105 2022-01-11 16:48:50.000000 tuzet2003-1.0.0/doc/_gallery/index.rst
--rw-rw-rw-   0        0        0     1946 2022-01-11 16:48:48.000000 tuzet2003-1.0.0/doc/_gallery/plot_eq_a12.rst
--rw-rw-rw-   0        0        0     2524 2022-01-11 16:48:47.000000 tuzet2003-1.0.0/doc/_gallery/plot_eq_b1.rst
--rw-rw-rw-   0        0        0     2405 2022-01-11 16:48:49.000000 tuzet2003-1.0.0/doc/_gallery/plot_eq_b2.rst
--rw-rw-rw-   0        0        0     2547 2022-01-11 16:48:49.000000 tuzet2003-1.0.0/doc/_gallery/plot_eq_b3.rst
--rw-rw-rw-   0        0        0     2205 2022-01-11 16:48:50.000000 tuzet2003-1.0.0/doc/_gallery/plot_eq_b4.rst
--rw-rw-rw-   0        0        0     2157 2022-01-11 16:48:46.000000 tuzet2003-1.0.0/doc/_gallery/plot_fig2.rst
--rw-rw-rw-   0        0        0     4763 2022-01-11 16:50:41.000000 tuzet2003-1.0.0/doc/_gallery/plot_fig5.rst
--rw-rw-rw-   0        0        0     2081 2022-01-11 16:48:47.000000 tuzet2003-1.0.0/doc/_gallery/plot_fig6a.rst
--rw-rw-rw-   0        0        0     2820 2022-01-11 16:48:47.000000 tuzet2003-1.0.0/doc/_gallery/plot_net_photosynthesis.rst
--rw-rw-rw-   0        0        0     2929 2022-01-11 16:48:49.000000 tuzet2003-1.0.0/doc/_gallery/plot_soil_water_relations.rst
--rw-rw-rw-   0        0        0     2544 2022-01-11 16:50:42.000000 tuzet2003-1.0.0/doc/_gallery/sg_execution_times.rst
--rw-rw-rw-   0        0        0       29 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.235211 tuzet2003-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.235211 tuzet2003-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5093 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      593 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      164 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1392 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.243239 tuzet2003-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       83 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      359 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       36 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-06-13 12:14:39.326460 tuzet2003-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1882 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.134178 tuzet2003-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.263206 tuzet2003-1.0.0/src/tuzet2003/
--rw-rw-rw-   0        0        0      262 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/src/tuzet2003/__init__.py
--rw-rw-rw-   0        0        0    18136 2022-06-13 12:05:58.000000 tuzet2003-1.0.0/src/tuzet2003/appendix.py
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.310485 tuzet2003-1.0.0/src/tuzet2003/clean/
--rw-rw-rw-   0        0        0     5609 2022-01-05 10:52:41.000000 tuzet2003-1.0.0/src/tuzet2003/clean/fig2.csv
--rw-rw-rw-   0        0        0    16131 2022-01-10 09:57:29.000000 tuzet2003-1.0.0/src/tuzet2003/clean/fig5.csv
--rw-rw-rw-   0        0        0      134 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/src/tuzet2003/clean/readme.rst
--rw-rw-rw-   0        0        0      582 2022-01-06 08:29:05.000000 tuzet2003-1.0.0/src/tuzet2003/clean/table1.csv
--rw-rw-rw-   0        0        0      324 2022-01-06 08:29:09.000000 tuzet2003-1.0.0/src/tuzet2003/clean/table2.csv
--rw-rw-rw-   0        0        0      644 2022-01-07 14:36:41.000000 tuzet2003-1.0.0/src/tuzet2003/clean/table3.csv
--rw-rw-rw-   0        0        0     4317 2022-01-19 14:47:55.000000 tuzet2003-1.0.0/src/tuzet2003/external.py
--rw-rw-rw-   0        0        0      152 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/src/tuzet2003/info.py
--rw-rw-rw-   0        0        0    10359 2022-01-31 16:51:40.000000 tuzet2003-1.0.0/src/tuzet2003/leaf.py
--rw-rw-rw-   0        0        0     5133 2022-01-11 17:27:49.000000 tuzet2003-1.0.0/src/tuzet2003/raw.py
--rw-rw-rw-   0        0        0      367 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/src/tuzet2003/version.py
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.298460 tuzet2003-1.0.0/src/tuzet2003.egg-info/
--rw-rw-rw-   0        0        0     2287 2022-06-13 12:14:38.000000 tuzet2003-1.0.0/src/tuzet2003.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1368 2022-06-13 12:14:38.000000 tuzet2003-1.0.0/src/tuzet2003.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-13 12:14:38.000000 tuzet2003-1.0.0/src/tuzet2003.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-05 10:07:13.000000 tuzet2003-1.0.0/src/tuzet2003.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2022-06-13 12:14:38.000000 tuzet2003-1.0.0/src/tuzet2003.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-13 12:14:38.000000 tuzet2003-1.0.0/src/tuzet2003.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-13 12:14:39.318466 tuzet2003-1.0.0/test/
--rw-rw-rw-   0        0        0      973 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       84 2022-06-13 12:08:48.000000 tuzet2003-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.972125 tuzet2003-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3313 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3323 2024-05-29 13:42:28.971144 tuzet2003-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1476 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.921633 tuzet2003-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.936224 tuzet2003-1.1.0/doc/_gallery/
+-rw-rw-rw-   0        0        0     4105 2022-01-11 16:48:50.000000 tuzet2003-1.1.0/doc/_gallery/index.rst
+-rw-rw-rw-   0        0        0     1946 2022-01-11 16:48:48.000000 tuzet2003-1.1.0/doc/_gallery/plot_eq_a12.rst
+-rw-rw-rw-   0        0        0     2524 2022-01-11 16:48:47.000000 tuzet2003-1.1.0/doc/_gallery/plot_eq_b1.rst
+-rw-rw-rw-   0        0        0     2405 2022-01-11 16:48:49.000000 tuzet2003-1.1.0/doc/_gallery/plot_eq_b2.rst
+-rw-rw-rw-   0        0        0     2547 2022-01-11 16:48:49.000000 tuzet2003-1.1.0/doc/_gallery/plot_eq_b3.rst
+-rw-rw-rw-   0        0        0     2205 2022-01-11 16:48:50.000000 tuzet2003-1.1.0/doc/_gallery/plot_eq_b4.rst
+-rw-rw-rw-   0        0        0     2157 2022-01-11 16:48:46.000000 tuzet2003-1.1.0/doc/_gallery/plot_fig2.rst
+-rw-rw-rw-   0        0        0     4763 2022-01-11 16:50:41.000000 tuzet2003-1.1.0/doc/_gallery/plot_fig5.rst
+-rw-rw-rw-   0        0        0     2081 2022-01-11 16:48:47.000000 tuzet2003-1.1.0/doc/_gallery/plot_fig6a.rst
+-rw-rw-rw-   0        0        0     2820 2022-01-11 16:48:47.000000 tuzet2003-1.1.0/doc/_gallery/plot_net_photosynthesis.rst
+-rw-rw-rw-   0        0        0     2929 2022-01-11 16:48:49.000000 tuzet2003-1.1.0/doc/_gallery/plot_soil_water_relations.rst
+-rw-rw-rw-   0        0        0     2544 2022-01-11 16:50:42.000000 tuzet2003-1.1.0/doc/_gallery/sg_execution_times.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.937226 tuzet2003-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.938226 tuzet2003-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5093 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      593 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      219 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1404 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.940773 tuzet2003-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2331 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      359 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       36 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:42:28.972125 tuzet2003-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.888695 tuzet2003-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.951719 tuzet2003-1.1.0/src/tuzet2003/
+-rw-rw-rw-   0        0        0      254 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/src/tuzet2003/__init__.py
+-rw-rw-rw-   0        0        0    18136 2022-06-13 12:05:58.000000 tuzet2003-1.1.0/src/tuzet2003/appendix.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.965345 tuzet2003-1.1.0/src/tuzet2003/clean/
+-rw-rw-rw-   0        0        0     5609 2024-05-29 13:37:54.000000 tuzet2003-1.1.0/src/tuzet2003/clean/fig2.csv
+-rw-rw-rw-   0        0        0    16131 2024-05-29 13:37:58.000000 tuzet2003-1.1.0/src/tuzet2003/clean/fig5.csv
+-rw-rw-rw-   0        0        0      134 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/src/tuzet2003/clean/readme.rst
+-rw-rw-rw-   0        0        0      582 2024-05-29 13:38:01.000000 tuzet2003-1.1.0/src/tuzet2003/clean/table1.csv
+-rw-rw-rw-   0        0        0      324 2024-05-29 13:38:04.000000 tuzet2003-1.1.0/src/tuzet2003/clean/table2.csv
+-rw-rw-rw-   0        0        0      644 2024-05-29 13:38:06.000000 tuzet2003-1.1.0/src/tuzet2003/clean/table3.csv
+-rw-rw-rw-   0        0        0     4317 2022-01-19 14:47:55.000000 tuzet2003-1.1.0/src/tuzet2003/external.py
+-rw-rw-rw-   0        0        0      379 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/src/tuzet2003/info.py
+-rw-rw-rw-   0        0        0    10359 2022-01-31 16:51:40.000000 tuzet2003-1.1.0/src/tuzet2003/leaf.py
+-rw-rw-rw-   0        0        0     5133 2022-01-11 17:27:49.000000 tuzet2003-1.1.0/src/tuzet2003/raw.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/src/tuzet2003/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.969141 tuzet2003-1.1.0/src/tuzet2003.egg-info/
+-rw-rw-rw-   0        0        0     3323 2024-05-29 13:42:28.000000 tuzet2003-1.1.0/src/tuzet2003.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1316 2024-05-29 13:42:28.000000 tuzet2003-1.1.0/src/tuzet2003.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:42:28.000000 tuzet2003-1.1.0/src/tuzet2003.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-05-29 13:42:28.000000 tuzet2003-1.1.0/src/tuzet2003.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 13:42:28.000000 tuzet2003-1.1.0/src/tuzet2003.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:42:28.968382 tuzet2003-1.1.0/test/
+-rw-rw-rw-   0        0        0      985 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      377 2024-05-29 13:39:06.000000 tuzet2003-1.1.0/test/test_packaging.py
```

### Comparing `tuzet2003-1.0.0/CONTRIBUTING.rst` & `tuzet2003-1.1.0/CONTRIBUTING.rst`

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

### Comparing `tuzet2003-1.0.0/LICENSE` & `tuzet2003-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/README.rst` & `tuzet2003-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ========================
 tuzet2003
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/tuzet2003/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/tuzet2003/
-
 .. image:: https://b326.gitlab.io/tuzet2003/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/tuzet2003/1.0.0/
+    :target: https://pypi.org/project/tuzet2003/1.1.0/
 
 .. image:: https://b326.gitlab.io/tuzet2003/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/tuzet2003
 
+.. image:: https://b326.gitlab.io/tuzet2003/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/tuzet2003/
+
 .. image:: https://badge.fury.io/py/tuzet2003.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/tuzet2003
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/tuzet2003/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/tuzet2003/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/tuzet2003/badges/main/coverage.svg
```

### Comparing `tuzet2003-1.0.0/doc/Makefile` & `tuzet2003-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/index.rst` & `tuzet2003-1.1.0/doc/_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_eq_a12.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_eq_a12.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_eq_b1.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_eq_b1.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_eq_b2.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_eq_b2.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_eq_b3.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_eq_b3.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_eq_b4.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_eq_b4.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_fig2.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_fig2.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_fig5.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_fig5.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_fig6a.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_fig6a.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_net_photosynthesis.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_net_photosynthesis.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/plot_soil_water_relations.rst` & `tuzet2003-1.1.0/doc/_gallery/plot_soil_water_relations.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/_gallery/sg_execution_times.rst` & `tuzet2003-1.1.0/doc/_gallery/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/biblio/biblio.rst` & `tuzet2003-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/conf.py` & `tuzet2003-1.1.0/doc/conf.py`

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

### Comparing `tuzet2003-1.0.0/doc/index.rst` & `tuzet2003-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/make.bat` & `tuzet2003-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/doc/readme.rst` & `tuzet2003-1.1.0/doc/readme.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/tuzet2003/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/tuzet2003/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/tuzet2003/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/tuzet2003/1.0.0/
+    :target: https://pypi.org/project/tuzet2003/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/tuzet2003/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/tuzet2003
 
+
+.. image:: https://b326.gitlab.io/tuzet2003/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/tuzet2003/
+
+
 .. image:: https://badge.fury.io/py/tuzet2003.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/tuzet2003
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/tuzet2003/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/tuzet2003/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/tuzet2003/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/tuzet2003/commits/main
```

### Comparing `tuzet2003-1.0.0/src/tuzet2003/appendix.py` & `tuzet2003-1.1.0/src/tuzet2003/appendix.py`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/clean/fig2.csv` & `tuzet2003-1.1.0/src/tuzet2003/clean/fig2.csv`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/clean/fig5.csv` & `tuzet2003-1.1.0/src/tuzet2003/clean/fig5.csv`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/clean/table1.csv` & `tuzet2003-1.1.0/src/tuzet2003/clean/table1.csv`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/clean/table3.csv` & `tuzet2003-1.1.0/src/tuzet2003/clean/table3.csv`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/external.py` & `tuzet2003-1.1.0/src/tuzet2003/external.py`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/leaf.py` & `tuzet2003-1.1.0/src/tuzet2003/leaf.py`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003/raw.py` & `tuzet2003-1.1.0/src/tuzet2003/raw.py`

 * *Files identical despite different names*

### Comparing `tuzet2003-1.0.0/src/tuzet2003.egg-info/SOURCES.txt` & `tuzet2003-1.1.0/src/tuzet2003.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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
@@ -41,15 +39,14 @@
 src/tuzet2003/info.py
 src/tuzet2003/leaf.py
 src/tuzet2003/raw.py
 src/tuzet2003/version.py
 src/tuzet2003.egg-info/PKG-INFO
 src/tuzet2003.egg-info/SOURCES.txt
 src/tuzet2003.egg-info/dependency_links.txt
-src/tuzet2003.egg-info/not-zip-safe
 src/tuzet2003.egg-info/requires.txt
 src/tuzet2003.egg-info/top_level.txt
 src/tuzet2003/clean/fig2.csv
 src/tuzet2003/clean/fig5.csv
 src/tuzet2003/clean/readme.rst
 src/tuzet2003/clean/table1.csv
 src/tuzet2003/clean/table2.csv
```

### Comparing `tuzet2003-1.0.0/test/conftest.py` & `tuzet2003-1.1.0/test/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=tuzet2003")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=tuzet2003")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

