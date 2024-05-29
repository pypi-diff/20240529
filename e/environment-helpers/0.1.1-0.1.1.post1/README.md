# Comparing `tmp/environment_helpers-0.1.1.tar.gz` & `tmp/environment_helpers-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "environment_helpers-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "environment_helpers-0.1.1.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `environment_helpers-0.1.1.tar` & `environment_helpers-0.1.1.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2024-03-26 01:01:19.504125 environment_helpers-0.1.1/LICENSE
--rw-r--r--   0        0        0      195 2024-03-27 18:15:42.865584 environment_helpers-0.1.1/README.md
--rw-r--r--   0        0        0     4020 2024-04-18 00:00:20.081702 environment_helpers-0.1.1/environment_helpers/__init__.py
--rw-r--r--   0        0        0      408 2024-04-18 00:00:11.678138 environment_helpers-0.1.1/environment_helpers/_scripts/call.py
--rw-r--r--   0        0        0      348 2024-03-26 03:25:02.457553 environment_helpers-0.1.1/environment_helpers/_scripts/launcher-kind.py
--rw-r--r--   0        0        0      188 2024-03-26 01:03:58.624127 environment_helpers-0.1.1/environment_helpers/_scripts/scheme.py
--rw-r--r--   0        0        0     2033 2024-03-26 03:23:13.784219 environment_helpers-0.1.1/environment_helpers/_scripts/system-scheme.py
--rw-r--r--   0        0        0      197 2024-03-25 22:17:38.794017 environment_helpers-0.1.1/environment_helpers/_scripts/version.py
--rw-r--r--   0        0        0     2112 2024-03-28 17:29:08.173170 environment_helpers-0.1.1/environment_helpers/build.py
--rw-r--r--   0        0        0     1013 2024-04-18 00:00:19.691692 environment_helpers-0.1.1/environment_helpers/install.py
--rw-r--r--   0        0        0     4842 2024-04-18 00:00:19.951699 environment_helpers-0.1.1/environment_helpers/introspect.py
--rw-r--r--   0        0        0     1780 2024-04-18 00:00:20.081702 environment_helpers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 environment_helpers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0      195 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/README.md
+-rw-r--r--   0        0        0     4026 2024-05-29 12:42:40.652855 environment_helpers-0.1.1.post1/environment_helpers/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/call.py
+-rw-r--r--   0        0        0      348 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/launcher-kind.py
+-rw-r--r--   0        0        0      188 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/scheme.py
+-rw-r--r--   0        0        0     2033 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/system-scheme.py
+-rw-r--r--   0        0        0      197 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/_scripts/version.py
+-rw-r--r--   0        0        0     2112 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/build.py
+-rw-r--r--   0        0        0     1013 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/install.py
+-rw-r--r--   0        0        0     4799 2024-05-29 12:42:27.075752 environment_helpers-0.1.1.post1/environment_helpers/introspect.py
+-rw-r--r--   0        0        0     1894 2024-05-29 12:42:40.652855 environment_helpers-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 environment_helpers-0.1.1.post1/PKG-INFO
```

### Comparing `environment_helpers-0.1.1/LICENSE` & `environment_helpers-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.1/environment_helpers/__init__.py` & `environment_helpers-0.1.1.post1/environment_helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Any, Collection, Literal, Optional, Protocol
 
 import environment_helpers.build
 import environment_helpers.install
 import environment_helpers.introspect
 
 
-__version__ = '0.1.1'
+__version__ = '0.1.1.post1'
 
 
 class Environment(Protocol):
     """Object representing a Python environment."""
 
     @property
     def base(self) -> pathlib.Path: ...
```

### Comparing `environment_helpers-0.1.1/environment_helpers/_scripts/system-scheme.py` & `environment_helpers-0.1.1.post1/environment_helpers/_scripts/system-scheme.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.1/environment_helpers/build.py` & `environment_helpers-0.1.1.post1/environment_helpers/build.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.1/environment_helpers/install.py` & `environment_helpers-0.1.1.post1/environment_helpers/install.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.1/environment_helpers/introspect.py` & `environment_helpers-0.1.1.post1/environment_helpers/introspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import os
 import pickle
 import subprocess
 import sys
 import sysconfig
 import warnings
 
-from collections.abc import Sequence
-from typing import Any, Callable, Dict, Literal, NamedTuple, Optional, TypedDict, TypeVar, Union
+from typing import Any, Callable, Literal, NamedTuple, Optional, TypedDict, TypeVar, Union
 
 
 if sys.version_info >= (3, 9):
     import importlib.resources as importlib_resources
 else:
     import importlib_resources
```

### Comparing `environment_helpers-0.1.1/pyproject.toml` & `environment_helpers-0.1.1.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['flit-core >= 3.4']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'environment-helpers'
-version = '0.1.1'
+version = '0.1.1.post1'
 description = 'Collection of helpers for managing Python environments'
 readme = 'README.md'
 requires-python = '>= 3.8'
 license.file = 'LICENSE'
 authors = [
   { name = 'Filipe Laíns', email = 'lains@riseup.net' },
 ]
@@ -27,14 +27,21 @@
 ]
 urls.homepage = 'https://github.com/FFY00/environment-helpers'
 urls.changelog = 'https://environment-helpers.readthedocs.io/en/stable/changelog.html'
 
 dependencies = [
   'build >= 0.5.0',
   'installer >= 0.5.0',
+  'importlib_resources >= 5.0; python_version < "3.10"',
+]
+
+[project.optional-dependencies]
+test = [
+  'pytest >= 7',
+  'podman >= 5',
 ]
 
 [tool.coverage.html]
 show_contexts = true
 
 [tool.mypy]
 files = 'src'
@@ -52,15 +59,14 @@
 [tool.ruff.lint]
 extend-select = [
   'W',    # pycodestyle
   'C90',  # mccabe
   'I',    # isort
   'UP',   # pyupgrade
   'YTT',  # flake8-2020
-  'B',    # flake8-bugbear
   'A',    # flake8-builtins
   'C4',   # flake8-comprehensions
   'T20',  # flake8-pyi
   'PT',   # flake8-pytest-style
   'PGH',  # pygrep-hooks
   'RUF',  # ruff
 ]
```

