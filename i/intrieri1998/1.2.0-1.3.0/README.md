# Comparing `tmp/intrieri1998-1.2.0.tar.gz` & `tmp/intrieri1998-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intrieri1998-1.2.0.tar", last modified: Tue Apr  5 16:46:00 2022, max compression
+gzip compressed data, was "intrieri1998-1.3.0.tar", last modified: Wed May 29 09:35:25 2024, max compression
```

## Comparing `intrieri1998-1.2.0.tar` & `intrieri1998-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.641525 intrieri1998-1.2.0/
--rw-rw-rw-   0        0        0      316 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3342 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      440 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1988 2022-04-05 16:46:00.645521 intrieri1998-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1166 2022-04-05 16:41:11.000000 intrieri1998-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.544485 intrieri1998-1.2.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.548518 intrieri1998-1.2.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.552502 intrieri1998-1.2.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5124 2022-04-05 16:41:11.000000 intrieri1998-1.2.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/history.rst
--rw-rw-rw-   0        0        0      599 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/index.rst
--rw-rw-rw-   0        0        0      167 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/management.rst
--rw-rw-rw-   0        0        0     1083 2022-04-05 16:41:11.000000 intrieri1998-1.2.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.560493 intrieri1998-1.2.0/doc/user/
--rw-rw-rw-   0        0        0       83 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      352 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-04-05 16:46:00.645521 intrieri1998-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1877 2022-04-05 16:41:11.000000 intrieri1998-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.441455 intrieri1998-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.580483 intrieri1998-1.2.0/src/intrieri1998/
--rw-rw-rw-   0        0        0      263 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/src/intrieri1998/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.633605 intrieri1998-1.2.0/src/intrieri1998/clean/
--rw-rw-rw-   0        0        0     6537 2022-03-31 07:25:31.000000 intrieri1998-1.2.0/src/intrieri1998/clean/fig3.csv
--rw-rw-rw-   0        0        0     4984 2022-03-31 09:20:08.000000 intrieri1998-1.2.0/src/intrieri1998/clean/fig4.csv
--rw-rw-rw-   0        0        0     2570 2022-03-31 08:25:07.000000 intrieri1998-1.2.0/src/intrieri1998/clean/fig5.csv
--rw-rw-rw-   0        0        0      525 2022-04-05 16:41:11.000000 intrieri1998-1.2.0/src/intrieri1998/clean/fig6.csv
--rw-rw-rw-   0        0        0     3694 2022-03-31 09:33:04.000000 intrieri1998-1.2.0/src/intrieri1998/clean/fig7.csv
--rw-rw-rw-   0        0        0     1238 2022-03-31 09:44:24.000000 intrieri1998-1.2.0/src/intrieri1998/clean/fig8.csv
--rw-rw-rw-   0        0        0      916 2022-04-04 15:20:41.000000 intrieri1998-1.2.0/src/intrieri1998/clean/info.json
--rw-rw-rw-   0        0        0      134 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/src/intrieri1998/clean/readme.rst
--rw-rw-rw-   0        0        0      527 2022-03-31 10:09:10.000000 intrieri1998-1.2.0/src/intrieri1998/clean/table.csv
--rw-rw-rw-   0        0        0      174 2022-03-31 08:39:49.000000 intrieri1998-1.2.0/src/intrieri1998/fig5.py
--rw-rw-rw-   0        0        0       85 2022-03-31 08:51:31.000000 intrieri1998-1.2.0/src/intrieri1998/fig6.py
--rw-rw-rw-   0        0        0      134 2022-03-31 09:58:10.000000 intrieri1998-1.2.0/src/intrieri1998/fig8.py
--rw-rw-rw-   0        0        0      152 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/src/intrieri1998/info.py
--rw-rw-rw-   0        0        0      367 2022-04-05 16:41:11.000000 intrieri1998-1.2.0/src/intrieri1998/version.py
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.605519 intrieri1998-1.2.0/src/intrieri1998.egg-info/
--rw-rw-rw-   0        0        0     1988 2022-04-05 16:46:00.000000 intrieri1998-1.2.0/src/intrieri1998.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1080 2022-04-05 16:46:00.000000 intrieri1998-1.2.0/src/intrieri1998.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-05 16:46:00.000000 intrieri1998-1.2.0/src/intrieri1998.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-30 15:54:53.000000 intrieri1998-1.2.0/src/intrieri1998.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2022-04-05 16:46:00.000000 intrieri1998-1.2.0/src/intrieri1998.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-05 16:46:00.641525 intrieri1998-1.2.0/test/
--rw-rw-rw-   0        0        0      976 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/test/conftest.py
--rw-rw-rw-   0        0        0       90 2022-04-05 16:37:24.000000 intrieri1998-1.2.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.361295 intrieri1998-1.3.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3343 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3372 2024-05-29 09:35:25.360295 intrieri1998-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1528 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.327549 intrieri1998-1.3.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.327549 intrieri1998-1.3.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.328548 intrieri1998-1.3.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5124 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/history.rst
+-rw-rw-rw-   0        0        0      599 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/index.rst
+-rw-rw-rw-   0        0        0      222 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1453 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.331551 intrieri1998-1.3.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2338 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      352 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:35:25.361295 intrieri1998-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.293610 intrieri1998-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.338549 intrieri1998-1.3.0/src/intrieri1998/
+-rw-rw-rw-   0        0        0      255 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/src/intrieri1998/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.355298 intrieri1998-1.3.0/src/intrieri1998/clean/
+-rw-rw-rw-   0        0        0     6537 2024-05-29 09:25:56.000000 intrieri1998-1.3.0/src/intrieri1998/clean/fig3.csv
+-rw-rw-rw-   0        0        0     4984 2024-05-29 09:26:00.000000 intrieri1998-1.3.0/src/intrieri1998/clean/fig4.csv
+-rw-rw-rw-   0        0        0     2570 2024-05-29 09:26:04.000000 intrieri1998-1.3.0/src/intrieri1998/clean/fig5.csv
+-rw-rw-rw-   0        0        0      525 2024-05-29 09:26:07.000000 intrieri1998-1.3.0/src/intrieri1998/clean/fig6.csv
+-rw-rw-rw-   0        0        0     3694 2024-05-29 09:26:10.000000 intrieri1998-1.3.0/src/intrieri1998/clean/fig7.csv
+-rw-rw-rw-   0        0        0     1238 2024-05-29 09:26:14.000000 intrieri1998-1.3.0/src/intrieri1998/clean/fig8.csv
+-rw-rw-rw-   0        0        0      916 2024-05-29 09:26:17.000000 intrieri1998-1.3.0/src/intrieri1998/clean/info.json
+-rw-rw-rw-   0        0        0      134 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/src/intrieri1998/clean/readme.rst
+-rw-rw-rw-   0        0        0      527 2024-05-29 09:26:22.000000 intrieri1998-1.3.0/src/intrieri1998/clean/table.csv
+-rw-rw-rw-   0        0        0      174 2022-03-31 08:39:49.000000 intrieri1998-1.3.0/src/intrieri1998/fig5.py
+-rw-rw-rw-   0        0        0       85 2022-03-31 08:51:31.000000 intrieri1998-1.3.0/src/intrieri1998/fig6.py
+-rw-rw-rw-   0        0        0      134 2022-03-31 09:58:10.000000 intrieri1998-1.3.0/src/intrieri1998/fig8.py
+-rw-rw-rw-   0        0        0      379 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/src/intrieri1998/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/src/intrieri1998/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.359295 intrieri1998-1.3.0/src/intrieri1998.egg-info/
+-rw-rw-rw-   0        0        0     3372 2024-05-29 09:35:25.000000 intrieri1998-1.3.0/src/intrieri1998.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2024-05-29 09:35:25.000000 intrieri1998-1.3.0/src/intrieri1998.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:35:25.000000 intrieri1998-1.3.0/src/intrieri1998.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-29 09:35:25.000000 intrieri1998-1.3.0/src/intrieri1998.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 09:35:25.000000 intrieri1998-1.3.0/src/intrieri1998.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:35:25.357296 intrieri1998-1.3.0/test/
+-rw-rw-rw-   0        0        0      988 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/test/conftest.py
+-rw-rw-rw-   0        0        0      389 2024-05-29 09:27:58.000000 intrieri1998-1.3.0/test/test_packaging.py
```

### Comparing `intrieri1998-1.2.0/CONTRIBUTING.rst` & `intrieri1998-1.3.0/CONTRIBUTING.rst`

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

### Comparing `intrieri1998-1.2.0/LICENSE` & `intrieri1998-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/PKG-INFO` & `intrieri1998-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,88 @@
 Metadata-Version: 2.1
 Name: intrieri1998
-Version: 1.2.0
+Version: 1.3.0
 Summary: Data and formalisms from Intrieri et al. (1998)
-Home-page: https://gitlab.com/b326/intrieri1998
-Author: revesansparole
-Author-email: revesansparole@gmail.com
+Author-email: revesansparole <revesansparole@gmail.com>
+Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>
 License: cc_by_nc
-Platform: UNKNOWN
+Project-URL: repository, https://gitlab.com/b326/intrieri1998
+Project-URL: pip, https://pypi.org/project/intrieri1998/1.3.0/
+Project-URL: conda, https://anaconda.org/revesansparole/intrieri1998
+Project-URL: doc, https://b326.gitlab.io/intrieri1998/
+Project-URL: pypi, https://badge.fury.io/py/intrieri1998
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Provides-Extra: dvlpt
+Requires-Dist: twine; extra == "dvlpt"
+Provides-Extra: example
+Requires-Dist: matplotlib; extra == "example"
+Requires-Dist: pandas; extra == "example"
+Provides-Extra: script
+Requires-Dist: graphextract; extra == "script"
+Requires-Dist: numpy; extra == "script"
+Requires-Dist: pandas; extra == "script"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 ========================
 intrieri1998
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/intrieri1998/
-
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/intrieri1998/1.2.0/
+    :target: https://pypi.org/project/intrieri1998/1.3.0/
 
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/intrieri1998
 
+.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/intrieri1998/
+
 .. image:: https://badge.fury.io/py/intrieri1998.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/intrieri1998
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/intrieri1998/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/intrieri1998/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/intrieri1998/commits/main
-.. #}
-
-Data and formalisms from Intrieri et al. (1998)
-
 
+prod: |prod_build|_ |prod_coverage|_
 
-=======
-History
-=======
+.. |prod_build| image:: https://gitlab.com/b326/intrieri1998/badges/prod/pipeline.svg
+.. _prod_build: https://gitlab.com/b326/intrieri1998/commits/prod
 
-creation (2022-03-30)
-------------------------
-
-* First release on PyPI.
+.. |prod_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/prod/coverage.svg
+.. _prod_coverage: https://gitlab.com/b326/intrieri1998/commits/prod
+.. #}
 
+Data and formalisms from Intrieri et al. (1998)
```

### Comparing `intrieri1998-1.2.0/README.rst` & `intrieri1998-1.3.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 ========================
 intrieri1998
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/intrieri1998/
-
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/intrieri1998/1.2.0/
+    :target: https://pypi.org/project/intrieri1998/1.3.0/
 
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/intrieri1998
 
+.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/intrieri1998/
+
 .. image:: https://badge.fury.io/py/intrieri1998.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/intrieri1998
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/intrieri1998/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/intrieri1998/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/intrieri1998/commits/main
+
+prod: |prod_build|_ |prod_coverage|_
+
+.. |prod_build| image:: https://gitlab.com/b326/intrieri1998/badges/prod/pipeline.svg
+.. _prod_build: https://gitlab.com/b326/intrieri1998/commits/prod
+
+.. |prod_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/prod/coverage.svg
+.. _prod_coverage: https://gitlab.com/b326/intrieri1998/commits/prod
 .. #}
 
 Data and formalisms from Intrieri et al. (1998)
```

### Comparing `intrieri1998-1.2.0/doc/Makefile` & `intrieri1998-1.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/doc/biblio/biblio.rst` & `intrieri1998-1.3.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/doc/conf.py` & `intrieri1998-1.3.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.2.0"
+version = "1.3.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.2.0"
+release = "1.3.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `intrieri1998-1.2.0/doc/index.rst` & `intrieri1998-1.3.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/doc/make.bat` & `intrieri1998-1.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/doc/readme.rst` & `intrieri1998-1.3.0/doc/readme.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/intrieri1998/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/intrieri1998/1.2.0/
+    :target: https://pypi.org/project/intrieri1998/1.3.0/
+
 
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/intrieri1998
 
+
+.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/intrieri1998/
+
+
 .. image:: https://badge.fury.io/py/intrieri1998.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/intrieri1998
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/intrieri1998/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/intrieri1998/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/intrieri1998/commits/main
+
+prod: |prod_build|_ |prod_coverage|_
+
+.. |prod_build| image:: https://gitlab.com/b326/intrieri1998/badges/prod/pipeline.svg
+.. _prod_build: https://gitlab.com/b326/intrieri1998/commits/prod
+
+.. |prod_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/prod/coverage.svg
+.. _prod_coverage: https://gitlab.com/b326/intrieri1998/commits/prod
 .. #}
 
 Data and formalisms from Intrieri et al. (1998)
```

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/fig3.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/fig3.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/fig4.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/fig4.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/fig5.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/fig5.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/fig6.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/fig6.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/fig7.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/fig7.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/fig8.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/fig8.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/info.json` & `intrieri1998-1.3.0/src/intrieri1998/clean/info.json`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998/clean/table.csv` & `intrieri1998-1.3.0/src/intrieri1998/clean/table.csv`

 * *Files identical despite different names*

### Comparing `intrieri1998-1.2.0/src/intrieri1998.egg-info/PKG-INFO` & `intrieri1998-1.3.0/src/intrieri1998.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,88 @@
 Metadata-Version: 2.1
 Name: intrieri1998
-Version: 1.2.0
+Version: 1.3.0
 Summary: Data and formalisms from Intrieri et al. (1998)
-Home-page: https://gitlab.com/b326/intrieri1998
-Author: revesansparole
-Author-email: revesansparole@gmail.com
+Author-email: revesansparole <revesansparole@gmail.com>
+Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>
 License: cc_by_nc
-Platform: UNKNOWN
+Project-URL: repository, https://gitlab.com/b326/intrieri1998
+Project-URL: pip, https://pypi.org/project/intrieri1998/1.3.0/
+Project-URL: conda, https://anaconda.org/revesansparole/intrieri1998
+Project-URL: doc, https://b326.gitlab.io/intrieri1998/
+Project-URL: pypi, https://badge.fury.io/py/intrieri1998
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Provides-Extra: dvlpt
+Requires-Dist: twine; extra == "dvlpt"
+Provides-Extra: example
+Requires-Dist: matplotlib; extra == "example"
+Requires-Dist: pandas; extra == "example"
+Provides-Extra: script
+Requires-Dist: graphextract; extra == "script"
+Requires-Dist: numpy; extra == "script"
+Requires-Dist: pandas; extra == "script"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 ========================
 intrieri1998
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/intrieri1998/
-
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/intrieri1998/1.2.0/
+    :target: https://pypi.org/project/intrieri1998/1.3.0/
 
 .. image:: https://b326.gitlab.io/intrieri1998/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/intrieri1998
 
+.. image:: https://b326.gitlab.io/intrieri1998/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/intrieri1998/
+
 .. image:: https://badge.fury.io/py/intrieri1998.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/intrieri1998
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/intrieri1998/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/intrieri1998/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/intrieri1998/commits/main
-.. #}
-
-Data and formalisms from Intrieri et al. (1998)
-
 
+prod: |prod_build|_ |prod_coverage|_
 
-=======
-History
-=======
+.. |prod_build| image:: https://gitlab.com/b326/intrieri1998/badges/prod/pipeline.svg
+.. _prod_build: https://gitlab.com/b326/intrieri1998/commits/prod
 
-creation (2022-03-30)
-------------------------
-
-* First release on PyPI.
+.. |prod_coverage| image:: https://gitlab.com/b326/intrieri1998/badges/prod/coverage.svg
+.. _prod_coverage: https://gitlab.com/b326/intrieri1998/commits/prod
+.. #}
 
+Data and formalisms from Intrieri et al. (1998)
```

### Comparing `intrieri1998-1.2.0/src/intrieri1998.egg-info/SOURCES.txt` & `intrieri1998-1.3.0/src/intrieri1998.egg-info/SOURCES.txt`

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
@@ -28,15 +26,15 @@
 src/intrieri1998/fig6.py
 src/intrieri1998/fig8.py
 src/intrieri1998/info.py
 src/intrieri1998/version.py
 src/intrieri1998.egg-info/PKG-INFO
 src/intrieri1998.egg-info/SOURCES.txt
 src/intrieri1998.egg-info/dependency_links.txt
-src/intrieri1998.egg-info/not-zip-safe
+src/intrieri1998.egg-info/requires.txt
 src/intrieri1998.egg-info/top_level.txt
 src/intrieri1998/clean/fig3.csv
 src/intrieri1998/clean/fig4.csv
 src/intrieri1998/clean/fig5.csv
 src/intrieri1998/clean/fig6.csv
 src/intrieri1998/clean/fig7.csv
 src/intrieri1998/clean/fig8.csv
```

### Comparing `intrieri1998-1.2.0/test/conftest.py` & `intrieri1998-1.3.0/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=intrieri1998")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=intrieri1998")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

