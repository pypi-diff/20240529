# Comparing `tmp/saxton2006-1.0.1.tar.gz` & `tmp/saxton2006-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saxton2006-1.0.1.tar", last modified: Mon Aug 16 09:37:41 2021, max compression
+gzip compressed data, was "saxton2006-1.1.0.tar", last modified: Wed May 29 13:31:17 2024, max compression
```

## Comparing `saxton2006-1.0.1.tar` & `saxton2006-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,49 @@
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.437863 saxton2006-1.0.1/
--rw-rw-rw-   0        0        0      352 2021-08-16 09:30:18.000000 saxton2006-1.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3332 2021-08-16 09:30:18.000000 saxton2006-1.0.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2021-08-16 09:30:18.000000 saxton2006-1.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2021-08-16 09:30:18.000000 saxton2006-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      438 2021-08-16 09:30:18.000000 saxton2006-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2746 2021-08-16 09:37:41.437863 saxton2006-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1529 2021-08-16 09:30:18.000000 saxton2006-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.373868 saxton2006-1.0.1/doc/
--rw-rw-rw-   0        0        0     6967 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/Makefile
--rw-rw-rw-   0        0        0       29 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.377863 saxton2006-1.0.1/doc/badges/
--rw-rw-rw-   0        0        0      227 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.377863 saxton2006-1.0.1/doc/biblio/
--rw-rw-rw-   0        0        0      513 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5104 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/conf.py
--rw-rw-rw-   0        0        0       34 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/history.rst
--rw-rw-rw-   0        0        0      512 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/index.rst
--rw-rw-rw-   0        0        0      165 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/make.bat
--rw-rw-rw-   0        0        0      128 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/management.rst
--rw-rw-rw-   0        0        0     1448 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.389870 saxton2006-1.0.1/doc/user/
--rw-rw-rw-   0        0        0       83 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2021-08-16 09:30:18.000000 saxton2006-1.0.1/doc/user/overview.rst
--rw-rw-rw-   0        0        0      338 2021-08-16 09:30:18.000000 saxton2006-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       29 2021-08-16 09:30:18.000000 saxton2006-1.0.1/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2021-08-16 09:37:41.437863 saxton2006-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1888 2021-08-16 09:30:18.000000 saxton2006-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.309862 saxton2006-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.401861 saxton2006-1.0.1/src/saxton2006/
--rw-rw-rw-   0        0        0      272 2021-08-16 09:30:18.000000 saxton2006-1.0.1/src/saxton2006/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.421865 saxton2006-1.0.1/src/saxton2006/clean/
--rw-rw-rw-   0        0        0      134 2021-08-16 09:30:18.000000 saxton2006-1.0.1/src/saxton2006/clean/readme.rst
--rw-rw-rw-   0        0        0      870 2021-08-09 09:09:04.000000 saxton2006-1.0.1/src/saxton2006/clean/table3.csv
--rw-rw-rw-   0        0        0      193 2021-08-16 09:30:18.000000 saxton2006-1.0.1/src/saxton2006/info.py
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.425861 saxton2006-1.0.1/src/saxton2006/raw/
--rw-rw-rw-   0        0        0      117 2021-08-16 09:30:18.000000 saxton2006-1.0.1/src/saxton2006/raw/readme.rst
--rw-rw-rw-   0        0        0      688 2021-08-09 08:46:55.000000 saxton2006-1.0.1/src/saxton2006/raw/table3.csv
--rw-rw-rw-   0        0        0     8731 2021-08-09 11:52:19.000000 saxton2006-1.0.1/src/saxton2006/table1.py
--rw-rw-rw-   0        0        0      367 2021-08-16 09:30:18.000000 saxton2006-1.0.1/src/saxton2006/version.py
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.413861 saxton2006-1.0.1/src/saxton2006.egg-info/
--rw-rw-rw-   0        0        0     2746 2021-08-16 09:37:40.000000 saxton2006-1.0.1/src/saxton2006.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      866 2021-08-16 09:37:41.000000 saxton2006-1.0.1/src/saxton2006.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-16 09:37:40.000000 saxton2006-1.0.1/src/saxton2006.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-08-09 07:28:08.000000 saxton2006-1.0.1/src/saxton2006.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2021-08-16 09:37:40.000000 saxton2006-1.0.1/src/saxton2006.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-08-16 09:37:41.433861 saxton2006-1.0.1/test/
--rw-rw-rw-   0        0        0      974 2021-08-16 09:30:18.000000 saxton2006-1.0.1/test/conftest.py
--rw-rw-rw-   0        0        0       86 2021-08-16 09:30:18.000000 saxton2006-1.0.1/test/test_packaging.py
--rw-rw-rw-   0        0        0     1085 2021-08-09 11:52:19.000000 saxton2006-1.0.1/test/test_table1.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.751266 saxton2006-1.1.0/
+-rw-rw-rw-   0        0        0      352 2024-05-29 13:27:53.000000 saxton2006-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3323 2024-05-29 13:27:53.000000 saxton2006-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 13:27:53.000000 saxton2006-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 13:27:53.000000 saxton2006-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2960 2024-05-29 13:31:17.749265 saxton2006-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-05-29 13:27:53.000000 saxton2006-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.728264 saxton2006-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.729265 saxton2006-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.730264 saxton2006-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5104 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1071 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.731264 saxton2006-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 13:27:53.000000 saxton2006-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2362 2024-05-29 13:27:53.000000 saxton2006-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      338 2024-05-29 13:27:53.000000 saxton2006-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 13:27:53.000000 saxton2006-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:31:17.751266 saxton2006-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.695609 saxton2006-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.736265 saxton2006-1.1.0/src/saxton2006/
+-rw-rw-rw-   0        0        0      255 2024-05-29 13:27:53.000000 saxton2006-1.1.0/src/saxton2006/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.744264 saxton2006-1.1.0/src/saxton2006/clean/
+-rw-rw-rw-   0        0        0      134 2024-05-29 13:27:53.000000 saxton2006-1.1.0/src/saxton2006/clean/readme.rst
+-rw-rw-rw-   0        0        0      870 2024-05-29 13:26:36.000000 saxton2006-1.1.0/src/saxton2006/clean/table3.csv
+-rw-rw-rw-   0        0        0      379 2024-05-29 13:27:53.000000 saxton2006-1.1.0/src/saxton2006/info.py
+-rw-rw-rw-   0        0        0     8731 2021-08-09 11:52:19.000000 saxton2006-1.1.0/src/saxton2006/table1.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 13:27:53.000000 saxton2006-1.1.0/src/saxton2006/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.747264 saxton2006-1.1.0/src/saxton2006.egg-info/
+-rw-rw-rw-   0        0        0     2960 2024-05-29 13:31:17.000000 saxton2006-1.1.0/src/saxton2006.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-05-29 13:31:17.000000 saxton2006-1.1.0/src/saxton2006.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:31:17.000000 saxton2006-1.1.0/src/saxton2006.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2024-05-29 13:31:17.000000 saxton2006-1.1.0/src/saxton2006.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 13:31:17.000000 saxton2006-1.1.0/src/saxton2006.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:31:17.746264 saxton2006-1.1.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-29 13:27:53.000000 saxton2006-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      381 2024-05-29 13:27:53.000000 saxton2006-1.1.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0     1085 2021-08-09 11:52:19.000000 saxton2006-1.1.0/test/test_table1.py
```

### Comparing `saxton2006-1.0.1/CONTRIBUTING.rst` & `saxton2006-1.1.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -102,24 +102,24 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.8.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
 
     $ pytest test/test_XXX
 
 
 
 
-.. _issues: https://gitlab.com/revesansparole/saxton2006/issues
+.. _issues: https://gitlab.com/b326/saxton2006/issues
 
 .. _virtualenv: https://pypi.python.org/pypi/virtualenv
```

### Comparing `saxton2006-1.0.1/LICENSE` & `saxton2006-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saxton2006-1.0.1/README.rst` & `saxton2006-1.1.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 ========================
 saxton2006
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/saxton2006/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/saxton2006/
-
 .. image:: https://b326.gitlab.io/saxton2006/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/saxton2006/1.0.1/
+    :target: https://pypi.org/project/saxton2006/1.1.0/
 
 .. image:: https://b326.gitlab.io/saxton2006/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/saxton2006
 
+.. image:: https://b326.gitlab.io/saxton2006/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/saxton2006/
+
 .. image:: https://badge.fury.io/py/saxton2006.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/saxton2006
 
 .. #}
-.. {# pkglts, glabpkg, after doc
-
-develop: |dvlp_build|_ |dvlp_coverage|_
-
-.. |dvlp_build| image:: https://gitlab.com/b326/saxton2006/badges/develop/pipeline.svg
-.. _dvlp_build: https://gitlab.com/b326/saxton2006/commits/develop
-
-.. |dvlp_coverage| image:: https://gitlab.com/b326/saxton2006/badges/develop/coverage.svg
-.. _dvlp_coverage: https://gitlab.com/b326/saxton2006/commits/develop
-
+.. {# pkglts, glabpkg_dev, after doc
 
-master: |master_build|_ |master_coverage|_
+main: |main_build|_ |main_coverage|_
 
-.. |master_build| image:: https://gitlab.com/b326/saxton2006/badges/master/pipeline.svg
-.. _master_build: https://gitlab.com/b326/saxton2006/commits/master
+.. |main_build| image:: https://gitlab.com/b326/saxton2006/badges/main/pipeline.svg
+.. _main_build: https://gitlab.com/b326/saxton2006/commits/main
 
-.. |master_coverage| image:: https://gitlab.com/b326/saxton2006/badges/master/coverage.svg
-.. _master_coverage: https://gitlab.com/b326/saxton2006/commits/master
+.. |main_coverage| image:: https://gitlab.com/b326/saxton2006/badges/main/coverage.svg
+.. _main_coverage: https://gitlab.com/b326/saxton2006/commits/main
 .. #}
 
 Formalisms published in Saxton and Rawls (2006)
```

### Comparing `saxton2006-1.0.1/doc/Makefile` & `saxton2006-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `saxton2006-1.0.1/doc/biblio/biblio.rst` & `saxton2006-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `saxton2006-1.0.1/doc/conf.py` & `saxton2006-1.1.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.0.1"
+version = "1.1.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.1"
+release = "1.1.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `saxton2006-1.0.1/doc/index.rst` & `saxton2006-1.1.0/doc/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Welcome to saxton2006's documentation!
 ====================================================
 
 .. toctree::
-   :caption: Contents
-   :maxdepth: 2
+    :caption: Contents
+    :maxdepth: 2
 
-   readme
-   installation
-   usage
-   management
+    readme
+    installation
+    usage
 
 .. toctree::
-   :caption: User's documentation
-   :maxdepth: 2
+    :caption: User's documentation
+    :maxdepth: 2
 
-   user/index
-   _gallery/index
+    user/index
+    _gallery/index
 
 .. toctree::
-   :caption: Developer's documentation
-   :maxdepth: 4
+    :caption: Developer's documentation
+    :maxdepth: 4
 
-   Sources <_dvlpt/modules>
+    Sources <_dvlpt/modules>
 
-Indices and tables
-==================
+.. toctree::
+    :caption: Annexe
+    :maxdepth: 2
+
+    gitlab home <https://gitlab.com/b326/saxton2006>
+    management
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `saxton2006-1.0.1/doc/make.bat` & `saxton2006-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `saxton2006-1.0.1/doc/readme.rst` & `saxton2006-1.1.0/doc/readme.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/saxton2006/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/saxton2006/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/saxton2006/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/saxton2006/1.0.1/
+    :target: https://pypi.org/project/saxton2006/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/saxton2006/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/saxton2006
 
-.. image:: https://badge.fury.io/py/saxton2006.svg
-    :alt: PyPI version
-    :target: https://badge.fury.io/py/saxton2006
 
+.. image:: https://b326.gitlab.io/saxton2006/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/saxton2006/
 
-develop: |dvlp_build|_ |dvlp_coverage|_
 
-.. |dvlp_build| image:: https://gitlab.com/b326/saxton2006/badges/develop/pipeline.svg
-.. _dvlp_build: https://gitlab.com/b326/saxton2006/commits/develop
+.. image:: https://badge.fury.io/py/saxton2006.svg
+    :alt: PyPI version
+    :target: https://badge.fury.io/py/saxton2006
 
-.. |dvlp_coverage| image:: https://gitlab.com/b326/saxton2006/badges/develop/coverage.svg
-.. _dvlp_coverage: https://gitlab.com/b326/saxton2006/commits/develop
 
 
-master: |master_build|_ |master_coverage|_
 
-.. |master_build| image:: https://gitlab.com/b326/saxton2006/badges/master/pipeline.svg
-.. _master_build: https://gitlab.com/b326/saxton2006/commits/master
+main: |main_build|_ |main_coverage|_
 
-.. |master_coverage| image:: https://gitlab.com/b326/saxton2006/badges/master/coverage.svg
-.. _master_coverage: https://gitlab.com/b326/saxton2006/commits/master
+.. |main_build| image:: https://gitlab.com/b326/saxton2006/badges/main/pipeline.svg
+.. _main_build: https://gitlab.com/b326/saxton2006/commits/main
 
+.. |main_coverage| image:: https://gitlab.com/b326/saxton2006/badges/main/coverage.svg
+.. _main_coverage: https://gitlab.com/b326/saxton2006/commits/main
 .. #}
 
 Formalisms published in Saxton and Rawls (2006)
```

### Comparing `saxton2006-1.0.1/setup.py` & `saxton2006-1.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,94 @@
-# {# pkglts, pysetup.kwds
-# format setup arguments
-from pathlib import Path
-from setuptools import setup, find_packages
-
-short_descr = "Formalisms published in Saxton and Rawls (2006)"
-readme = open('README.rst').read()
-history = open('HISTORY.rst').read()
-
-# find packages
-pkgs = find_packages('src')
-
-src_dir = Path("src/saxton2006")
-
-data_files = []
-for pth in src_dir.rglob("*"):
-    if not pth.is_dir() and "__pycache__" not in pth.parts:
-        if pth.suffix in ['.json', '.ini', '.csv', '.rst', '.svg']:
-            data_files.append(str(pth.relative_to(src_dir)))
-
-pkg_data = {'saxton2006': data_files}
-
-setup_kwds = dict(
-    name='saxton2006',
-    version="1.0.1",
-    description=short_descr,
-    long_description=readme + '\n\n' + history,
-    author="revesansparole",
-    author_email="revesansparole@gmail.com",
-    url='https://gitlab.com/b326/saxton2006',
-    license='cc_by_nc',
-    zip_safe=False,
-
-    packages=pkgs,
-    
-    package_dir={'': 'src'},
-    
-    
-    package_data=pkg_data,
-    setup_requires=[
-        "pytest-runner",
-        ],
-    install_requires=[
-        ],
-    tests_require=[
-        "coverage",
-        "pandas",
-        "pytest",
-        "pytest-cov",
-        "pytest-mock",
-        ],
-    entry_points={},
-    keywords='',
-    
-    classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Natural Language :: English",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
-    ],
-    )
+# {# pkglts, pyproject.build
+[build-system]
+# Minimum requirements for the build system to execute.
+requires = ["setuptools", "wheel"]  # , "setuptools-scm"]  # PEP 508 specifications.
+build-backend = "setuptools.build_meta"  # we don't know if we need it
 # #}
-# change setup_kwds below before the next pkglts tag
 
-# do not change things below
-# {# pkglts, pysetup.call
-setup(**setup_kwds)
+# {# pkglts, pyproject.project
+[project]  # https://packaging.python.org/en/latest/specifications/pyproject-toml/
+name = "saxton2006"
+version = "1.1.0"
+description = "Formalisms published in Saxton and Rawls (2006)"
+readme = "README.rst"
+requires-python = ">= 3.8"
+license = {text = "cc_by_nc"}
+authors = [
+    {name = "revesansparole", email = "revesansparole@gmail.com"},
+]
+maintainers = [
+    {name = "revesansparole", email = "revesansparole@gmail.com"},
+    {name = "Jerome Chopard", email = "revesansparole@gmail.com"},
+    {name = "jchopard", email = "jerome.chopard@itk.fr"},
+]
+keywords = [
+]
+classifiers = [
+    "Development Status :: 2 - Pre-Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
+    "Natural Language :: English",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.8",
+]
+dependencies = [
+]
+
+[project.optional-dependencies]
+doc = [
+    "sphinx",
+    "sphinx-gallery",
+    "sphinx_rtd_theme",
+]
+dvlpt = [
+    "twine",
+]
+example = [
+    "matplotlib",
+    "numpy",
+]
+script = [
+    "pandas",
+]
+test = [
+    "coverage",
+    "pandas",
+    "pytest",
+    "pytest-cov",
+    "pytest-mock",
+]
+
+
+[project.urls]
+repository = "https://gitlab.com/b326/saxton2006"
+pip = "https://pypi.org/project/saxton2006/1.1.0/"
+conda = "https://anaconda.org/revesansparole/saxton2006"
+doc = "https://b326.gitlab.io/saxton2006/"
+pypi = "https://badge.fury.io/py/saxton2006"
+
+
+[tool.setuptools]
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ['*.json', '*.ini', '*.csv', '*.rst', '*.svg', ]
+
+# #}
+# {# pkglts, test, after pyproject.project
+[tool.pytest.ini_options]
+addopts = "--maxfail=2 -rf --cov=saxton2006"
+# #}
+
+# {# pkglts, pyproject.scripts
+[project.scripts]
+# #}
+
+# {# pkglts, pyproject.gui_scripts
+[project.gui-scripts]
 # #}
```

### Comparing `saxton2006-1.0.1/src/saxton2006/clean/table3.csv` & `saxton2006-1.1.0/src/saxton2006/clean/table3.csv`

 * *Files identical despite different names*

### Comparing `saxton2006-1.0.1/src/saxton2006/table1.py` & `saxton2006-1.1.0/src/saxton2006/table1.py`

 * *Files identical despite different names*

### Comparing `saxton2006-1.0.1/src/saxton2006.egg-info/SOURCES.txt` & `saxton2006-1.1.0/src/saxton2006.egg-info/SOURCES.txt`

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
@@ -26,16 +24,14 @@
 src/saxton2006/__init__.py
 src/saxton2006/info.py
 src/saxton2006/table1.py
 src/saxton2006/version.py
 src/saxton2006.egg-info/PKG-INFO
 src/saxton2006.egg-info/SOURCES.txt
 src/saxton2006.egg-info/dependency_links.txt
-src/saxton2006.egg-info/not-zip-safe
+src/saxton2006.egg-info/requires.txt
 src/saxton2006.egg-info/top_level.txt
 src/saxton2006/clean/readme.rst
 src/saxton2006/clean/table3.csv
-src/saxton2006/raw/readme.rst
-src/saxton2006/raw/table3.csv
 test/conftest.py
 test/test_packaging.py
 test/test_table1.py
```

### Comparing `saxton2006-1.0.1/test/conftest.py` & `saxton2006-1.1.0/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=saxton2006")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=saxton2006")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `saxton2006-1.0.1/test/test_table1.py` & `saxton2006-1.1.0/test/test_table1.py`

 * *Files identical despite different names*

