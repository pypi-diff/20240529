# Comparing `tmp/thx-0.5.1.tar.gz` & `tmp/thx-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thx-0.5.1.tar", last modified: Tue Sep 20 19:59:19 2022, max compression
+gzip compressed data, was "thx-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `thx-0.5.1.tar` & `thx-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0      180 2022-09-20 19:01:58.638668 thx-0.5.1/.flake8
--rw-r--r--   0        0        0     1806 2022-09-20 19:01:58.640355 thx-0.5.1/.gitignore
--rw-r--r--   0        0        0      156 2022-09-20 19:01:58.640617 thx-0.5.1/.readthedocs.yml
--rw-r--r--   0        0        0     2515 2022-09-20 19:47:37.523289 thx-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      975 2022-09-20 19:01:58.641508 thx-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1071 2022-09-20 19:01:58.641916 thx-0.5.1/LICENSE
--rw-r--r--   0        0        0     4087 2022-09-20 19:01:58.642142 thx-0.5.1/README.rst
--rw-r--r--   0        0        0      476 2022-09-20 19:01:58.642838 thx-0.5.1/docs/_static/custom.css
--rw-r--r--   0        0        0    42080 2022-09-20 19:01:58.643341 thx-0.5.1/docs/_static/omnilib.png
--rw-r--r--   0        0        0      342 2022-09-20 19:01:58.643735 thx-0.5.1/docs/_templates/badges.html
--rw-r--r--   0        0        0     1145 2022-09-20 19:01:58.644570 thx-0.5.1/docs/_templates/omnilib.html
--rw-r--r--   0        0        0       70 2022-09-20 19:01:58.645069 thx-0.5.1/docs/changelog.rst
--rw-r--r--   0        0        0     3097 2022-09-20 19:01:58.645248 thx-0.5.1/docs/conf.py
--rw-r--r--   0        0        0     5346 2022-09-20 19:01:58.645437 thx-0.5.1/docs/config.rst
--rw-r--r--   0        0        0       79 2022-09-20 19:01:58.645593 thx-0.5.1/docs/contributing.rst
--rw-r--r--   0        0        0      480 2022-09-20 19:01:58.645759 thx-0.5.1/docs/demo.rst
--rw-r--r--   0        0        0      751 2022-09-20 19:01:58.645948 thx-0.5.1/docs/guide.rst
--rw-r--r--   0        0        0      348 2022-09-20 19:01:58.646274 thx-0.5.1/docs/index.rst
--rw-r--r--   0        0        0     3947 2022-09-20 19:01:58.646538 thx-0.5.1/docs/recipes.rst
--rw-r--r--   0        0        0      823 2022-09-20 19:01:58.646779 thx-0.5.1/makefile
--rw-r--r--   0        0        0     1898 2022-09-20 19:33:06.510439 thx-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      175 2022-09-20 19:01:58.647140 thx-0.5.1/requirements-dev.txt
--rw-r--r--   0        0        0      166 2022-09-20 19:01:58.647341 thx-0.5.1/requirements.txt
--rw-r--r--   0        0        0      117 2022-09-20 19:01:58.647624 thx-0.5.1/thx/__init__.py
--rw-r--r--   0        0        0      128 2022-09-20 19:01:58.647776 thx-0.5.1/thx/__main__.py
--rw-r--r--   0        0        0      156 2022-09-20 19:47:37.569290 thx-0.5.1/thx/__version__.py
--rw-r--r--   0        0        0     4437 2022-09-20 19:01:58.648175 thx-0.5.1/thx/cli.py
--rw-r--r--   0        0        0     4946 2022-09-20 19:01:58.648388 thx-0.5.1/thx/config.py
--rw-r--r--   0        0        0     8078 2022-09-20 19:01:58.648575 thx-0.5.1/thx/context.py
--rw-r--r--   0        0        0     8484 2022-09-20 19:01:58.648754 thx-0.5.1/thx/core.py
--rw-r--r--   0        0        0     5305 2022-09-20 19:01:58.649078 thx-0.5.1/thx/main.py
--rw-r--r--   0        0        0        0 2022-09-20 19:01:58.649199 thx-0.5.1/thx/py.typed
--rw-r--r--   0        0        0     2353 2022-09-20 19:01:58.649383 thx-0.5.1/thx/runner.py
--rw-r--r--   0        0        0      243 2022-09-20 19:01:58.649682 thx-0.5.1/thx/tests/__init__.py
--rw-r--r--   0        0        0      322 2022-09-20 19:01:58.649848 thx-0.5.1/thx/tests/__main__.py
--rw-r--r--   0        0        0     2794 2022-09-20 19:01:58.650018 thx-0.5.1/thx/tests/cli.py
--rw-r--r--   0        0        0    12356 2022-09-20 19:01:58.650215 thx-0.5.1/thx/tests/config.py
--rw-r--r--   0        0        0    15655 2022-09-20 19:01:58.650408 thx-0.5.1/thx/tests/context.py
--rw-r--r--   0        0        0      582 2022-09-20 19:01:58.650560 thx-0.5.1/thx/tests/helper.py
--rw-r--r--   0        0        0     4941 2022-09-20 19:01:58.650722 thx-0.5.1/thx/tests/runner.py
--rw-r--r--   0        0        0     2899 2022-09-20 19:01:58.650946 thx-0.5.1/thx/tests/types.py
--rw-r--r--   0        0        0     4018 2022-09-20 19:01:58.651127 thx-0.5.1/thx/tests/utils.py
--rw-r--r--   0        0        0     4157 2022-09-20 19:01:58.651305 thx-0.5.1/thx/types.py
--rw-r--r--   0        0        0     3902 2022-09-20 19:01:58.651467 thx-0.5.1/thx/utils.py
--rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 thx-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2024-05-16 22:48:34.340067 thx-0.6.0/.flake8
+-rw-r--r--   0        0        0     1806 2024-05-16 22:48:34.340811 thx-0.6.0/.gitignore
+-rw-r--r--   0        0        0       50 2024-05-16 22:48:49.427652 thx-0.6.0/.mailmap
+-rw-r--r--   0        0        0      197 2024-05-29 04:44:29.432224 thx-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2920 2024-05-29 06:26:15.472012 thx-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      975 2024-05-16 22:48:34.341153 thx-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1071 2024-05-16 22:48:34.341262 thx-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3946 2024-05-29 04:44:29.433314 thx-0.6.0/README.rst
+-rw-r--r--   0        0        0      476 2024-05-16 22:48:34.341632 thx-0.6.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    42080 2024-05-16 22:48:34.341994 thx-0.6.0/docs/_static/omnilib.png
+-rw-r--r--   0        0        0      342 2024-05-16 22:48:34.342666 thx-0.6.0/docs/_templates/badges.html
+-rw-r--r--   0        0        0     1145 2024-05-16 22:48:34.342791 thx-0.6.0/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0       70 2024-05-16 22:48:34.342896 thx-0.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0     3097 2024-05-16 22:48:34.343016 thx-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     5551 2024-05-29 04:44:29.433816 thx-0.6.0/docs/config.rst
+-rw-r--r--   0        0        0       79 2024-05-16 22:48:34.343248 thx-0.6.0/docs/contributing.rst
+-rw-r--r--   0        0        0      480 2024-05-16 22:48:34.343359 thx-0.6.0/docs/demo.rst
+-rw-r--r--   0        0        0      751 2024-05-16 22:48:34.343470 thx-0.6.0/docs/guide.rst
+-rw-r--r--   0        0        0      348 2024-05-16 22:48:34.343574 thx-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0     3947 2024-05-16 22:48:34.343726 thx-0.6.0/docs/recipes.rst
+-rw-r--r--   0        0        0      753 2024-05-29 04:44:29.435090 thx-0.6.0/makefile
+-rw-r--r--   0        0        0     2534 2024-05-29 04:44:29.436001 thx-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-16 22:48:34.344423 thx-0.6.0/thx/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-16 22:48:34.344550 thx-0.6.0/thx/__main__.py
+-rw-r--r--   0        0        0      156 2024-05-29 06:26:15.483892 thx-0.6.0/thx/__version__.py
+-rw-r--r--   0        0        0     4523 2024-05-29 06:10:58.666783 thx-0.6.0/thx/cli.py
+-rw-r--r--   0        0        0     5057 2024-05-29 04:44:29.436535 thx-0.6.0/thx/config.py
+-rw-r--r--   0        0        0     8499 2024-05-29 06:10:58.667093 thx-0.6.0/thx/context.py
+-rw-r--r--   0        0        0     8536 2024-05-29 06:22:16.970616 thx-0.6.0/thx/core.py
+-rw-r--r--   0        0        0     5275 2024-05-29 04:44:29.438862 thx-0.6.0/thx/main.py
+-rw-r--r--   0        0        0        0 2024-05-16 22:48:34.345647 thx-0.6.0/thx/py.typed
+-rw-r--r--   0        0        0     2225 2024-05-29 06:10:58.667333 thx-0.6.0/thx/runner.py
+-rw-r--r--   0        0        0      243 2024-05-16 22:48:34.346017 thx-0.6.0/thx/tests/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-29 06:07:25.578659 thx-0.6.0/thx/tests/__main__.py
+-rw-r--r--   0        0        0     2804 2024-05-29 06:10:58.667592 thx-0.6.0/thx/tests/cli.py
+-rw-r--r--   0        0        0    12522 2024-05-29 04:44:29.440981 thx-0.6.0/thx/tests/config.py
+-rw-r--r--   0        0        0    17781 2024-05-29 06:10:58.667905 thx-0.6.0/thx/tests/context.py
+-rw-r--r--   0        0        0      582 2024-05-16 22:48:34.346766 thx-0.6.0/thx/tests/helper.py
+-rw-r--r--   0        0        0     4233 2024-05-29 06:10:58.668173 thx-0.6.0/thx/tests/runner.py
+-rw-r--r--   0        0        0     2899 2024-05-16 22:48:34.347048 thx-0.6.0/thx/tests/types.py
+-rw-r--r--   0        0        0     5385 2024-05-29 06:10:58.668433 thx-0.6.0/thx/tests/utils.py
+-rw-r--r--   0        0        0     4213 2024-05-29 04:44:29.442118 thx-0.6.0/thx/types.py
+-rw-r--r--   0        0        0     4413 2024-05-29 06:10:58.668691 thx-0.6.0/thx/utils.py
+-rw-r--r--   0        0        0     5618 1970-01-01 00:00:00.000000 thx-0.6.0/PKG-INFO
```

### Comparing `thx-0.5.1/.gitignore` & `thx-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/CHANGELOG.md` & `thx-0.6.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 thx
 ===
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v0.6.0
+------
+
+Feature release
+
+- Support for installing project with extras (#85)
+- Virtualenv bin/scripts dir is now added to `$PATH` (#82, #110)
+- Exclude `.thx/` virtualenv dir from watchdog events in watch mode (#71, #111)
+- Tested up to Python 3.12
+- Dropped support for Python 3.7
+
+```text
+$ git shortlog -s v0.5.1...v0.6.0
+    13	Amethyst Reese
+     1	Tim Hatch
+    18	dependabot[bot]
+```
+
+
 v0.5.1
 ------
 
 Bugfix release
 
 - Fix: exit with error code if virtualenvs fail to build (#40)
 - Fix: include stderr when python runtimes have unknown version (#39, #64)
 - Fix: better virtualenv and binary handling for Windows (#64)
 - Docs: updated user guide links and toml section names (#52)
 
 ```text
 $ git shortlog -s v0.5.0...v0.5.1
-    10	Amethyst Reese
-     2	John Reese
+    12	Amethyst Reese
      1	Tim Hatch
     12	dependabot[bot]
 ```
 
 
 v0.5.0
 ------
@@ -29,15 +47,15 @@
 Feature release
 
 - `watch_paths` is no longer required for watch mode
 - documentation improvements
 
 ```text
 $ git shortlog -s v0.4.0...v0.5.0
-    16	John Reese
+    16	Amethyst Reese
      4	dependabot[bot]
 ```
 
 
 v0.4.0
 ------
 
@@ -49,15 +67,15 @@
 - Feature: new builtin "list" and "dump-config" commands
 - Fix: handle errors when building virtualenvs
 - Fix: handle Python versions with local patches (`3.8.6+`)
 - Fix: support for Windows cmd prompt
 
 ```text
 $ git shortlog -s v0.4.0a1...v0.4.0
-     9	John Reese
+     9	Amethyst Reese
 ```
 
 
 v0.4.0a1
 --------
 
 Alpha release
@@ -65,15 +83,15 @@
 - Implemented 'list' and 'dump-config' commands
 - Added `--watch` mode
 - Added `job.show_output` flag
 - Support for Windows cmd.exe
 
 ```text
 $ git shortlog -s v0.3.0...v0.4.0a1
-    25	John Reese
+    25	Amethyst Reese
     11	dependabot[bot]
 ```
 
 
 v0.3.0
 ------
 
@@ -82,15 +100,15 @@
 - Better CLI presentation of jobs and results using Rich (#14)
 - New option `--live` to skip version detection (#15)
 - Better tracking of runtime versions available (#15)
 - Fixed benchmarking on Windows due to lack of time precision
 
 ```text
 $ git shortlog -s v0.2.0...v0.3.0
-     8	John Reese
+     8	Amethyst Reese
 ```
 
 
 v0.2.0
 ------
 
 Alpha release
@@ -103,28 +121,28 @@
 - Basic wall clock benchmarking
 - Reuse virtualenvs when possible
 
 See `pyproject.toml` for example job specs.
 
 ```text
 $ git shortlog -s v0.1.0...v0.2.0
-    16	John Reese
+    16	Amethyst Reese
     10	dependabot[bot]
 ```
 
 
 v0.1.0
 ------
 
 Initial release
 
 * Basic implementation of configuration, contexts, and job running
 
 ```text
 $ git shortlog -s v0.1.0
-    37	John Reese
+    37	Amethyst Reese
      2	dependabot[bot]
 ```
 
 [attribution-badge]:
     https://img.shields.io/badge/generated%20by-attribution-informational
 [attribution-url]: https://attribution.omnilib.dev
```

### Comparing `thx-0.5.1/CONTRIBUTING.md` & `thx-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/LICENSE` & `thx-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/README.rst` & `thx-0.6.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 thx
 ===
 
 Rapid development assistant, and fast command runner for Python projects.
 
-.. image:: https://img.shields.io/pypi/l/thx.svg
-   :target: https://github.com/omnilib/thx/blob/main/LICENSE
-   :alt: MIT Licensed
 .. image:: https://img.shields.io/pypi/v/thx.svg
    :target: https://pypi.org/project/thx
    :alt: PyPI Release
-.. image:: https://img.shields.io/badge/change-log-blue
-   :target: https://github.com/omnilib/thx/blob/main/CHANGELOG.md
-   :alt: Changelog
 .. image:: https://readthedocs.org/projects/thx/badge/?version=stable
    :target: https://thx.readthedocs.io/
    :alt: Documentation Status
-.. image:: https://github.com/omnilib/thx/workflows/Build/badge.svg
-   :target: https://github.com/omnilib/thx/actions
-   :alt: Build Status
+.. image:: https://img.shields.io/badge/change-log-blue
+   :target: https://github.com/omnilib/thx/blob/main/CHANGELOG.md
+   :alt: Changelog
+.. image:: https://img.shields.io/pypi/l/thx.svg
+   :target: https://github.com/omnilib/thx/blob/main/LICENSE
+   :alt: MIT Licensed
 
 
 `thx` ("thanks") is capable of running arbitrary jobs, configured via simple options
 in the `PEP 518 <https://peps.python.org/pep-0518/>`_ standardized ``pyproject.toml``.
 Jobs can be run on multiple Python versions at once, and independent steps can be
 executed in parallel for faster results.
```

### Comparing `thx-0.5.1/docs/_static/omnilib.png` & `thx-0.6.0/docs/_static/omnilib.png`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/docs/_templates/omnilib.html` & `thx-0.6.0/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/docs/conf.py` & `thx-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/docs/config.rst` & `thx-0.6.0/docs/config.rst`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,20 @@
 .. attribute:: default
     :type: list[str]
 
     When running `thx` without explicit job names, this option defines the default set
     of jobs that will be run. If not set and no jobs are requested, `thx` will output a
     list of known jobs, equivalent to running ``thx list``.
 
+.. attribute:: extras
+    :type: list[str]
+
+    This specifies a list of package "extras" or optional dpendendencies to be
+    installed when initializing virtual environments and installing the project.
+
 .. attribute:: python_versions
     :type: list[str]
 
     This specifies the version matrix that `thx` will use when running jobs. If not
     specified, `thx` will default to using the live runtime, equivalent to running
     with ``thx --live``.
```

### Comparing `thx-0.5.1/docs/guide.rst` & `thx-0.6.0/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/docs/recipes.rst` & `thx-0.6.0/docs/recipes.rst`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/makefile` & `thx-0.6.0/makefile`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 SRCS:=thx
+EXTRAS:=dev,docs
 
 .venv:
 	python -m venv .venv
-	source .venv/bin/activate && make setup dev
+	source .venv/bin/activate && make install
 	echo 'run `source .venv/bin/activate` to use virtualenv'
 
 venv: .venv
 
-dev:
-	python -m pip install -e .
-
-setup:
+install:
 	python -m pip install -U pip
-	python -m pip install -Ur requirements-dev.txt
-	python -m pip install -Ur requirements.txt
+	python -m pip install -e .[$(EXTRAS)]
 
 release: lint test clean
 	flit publish
 
 format:
 	python -m ufmt format $(SRCS)
```

### Comparing `thx-0.5.1/pyproject.toml` & `thx-0.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,74 @@
 [build-system]
 requires = ["flit_core >=3,<4"]
 build-backend = "flit_core.buildapi"
 
-[tool.flit.metadata]
-module = "thx"
-author = "Amethyst Reese"
-author-email = "amy@noswap.com"
-description-file = "README.rst"
-home-page = "https://github.com/omnilib/thx"
-requires = [
+[project]
+name = "thx"
+readme = "README.rst"
+license = {file="LICENSE"}
+dynamic = ["version", "description"]
+authors = [
+    {name="Amethyst Reese", email="amethyst@n7.gg"},
+]
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Topic :: Utilities",
+    "Typing :: Typed",
+]
+requires-python = ">=3.8"
+dependencies = [
     "aioitertools >= 0.10.0b1",
     "click >= 8.0",
     "packaging >= 21.0",
     "rich >= 11.0.0",
     "tomli >= 1.0",
     "trailrunner >= 1.1",
-    "typing_extensions >= 4.0; python_version < '3.11'",
+    "typing_extensions >= 4.0",
     "watchdog >= 2.1",
 ]
-requires-python = ">=3.7"
-classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Topic :: Utilities",
-    "Typing :: Typed",
+
+[project.optional-dependencies]
+dev = [
+    "aioitertools==v0.11.0",
+    "click==8.1.7",
+    "packaging==24.0",
+    "rich==13.7.1",
+    "tomli==2.0.1",
+    "trailrunner==1.4.0",
+    "typing_extensions == 4.1.1",
+    "watchdog==4.0.0",
+
+    "attribution==1.7.1",
+    "black==24.4.2",
+    "coverage==7.5.1",
+    "flit==3.9.0",
+    "flake8==7.0.0",
+    "mypy==1.10.0",
+    "ufmt==2.6.0",
+    "usort==1.0.8.post1",
+]
+docs = [
+    "sphinx==7.2.6; python_version > '3.8'",
+    "sphinx-mdinclude==0.6.1",
 ]
 
+[project.scripts]
+thx = "thx.main:main"
+
+[project.urls]
+Documentation = "https://thx.omnilib.dev"
+Github = "https://github.com/omnilib/thx"
+
 [tool.flit.sdist]
 exclude = [
     ".github/",
 ]
 
-[tool.flit.scripts]
-thx = "thx.main:main"
-
 [tool.attribution]
 name = "thx"
 package = "thx"
 ignored_authors = ["dependabot"]
 version_file = true
 signed_tags = false
 
@@ -54,35 +85,38 @@
 skip_covered = true
 
 [tool.mypy]
 python_version = "3.8"
 strict = true
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = "thx.core"
+disallow_untyped_calls = false
+
 [tool.thx]
 default = ["format", "docs", "test", "lint", "coverage"]
-python_versions = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python_versions = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+extras = ["dev", "docs"]
 
 [tool.thx.values]
 module = "thx"
 srcs = "thx"
 
 [tool.thx.jobs]
 docs = {run="sphinx-build -ab html docs html", once=true}
 format = {run="python -m ufmt format {srcs}", once=true}
 test = "python -m coverage run -m {module}.tests"
 
-[tool.thx.jobs.combine]
-requires = ["test"]
-run = "python -m coverage combine"
-once = true
-
 [tool.thx.jobs.coverage]
-requires = ["combine"]
-run = "python -m coverage report"
+requires = ["test"]
+run = [
+    "python -m coverage combine -q",
+    "python -m coverage report",
+]
 once = true
 show_output = true
 
 [tool.thx.jobs.lint]
 run = [
     "python -m mypy --install-types --non-interactive -p {module}",
     "python -m flake8 {srcs}",
```

### Comparing `thx-0.5.1/thx/cli.py` & `thx-0.6.0/thx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright 2022 Amethyst Reese
 # Licensed under the MIT License
 
 import logging
 from collections import defaultdict
 from dataclasses import dataclass, field
+from pathlib import Path
 from typing import Any, cast, Dict, List, Optional
 
 from rich.console import Group
 from rich.live import Live
 from rich.text import Text
 from rich.tree import Tree
 
 from .types import (
     Context,
+    ContextEvent,
     Event,
     Fail,
     Job,
     JobEvent,
     Reset,
     Result,
     Step,
@@ -26,15 +28,15 @@
 )
 
 LOG = logging.getLogger(__name__)
 
 
 @dataclass
 class RichRenderer:
-    venvs: Dict[Context, Event] = field(default_factory=dict)
+    venvs: Dict[Path, ContextEvent] = field(default_factory=dict)
     latest: Dict[Job, Dict[Context, Dict[Step, Event]]] = field(
         default_factory=lambda: defaultdict(lambda: defaultdict(dict))
     )
     view: Live = field(init=False)
 
     def __post_init__(self) -> None:
         self.view = Live(auto_refresh=False)
@@ -62,25 +64,26 @@
         if isinstance(event, Fail):
             group: Group = cast(Group, self.view.get_renderable())
             group.renderables.append(Tree("FAIL", style="red"))
             self.view.update(group, refresh=True)
             return
 
         if isinstance(event, (VenvCreate, VenvError, VenvReady)):
-            venvs[event.context] = event
+            venvs[event.context.venv] = event
         elif isinstance(event, JobEvent):
             step = event.step
             job = step.job
             latest[job][event.context][step] = event
 
         trees: List[Tree] = []
 
         if venvs and not all(isinstance(v, VenvReady) for v in venvs.values()):
             tree = Tree("Preparing virtualenvs...")
-            for context, event in venvs.items():
+            for _, event in venvs.items():
+                context = event.context
                 if isinstance(event, VenvReady):
                     text = Text(f"{context.python_version}> done", style="green")
                 elif isinstance(event, VenvError):
                     print(event)
                     text = Text(f"{context.python_version}> failed", style="red")
                     text.append(f"\n{event.error.cmd}", style="")
                     text.append("\n" + event.error.result.stdout, style="")
```

### Comparing `thx-0.5.1/thx/config.py` & `thx-0.6.0/thx/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,15 @@
             )
         ),
         reverse=True,
     )
     requirements: List[str] = ensure_listish(
         data.pop("requirements", None), "tool.thx.requirements"
     )
+    extras: List[str] = ensure_listish(data.pop("extras", None), "tool.thx.extras")
     watch_paths: Set[Path] = {
         Path(p)
         for p in ensure_listish(
             data.pop("watch_paths", None),
             "tool.thx.watch_paths",
         )
     }
@@ -163,14 +164,15 @@
         Config(
             root=root,
             default=default,
             jobs={cmd.name: cmd for cmd in jobs},
             values=values,
             versions=versions,
             requirements=requirements,
+            extras=extras,
             watch_paths=watch_paths,
         )
     )
 
 
 def reload_config(config: Config) -> Config:
     return load_config(config.root)
```

### Comparing `thx-0.5.1/thx/context.py` & `thx-0.6.0/thx/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 
 import logging
 import platform
 import re
 import shutil
 import subprocess
 import time
+from itertools import chain
 from pathlib import Path
 from typing import AsyncIterator, Dict, List, Optional, Sequence, Tuple
 
 from aioitertools.asyncio import as_generated
 
-from .runner import check_command, which
-
+from .runner import check_command
 from .types import (
     CommandError,
     Config,
     Context,
     Event,
     Options,
     StrPath,
     VenvCreate,
     VenvError,
     VenvReady,
     Version,
 )
-
-from .utils import timed, version_match
+from .utils import timed, venv_bin_path, version_match, which
 
 LOG = logging.getLogger(__name__)
 PYTHON_VERSION_RE = re.compile(r"Python (\d+\.\d+[a-zA-Z0-9-_.]+)\+?")
 PYTHON_VERSIONS: Dict[Path, Optional[Version]] = {}
 TIMESTAMP = "thx.timestamp"
 
 
@@ -76,19 +75,20 @@
     return PYTHON_VERSIONS[binary]
 
 
 def find_runtime(
     version: Version, venv: Optional[Path] = None
 ) -> Tuple[Optional[Path], Optional[Version]]:
     if venv and venv.is_dir():
-        bin_dir = venv / "bin"
-        if bin_dir.is_dir():
-            binary_path_str = shutil.which("python", path=f"{bin_dir.as_posix()}")
-            if binary_path_str:
-                return Path(binary_path_str), None
+        bin_dir = venv_bin_path(venv)
+        binary_path_str = shutil.which("python", path=bin_dir.as_posix())
+        if binary_path_str:
+            binary_path = Path(binary_path_str)
+            binary_version = runtime_version(binary_path)
+            return binary_path, binary_version
 
     # TODO: better way to find specific micro/pre/post versions?
     binary_names = [
         f"python{version.major}.{version.minor}",
         f"python{version.major}",
         "python",
     ]
@@ -156,18 +156,20 @@
 def needs_update(context: Context, config: Config) -> bool:
     """Compare timestamps of marker file and requirements files"""
     try:
         timestamp = context.venv / TIMESTAMP
         if timestamp.exists():
             base = timestamp.stat().st_mtime_ns
             newest = 0
-            reqs = project_requirements(config)
-            for req in reqs:
-                if req.exists():
-                    mod_time = req.stat().st_mtime_ns
+            for path in chain(
+                [config.root / "pyproject.toml"],
+                project_requirements(config),
+            ):
+                if path.exists():
+                    mod_time = path.stat().st_mtime_ns
                     newest = max(newest, mod_time)
             return newest > base
 
         else:
             LOG.debug("no timestamp for %s", context.venv)
 
     except Exception:
@@ -191,50 +193,57 @@
 
             # create virtualenv
             prompt = f"thx-{context.python_version}"
             if context.live:
                 import venv
 
                 venv.create(context.venv, prompt=prompt, with_pip=True)
-                new_python_path, _ = find_runtime(context.python_version, context.venv)
-                assert new_python_path is not None
-                context.python_path = new_python_path
 
             else:
                 await check_command(
                     [
                         context.python_path,
                         "-m",
                         "venv",
                         "--prompt",
                         prompt,
                         context.venv,
                     ]
                 )
 
+            new_python_path, new_python_version = find_runtime(
+                context.python_version, context.venv
+            )
+            context.python_path = new_python_path or context.python_path
+            context.python_version = new_python_version or context.python_version
+
             # upgrade pip
             yield VenvCreate(context, message="upgrading pip")
             await check_command(
                 [context.python_path, "-m", "pip", "install", "-U", "pip", "setuptools"]
             )
             pip = which("pip", context)
 
             # install requirements.txt
-            yield VenvCreate(context, message="installing requirements")
             requirements = project_requirements(config)
             if requirements:
+                yield VenvCreate(context, message="installing requirements")
                 LOG.debug("installing deps from %s", requirements)
                 cmd: List[StrPath] = [pip, "install", "-U"]
                 for requirement in requirements:
                     cmd.extend(["-r", requirement])
                 await check_command(cmd)
 
             # install local project
             yield VenvCreate(context, message="installing project")
-            await check_command([pip, "install", "-U", config.root])
+            if config.extras:
+                proj = f"{config.root}[{','.join(config.extras)}]"
+            else:
+                proj = str(config.root)
+            await check_command([pip, "install", "-U", proj])
 
             # timestamp marker
             content = f"{time.time_ns()}\n"
             (context.venv / TIMESTAMP).write_text(content)
 
         else:
             LOG.debug("reusing existing virtualenv %s", context.venv)
```

### Comparing `thx-0.5.1/thx/core.py` & `thx-0.6.0/thx/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Union,
 )
 
 from aioitertools.asyncio import as_generated
 from trailrunner.core import gitignore, pathspec
 from watchdog.events import FileSystemEvent, FileSystemEventHandler
 from watchdog.observers import Observer
+from watchdog.observers.api import BaseObserver
 
 from thx.config import reload_config
 
 from .context import prepare_contexts, resolve_contexts
 
 from .runner import prepare_job
 from .types import (
@@ -161,28 +162,29 @@
     if any(result.error for result in results):
         render(Fail())
         return 1
 
     return 0
 
 
-class ThxWatchdogHandler(FileSystemEventHandler):  # type: ignore
+class ThxWatchdogHandler(FileSystemEventHandler):
     EXCLUDES = [
         "__pycache__",
         ".git",
         ".hg",
         ".mypy_cache",
         ".coverage*",
         "*.swp",
+        ".thx",
     ]
 
     def __init__(
         self,
         options: Options,
-        observer: Observer,
+        observer: BaseObserver,
         render: Renderer,
     ):
         self.__options = options
         self.__observer = observer
         self.__render = render
 
         self.__root = options.config.root
```

### Comparing `thx-0.5.1/thx/main.py` & `thx-0.6.0/thx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Licensed under the MIT License
 
 import asyncio
 import logging
 import shutil
 import sys
 from functools import partial
-from typing import Any, cast, List, Optional, Sequence
+from typing import Any, List, Optional, Sequence
 
 import click
 from rich.logging import RichHandler
 
 from . import __doc__
 from .__version__ import __version__
 from .cli import RichRenderer
@@ -47,16 +47,16 @@
     def create_command(self, name: str) -> Optional[click.Command]:
         if name == "":
             return click.Command("", help="", callback=lambda: True)
         if name in self.config.jobs:
             job = self.config.jobs[name]
             exe = "; ".join(r for r in job.run)
             desc = f"Run `{exe}`"
-            cb = partial(queue_job, name)
-            cb = click.pass_context(cb)
+            cbp = partial(queue_job, name)
+            cb = click.pass_context(cbp)
             return click.Command(name, callback=cb, help=desc)
         return None
 
     def get_command(self, ctx: click.Context, name: str) -> Optional[click.Command]:
         return super().get_command(ctx, name) or self.create_command(name)
 
 
@@ -83,21 +83,19 @@
     live: bool,
     watch: bool,
     python: Optional[Version],
 ) -> None:
     """
     Setup options and load config
     """
-    group = cast(ThxGroup, main)
-
     if live and python:
         raise click.UsageError("Cannot specify both --live and --python")
 
     ctx.ensure_object(Options)
-    ctx.obj.config = group.config
+    ctx.obj.config = main.config
     ctx.obj.benchmark = benchmark
     ctx.obj.debug = debug
     ctx.obj.clean = clean
     ctx.obj.live = live
     ctx.obj.watch = watch
     ctx.obj.python = python
 
@@ -115,15 +113,17 @@
 
     if sys.version_info < (3, 8) and sys.platform == "win32":
         asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
 
 
 @main.result_callback()
 @click.pass_context
-def process_request(ctx: click.Context, results: Sequence[Any], **kwargs: Any) -> None:
+def process_request(
+    ctx: click.Context, /, results: Sequence[Any], **kwargs: Any
+) -> None:
     """
     All click commands finished, start any jobs necessary
     """
     options: Options = ctx.obj
     if options.exit:
         return
```

### Comparing `thx-0.5.1/thx/runner.py` & `thx-0.6.0/thx/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 # Copyright 2022 Amethyst Reese
 # Licensed under the MIT License
 
 import asyncio
 import logging
-import platform
+import os
 import shlex
-import shutil
 from asyncio.subprocess import PIPE
 from dataclasses import dataclass
-from typing import List, Sequence
+from typing import Dict, List, Optional, Sequence
 
 from .types import (
     CommandError,
     CommandResult,
     Config,
     Context,
     Job,
     Result,
     Step,
     StrPath,
 )
+from .utils import venv_bin_path, which
 
 LOG = logging.getLogger(__name__)
 
 
-def which(name: str, context: Context) -> str:
-    if platform.system() == "Windows":
-        bin_path = (context.venv / "Scripts").as_posix()
-    else:
-        bin_path = (context.venv / "bin").as_posix()
-    binary = shutil.which(name, path=bin_path)
-    if binary is None:
-        binary = shutil.which(name)
-        if binary is None:
-            return name
-    return binary
-
-
 def render_command(run: str, context: Context, config: Config) -> Sequence[str]:
     run = run.format(**config.values, python_version=context.python_version)
     cmd = shlex.split(run)
     cmd[0] = which(cmd[0], context)
     return tuple(cmd)
 
 
-async def run_command(command: Sequence[StrPath]) -> CommandResult:
+async def run_command(
+    command: Sequence[StrPath], context: Optional[Context] = None
+) -> CommandResult:
     cmd: Sequence[str] = [str(c) for c in command]
-    proc = await asyncio.create_subprocess_exec(*cmd, stdout=PIPE, stderr=PIPE)
+    new_env: Optional[Dict[str, str]] = None
+    if context:
+        new_env = os.environ.copy()
+        new_env["PATH"] = f"{venv_bin_path(context.venv)}{os.pathsep}{new_env['PATH']}"
+    proc = await asyncio.create_subprocess_exec(
+        *cmd, stdout=PIPE, stderr=PIPE, env=new_env
+    )
     stdout, stderr = await proc.communicate()
     assert proc.returncode is not None
-    cmd_str = " ".join(shlex.quote(arg) for arg in cmd)
-    LOG.debug("command `%s` finished with code %d", cmd_str, proc.returncode)
+    LOG.debug("command `%s` finished with code %d", shlex.join(cmd), proc.returncode)
 
     return CommandResult(
         proc.returncode, stdout.decode("utf-8"), stderr.decode("utf-8")
     )
 
 
 async def check_command(command: Sequence[StrPath]) -> CommandResult:
@@ -65,15 +59,15 @@
 
     return result
 
 
 @dataclass(frozen=True)
 class JobStep(Step):
     async def run(self) -> Result:
-        result = await run_command(self.cmd)
+        result = await run_command(self.cmd, self.context)
 
         return Result(
             step=self,
             context=self.context,
             exit_code=result.exit_code,
             stdout=result.stdout,
             stderr=result.stderr,
```

### Comparing `thx-0.5.1/thx/tests/cli.py` & `thx-0.6.0/thx/tests/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         ]
 
         for event in events:
             ctx = event.context
             live_mock.return_value.reset_mock()
             render(event)
 
-            self.assertIn(ctx, render.venvs)
-            self.assertEqual(event, render.venvs[ctx])
+            self.assertIn(ctx.venv, render.venvs)
+            self.assertEqual(event, render.venvs[ctx.venv])
             live_mock.return_value.update.assert_called_once()
 
     def test_render_job(self, live_mock: MagicMock) -> None:
         render = RichRenderer()
         event: Event
 
         job = Job("foo", ("/bin/true", "/bin/false"))
```

### Comparing `thx-0.5.1/thx/tests/config.py` & `thx-0.6.0/thx/tests/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,16 @@
 
     def test_complex_config(self) -> None:
         with fake_pyproject(
             """
             [tool.thx]
             default = ["test", "lint"]
             module = "foobar"
+            requirements = "requirements/dev.txt"
+            extras = "docs"
             watch_paths = ["foobar", "pyproject.toml"]
 
             [tool.thx.values]
             something = "else"
 
             [tool.thx.jobs]
             format = ["black {module}"]
@@ -200,14 +202,16 @@
                         ),
                     ),
                     "publish": Job(
                         name="publish", run=("flit publish",), requires=("test", "lint")
                     ),
                 },
                 values={"module": "foobar", "something": "else"},
+                requirements=["requirements/dev.txt"],
+                extras=["docs"],
                 watch_paths={Path("foobar"), Path("pyproject.toml")},
             )
             result = load_config(td)
             self.assertDictEqual(expected.jobs, result.jobs)
             self.assertDictEqual(expected.values, result.values)
             self.assertEqual(expected, result)
```

### Comparing `thx-0.5.1/thx/tests/context.py` & `thx-0.6.0/thx/tests/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2022 Amethyst Reese
 # Licensed under the MIT License
 
+import asyncio
 import platform
 import subprocess
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import AsyncIterator, List, Optional, Sequence, Tuple
 from unittest import TestCase
 from unittest.mock import call, Mock, patch
@@ -19,14 +20,15 @@
     Event,
     Options,
     StrPath,
     VenvCreate,
     VenvReady,
     Version,
 )
+from ..utils import venv_bin_path
 
 TEST_VERSIONS = [
     Version(v)
     for v in (
         "3.5",
         "3.6.5",
         "3.8",
@@ -112,16 +114,16 @@
     def test_find_runtime_no_venv_binary_found(
         self, runtime_mock: Mock, which_mock: Mock
     ) -> None:
         with TemporaryDirectory() as td:
             tdp = Path(td).resolve()
             config = Config(root=tdp)
 
-            which_mock.side_effect = (
-                lambda b: f"/fake/bin/{b}" if "." not in b else None
+            which_mock.side_effect = lambda b: (
+                f"/fake/bin/{b}" if "." not in b else None
             )
 
             for version in TEST_VERSIONS:
                 runtime_mock.reset_mock()
                 runtime_mock.side_effect = lambda b: version
                 which_mock.reset_mock()
 
@@ -223,29 +225,29 @@
             which_mock.side_effect = lambda b, path: f"{path}/{b}"
 
             for version in TEST_VERSIONS:
                 which_mock.reset_mock()
 
                 with self.subTest(version):
                     venv = context.venv_path(config, version)
-                    (venv / "bin").mkdir(parents=True, exist_ok=True)
+                    bin_dir = venv_bin_path(venv)
+                    bin_dir.mkdir(parents=True, exist_ok=True)
 
-                    expected = venv / "bin" / "python"
+                    expected = bin_dir / "python"
                     result, _ = context.find_runtime(version, venv)
                     self.assertEqual(expected, result)
 
                     which_mock.assert_has_calls(
                         [
                             call(
                                 "python",
-                                path=(venv / "bin").as_posix(),
+                                path=bin_dir.as_posix(),
                             ),
                         ]
                     )
-                    runtime_mock.assert_not_called()
 
     @patch("thx.context.find_runtime")
     def test_resolve_contexts_no_config(self, runtime_mock: Mock) -> None:
         with TemporaryDirectory() as td:
             tdp = Path(td).resolve()
             config = Config(root=tdp)
             active_version = Version(platform.python_version())
@@ -336,14 +338,16 @@
                 self.assertListEqual(expected, reqs)
 
     @async_test
     async def test_needs_update(self) -> None:
         with TemporaryDirectory() as td:
             tdp = Path(td).resolve()
 
+            pyproj = tdp / "pyproject.toml"
+            pyproj.write_text("\n")
             reqs = tdp / "requirements.txt"
             reqs.write_text("\n")
 
             venv = tdp / ".thx" / "venv" / "3.4"
             ctx = Context(Version("3.4"), venv / "bin" / "python", venv)
             config = Config(root=tdp)
 
@@ -351,14 +355,70 @@
                 self.assertTrue(context.needs_update(ctx, config))
 
             with self.subTest("fake venv"):
                 venv.mkdir(parents=True)
                 (venv / context.TIMESTAMP).write_text("0\n")
                 self.assertFalse(context.needs_update(ctx, config))
 
+            with self.subTest("touch pyproject.toml"):
+                await asyncio.sleep(0.01)
+                pyproj.write_text("\n\n")
+                self.assertTrue(context.needs_update(ctx, config))
+
+    @patch("thx.context.check_command")
+    @patch("thx.context.which")
+    @async_test
+    async def test_prepare_virtualenv_extras(
+        self, which_mock: Mock, run_mock: Mock
+    ) -> None:
+        self.maxDiff = None
+
+        async def fake_check_command(cmd: Sequence[StrPath]) -> CommandResult:
+            return CommandResult(0, "", "")
+
+        run_mock.side_effect = fake_check_command
+        which_mock.side_effect = lambda b, ctx: f"{ctx.venv / 'bin'}/{b}"
+
+        with TemporaryDirectory() as td:
+            tdp = Path(td).resolve()
+            venv = tdp / ".thx" / "venv" / "3.9"
+            venv.mkdir(parents=True)
+
+            config = Config(root=tdp, extras=["more"])
+            ctx = Context(Version("3.9"), venv / "bin" / "python", venv)
+            pip = which_mock("pip", ctx)
+            reqs = context.project_requirements(config)
+            self.assertEqual([], reqs)
+
+            events = [event async for event in context.prepare_virtualenv(ctx, config)]
+            expected = [
+                VenvCreate(ctx, "creating virtualenv"),
+                VenvCreate(ctx, "upgrading pip"),
+                VenvCreate(ctx, "installing project"),
+                VenvReady(ctx),
+            ]
+            self.assertEqual(expected, events)
+
+            run_mock.assert_has_calls(
+                [
+                    call(
+                        [
+                            ctx.python_path,
+                            "-m",
+                            "pip",
+                            "install",
+                            "-U",
+                            "pip",
+                            "setuptools",
+                        ]
+                    ),
+                    call([pip, "install", "-U", str(config.root) + "[more]"]),
+                ],
+            )
+
     @patch("thx.context.check_command")
     @patch("thx.context.which")
     @async_test
     async def test_prepare_virtualenv_live(
         self, which_mock: Mock, run_mock: Mock
     ) -> None:
         async def fake_check_command(cmd: Sequence[StrPath]) -> CommandResult:
@@ -393,15 +453,15 @@
                             "install",
                             "-U",
                             "pip",
                             "setuptools",
                         ]
                     ),
                     call([pip, "install", "-U", "-r", reqs]),
-                    call([pip, "install", "-U", config.root]),
+                    call([pip, "install", "-U", str(config.root)]),
                 ]
             )
 
             # should reuse virtualenv
             run_mock.reset_mock()
 
             expected = [VenvReady(ctx)]
```

### Comparing `thx-0.5.1/thx/tests/helper.py` & `thx-0.6.0/thx/tests/helper.py`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/thx/tests/runner.py` & `thx-0.6.0/thx/tests/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,32 @@
 # Copyright 2022 Amethyst Reese
 # Licensed under the MIT License
 
-import platform
 import sys
+from asyncio.subprocess import PIPE
 from pathlib import Path
 from unittest import skipIf, TestCase
-from unittest.mock import call, Mock, patch
+from unittest.mock import ANY, Mock, patch
 
 from .. import runner
 from ..types import CommandError, CommandResult, Config, Context, Job, Result, Version
+from ..utils import venv_bin_path
 from .helper import async_test
 
 
 class RunnerTest(TestCase):
-    @patch("thx.runner.shutil.which")
-    def test_which(self, which_mock: Mock) -> None:
-        context = Context(Version("3.10"), Path(), Path("/fake/venv"))
-        fake_venv_bin = (
-            "/fake/venv/Scripts" if platform.system() == "Windows" else "/fake/venv/bin"
-        )
-        with self.subTest("found"):
-            which_mock.side_effect = lambda b, path: f"/usr/bin/{b}"
-            self.assertEqual("/usr/bin/frobfrob", runner.which("frobfrob", context))
-            which_mock.assert_has_calls([call("frobfrob", path=fake_venv_bin)])
-
-        with self.subTest("not in venv"):
-            which_mock.side_effect = [None, "/usr/bin/scoop"]
-            self.assertEqual("/usr/bin/scoop", runner.which("scoop", context))
-            which_mock.assert_has_calls(
-                [
-                    call("scoop", path=fake_venv_bin),
-                    call("scoop"),
-                ]
-            )
-
-        with self.subTest("not found"):
-            which_mock.side_effect = None
-            which_mock.return_value = None
-            self.assertEqual("frobfrob", runner.which("frobfrob", context))
-            which_mock.assert_has_calls(
-                [
-                    call("frobfrob", path=fake_venv_bin),
-                    call("frobfrob"),
-                ]
-            )
-
     @patch("thx.runner.which")
     def test_render_command(self, which_mock: Mock) -> None:
         which_mock.return_value = "/opt/bin/frobfrob"
         config = Config(values={"module": "alpha"})
         context = Context(Version("3.8"), Path(), Path())
         result = runner.render_command("frobfrob check {module}.tests", context, config)
         self.assertEqual(("/opt/bin/frobfrob", "check", "alpha.tests"), result)
 
-    @patch("thx.runner.shutil.which", return_value=None)
+    @patch("thx.utils.shutil.which", return_value=None)
     def test_prepare_job(self, which_mock: Mock) -> None:
         config = Config(values={"module": "beta"})
         context = Context(Version("3.9"), Path(), Path())
         run = [
             "echo 'hello world'",
             "flake8 {module}",
             "python -m {module}.tests",
@@ -86,14 +55,26 @@
         exec_mock.return_value.communicate.return_value = b"nothing", b"error!"
 
         with patch("thx.runner.asyncio.create_subprocess_exec", exec_mock):
             result = await runner.run_command(("/fake/binary", "something"))
             expected = CommandResult(0, "nothing", "error!")
             self.assertEqual(expected, result)
 
+            ctx = Context(Version("3.8"), Path("/fake/python"), Path("/fake"))
+            result = await runner.run_command(("/fake/binary", "something"), ctx)
+            expected = CommandResult(0, "nothing", "error!")
+            self.assertEqual(expected, result)
+            exec_mock.assert_called_with(
+                "/fake/binary", "something", stdout=PIPE, stderr=PIPE, env=ANY
+            )
+            self.assertIn(
+                str(venv_bin_path(ctx.venv)),
+                exec_mock.call_args.kwargs["env"]["PATH"],
+            )
+
     @skipIf(sys.version_info < (3, 8), "no asyncmock on 3.7")
     @async_test
     async def test_check_command(self) -> None:
         from unittest.mock import AsyncMock
 
         exec_mock = AsyncMock()
         exec_mock.return_value.returncode = 0
```

### Comparing `thx-0.5.1/thx/tests/types.py` & `thx-0.6.0/thx/tests/types.py`

 * *Files identical despite different names*

### Comparing `thx-0.5.1/thx/types.py` & `thx-0.6.0/thx/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 class Config:
     root: Path = field(default_factory=Path.cwd)
     jobs: Mapping[str, Job] = field(default_factory=dict)
     default: Sequence[str] = field(default_factory=list)
     values: Mapping[str, str] = field(default_factory=dict)
     versions: Sequence[Version] = field(default_factory=list)
     requirements: Sequence[str] = field(default_factory=list)
+    extras: Sequence[str] = field(default_factory=list)
     watch_paths: Set[Path] = field(default_factory=set)
 
     def __post_init__(self) -> None:
         self.default = tuple(d.casefold() for d in self.default)
 
 
 @dataclass(unsafe_hash=True)
```

### Comparing `thx-0.5.1/thx/utils.py` & `thx-0.6.0/thx/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Copyright 2022 Amethyst Reese
 # Licensed under the MIT License
 
 import logging
+import platform
+import shutil
 from asyncio import iscoroutinefunction
 from dataclasses import dataclass, field, replace
 from functools import wraps
 from itertools import zip_longest
+from pathlib import Path
 from time import monotonic_ns
 from typing import Any, Callable, List, Optional, TypeVar
 
 from typing_extensions import ParamSpec
 
 from .types import Context, Job, Step, Version
 
@@ -105,14 +108,32 @@
     global TIMINGS
 
     result = list(sorted(TIMINGS))
     TIMINGS.clear()
     return result
 
 
+def venv_bin_path(venv: Path) -> Path:
+    if platform.system() == "Windows":
+        bin_path = venv / "Scripts"
+    else:
+        bin_path = venv / "bin"
+    return bin_path
+
+
+def which(name: str, context: Context) -> str:
+    bin_path = venv_bin_path(context.venv).as_posix()
+    binary = shutil.which(name, path=bin_path)
+    if binary is None:
+        binary = shutil.which(name)
+        if binary is None:
+            return name
+    return binary
+
+
 def version_match(versions: List[Version], target: Version) -> List[Version]:
     matches: List[Version] = []
     for version in versions:
         if all(
             v == t or t is None for v, t in zip_longest(version.release, target.release)
         ):
             if target.pre and target.pre != version.pre:
```

