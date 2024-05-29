# Comparing `tmp/garcia2009-1.1.0.tar.gz` & `tmp/garcia2009-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garcia2009-1.1.0.tar", last modified: Mon Sep 26 08:20:28 2022, max compression
+gzip compressed data, was "garcia2009-1.2.0.tar", last modified: Wed May 29 08:24:07 2024, max compression
```

## Comparing `garcia2009-1.1.0.tar` & `garcia2009-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.960065 garcia2009-1.1.0/
--rw-rw-rw-   0        0        0      316 2022-09-26 08:16:02.000000 garcia2009-1.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3322 2022-09-26 08:16:02.000000 garcia2009-1.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-09-26 08:16:02.000000 garcia2009-1.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-09-26 08:16:02.000000 garcia2009-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      438 2022-09-26 08:16:02.000000 garcia2009-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2358 2022-09-26 08:20:28.960065 garcia2009-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2022-09-26 08:16:02.000000 garcia2009-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.892033 garcia2009-1.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.896028 garcia2009-1.1.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.900029 garcia2009-1.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5127 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      595 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      165 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1432 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.904026 garcia2009-1.1.0/doc/user/
--rw-rw-rw-   0        0        0       86 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-09-26 08:16:02.000000 garcia2009-1.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      311 2022-09-26 08:16:02.000000 garcia2009-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-09-26 08:16:02.000000 garcia2009-1.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-09-26 08:20:28.964035 garcia2009-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1892 2022-09-26 08:16:02.000000 garcia2009-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.828320 garcia2009-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.920027 garcia2009-1.1.0/src/garcia2009/
--rw-rw-rw-   0        0        0      286 2022-09-26 08:16:02.000000 garcia2009-1.1.0/src/garcia2009/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.952030 garcia2009-1.1.0/src/garcia2009/clean/
--rw-rw-rw-   0        0        0      134 2022-09-26 08:16:02.000000 garcia2009-1.1.0/src/garcia2009/clean/readme.rst
--rw-rw-rw-   0        0        0      288 2022-05-19 08:46:42.000000 garcia2009-1.1.0/src/garcia2009/clean/table5.csv
--rw-rw-rw-   0        0        0      725 2022-05-19 08:46:45.000000 garcia2009-1.1.0/src/garcia2009/clean/table8.csv
--rw-rw-rw-   0        0        0     1645 2022-04-25 10:05:24.000000 garcia2009-1.1.0/src/garcia2009/formalism.py
--rw-rw-rw-   0        0        0      152 2022-09-26 08:16:02.000000 garcia2009-1.1.0/src/garcia2009/info.py
--rw-rw-rw-   0        0        0      822 2022-09-26 08:10:21.000000 garcia2009-1.1.0/src/garcia2009/params.py
--rw-rw-rw-   0        0        0      367 2022-09-26 08:16:02.000000 garcia2009-1.1.0/src/garcia2009/version.py
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.944030 garcia2009-1.1.0/src/garcia2009.egg-info/
--rw-rw-rw-   0        0        0     2358 2022-09-26 08:20:28.000000 garcia2009-1.1.0/src/garcia2009.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      846 2022-09-26 08:20:28.000000 garcia2009-1.1.0/src/garcia2009.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-26 08:20:28.000000 garcia2009-1.1.0/src/garcia2009.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-19 08:45:53.000000 garcia2009-1.1.0/src/garcia2009.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2022-09-26 08:20:28.000000 garcia2009-1.1.0/src/garcia2009.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-26 08:20:28.956028 garcia2009-1.1.0/test/
--rw-rw-rw-   0        0        0      974 2022-09-26 08:16:02.000000 garcia2009-1.1.0/test/conftest.py
--rw-rw-rw-   0        0        0       86 2022-09-26 08:16:02.000000 garcia2009-1.1.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.919345 garcia2009-1.2.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 08:19:13.000000 garcia2009-1.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3323 2024-05-29 08:19:13.000000 garcia2009-1.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 08:19:13.000000 garcia2009-1.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 08:19:13.000000 garcia2009-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3165 2024-05-29 08:24:07.917346 garcia2009-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1517 2024-05-29 08:19:13.000000 garcia2009-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.892340 garcia2009-1.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.893341 garcia2009-1.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.894341 garcia2009-1.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5127 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1444 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.896341 garcia2009-1.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 08:19:13.000000 garcia2009-1.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2235 2024-05-29 08:19:13.000000 garcia2009-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      311 2024-05-29 08:19:13.000000 garcia2009-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:19:13.000000 garcia2009-1.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:24:07.919345 garcia2009-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.853811 garcia2009-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.902341 garcia2009-1.2.0/src/garcia2009/
+-rw-rw-rw-   0        0        0      278 2024-05-29 08:19:13.000000 garcia2009-1.2.0/src/garcia2009/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.912341 garcia2009-1.2.0/src/garcia2009/clean/
+-rw-rw-rw-   0        0        0      134 2024-05-29 08:19:13.000000 garcia2009-1.2.0/src/garcia2009/clean/readme.rst
+-rw-rw-rw-   0        0        0      288 2024-05-29 08:18:23.000000 garcia2009-1.2.0/src/garcia2009/clean/table5.csv
+-rw-rw-rw-   0        0        0      725 2024-05-29 08:18:26.000000 garcia2009-1.2.0/src/garcia2009/clean/table8.csv
+-rw-rw-rw-   0        0        0     1645 2022-04-25 10:05:24.000000 garcia2009-1.2.0/src/garcia2009/formalism.py
+-rw-rw-rw-   0        0        0      379 2024-05-29 08:19:13.000000 garcia2009-1.2.0/src/garcia2009/info.py
+-rw-rw-rw-   0        0        0      822 2022-09-26 08:10:21.000000 garcia2009-1.2.0/src/garcia2009/params.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 08:19:13.000000 garcia2009-1.2.0/src/garcia2009/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.915341 garcia2009-1.2.0/src/garcia2009.egg-info/
+-rw-rw-rw-   0        0        0     3165 2024-05-29 08:24:07.000000 garcia2009-1.2.0/src/garcia2009.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2024-05-29 08:24:07.000000 garcia2009-1.2.0/src/garcia2009.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:24:07.000000 garcia2009-1.2.0/src/garcia2009.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-29 08:24:07.000000 garcia2009-1.2.0/src/garcia2009.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 08:24:07.000000 garcia2009-1.2.0/src/garcia2009.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 08:24:07.914341 garcia2009-1.2.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-29 08:19:13.000000 garcia2009-1.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0      381 2024-05-29 08:19:13.000000 garcia2009-1.2.0/test/test_packaging.py
```

### Comparing `garcia2009-1.1.0/CONTRIBUTING.rst` & `garcia2009-1.2.0/CONTRIBUTING.rst`

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

### Comparing `garcia2009-1.1.0/LICENSE` & `garcia2009-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/README.rst` & `garcia2009-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ========================
 garcia2009
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/garcia2009/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/garcia2009/
-
 .. image:: https://b326.gitlab.io/garcia2009/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/garcia2009/1.1.0/
+    :target: https://pypi.org/project/garcia2009/1.2.0/
 
 .. image:: https://b326.gitlab.io/garcia2009/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/garcia2009
 
+.. image:: https://b326.gitlab.io/garcia2009/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/garcia2009/
+
 .. image:: https://badge.fury.io/py/garcia2009.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/garcia2009
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/garcia2009/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/garcia2009/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/garcia2009/badges/main/coverage.svg
```

### Comparing `garcia2009-1.1.0/doc/Makefile` & `garcia2009-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/doc/biblio/biblio.rst` & `garcia2009-1.2.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/doc/conf.py` & `garcia2009-1.2.0/doc/conf.py`

 * *Files 1% similar despite different names*

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

### Comparing `garcia2009-1.1.0/doc/index.rst` & `garcia2009-1.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/doc/make.bat` & `garcia2009-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/doc/readme.rst` & `garcia2009-1.2.0/doc/readme.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/garcia2009/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/garcia2009/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/garcia2009/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/garcia2009/1.1.0/
+    :target: https://pypi.org/project/garcia2009/1.2.0/
+
 
 .. image:: https://b326.gitlab.io/garcia2009/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/garcia2009
 
+
+.. image:: https://b326.gitlab.io/garcia2009/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/garcia2009/
+
+
 .. image:: https://badge.fury.io/py/garcia2009.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/garcia2009
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/garcia2009/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/garcia2009/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/garcia2009/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/garcia2009/commits/main
```

### Comparing `garcia2009-1.1.0/src/garcia2009/clean/table8.csv` & `garcia2009-1.2.0/src/garcia2009/clean/table8.csv`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/src/garcia2009/formalism.py` & `garcia2009-1.2.0/src/garcia2009/formalism.py`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/src/garcia2009/params.py` & `garcia2009-1.2.0/src/garcia2009/params.py`

 * *Files identical despite different names*

### Comparing `garcia2009-1.1.0/src/garcia2009.egg-info/SOURCES.txt` & `garcia2009-1.2.0/src/garcia2009.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

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
@@ -27,14 +25,14 @@
 src/garcia2009/formalism.py
 src/garcia2009/info.py
 src/garcia2009/params.py
 src/garcia2009/version.py
 src/garcia2009.egg-info/PKG-INFO
 src/garcia2009.egg-info/SOURCES.txt
 src/garcia2009.egg-info/dependency_links.txt
-src/garcia2009.egg-info/not-zip-safe
+src/garcia2009.egg-info/requires.txt
 src/garcia2009.egg-info/top_level.txt
 src/garcia2009/clean/readme.rst
 src/garcia2009/clean/table5.csv
 src/garcia2009/clean/table8.csv
 test/conftest.py
 test/test_packaging.py
```

### Comparing `garcia2009-1.1.0/test/conftest.py` & `garcia2009-1.2.0/test/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=garcia2009")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=garcia2009")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

