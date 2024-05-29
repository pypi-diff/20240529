# Comparing `tmp/greer2018-1.0.0.tar.gz` & `tmp/greer2018-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greer2018-1.0.0.tar", last modified: Thu Mar  9 18:07:06 2023, max compression
+gzip compressed data, was "greer2018-1.1.0.tar", last modified: Wed May 29 08:57:14 2024, max compression
```

## Comparing `greer2018-1.0.0.tar` & `greer2018-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.352435 greer2018-1.0.0/
--rw-rw-rw-   0        0        0      316 2023-03-09 18:04:25.000000 greer2018-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3313 2023-03-09 18:04:25.000000 greer2018-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2023-03-09 18:04:25.000000 greer2018-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2023-03-09 18:04:25.000000 greer2018-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      437 2023-03-09 18:04:26.000000 greer2018-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2264 2023-03-09 18:07:06.352435 greer2018-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1474 2023-03-09 18:04:25.000000 greer2018-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.224120 greer2018-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2023-03-09 18:04:26.000000 greer2018-1.0.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2023-03-09 18:04:26.000000 greer2018-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.228296 greer2018-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      282 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.252436 greer2018-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5091 2023-03-09 18:04:25.000000 greer2018-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      593 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      219 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-03-09 18:04:26.000000 greer2018-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1394 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.272434 greer2018-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       86 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2023-03-09 18:04:27.000000 greer2018-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      360 2023-03-09 18:04:25.000000 greer2018-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2023-03-09 18:04:25.000000 greer2018-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2023-03-09 18:07:06.362435 greer2018-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1881 2023-03-09 18:04:26.000000 greer2018-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:05.964721 greer2018-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.282443 greer2018-1.0.0/src/greer2018/
--rw-rw-rw-   0        0        0      260 2023-03-09 18:04:26.000000 greer2018-1.0.0/src/greer2018/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.332446 greer2018-1.0.0/src/greer2018/clean/
--rw-rw-rw-   0        0        0     2055 2023-03-09 16:30:54.000000 greer2018-1.0.0/src/greer2018/clean/net_photosynthesis.csv
--rw-rw-rw-   0        0        0      841 2023-03-09 16:30:36.000000 greer2018-1.0.0/src/greer2018/clean/net_photosynthesis_max.csv
--rw-rw-rw-   0        0        0      134 2023-03-09 18:04:27.000000 greer2018-1.0.0/src/greer2018/clean/readme.rst
--rw-rw-rw-   0        0        0      152 2023-03-09 18:04:27.000000 greer2018-1.0.0/src/greer2018/info.py
--rw-rw-rw-   0        0        0      367 2023-03-09 18:04:26.000000 greer2018-1.0.0/src/greer2018/version.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.312434 greer2018-1.0.0/src/greer2018.egg-info/
--rw-rw-rw-   0        0        0     2264 2023-03-09 18:07:05.000000 greer2018-1.0.0/src/greer2018.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2023-03-09 18:07:05.000000 greer2018-1.0.0/src/greer2018.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 18:07:05.000000 greer2018-1.0.0/src/greer2018.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 18:05:54.000000 greer2018-1.0.0/src/greer2018.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-03-09 18:07:05.000000 greer2018-1.0.0/src/greer2018.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 18:07:06.352435 greer2018-1.0.0/test/
--rw-rw-rw-   0        0        0      973 2023-03-09 18:04:26.000000 greer2018-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0      530 2023-03-09 16:31:16.000000 greer2018-1.0.0/test/test_net_photosynthesis.py
--rw-rw-rw-   0        0        0      533 2023-03-09 16:31:17.000000 greer2018-1.0.0/test/test_net_photosynthesis_max.py
--rw-rw-rw-   0        0        0       84 2023-03-09 18:04:27.000000 greer2018-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.341325 greer2018-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-29 08:54:04.000000 greer2018-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3313 2024-05-29 08:54:04.000000 greer2018-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-29 08:54:04.000000 greer2018-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-29 08:54:04.000000 greer2018-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3338 2024-05-29 08:57:14.339326 greer2018-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1474 2024-05-29 08:54:04.000000 greer2018-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.302072 greer2018-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-29 08:54:04.000000 greer2018-1.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.304072 greer2018-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.305165 greer2018-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5091 2024-05-29 08:54:04.000000 greer2018-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      593 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      219 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-29 08:54:04.000000 greer2018-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1402 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.308072 greer2018-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-29 08:54:05.000000 greer2018-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2329 2024-05-29 08:54:05.000000 greer2018-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      360 2024-05-29 08:54:04.000000 greer2018-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:54:04.000000 greer2018-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:57:14.341325 greer2018-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.260048 greer2018-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.311072 greer2018-1.1.0/src/greer2018/
+-rw-rw-rw-   0        0        0      252 2024-05-29 08:54:04.000000 greer2018-1.1.0/src/greer2018/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.326138 greer2018-1.1.0/src/greer2018/clean/
+-rw-rw-rw-   0        0        0     2055 2024-05-29 08:53:21.000000 greer2018-1.1.0/src/greer2018/clean/net_photosynthesis.csv
+-rw-rw-rw-   0        0        0      841 2024-05-29 08:53:26.000000 greer2018-1.1.0/src/greer2018/clean/net_photosynthesis_max.csv
+-rw-rw-rw-   0        0        0      134 2024-05-29 08:54:05.000000 greer2018-1.1.0/src/greer2018/clean/readme.rst
+-rw-rw-rw-   0        0        0      379 2024-05-29 08:54:05.000000 greer2018-1.1.0/src/greer2018/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-29 08:54:04.000000 greer2018-1.1.0/src/greer2018/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.337325 greer2018-1.1.0/src/greer2018.egg-info/
+-rw-rw-rw-   0        0        0     3338 2024-05-29 08:57:14.000000 greer2018-1.1.0/src/greer2018.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-05-29 08:57:14.000000 greer2018-1.1.0/src/greer2018.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:57:14.000000 greer2018-1.1.0/src/greer2018.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-05-29 08:57:14.000000 greer2018-1.1.0/src/greer2018.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 08:57:14.000000 greer2018-1.1.0/src/greer2018.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 08:57:14.335382 greer2018-1.1.0/test/
+-rw-rw-rw-   0        0        0      985 2024-05-29 08:54:05.000000 greer2018-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      530 2023-03-09 16:31:16.000000 greer2018-1.1.0/test/test_net_photosynthesis.py
+-rw-rw-rw-   0        0        0      533 2023-03-09 16:31:17.000000 greer2018-1.1.0/test/test_net_photosynthesis_max.py
+-rw-rw-rw-   0        0        0      377 2024-05-29 08:54:05.000000 greer2018-1.1.0/test/test_packaging.py
```

### Comparing `greer2018-1.0.0/CONTRIBUTING.rst` & `greer2018-1.1.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 310.
+  3. The pull request should work for Python 3.9.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `greer2018-1.0.0/LICENSE` & `greer2018-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/README.rst` & `greer2018-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 greer2018
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/greer2018/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/greer2018/1.0.0/
+    :target: https://pypi.org/project/greer2018/1.1.0/
 
 .. image:: https://b326.gitlab.io/greer2018/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/greer2018
 
 .. image:: https://b326.gitlab.io/greer2018/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `greer2018-1.0.0/doc/Makefile` & `greer2018-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/doc/biblio/biblio.rst` & `greer2018-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/doc/conf.py` & `greer2018-1.1.0/doc/conf.py`

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

### Comparing `greer2018-1.0.0/doc/index.rst` & `greer2018-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/doc/make.bat` & `greer2018-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/doc/readme.rst` & `greer2018-1.1.0/doc/readme.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Overview
 ========
 
 .. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/greer2018/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/greer2018/1.0.0/
+    :target: https://pypi.org/project/greer2018/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/greer2018/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/greer2018
 
+
 .. image:: https://b326.gitlab.io/greer2018/_images/badge_doc.svg
     :alt: Documentation status
     :target: https://b326.gitlab.io/greer2018/
 
+
 .. image:: https://badge.fury.io/py/greer2018.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/greer2018
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/greer2018/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/greer2018/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/greer2018/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/greer2018/commits/main
```

### Comparing `greer2018-1.0.0/setup.py` & `greer2018-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,95 @@
-# {# pkglts, pysetup.kwds
-# format setup arguments
-from pathlib import Path
-from setuptools import setup, find_packages
-
-short_descr = "Data and formalisms from Greer et al. (2018)"
-readme = open('README.rst').read()
-history = open('HISTORY.rst').read()
-
-# find packages
-pkgs = find_packages('src')
-
-src_dir = Path("src/greer2018")
-
-data_files = []
-for pth in src_dir.rglob("*"):
-    if not pth.is_dir() and "__pycache__" not in pth.parts:
-        if pth.suffix in ['.json', '.ini', '.csv', '.rst', '.svg']:
-            data_files.append(str(pth.relative_to(src_dir)))
-
-pkg_data = {'greer2018': data_files}
-
-setup_kwds = dict(
-    name='greer2018',
-    version="1.0.0",
-    description=short_descr,
-    long_description=readme + '\n\n' + history,
-    author="revesansparole",
-    author_email="revesansparole@gmail.com",
-    url='https://gitlab.com/b326/greer2018',
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
-        "Programming Language :: Python :: 3.9",
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
+name = "greer2018"
+version = "1.1.0"
+description = "Data and formalisms from Greer et al. (2018)"
+readme = "README.rst"
+requires-python = ">= 3.9"
+license = {text = "cc_by_nc"}
+authors = [
+    {name = "revesansparole", email = "revesansparole@gmail.com"},
+]
+maintainers = [
+    {name = "revesansparole", email = "revesansparole@gmail.com"},
+    {name = "Jerome Chopard", email = "revesansparole@gmail.com"},
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
+    "Programming Language :: Python :: 3.9",
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
+    "pandas",
+    "scipy",
+]
+script = [
+    "graphextract",
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
+repository = "https://gitlab.com/b326/greer2018"
+pip = "https://pypi.org/project/greer2018/1.1.0/"
+conda = "https://anaconda.org/revesansparole/greer2018"
+doc = "https://b326.gitlab.io/greer2018/"
+pypi = "https://badge.fury.io/py/greer2018"
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
+addopts = "--maxfail=2 -rf --cov=greer2018"
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

### Comparing `greer2018-1.0.0/src/greer2018/clean/net_photosynthesis.csv` & `greer2018-1.1.0/src/greer2018/clean/net_photosynthesis.csv`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/src/greer2018/clean/net_photosynthesis_max.csv` & `greer2018-1.1.0/src/greer2018/clean/net_photosynthesis_max.csv`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/src/greer2018.egg-info/SOURCES.txt` & `greer2018-1.1.0/src/greer2018.egg-info/SOURCES.txt`

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
@@ -25,15 +23,15 @@
 doc/user/overview.rst
 src/greer2018/__init__.py
 src/greer2018/info.py
 src/greer2018/version.py
 src/greer2018.egg-info/PKG-INFO
 src/greer2018.egg-info/SOURCES.txt
 src/greer2018.egg-info/dependency_links.txt
-src/greer2018.egg-info/not-zip-safe
+src/greer2018.egg-info/requires.txt
 src/greer2018.egg-info/top_level.txt
 src/greer2018/clean/net_photosynthesis.csv
 src/greer2018/clean/net_photosynthesis_max.csv
 src/greer2018/clean/readme.rst
 test/conftest.py
 test/test_net_photosynthesis.py
 test/test_net_photosynthesis_max.py
```

### Comparing `greer2018-1.0.0/test/conftest.py` & `greer2018-1.1.0/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=greer2018")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=greer2018")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `greer2018-1.0.0/test/test_net_photosynthesis.py` & `greer2018-1.1.0/test/test_net_photosynthesis.py`

 * *Files identical despite different names*

### Comparing `greer2018-1.0.0/test/test_net_photosynthesis_max.py` & `greer2018-1.1.0/test/test_net_photosynthesis_max.py`

 * *Files identical despite different names*

