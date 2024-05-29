# Comparing `tmp/pymeilisearch-0.3.1.tar.gz` & `tmp/pymeilisearch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeilisearch-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pymeilisearch-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pymeilisearch-0.3.1.tar` & `pymeilisearch-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1089 2023-10-11 14:38:52.773745 pymeilisearch-0.3.1/LICENSE
--rw-r--r--   0        0        0     4870 2023-10-11 14:38:52.773745 pymeilisearch-0.3.1/README.rst
--rw-r--r--   0        0        0     2140 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      317 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/__init__.py
--rw-r--r--   0        0        0      167 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/__main__.py
--rw-r--r--   0        0        0     4082 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/all_doc_indexer.py
--rw-r--r--   0        0        0     3797 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/cli.py
--rw-r--r--   0        0        0     3195 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/client.py
--rw-r--r--   0        0        0     5239 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/create_indexes.py
--rw-r--r--   0        0        0     5361 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/get_pages.py
--rw-r--r--   0        0        0     8273 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/scraper.py
--rw-r--r--   0        0        0     3761 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/server.py
--rw-r--r--   0        0        0     3852 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/__init__.py
--rw-r--r--   0        0        0      412 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/default.json
--rw-r--r--   0        0        0      644 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/sphinx_pydata.json
--rw-r--r--   0        0        0     1349 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/utils.py
--rw-r--r--   0        0        0     3665 2023-10-11 14:38:52.777745 pymeilisearch-0.3.1/src/ansys/tools/meilisearch/utils.py
--rw-r--r--   0        0        0     6742 1970-01-01 00:00:00.000000 pymeilisearch-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-29 09:03:39.345649 pymeilisearch-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4870 2024-05-29 09:03:39.345649 pymeilisearch-0.3.2/README.rst
+-rw-r--r--   0        0        0     2143 2024-05-29 09:03:39.345649 pymeilisearch-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      317 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/__init__.py
+-rw-r--r--   0        0        0      167 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/__main__.py
+-rw-r--r--   0        0        0     4083 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/all_doc_indexer.py
+-rw-r--r--   0        0        0     3798 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/cli.py
+-rw-r--r--   0        0        0     3196 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/client.py
+-rw-r--r--   0        0        0     5240 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/create_indexes.py
+-rw-r--r--   0        0        0     5362 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/get_pages.py
+-rw-r--r--   0        0        0     8274 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/scraper.py
+-rw-r--r--   0        0        0     3761 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/server.py
+-rw-r--r--   0        0        0     3853 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/default.json
+-rw-r--r--   0        0        0      644 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/sphinx_pydata.json
+-rw-r--r--   0        0        0     1350 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/utils.py
+-rw-r--r--   0        0        0     3666 2024-05-29 09:03:39.349649 pymeilisearch-0.3.2/src/ansys/tools/meilisearch/utils.py
+-rw-r--r--   0        0        0     6745 1970-01-01 00:00:00.000000 pymeilisearch-0.3.2/PKG-INFO
```

### Comparing `pymeilisearch-0.3.1/LICENSE` & `pymeilisearch-0.3.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 ANSYS, Inc. All rights reserved.
+Copyright (c) 2023-2024 ANSYS, Inc. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymeilisearch-0.3.1/README.rst` & `pymeilisearch-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.3.1/pyproject.toml` & `pymeilisearch-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pymeilisearch"
-version = "0.3.1"
+version = "0.3.2"
 description = " A Python library for effortless indexing and searching of documentation using MeiliSearch."
 readme = "README.rst"
-requires-python = ">=3.8,<4"
+requires-python = ">=3.9,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys Core Team", email = "pyansys.core@ansys.com"},
 ]
@@ -24,34 +24,34 @@
 ]
 dependencies = [
     "importlib-metadata>=4.0",
     "PyGithub>=1.58.0",
     "jinja2>=3.1.2",
     "meilisearch>=0.24.0",
     "click>=8",
-    "pymeilisearch-scraper>=0.2.3",
+    "pymeilisearch-scraper>=0.2.3,<3",
     "pyOpenSSL>=23.2.0",
     "cryptography>=41.0.4",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.4.2",
-    "pytest-cov==4.1.0",
-    "docker==6.1.3",
+    "pytest==8.2.1",
+    "pytest-cov==5.0.0",
+    "docker==7.1.0",
 ]
 doc = [
-    "ansys-sphinx-theme==0.12.3",
-    "numpydoc==1.6.0",
+    "ansys-sphinx-theme==0.16.2",
+    "numpydoc==1.7.0",
     "Sphinx==6.2.1",
-    "sphinx-design==0.5.0",
+    "sphinx-design==0.6.0",
     "sphinx-jinja==2.0.2",
-    "sphinx-autoapi==3.0.0",
+    "sphinx-autoapi==3.1.1",
     "sphinx-copybutton==0.5.2",
-    "sphinx-notfound-page==1.0.0",
+    "sphinx-notfound-page==1.0.2",
     "sphinx-jinja==2.0.2",
 ]
 
 [tool.flit.module]
 name = "ansys.tools.meilisearch"
 
 [project.scripts]
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/all_doc_indexer.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/all_doc_indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for indexing all public documents in Meilisearch."""
+
 from typing import List
 
 import requests
 
 from ansys.tools.meilisearch.client import MeilisearchClient
 from ansys.tools.meilisearch.utils import MeilisearchUtils
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/cli.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PyMeilisearch CLI module."""
+
 import os
 import pathlib
 
 import click
 
 from ansys.tools.meilisearch import __version__
 from ansys.tools.meilisearch.create_indexes import (
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/client.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module providing the Meilisearch client."""
+
 import os
 
 from meilisearch import Client
 
 
 class BaseClient:
     """Provides the base class for the Meilisearch client."""
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/create_indexes.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/create_indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Create an index for each public GitHub page for each repository in
 one or more organizations using Sphinx.
 """
+
 import os
 
 from ansys.tools.meilisearch.client import MeilisearchClient
 from ansys.tools.meilisearch.get_pages import GitHubPages
 from ansys.tools.meilisearch.scraper import WebScraper
 from ansys.tools.meilisearch.templates.utils import is_sphinx
 from ansys.tools.meilisearch.utils import MeilisearchUtils
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/get_pages.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/get_pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Query for public GitHub pages.
 """
+
 import os
 import urllib.request
 import warnings
 
 from github import Auth, Github
 import requests
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/scraper.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for scaping web pages."""
+
 import contextlib
 import io
 import os
 import tempfile
 
 import requests
 from scraper.src.index import run_config
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/server.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/server.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/__init__.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PyMeilisearch templates subpackage."""
+
 import json
 import pathlib
 from typing import Union
 
 from jinja2 import Template
 
 DEFAULT_TEMPLATE = pathlib.Path(__file__).parent.resolve() / "default.json"
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/sphinx_pydata.json` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/sphinx_pydata.json`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/templates/utils.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/templates/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Templates utilities module."""
+
 import re
 
 import requests
 
 
 def get_template(url: str) -> str:
     """
```

### Comparing `pymeilisearch-0.3.1/src/ansys/tools/meilisearch/utils.py` & `pymeilisearch-0.3.2/src/ansys/tools/meilisearch/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides utilities for Meilisearch."""
+
 import json
 import time
 from typing import List
 
 import requests
 
 from ansys.tools.meilisearch.client import MeilisearchClient
```

### Comparing `pymeilisearch-0.3.1/PKG-INFO` & `pymeilisearch-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pymeilisearch
-Version: 0.3.1
+Version: 0.3.2
 Summary:  A Python library for effortless indexing and searching of documentation using MeiliSearch.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys Core Team <pyansys.core@ansys.com>
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: PyGithub>=1.58.0
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: meilisearch>=0.24.0
 Requires-Dist: click>=8
-Requires-Dist: pymeilisearch-scraper>=0.2.3
+Requires-Dist: pymeilisearch-scraper>=0.2.3,<3
 Requires-Dist: pyOpenSSL>=23.2.0
 Requires-Dist: cryptography>=41.0.4
-Requires-Dist: ansys-sphinx-theme==0.12.3 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.16.2 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
-Requires-Dist: sphinx-design==0.5.0 ; extra == "doc"
+Requires-Dist: sphinx-design==0.6.0 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
-Requires-Dist: sphinx-autoapi==3.0.0 ; extra == "doc"
+Requires-Dist: sphinx-autoapi==3.1.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: sphinx-notfound-page==1.0.0 ; extra == "doc"
+Requires-Dist: sphinx-notfound-page==1.0.2 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
-Requires-Dist: pytest==7.4.2 ; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
-Requires-Dist: docker==6.1.3 ; extra == "tests"
+Requires-Dist: pytest==8.2.1 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
+Requires-Dist: docker==7.1.0 ; extra == "tests"
 Project-URL: Discussions, https://github.com/ansys/pymeilisearch/discussions
 Project-URL: Documentation, https://pymeilisearch.docs.ansys.com
 Project-URL: Homepage, https://github.com/ansys/pymeilisearch
 Project-URL: Releases, https://github.com/ansys/pymeilisearch/releases
 Project-URL: Source, https://github.com/ansys/pymeilisearch
 Project-URL: Tracker, https://github.com/ansys/pymeilisearch/issues
 Provides-Extra: doc
```

