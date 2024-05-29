# Comparing `tmp/intrieri1997-1.0.0.tar.gz` & `tmp/intrieri1997-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intrieri1997-1.0.0.tar", last modified: Thu Apr  7 13:34:45 2022, max compression
+gzip compressed data, was "intrieri1997-1.1.0.tar", last modified: Wed May 29 09:21:30 2024, max compression
```

## Comparing `intrieri1997-1.0.0.tar` & `intrieri1997-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.119244 intrieri1997-1.0.0/
--rw-rw-rw-   0        0        0      316 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3342 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      440 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2358 2022-04-07 13:34:45.119244 intrieri1997-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.032709 intrieri1997-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.036714 intrieri1997-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.036714 intrieri1997-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5130 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      599 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      167 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1447 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.044713 intrieri1997-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       86 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      352 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-04-07 13:34:45.123244 intrieri1997-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1883 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:44.980708 intrieri1997-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.063242 intrieri1997-1.0.0/src/intrieri1997/
--rw-rw-rw-   0        0        0      269 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/src/intrieri1997/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.111244 intrieri1997-1.0.0/src/intrieri1997/clean/
--rw-rw-rw-   0        0        0      254 2022-04-07 13:17:11.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig10a.csv
--rw-rw-rw-   0        0        0      318 2022-04-07 13:17:11.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig10b.csv
--rw-rw-rw-   0        0        0     1398 2022-04-06 13:42:13.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig3.csv
--rw-rw-rw-   0        0        0    12980 2022-04-07 07:27:50.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig4.csv
--rw-rw-rw-   0        0        0     8991 2022-04-07 07:55:02.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig5.csv
--rw-rw-rw-   0        0        0      561 2022-04-07 08:14:41.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig6.csv
--rw-rw-rw-   0        0        0      796 2022-04-07 10:06:54.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig7.csv
--rw-rw-rw-   0        0        0      710 2022-04-07 11:39:40.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig8.csv
--rw-rw-rw-   0        0        0      497 2022-04-07 12:30:24.000000 intrieri1997-1.0.0/src/intrieri1997/clean/fig9.csv
--rw-rw-rw-   0        0        0      916 2022-04-07 12:52:20.000000 intrieri1997-1.0.0/src/intrieri1997/clean/info.json
--rw-rw-rw-   0        0        0      134 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/src/intrieri1997/clean/readme.rst
--rw-rw-rw-   0        0        0      597 2022-04-07 11:20:23.000000 intrieri1997-1.0.0/src/intrieri1997/clean/table1.csv
--rw-rw-rw-   0        0        0     1107 2022-04-07 12:49:48.000000 intrieri1997-1.0.0/src/intrieri1997/clean/table2.csv
--rw-rw-rw-   0        0        0      223 2022-04-07 13:21:04.000000 intrieri1997-1.0.0/src/intrieri1997/fig10.py
--rw-rw-rw-   0        0        0      342 2022-04-07 08:17:07.000000 intrieri1997-1.0.0/src/intrieri1997/fig3.py
--rw-rw-rw-   0        0        0      208 2022-04-07 08:26:13.000000 intrieri1997-1.0.0/src/intrieri1997/fig6.py
--rw-rw-rw-   0        0        0      100 2022-04-07 10:08:18.000000 intrieri1997-1.0.0/src/intrieri1997/fig7.py
--rw-rw-rw-   0        0        0      121 2022-04-07 11:42:21.000000 intrieri1997-1.0.0/src/intrieri1997/fig8.py
--rw-rw-rw-   0        0        0       89 2022-04-07 12:25:04.000000 intrieri1997-1.0.0/src/intrieri1997/fig9.py
--rw-rw-rw-   0        0        0      152 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/src/intrieri1997/info.py
--rw-rw-rw-   0        0        0      367 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/src/intrieri1997/version.py
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.083263 intrieri1997-1.0.0/src/intrieri1997.egg-info/
--rw-rw-rw-   0        0        0     2358 2022-04-07 13:34:44.000000 intrieri1997-1.0.0/src/intrieri1997.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1291 2022-04-07 13:34:44.000000 intrieri1997-1.0.0/src/intrieri1997.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-07 13:34:44.000000 intrieri1997-1.0.0/src/intrieri1997.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-04-06 13:41:56.000000 intrieri1997-1.0.0/src/intrieri1997.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2022-04-07 13:34:44.000000 intrieri1997-1.0.0/src/intrieri1997.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-07 13:34:45.115243 intrieri1997-1.0.0/test/
--rw-rw-rw-   0        0        0      976 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       90 2022-04-07 13:27:01.000000 intrieri1997-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.645765 intrieri1997-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3349 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3384 2024-05-29 09:21:30.644608 intrieri1997-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1534 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.603893 intrieri1997-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.604918 intrieri1997-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.605893 intrieri1997-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5130 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      599 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      222 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1459 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.607894 intrieri1997-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2344 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      352 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:21:30.645765 intrieri1997-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.572856 intrieri1997-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.617895 intrieri1997-1.1.0/src/intrieri1997/
+-rw-rw-rw-   0        0        0      261 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/src/intrieri1997/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.639610 intrieri1997-1.1.0/src/intrieri1997/clean/
+-rw-rw-rw-   0        0        0      254 2024-05-29 09:16:46.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig10a.csv
+-rw-rw-rw-   0        0        0      318 2024-05-29 09:16:46.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig10b.csv
+-rw-rw-rw-   0        0        0     1398 2024-05-29 09:16:50.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig3.csv
+-rw-rw-rw-   0        0        0    12980 2024-05-29 09:16:55.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig4.csv
+-rw-rw-rw-   0        0        0     8991 2024-05-29 09:17:02.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig5.csv
+-rw-rw-rw-   0        0        0      561 2024-05-29 09:17:06.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig6.csv
+-rw-rw-rw-   0        0        0      796 2024-05-29 09:17:10.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig7.csv
+-rw-rw-rw-   0        0        0      710 2024-05-29 09:17:56.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig8.csv
+-rw-rw-rw-   0        0        0      497 2024-05-29 09:17:18.000000 intrieri1997-1.1.0/src/intrieri1997/clean/fig9.csv
+-rw-rw-rw-   0        0        0      916 2024-05-29 09:17:21.000000 intrieri1997-1.1.0/src/intrieri1997/clean/info.json
+-rw-rw-rw-   0        0        0      134 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/src/intrieri1997/clean/readme.rst
+-rw-rw-rw-   0        0        0      597 2024-05-29 09:17:26.000000 intrieri1997-1.1.0/src/intrieri1997/clean/table1.csv
+-rw-rw-rw-   0        0        0     1107 2024-05-29 09:17:29.000000 intrieri1997-1.1.0/src/intrieri1997/clean/table2.csv
+-rw-rw-rw-   0        0        0      223 2022-04-07 13:21:04.000000 intrieri1997-1.1.0/src/intrieri1997/fig10.py
+-rw-rw-rw-   0        0        0      342 2022-04-07 08:17:07.000000 intrieri1997-1.1.0/src/intrieri1997/fig3.py
+-rw-rw-rw-   0        0        0      208 2022-04-07 08:26:13.000000 intrieri1997-1.1.0/src/intrieri1997/fig6.py
+-rw-rw-rw-   0        0        0      100 2022-04-07 10:08:18.000000 intrieri1997-1.1.0/src/intrieri1997/fig7.py
+-rw-rw-rw-   0        0        0      121 2022-04-07 11:42:21.000000 intrieri1997-1.1.0/src/intrieri1997/fig8.py
+-rw-rw-rw-   0        0        0       89 2022-04-07 12:25:04.000000 intrieri1997-1.1.0/src/intrieri1997/fig9.py
+-rw-rw-rw-   0        0        0      379 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/src/intrieri1997/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/src/intrieri1997/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.642608 intrieri1997-1.1.0/src/intrieri1997.egg-info/
+-rw-rw-rw-   0        0        0     3384 2024-05-29 09:21:30.000000 intrieri1997-1.1.0/src/intrieri1997.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1275 2024-05-29 09:21:30.000000 intrieri1997-1.1.0/src/intrieri1997.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:21:30.000000 intrieri1997-1.1.0/src/intrieri1997.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-29 09:21:30.000000 intrieri1997-1.1.0/src/intrieri1997.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 09:21:30.000000 intrieri1997-1.1.0/src/intrieri1997.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:30.640608 intrieri1997-1.1.0/test/
+-rw-rw-rw-   0        0        0      988 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      389 2024-05-29 09:18:31.000000 intrieri1997-1.1.0/test/test_packaging.py
```

### Comparing `intrieri1997-1.0.0/CONTRIBUTING.rst` & `intrieri1997-1.1.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.11, 3.9.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `intrieri1997-1.0.0/LICENSE` & `intrieri1997-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/README.rst` & `intrieri1997-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ========================
 intrieri1997
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/intrieri1997/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/intrieri1997/
-
 .. image:: https://b326.gitlab.io/intrieri1997/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/intrieri1997/1.0.0/
+    :target: https://pypi.org/project/intrieri1997/1.1.0/
 
 .. image:: https://b326.gitlab.io/intrieri1997/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/intrieri1997
 
+.. image:: https://b326.gitlab.io/intrieri1997/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/intrieri1997/
+
 .. image:: https://badge.fury.io/py/intrieri1997.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/intrieri1997
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/intrieri1997/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/intrieri1997/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/intrieri1997/badges/main/coverage.svg
```

### Comparing `intrieri1997-1.0.0/doc/Makefile` & `intrieri1997-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/doc/biblio/biblio.rst` & `intrieri1997-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/doc/conf.py` & `intrieri1997-1.1.0/doc/conf.py`

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

### Comparing `intrieri1997-1.0.0/doc/index.rst` & `intrieri1997-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/doc/make.bat` & `intrieri1997-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/doc/readme.rst` & `intrieri1997-1.1.0/doc/readme.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/intrieri1997/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/intrieri1997/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/intrieri1997/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/intrieri1997/1.0.0/
+    :target: https://pypi.org/project/intrieri1997/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/intrieri1997/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/intrieri1997
 
+
+.. image:: https://b326.gitlab.io/intrieri1997/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/intrieri1997/
+
+
 .. image:: https://badge.fury.io/py/intrieri1997.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/intrieri1997
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/intrieri1997/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/intrieri1997/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/intrieri1997/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/intrieri1997/commits/main
```

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/fig3.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/fig3.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/fig4.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/fig4.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/fig5.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/fig5.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/fig6.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/fig6.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/fig7.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/fig7.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/fig8.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/fig8.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/info.json` & `intrieri1997-1.1.0/src/intrieri1997/clean/info.json`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/table1.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/table1.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997/clean/table2.csv` & `intrieri1997-1.1.0/src/intrieri1997/clean/table2.csv`

 * *Files identical despite different names*

### Comparing `intrieri1997-1.0.0/src/intrieri1997.egg-info/SOURCES.txt` & `intrieri1997-1.1.0/src/intrieri1997.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
 src/intrieri1997/fig8.py
 src/intrieri1997/fig9.py
 src/intrieri1997/info.py
 src/intrieri1997/version.py
 src/intrieri1997.egg-info/PKG-INFO
 src/intrieri1997.egg-info/SOURCES.txt
 src/intrieri1997.egg-info/dependency_links.txt
-src/intrieri1997.egg-info/not-zip-safe
+src/intrieri1997.egg-info/requires.txt
 src/intrieri1997.egg-info/top_level.txt
 src/intrieri1997/clean/fig10a.csv
 src/intrieri1997/clean/fig10b.csv
 src/intrieri1997/clean/fig3.csv
 src/intrieri1997/clean/fig4.csv
 src/intrieri1997/clean/fig5.csv
 src/intrieri1997/clean/fig6.csv
```

### Comparing `intrieri1997-1.0.0/test/conftest.py` & `intrieri1997-1.1.0/test/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=intrieri1997")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=intrieri1997")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

