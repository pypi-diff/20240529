# Comparing `tmp/zhu2020-1.0.0.tar.gz` & `tmp/zhu2020-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhu2020-1.0.0.tar", last modified: Mon Sep 26 07:40:58 2022, max compression
+gzip compressed data, was "zhu2020-1.1.0.tar", last modified: Wed May 29 14:24:11 2024, max compression
```

## Comparing `zhu2020-1.0.0.tar` & `zhu2020-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:58.042297 zhu2020-1.0.0/
--rw-rw-rw-   0        0        0      316 2022-09-26 07:13:34.000000 zhu2020-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3292 2022-09-26 07:13:34.000000 zhu2020-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-09-26 07:13:34.000000 zhu2020-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-09-26 07:13:34.000000 zhu2020-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      435 2022-09-26 07:13:34.000000 zhu2020-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2223 2022-09-26 07:40:58.042297 zhu2020-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1425 2022-09-26 07:13:34.000000 zhu2020-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:57.926290 zhu2020-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:57.929289 zhu2020-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:57.933294 zhu2020-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5060 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      589 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      162 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1347 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:57.943294 zhu2020-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       86 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-09-26 07:13:34.000000 zhu2020-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      278 2022-09-26 07:13:34.000000 zhu2020-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-09-26 07:13:34.000000 zhu2020-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-09-26 07:40:58.047295 zhu2020-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1843 2022-09-26 07:13:34.000000 zhu2020-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:57.830288 zhu2020-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:57.963289 zhu2020-1.0.0/src/zhu2020/
--rw-rw-rw-   0        0        0      249 2022-09-26 07:13:34.000000 zhu2020-1.0.0/src/zhu2020/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:58.017295 zhu2020-1.0.0/src/zhu2020/clean/
--rw-rw-rw-   0        0        0      134 2022-09-26 07:13:34.000000 zhu2020-1.0.0/src/zhu2020/clean/readme.rst
--rw-rw-rw-   0        0        0      835 2022-09-26 07:05:20.000000 zhu2020-1.0.0/src/zhu2020/clean/table1.csv
--rw-rw-rw-   0        0        0      152 2022-09-26 07:13:34.000000 zhu2020-1.0.0/src/zhu2020/info.py
--rw-rw-rw-   0        0        0      644 2022-09-26 07:06:51.000000 zhu2020-1.0.0/src/zhu2020/raw.py
--rw-rw-rw-   0        0        0     1447 2022-05-19 12:26:10.000000 zhu2020-1.0.0/src/zhu2020/table1.py
--rw-rw-rw-   0        0        0      367 2022-09-26 07:13:34.000000 zhu2020-1.0.0/src/zhu2020/version.py
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:58.009292 zhu2020-1.0.0/src/zhu2020.egg-info/
--rw-rw-rw-   0        0        0     2223 2022-09-26 07:40:57.000000 zhu2020-1.0.0/src/zhu2020.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      808 2022-09-26 07:40:57.000000 zhu2020-1.0.0/src/zhu2020.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-26 07:40:57.000000 zhu2020-1.0.0/src/zhu2020.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-26 06:59:16.000000 zhu2020-1.0.0/src/zhu2020.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2022-09-26 07:40:57.000000 zhu2020-1.0.0/src/zhu2020.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-26 07:40:58.038294 zhu2020-1.0.0/test/
--rw-rw-rw-   0        0        0      971 2022-09-26 07:13:34.000000 zhu2020-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       80 2022-09-26 07:13:34.000000 zhu2020-1.0.0/test/test_packaging.py
--rw-rw-rw-   0        0        0      276 2022-09-26 07:15:45.000000 zhu2020-1.0.0/test/test_raw.py
--rw-rw-rw-   0        0        0      843 2022-09-26 07:31:33.000000 zhu2020-1.0.0/test/test_yield.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.983550 zhu2020-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 14:19:49.000000 zhu2020-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3293 2024-05-29 14:19:49.000000 zhu2020-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 14:19:49.000000 zhu2020-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 14:19:49.000000 zhu2020-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3025 2024-05-29 14:24:11.982552 zhu2020-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1429 2024-05-29 14:19:49.000000 zhu2020-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.956184 zhu2020-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.957183 zhu2020-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.958184 zhu2020-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5060 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      589 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      217 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1359 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.959184 zhu2020-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 14:19:49.000000 zhu2020-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2204 2024-05-29 14:19:49.000000 zhu2020-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      298 2024-05-29 14:19:49.000000 zhu2020-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 14:19:49.000000 zhu2020-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:24:11.983550 zhu2020-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.934185 zhu2020-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.967185 zhu2020-1.1.0/src/zhu2020/
+-rw-rw-rw-   0        0        0      241 2024-05-29 14:19:49.000000 zhu2020-1.1.0/src/zhu2020/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.974419 zhu2020-1.1.0/src/zhu2020/clean/
+-rw-rw-rw-   0        0        0      134 2024-05-29 14:19:49.000000 zhu2020-1.1.0/src/zhu2020/clean/readme.rst
+-rw-rw-rw-   0        0        0      835 2024-05-29 14:18:10.000000 zhu2020-1.1.0/src/zhu2020/clean/table1.csv
+-rw-rw-rw-   0        0        0      379 2024-05-29 14:19:49.000000 zhu2020-1.1.0/src/zhu2020/info.py
+-rw-rw-rw-   0        0        0      644 2022-09-26 07:06:51.000000 zhu2020-1.1.0/src/zhu2020/raw.py
+-rw-rw-rw-   0        0        0     1447 2022-05-19 12:26:10.000000 zhu2020-1.1.0/src/zhu2020/table1.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 14:19:49.000000 zhu2020-1.1.0/src/zhu2020/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.980475 zhu2020-1.1.0/src/zhu2020.egg-info/
+-rw-rw-rw-   0        0        0     3025 2024-05-29 14:24:11.000000 zhu2020-1.1.0/src/zhu2020.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2024-05-29 14:24:11.000000 zhu2020-1.1.0/src/zhu2020.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:24:11.000000 zhu2020-1.1.0/src/zhu2020.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2024-05-29 14:24:11.000000 zhu2020-1.1.0/src/zhu2020.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 14:24:11.000000 zhu2020-1.1.0/src/zhu2020.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 14:24:11.979148 zhu2020-1.1.0/test/
+-rw-rw-rw-   0        0        0      983 2024-05-29 14:19:49.000000 zhu2020-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      369 2024-05-29 14:19:49.000000 zhu2020-1.1.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0      276 2022-09-26 07:15:45.000000 zhu2020-1.1.0/test/test_raw.py
+-rw-rw-rw-   0        0        0      843 2022-09-26 07:31:33.000000 zhu2020-1.1.0/test/test_yield.py
```

### Comparing `zhu2020-1.0.0/CONTRIBUTING.rst` & `zhu2020-1.1.0/CONTRIBUTING.rst`

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

### Comparing `zhu2020-1.0.0/LICENSE` & `zhu2020-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/PKG-INFO` & `zhu2020-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,70 @@
 Metadata-Version: 2.1
 Name: zhu2020
-Version: 1.0.0
+Version: 1.1.0
 Summary: Data and formalisms from Zhu 2020
-Home-page: https://gitlab.com/b326/zhu2020
-Author: revesansparole
-Author-email: revesansparole@gmail.com
+Author-email: revesansparole <revesansparole@gmail.com>
+Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>
 License: cc_by_nc
-Platform: UNKNOWN
+Project-URL: repository, https://gitlab.com/b326/zhu2020
+Project-URL: pip, https://pypi.org/project/zhu2020/1.1.0/
+Project-URL: conda, https://anaconda.org/revesansparole/zhu2020
+Project-URL: doc, https://b326.gitlab.io/zhu2020/
+Project-URL: pypi, https://badge.fury.io/py/zhu2020
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
+Provides-Extra: script
+Requires-Dist: pandas; extra == "script"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 ========================
 zhu2020
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/zhu2020/
-
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/zhu2020/1.0.0/
+    :target: https://pypi.org/project/zhu2020/1.1.0/
 
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/zhu2020
 
+.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/zhu2020/
+
 .. image:: https://badge.fury.io/py/zhu2020.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/zhu2020
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/zhu2020/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/zhu2020/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/zhu2020/badges/main/coverage.svg
@@ -58,19 +77,7 @@
 
 .. |prod_coverage| image:: https://gitlab.com/b326/zhu2020/badges/prod/coverage.svg
 .. _prod_coverage: https://gitlab.com/b326/zhu2020/commits/prod
 .. #}
 
 Data and formalisms from Zhu 2020
 
-
-
-=======
-History
-=======
-
-creation (2022-09-26)
-------------------------
-
-* First release on PyPI.
-
-
```

### Comparing `zhu2020-1.0.0/README.rst` & `zhu2020-1.1.0/doc/readme.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-========================
-zhu2020
-========================
+Overview
+========
 
-.. {# pkglts, doc
-
-.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/zhu2020/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/zhu2020/1.0.0/
+    :target: https://pypi.org/project/zhu2020/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/zhu2020
 
+
+.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/zhu2020/
+
+
 .. image:: https://badge.fury.io/py/zhu2020.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/zhu2020
 
-.. #}
-.. {# pkglts, glabpkg, after doc
+
+
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/zhu2020/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/zhu2020/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/zhu2020/badges/main/coverage.svg
@@ -37,8 +39,7 @@
 .. _prod_build: https://gitlab.com/b326/zhu2020/commits/prod
 
 .. |prod_coverage| image:: https://gitlab.com/b326/zhu2020/badges/prod/coverage.svg
 .. _prod_coverage: https://gitlab.com/b326/zhu2020/commits/prod
 .. #}
 
 Data and formalisms from Zhu 2020
-
```

### Comparing `zhu2020-1.0.0/doc/Makefile` & `zhu2020-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/doc/biblio/biblio.rst` & `zhu2020-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/doc/conf.py` & `zhu2020-1.1.0/doc/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `zhu2020-1.0.0/doc/index.rst` & `zhu2020-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/doc/make.bat` & `zhu2020-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/doc/readme.rst` & `zhu2020-1.1.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-Overview
-========
+========================
+zhu2020
+========================
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/zhu2020/
+.. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/zhu2020/1.0.0/
+    :target: https://pypi.org/project/zhu2020/1.1.0/
 
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/zhu2020
 
+.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/zhu2020/
+
 .. image:: https://badge.fury.io/py/zhu2020.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/zhu2020
 
-
+.. #}
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/zhu2020/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/zhu2020/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/zhu2020/badges/main/coverage.svg
@@ -35,7 +37,8 @@
 .. _prod_build: https://gitlab.com/b326/zhu2020/commits/prod
 
 .. |prod_coverage| image:: https://gitlab.com/b326/zhu2020/badges/prod/coverage.svg
 .. _prod_coverage: https://gitlab.com/b326/zhu2020/commits/prod
 .. #}
 
 Data and formalisms from Zhu 2020
+
```

### Comparing `zhu2020-1.0.0/src/zhu2020/clean/table1.csv` & `zhu2020-1.1.0/src/zhu2020/clean/table1.csv`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/src/zhu2020/raw.py` & `zhu2020-1.1.0/src/zhu2020/raw.py`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/src/zhu2020/table1.py` & `zhu2020-1.1.0/src/zhu2020/table1.py`

 * *Files identical despite different names*

### Comparing `zhu2020-1.0.0/src/zhu2020.egg-info/PKG-INFO` & `zhu2020-1.1.0/src/zhu2020.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,70 @@
 Metadata-Version: 2.1
 Name: zhu2020
-Version: 1.0.0
+Version: 1.1.0
 Summary: Data and formalisms from Zhu 2020
-Home-page: https://gitlab.com/b326/zhu2020
-Author: revesansparole
-Author-email: revesansparole@gmail.com
+Author-email: revesansparole <revesansparole@gmail.com>
+Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>
 License: cc_by_nc
-Platform: UNKNOWN
+Project-URL: repository, https://gitlab.com/b326/zhu2020
+Project-URL: pip, https://pypi.org/project/zhu2020/1.1.0/
+Project-URL: conda, https://anaconda.org/revesansparole/zhu2020
+Project-URL: doc, https://b326.gitlab.io/zhu2020/
+Project-URL: pypi, https://badge.fury.io/py/zhu2020
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
+Provides-Extra: script
+Requires-Dist: pandas; extra == "script"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 ========================
 zhu2020
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/zhu2020/
-
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/zhu2020/1.0.0/
+    :target: https://pypi.org/project/zhu2020/1.1.0/
 
 .. image:: https://b326.gitlab.io/zhu2020/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/zhu2020
 
+.. image:: https://b326.gitlab.io/zhu2020/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/zhu2020/
+
 .. image:: https://badge.fury.io/py/zhu2020.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/zhu2020
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/zhu2020/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/zhu2020/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/zhu2020/badges/main/coverage.svg
@@ -58,19 +77,7 @@
 
 .. |prod_coverage| image:: https://gitlab.com/b326/zhu2020/badges/prod/coverage.svg
 .. _prod_coverage: https://gitlab.com/b326/zhu2020/commits/prod
 .. #}
 
 Data and formalisms from Zhu 2020
 
-
-
-=======
-History
-=======
-
-creation (2022-09-26)
-------------------------
-
-* First release on PyPI.
-
-
```

### Comparing `zhu2020-1.0.0/src/zhu2020.egg-info/SOURCES.txt` & `zhu2020-1.1.0/src/zhu2020.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

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
 src/zhu2020/info.py
 src/zhu2020/raw.py
 src/zhu2020/table1.py
 src/zhu2020/version.py
 src/zhu2020.egg-info/PKG-INFO
 src/zhu2020.egg-info/SOURCES.txt
 src/zhu2020.egg-info/dependency_links.txt
-src/zhu2020.egg-info/not-zip-safe
+src/zhu2020.egg-info/requires.txt
 src/zhu2020.egg-info/top_level.txt
 src/zhu2020/clean/readme.rst
 src/zhu2020/clean/table1.csv
 test/conftest.py
 test/test_packaging.py
 test/test_raw.py
 test/test_yield.py
```

### Comparing `zhu2020-1.0.0/test/conftest.py` & `zhu2020-1.1.0/test/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=zhu2020")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=zhu2020")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `zhu2020-1.0.0/test/test_yield.py` & `zhu2020-1.1.0/test/test_yield.py`

 * *Files identical despite different names*

