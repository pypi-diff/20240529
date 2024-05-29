# Comparing `tmp/screenpy-4.2.4.tar.gz` & `tmp/screenpy-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy-4.2.4.tar", max compression
+gzip compressed data, was "screenpy-4.2.5.tar", max compression
```

## Comparing `screenpy-4.2.4.tar` & `screenpy-4.2.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0     1071 2024-02-21 18:24:47.255412 screenpy-4.2.4/LICENSE
--rw-r--r--   0        0        0     2845 2024-02-21 18:24:47.255412 screenpy-4.2.4/README.md
--rw-r--r--   0        0        0     6973 2024-02-21 18:24:47.255412 screenpy-4.2.4/pyproject.toml
--rw-r--r--   0        0        0     2355 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/__init__.py
--rw-r--r--   0        0        0      730 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/__version__.py
--rw-r--r--   0        0        0     2198 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/__init__.py
--rw-r--r--   0        0        0     1134 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/attach_the_file.py
--rw-r--r--   0        0        0     1504 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/debug.py
--rw-r--r--   0        0        0     3409 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/either.py
--rw-r--r--   0        0        0     6177 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/eventually.py
--rw-r--r--   0        0        0     1437 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/log.py
--rw-r--r--   0        0        0     2739 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/make_note.py
--rw-r--r--   0        0        0     3078 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/pause.py
--rw-r--r--   0        0        0     2450 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/see.py
--rw-r--r--   0        0        0     2265 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/see_all_of.py
--rw-r--r--   0        0        0     2670 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/see_any_of.py
--rw-r--r--   0        0        0     3023 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actions/silently.py
--rw-r--r--   0        0        0     9376 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/actor.py
--rw-r--r--   0        0        0     5066 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/configuration.py
--rw-r--r--   0        0        0      938 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/directions.py
--rw-r--r--   0        0        0     1231 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/director.py
--rw-r--r--   0        0        0     1335 2024-02-21 18:24:47.255412 screenpy-4.2.4/screenpy/exceptions.py
--rw-r--r--   0        0        0     1413 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/given_when_then.py
--rw-r--r--   0        0        0      367 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/narration/__init__.py
--rw-r--r--   0        0        0      293 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/narration/gravitas.py
--rw-r--r--   0        0        0     9742 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/narration/narrator.py
--rw-r--r--   0        0        0      275 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/narration/stdout_adapter/__init__.py
--rw-r--r--   0        0        0      877 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/narration/stdout_adapter/configuration.py
--rw-r--r--   0        0        0     5073 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/narration/stdout_adapter/stdout_adapter.py
--rw-r--r--   0        0        0     4442 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/pacing.py
--rw-r--r--   0        0        0     4345 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/protocols.py
--rw-r--r--   0        0        0       39 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/py.typed
--rw-r--r--   0        0        0     2593 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/__init__.py
--rw-r--r--   0        0        0     3858 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/base_resolution.py
--rw-r--r--   0        0        0     1059 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/contains_item_matching.py
--rw-r--r--   0        0        0     2845 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/contains_the_entry.py
--rw-r--r--   0        0        0      956 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/contains_the_item.py
--rw-r--r--   0        0        0      966 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/contains_the_key.py
--rw-r--r--   0        0        0      862 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/contains_the_text.py
--rw-r--r--   0        0        0      976 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/contains_the_value.py
--rw-r--r--   0        0        0       39 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/custom_matchers/__init__.py
--rw-r--r--   0        0        0     3019 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/custom_matchers/is_in_bounds.py
--rw-r--r--   0        0        0     1800 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py
--rw-r--r--   0        0        0      889 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/ends_with.py
--rw-r--r--   0        0        0      868 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/has_length.py
--rw-r--r--   0        0        0      893 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_close_to.py
--rw-r--r--   0        0        0      611 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_empty.py
--rw-r--r--   0        0        0      845 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_equal_to.py
--rw-r--r--   0        0        0      885 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_greater_than.py
--rw-r--r--   0        0        0      985 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_greater_than_or_equal_to.py
--rw-r--r--   0        0        0     1769 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_in_range.py
--rw-r--r--   0        0        0      874 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_less_than.py
--rw-r--r--   0        0        0      958 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_less_than_or_equal_to.py
--rw-r--r--   0        0        0      959 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/is_not.py
--rw-r--r--   0        0        0      864 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/matches.py
--rw-r--r--   0        0        0      832 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/reads_exactly.py
--rw-r--r--   0        0        0      887 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/resolutions/starts_with.py
--rw-r--r--   0        0        0     2514 2024-02-21 18:24:47.259412 screenpy-4.2.4/screenpy/speech_tools.py
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 screenpy-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-29 15:03:14.903309 screenpy-4.2.5/LICENSE
+-rw-r--r--   0        0        0     2852 2024-05-29 15:03:14.903309 screenpy-4.2.5/README.md
+-rw-r--r--   0        0        0     7036 2024-05-29 15:03:14.903309 screenpy-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2355 2024-05-29 15:03:14.903309 screenpy-4.2.5/screenpy/__init__.py
+-rw-r--r--   0        0        0      730 2024-05-29 15:03:14.903309 screenpy-4.2.5/screenpy/__version__.py
+-rw-r--r--   0        0        0     2259 2024-05-29 15:03:14.903309 screenpy-4.2.5/screenpy/actions/__init__.py
+-rw-r--r--   0        0        0     1226 2024-05-29 15:03:14.903309 screenpy-4.2.5/screenpy/actions/attach_the_file.py
+-rw-r--r--   0        0        0     1504 2024-05-29 15:03:14.903309 screenpy-4.2.5/screenpy/actions/debug.py
+-rw-r--r--   0        0        0     3239 2024-05-29 15:03:14.903309 screenpy-4.2.5/screenpy/actions/either.py
+-rw-r--r--   0        0        0     5373 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/eventually.py
+-rw-r--r--   0        0        0     1534 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/log.py
+-rw-r--r--   0        0        0     2779 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/make_note.py
+-rw-r--r--   0        0        0     2919 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/pause.py
+-rw-r--r--   0        0        0     2604 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/see.py
+-rw-r--r--   0        0        0     2265 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/see_all_of.py
+-rw-r--r--   0        0        0     2670 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/see_any_of.py
+-rw-r--r--   0        0        0     3023 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/silently.py
+-rw-r--r--   0        0        0     3418 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actions/stop.py
+-rw-r--r--   0        0        0     6536 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/actor.py
+-rw-r--r--   0        0        0     5066 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/configuration.py
+-rw-r--r--   0        0        0      938 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/directions.py
+-rw-r--r--   0        0        0     1231 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/director.py
+-rw-r--r--   0        0        0     1335 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/exceptions.py
+-rw-r--r--   0        0        0     1413 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/given_when_then.py
+-rw-r--r--   0        0        0      367 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/narration/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/narration/gravitas.py
+-rw-r--r--   0        0        0     9742 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/narration/narrator.py
+-rw-r--r--   0        0        0      275 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/narration/stdout_adapter/__init__.py
+-rw-r--r--   0        0        0      877 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/narration/stdout_adapter/configuration.py
+-rw-r--r--   0        0        0     5073 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/narration/stdout_adapter/stdout_adapter.py
+-rw-r--r--   0        0        0     4442 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/pacing.py
+-rw-r--r--   0        0        0     4345 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/protocols.py
+-rw-r--r--   0        0        0       39 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/py.typed
+-rw-r--r--   0        0        0     2593 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/__init__.py
+-rw-r--r--   0        0        0     3858 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/base_resolution.py
+-rw-r--r--   0        0        0     1059 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/contains_item_matching.py
+-rw-r--r--   0        0        0     3052 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/contains_the_entry.py
+-rw-r--r--   0        0        0     1132 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/contains_the_item.py
+-rw-r--r--   0        0        0     1141 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/contains_the_key.py
+-rw-r--r--   0        0        0      960 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/contains_the_text.py
+-rw-r--r--   0        0        0     1153 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/contains_the_value.py
+-rw-r--r--   0        0        0       39 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/custom_matchers/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/custom_matchers/is_in_bounds.py
+-rw-r--r--   0        0        0     1800 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py
+-rw-r--r--   0        0        0      990 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/ends_with.py
+-rw-r--r--   0        0        0      991 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/has_length.py
+-rw-r--r--   0        0        0      893 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_close_to.py
+-rw-r--r--   0        0        0      611 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_empty.py
+-rw-r--r--   0        0        0     1042 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_equal_to.py
+-rw-r--r--   0        0        0     1067 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_greater_than.py
+-rw-r--r--   0        0        0     1167 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_greater_than_or_equal_to.py
+-rw-r--r--   0        0        0     1965 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_in_range.py
+-rw-r--r--   0        0        0     1075 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_less_than.py
+-rw-r--r--   0        0        0     1159 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_less_than_or_equal_to.py
+-rw-r--r--   0        0        0     1058 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/is_not.py
+-rw-r--r--   0        0        0     1460 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/matches.py
+-rw-r--r--   0        0        0      930 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/reads_exactly.py
+-rw-r--r--   0        0        0      987 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/resolutions/starts_with.py
+-rw-r--r--   0        0        0     2581 2024-05-29 15:03:14.907309 screenpy-4.2.5/screenpy/speech_tools.py
+-rw-r--r--   0        0        0     5588 1970-01-01 00:00:00.000000 screenpy-4.2.5/PKG-INFO
```

### Comparing `screenpy-4.2.4/LICENSE` & `screenpy-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/README.md` & `screenpy-4.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ScreenPy
 ========
+
 [![Build Status](../../actions/workflows/tests.yml/badge.svg)](../../actions/workflows/tests.yml)
 [![Build Status](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)
 
 [![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy.svg)](https://pypi.org/project/screenpy)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -49,25 +50,25 @@
 
 Installation
 ------------
     pip install screenpy
 
 
 Documentation
-----------
+-------------
 Please check out the [Read The Docs documentation](https://screenpy-docs.readthedocs.io/en/latest/) for the latest information about this module!
 
 
 Contributing
 ------------
 You want to contribute? Great! Here are the things you should do before submitting your PR:
 
 1. Fork the repo and git clone your fork.
 1. `dev` install the project package:
-   1. `pip install -e .[dev]` 
-   1. Optional (poetry users):
-      1. `poetry install --extras dev`
+    1. `pip install -e .[dev]`
+    1. Optional (poetry users):
+        1. `poetry install --extras dev`
 1. Run `pre-commit install` once.
 1. Run `tox` to perform tests frequently.
 1. Create pull-request from your branch.
 
 That's it! :)
```

### Comparing `screenpy-4.2.4/pyproject.toml` & `screenpy-4.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     "EM101", "EM102",
     "TCH001", "TCH002", "TCH003", "TCH004",
     "C419",
     "D200", "D205", "D415",
     "PT003", "PT006", "PT018",
     "RET504",
     "UP006", "UP007",
+    "W291",
 ]
 
 [tool.ruff.lint.flake8-pytest-style]
 mark-parentheses = false
 
 [tool.ruff.lint.pycodestyle]
 ignore-overlong-task-comments = true
@@ -133,15 +134,15 @@
 "tests/test_pacing.py" = [
     "FA100",  # we are purposely testing pacing without future annotations.
 ]
 
 
 [tool.poetry]
 name = "screenpy"
-version = "4.2.4"
+version = "4.2.5"
 description = "Screenplay pattern base for Python automated test suites."
 authors = ["Perry Goy <perry.goy@gmail.com>"]
 maintainers = ["Gabe Langton", "Marcel Wilson"]
 license = "MIT"
 repository = "https://github.com/ScreenPyHQ/screenpy"
 documentation = "https://screenpy-docs.readthedocs.io"
 readme = "README.md"
@@ -158,78 +159,78 @@
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: BDD",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
 ]
 
-
 # It's possible to add optional dependencies with the poetry CLI tool using:
 #   poetry add --optional some_dev_pkg
 # This will set `optional = true` flag in [tool.poetry.dependencies], as seen below
 # But then you need to remember to manually edit the [tool.poetry.extras] dev section
 # and declare the package. This allows `pip install .[dev]` to work as expected
 # Poetry users will need to use the `--extras dev` option rather than the `--with dev`
 # so we dont have two different sets of package versions to update.
 
-
 [tool.poetry.dependencies]
 python = "^3.8"
 
 importlib_metadata = {version = "*", python = "3.8.*"}
 pydantic = "*"
 pydantic-settings = "*"
 PyHamcrest = ">=2.0.0"
 tomli = {version = ">=2.0.1", python = "<3.11"}
 typing_extensions = ">=4.8.0"
 
 # convenience packages for development
-autodoc-pydantic = {version = "*", optional = true}
 black = {version = "*", optional = true}
 coverage = {version = "*", optional = true}
+cruft = {version = "*", optional = true}
 mypy = {version = "*", optional = true}
 pre-commit = {version = "*", optional = true}
 pytest = {version = "*", optional = true}
 pytest-mock = {version = "*", optional = true}
-ruff = {version = ">=0.1.13", optional = true}
+ruff = {version = ">=0.2.0", optional = true}
+sphinx = {version = "*", optional = true}
+sphinx-rtd-theme = {version = "*", optional = true}
+tox = {version = "*", optional = true}
+
+autodoc-pydantic = {version = "*", optional = true}
 screenpy-adapter_allure = {version = "^4.0.1", optional = true}
 screenpy-appium = {version = "*", optional = true}
 screenpy-playwright = {version = "*", optional = true}
 screenpy-pyotp = {version = "^4.0.1", optional = true}
 screenpy-requests = {version = "^4.0.1", optional = true}
 screenpy-selenium = {version = "^4.0.3", optional = true}
-sphinx = {version = "*", optional = true}
-sphinx-rtd-theme = {version = "*", optional = true}
-tox = {version = "*", optional = true}
-
 
 [tool.poetry.extras]
-allure = ["screenpy-adapter-allure"]
-appium = ["screenpy-appium"]
-playwright = ["screenpy-playwright"]
-pyotp = ["screenpy-pyotp"]
-requests = ["screenpy-requests"]
-selenium = ["screenpy-selenium"]
 dev = [
     "autodoc-pydantic",
     "black",
     "coverage",
+    "cruft",
     "mypy",
     "pre-commit",
-    "pytest-mock",
     "pytest",
+    "pytest-mock",
     "ruff",
     "sphinx",
     "sphinx-rtd-theme",
     "tox",
 ]
 test = [
     "coverage",
-    "pytest-mock",
     "pytest",
+    "pytest-mock",
 ]
 docs = [
     "autodoc-pydantic",
     "sphinx",
     "sphinx-rtd-theme",
 ]
 
+allure = ["screenpy-adapter-allure"]
+appium = ["screenpy-appium"]
+playwright = ["screenpy-playwright"]
+pyotp = ["screenpy-pyotp"]
+requests = ["screenpy-requests"]
+selenium = ["screenpy-selenium"]
```

### Comparing `screenpy-4.2.4/screenpy/__init__.py` & `screenpy-4.2.5/screenpy/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/__version__.py` & `screenpy-4.2.5/screenpy/__version__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/actions/__init__.py` & `screenpy-4.2.5/screenpy/actions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from .log import Log
 from .make_note import MakeNote
 from .pause import Pause
 from .see import See
 from .see_all_of import SeeAllOf
 from .see_any_of import SeeAnyOf
 from .silently import Silently
+from .stop import Stop
 
 # Natural-language-enabling syntactic sugar
 AttachFile = AttachAFile = AttachTheFile
 AttachesFile = AttachesAFile = AttachesTheFile = AttachTheFile
 Observe = Verify = Confirm = Assert = See
 Observes = Verifies = Confirms = Asserts = Sees = See
 ObserveAllOf = VerifyAllOf = ConfirmAllOf = AssertAllOf = SeeAllOf
 ObservesAllOf = VerifiesAllOf = ConfirmsAllOf = AssertsAllOf = SeesAllOf = SeeAllOf
 ObserveAnyOf = VerifyAnyOf = ConfirmAnyOf = AssertAnyOf = SeeAnyOf
 ObservesAnyOf = VerifiesAnyOf = ConfirmsAnyOf = AssertsAnyOf = SeesAnyOf = SeeAnyOf
 Quietly = Silently
 Sleep = Pause
 Sleeps = Pauses = Pause
+Stops = Stop
 TakeNote = MakeNote
 TakesNote = MakesNote = MakeNote
 Attempts = AttemptsTo = GoesFor = Tries = TriesTo = Either
 TryTo = Attempt = AttemptTo = GoFor = Try = Either
 
 
 __all__ = [
@@ -75,14 +77,16 @@
     "SeeAnyOf",
     "Sees",
     "SeesAllOf",
     "SeesAnyOf",
     "Silently",
     "Sleep",
     "Sleeps",
+    "Stop",
+    "Stops",
     "TakeNote",
     "TakesNote",
     "Tries",
     "TriesTo",
     "Try",
     "TryTo",
     "Verifies",
```

### Comparing `screenpy-4.2.4/screenpy/actions/attach_the_file.py` & `screenpy-4.2.5/screenpy/actions/attach_the_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,25 @@
         the_actor.attempts_to(AttachTheFile(filepath))
 
         the_actor.attempts_to(
             AttachTheFile(filepath, attachment_type=AttachmentTypes.PNG)
         )
     """
 
+    @property
+    def filename(self) -> str:
+        """Get the filename from the filepath."""
+        return os.path.basename(self.filepath)
+
     def describe(self) -> str:
         """Describe the Action in present tense."""
         return f"Attach a file named {self.filename}."
 
     # no beat, to make reading reports easier.
     def perform_as(self, _: Actor) -> None:
         """Direct the Narrator to attach a file."""
         the_narrator.attaches_a_file(self.filepath, **self.attach_kwargs)
 
     # ANN401 ignored here to allow for new adapters to use any kwargs.
     def __init__(self, filepath: str, **kwargs: Any) -> None:  # noqa: ANN401
         self.filepath = filepath
-        self.filename = os.path.basename(filepath)
         self.attach_kwargs = kwargs
```

### Comparing `screenpy-4.2.4/screenpy/actions/debug.py` & `screenpy-4.2.5/screenpy/actions/debug.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/actions/either.py` & `screenpy-4.2.5/screenpy/actions/either.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class Either:
     """Perform one of two branching performances.
 
     Simulates a try/except block while still following Screenplay Pattern.
 
     By default, ``Either`` catches AssertionErrors, so you can use
     :class:`~screenpy.actions.See` to decide which path to follow. Use the
-    :meth:`~screenpy.actions.Either.ignoring` method to ignore other exceptions.
+    :meth:`ignoring` method to ignore other exceptions.
 
     Examples::
 
         the_actor.will(Either(DoAction()).or_(DoDifferentAction())
 
         the_actor.will(
             Either(DoAction()).otherwise(DoDifferentAction()).ignoring(
@@ -42,41 +42,23 @@
             Either(CheckIfOnDomain(URL())).or_(Open.their_browser_on(URL())
         )
     """
 
     except_performables: tuple[Performable, ...]
     ignore_exceptions: tuple[type[BaseException], ...]
 
-    def perform_as(self, the_actor: Actor) -> None:
-        """Direct the Actor to perform one of two performances."""
-        # kinking the cable before the attempt
-        # avoids explaning what the actor tries to do.
-        # logs the first attempt only if it succeeds
-        # or if UNABRIDGED_NARRATION is enabled
-        with the_narrator.mic_cable_kinked():
-            try:
-                the_actor.will(*self.try_performables)
-            except self.ignore_exceptions:
-                if not settings.UNABRIDGED_NARRATION:
-                    the_narrator.clear_backup()
-            else:
-                return
-
-        the_actor.will(*self.except_performables)
-        return
-
     def or_(self, *except_performables: Performable) -> Self:
         """Provide the alternative routine to perform.
 
         Aliases:
-            * :meth:`~screenpy.actions.Either.except_`
-            * :meth:`~screenpy.actions.Either.else_`
-            * :meth:`~screenpy.actions.Either.otherwise`
-            * :meth:`~screenpy.actions.Either.alternatively`
-            * :meth:`~screenpy.actions.Either.failing_that`
+            * ``except_``
+            * ``else_``
+            * ``otherwise``
+            * ``alternatively``
+            * ``failing_that``
         """
         self.except_performables = except_performables
         return self
 
     except_ = else_ = otherwise = alternatively = failing_that = or_
 
     def ignoring(self, *ignored_exceptions: type[BaseException]) -> Self:
@@ -91,10 +73,28 @@
         )
         except_summary = ", ".join(
             get_additive_description(action) for action in self.except_performables
         )
 
         return f"Either {try_summary} or {except_summary}"
 
+    def perform_as(self, the_actor: Actor) -> None:
+        """Direct the Actor to perform one of two performances."""
+        # kinking the cable before the attempt
+        # avoids explaning what the actor tries to do.
+        # logs the first attempt only if it succeeds
+        # or if UNABRIDGED_NARRATION is enabled
+        with the_narrator.mic_cable_kinked():
+            try:
+                the_actor.will(*self.try_performables)
+            except self.ignore_exceptions:
+                if not settings.UNABRIDGED_NARRATION:
+                    the_narrator.clear_backup()
+            else:
+                return
+
+        the_actor.will(*self.except_performables)
+        return
+
     def __init__(self, *first: Performable) -> None:
         self.try_performables: tuple[Performable, ...] = first
         self.ignore_exceptions = (AssertionError,)
```

### Comparing `screenpy-4.2.4/screenpy/actions/eventually.py` & `screenpy-4.2.5/screenpy/actions/eventually.py`

 * *Files 17% similar despite different names*

```diff
@@ -77,49 +77,38 @@
             """Just in case the author forgets to use a unit method."""
             the_actor.attempts_to(self.eventually)
 
     def for_(self, amount: float) -> _TimeframeBuilder:
         """Set for how long the actor should continue trying.
 
         Aliases:
-            * :meth:`~screenpy.actions.Eventually.trying_for_no_longer_than`
-            * :meth:`~screenpy.actions.Eventually.trying_for`
-            * :meth:`~screenpy.actions.Eventually.waiting_for`
+            * ``trying_for_no_longer_than``
+            * ``trying_for``
+            * ``waiting_for``
         """
         return self._TimeframeBuilder(self, amount, "timeout")
 
-    def trying_for_no_longer_than(self, amount: float) -> _TimeframeBuilder:
-        """Alias for :meth:`~screenpy.actions.Eventually.for_`."""
-        return self.for_(amount)
-
-    def trying_for(self, amount: float) -> _TimeframeBuilder:
-        """Alias for :meth:`~screenpy.actions.Eventually.for_`."""
-        return self.for_(amount)
-
-    def waiting_for(self, amount: float) -> _TimeframeBuilder:
-        """Alias for :meth:`~screenpy.actions.Eventually.for_`."""
-        return self.for_(amount)
+    trying_for_no_longer_than = trying_for = waiting_for = for_
 
     def polling(self, amount: float) -> _TimeframeBuilder:
         """Adjust the polling frequency.
 
         Aliases:
-            * :meth:`~screenpy.actions.Eventually.polling_every`
-            * :meth:`~screenpy.actions.Eventually.trying_every`
+            * ``polling_every``
+            * ``trying_every``
         """
         self.poll = amount
         return self._TimeframeBuilder(self, amount, "poll")
 
-    def polling_every(self, amount: float) -> _TimeframeBuilder:
-        """Alias for :meth:`~screenpy.actions.Eventually.polling`."""
-        return self.polling(amount)
-
-    def trying_every(self, amount: float) -> _TimeframeBuilder:
-        """Alias for :meth:`~screenpy.actions.Eventually.polling`."""
-        return self.polling(amount)
+    polling_every = trying_every = polling
+
+    @property
+    def performable_to_log(self) -> str:
+        """Represent the Performable in a log-friendly way."""
+        return get_additive_description(self.performable)
 
     def describe(self) -> str:
         """Describe the Action in present tense."""
         return f"Eventually {self.performable_to_log}."
 
     @beat("{} tries to {performable_to_log}, eventually.")
     def perform_as(self, the_actor: Actor) -> None:
@@ -155,15 +144,14 @@
             f"{the_actor} tried to Eventually {self.performable_to_log} {count} times"
             f" over {self.timeout} seconds, but got:\n    {unique_errors_message}"
         )
         raise DeliveryError(msg) from self.caught_error
 
     def __init__(self, performable: Performable) -> None:
         self.performable = performable
-        self.performable_to_log = get_additive_description(self.performable)
         self.caught_error = None
         self.unique_errors: list[BaseException] = []
         self.timeout = settings.TIMEOUT
         self.poll = settings.POLLING
 
 
 def same_exception(exc1: BaseException, exc2: BaseException) -> bool:
```

### Comparing `screenpy-4.2.4/screenpy/actions/log.py` & `screenpy-4.2.5/screenpy/actions/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,19 +29,23 @@
     """
 
     @classmethod
     def the(cls, question: T_Q) -> Self:
         """Supply the Question to answer."""
         return cls(question)
 
+    @property
+    def question_to_log(self) -> str:
+        """Represent the Question in a log-friendly way."""
+        return get_additive_description(self.question)
+
     @beat("{} examines {question_to_log}.")
     def perform_as(self, the_actor: Actor) -> None:
         """Direct the Actor to announce the answer to the Question."""
         if isinstance(self.question, Answerable):
             self.question.answered_by(the_actor)
         else:
             # must be a value instead of a Question!
             aside(f"the value is: {represent_prop(self.question)}")
 
     def __init__(self, question: T_Q) -> None:
         self.question = question
-        self.question_to_log = get_additive_description(self.question)
```

### Comparing `screenpy-4.2.4/screenpy/actions/make_note.py` & `screenpy-4.2.5/screenpy/actions/make_note.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,40 +33,46 @@
             MakeNote.of_the(Number.of(BALLOONS)).as_("excitement gauge"),
         )
 
         the_actor.attempts_to(MakeNote.of_the(items).as_("items list"))
     """
 
     key: str | None
-    key_to_log: str | None
     question: T_Q
 
     @classmethod
     def of(cls, question: T_Q) -> Self:
         """Supply the Question to answer and its arguments.
 
         Aliases:
-            * :meth:`~screenpy.actions.MakeNote.of_the`
+            * ``of_the``
         """
         return cls(question)
 
     @classmethod
     def of_the(cls, question: T_Q) -> Self:
-        """Alias for :meth:`~screenpy.actions.MakeNote.of`."""
+        """Alias for :meth:`of`.
+
+        Workaround for https://github.com/python/mypy/issues/6700
+        """
         return cls.of(question)
 
     def as_(self, key: str) -> Self:
         """Set the key to use to recall this noted value."""
         self.key = key
-        self.key_to_log = represent_prop(key)
         return self
 
+    @property
+    def key_to_log(self) -> str | None:
+        """Represent the key in a log-friendly way."""
+        return represent_prop(self.key)
+
     def describe(self) -> str:
         """Describe the Action in present tense."""
-        return f"Make a note under {represent_prop(self.key)}."
+        return f"Make a note under {self.key_to_log}."
 
     @beat("{} jots something down under {key_to_log}.")
     def perform_as(self, the_actor: Actor) -> None:
         """Direct the Actor to take a note."""
         if self.key is None:
             msg = "No key was provided to name this note."
             raise UnableToAct(msg)
@@ -86,8 +92,7 @@
     def __init__(
         self,
         question: T_Q,
         key: str | None = None,
     ) -> None:
         self.question = question
         self.key = key
-        self.key_to_log = represent_prop(key)
```

### Comparing `screenpy-4.2.4/screenpy/actions/pause.py` & `screenpy-4.2.5/screenpy/actions/pause.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,23 +46,21 @@
         """Specify how many seconds or milliseconds to wait for."""
         return cls(number)
 
     def seconds_because(self, reason: str) -> Self:
         """Use seconds and provide a reason for the pause.
 
         Aliases:
-            * :meth:`~screenpy.actions.Pause.second_because`
+            * ``second_because``
         """
         self.unit = f"second{'s' if self.number != 1 else ''}"
         self.reason = self._massage_reason(reason)
         return self
 
-    def second_because(self, reason: str) -> Self:
-        """Alias for :meth:`~screenpy.actions.Pause.seconds_because`."""
-        return self.seconds_because(reason)
+    second_because = seconds_because
 
     def milliseconds_because(self, reason: str) -> Self:
         """Use milliseconds and provide a reason for the pause."""
         self.unit = f"millisecond{'s' if self.number != 1 else ''}"
         self.time = self.time / 1000.0
         self.reason = self._massage_reason(reason)
         return self
```

### Comparing `screenpy-4.2.4/screenpy/actions/see.py` & `screenpy-4.2.5/screenpy/actions/see.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,23 +37,31 @@
 
         the_actor.should(
             See.the(list_of_items, ContainsTheItem("juice extractor")),
         )
     """
 
     question: T_Q
-    question_to_log: str
     resolution: T_R
-    resolution_to_log: str
 
     @classmethod
     def the(cls, question: T_Q, resolution: T_R) -> Self:
         """Supply the Question (or value) and Resolution to test."""
         return cls(question, resolution)
 
+    @property
+    def question_to_log(self) -> str:
+        """Represent the Question in a log-friendly way."""
+        return get_additive_description(self.question)
+
+    @property
+    def resolution_to_log(self) -> str:
+        """Represent the Resolution in a log-friendly way."""
+        return get_additive_description(self.resolution)
+
     def describe(self) -> str:
         """Describe the Action in present tense."""
         return f"See if {self.question_to_log} is {self.resolution_to_log}."
 
     @beat("{} sees if {question_to_log} is {resolution_to_log}.")
     def perform_as(self, the_actor: Actor) -> None:
         """Direct the Actor to make an observation."""
@@ -68,10 +76,8 @@
         if isinstance(self.question, ErrorKeeper):
             reason = f"{self.question.caught_exception}"
 
         assert_that(value, self.resolution.resolve(), reason)
 
     def __init__(self, question: T_Q, resolution: T_R) -> None:
         self.question = question
-        self.question_to_log = get_additive_description(question)
         self.resolution = resolution
-        self.resolution_to_log = get_additive_description(resolution)
```

### Comparing `screenpy-4.2.4/screenpy/actions/see_all_of.py` & `screenpy-4.2.5/screenpy/actions/see_all_of.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/actions/see_any_of.py` & `screenpy-4.2.5/screenpy/actions/see_any_of.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/actions/silently.py` & `screenpy-4.2.5/screenpy/actions/silently.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/configuration.py` & `screenpy-4.2.5/screenpy/configuration.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/directions.py` & `screenpy-4.2.5/screenpy/directions.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/director.py` & `screenpy-4.2.5/screenpy/director.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/exceptions.py` & `screenpy-4.2.5/screenpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/given_when_then.py` & `screenpy-4.2.5/screenpy/given_when_then.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/narration/narrator.py` & `screenpy-4.2.5/screenpy/narration/narrator.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/narration/stdout_adapter/configuration.py` & `screenpy-4.2.5/screenpy/narration/stdout_adapter/configuration.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/narration/stdout_adapter/stdout_adapter.py` & `screenpy-4.2.5/screenpy/narration/stdout_adapter/stdout_adapter.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/pacing.py` & `screenpy-4.2.5/screenpy/pacing.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/protocols.py` & `screenpy-4.2.5/screenpy/protocols.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/__init__.py` & `screenpy-4.2.5/screenpy/resolutions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/base_resolution.py` & `screenpy-4.2.5/screenpy/resolutions/base_resolution.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/contains_item_matching.py` & `screenpy-4.2.5/screenpy/resolutions/contains_item_matching.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/contains_the_entry.py` & `screenpy-4.2.5/screenpy/resolutions/contains_the_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,26 @@
                 EnglishDictionary(), ContainsTheEntry({"Python": "a large snake."})
             )
         )
 
         the_actor.should(See.the(MathTestAnswers(), ContainsTheEntry("Problem3", 45)))
     """
 
+    @property
+    def entry_plural(self) -> str:
+        """Decide if we need "entry" or "entries" in the beat message."""
+        return "entries" if len(self.entries) != 1 else "entry"
+
+    @property
+    def entries_to_log(self) -> str:
+        """Represent the entries in a log-friendly way."""
+        return ", ".join(
+            f"{represent_prop(k)}->{represent_prop(v)}" for k, v in self.entries.items()
+        )
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"A mapping with the {self.entry_plural} {self.entries_to_log}."
 
     @beat("... hoping it's a mapping with the {entry_plural} {entries_to_log}")
     def resolve(self) -> Matcher[Mapping]:
         """Produce the Matcher to make the assertion."""
@@ -73,11 +85,7 @@
                 self.entries = dict(kv_args, **kv_kwargs)
             except ValueError:
                 # given a list of implicitly paired arguments
                 pairs: Iterable[tuple[Any, Any]] = [
                     (kv_args[i], kv_args[i + 1]) for i in range(0, len(kv_args), 2)
                 ]
                 self.entries = dict(pairs, **kv_kwargs)
-        self.entry_plural = "entries" if len(self.entries) != 1 else "entry"
-        self.entries_to_log = ", ".join(
-            f"{represent_prop(k)}->{represent_prop(v)}" for k, v in self.entries.items()
-        )
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/contains_the_item.py` & `screenpy-4.2.5/screenpy/resolutions/contains_the_key.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-"""Matches a list that contains the desired item."""
+"""Matches a dictionary that contains the desired key."""
 
-from typing import Generic, Sequence, TypeVar
+from __future__ import annotations
 
-from hamcrest import has_item
-from hamcrest.core.matcher import Matcher
+from typing import TYPE_CHECKING, Any, Generic, Hashable, Mapping, TypeVar
+
+from hamcrest import has_key
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
-T = TypeVar("T")
+if TYPE_CHECKING:
+    from hamcrest.core.matcher import Matcher
+
+K = TypeVar("K", bound=Hashable)
 
 
-class ContainsTheItem(Generic[T]):
-    """Match an iterable containing a specific item.
+class ContainsTheKey(Generic[K]):
+    """Match a dictionary containing a specific key.
 
     Examples::
 
-        the_actor.should(
-            See.the(Text.of_all(SEARCH_RESULTS), ContainsTheItem("The Droids"))
-        )
+        the_actor.should(See.the(LastResponseBody(), ContainsTheKey("skeleton")))
     """
 
+    @property
+    def key_to_log(self) -> str | K:
+        """Represent the key in a log-friendly way."""
+        return represent_prop(self.key)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"A sequence containing {self.item_to_log}."
+        return f"Containing the key {self.key_to_log}."
 
-    @beat("... hoping it contains {item_to_log}.")
-    def resolve(self) -> Matcher[Sequence[T]]:
+    @beat("... hoping it's a dict containing the key {key_to_log}.")
+    def resolve(self) -> Matcher[Mapping[K, Any]]:
         """Produce the Matcher to make the assertion."""
-        return has_item(self.item)
+        return has_key(self.key)
 
-    def __init__(self, item: T) -> None:
-        self.item = item
-        self.item_to_log = represent_prop(item)
+    def __init__(self, key: K) -> None:
+        self.key = key
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/contains_the_key.py` & `screenpy-4.2.5/screenpy/resolutions/contains_the_text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-"""Matches a dictionary that contains the desired key."""
+"""Matches a substring in a string."""
 
-from typing import Any, Generic, Hashable, Mapping, TypeVar
-
-from hamcrest import has_key
+from hamcrest import contains_string
 from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
-K = TypeVar("K", bound=Hashable)
-
 
-class ContainsTheKey(Generic[K]):
-    """Match a dictionary containing a specific key.
+class ContainsTheText:
+    """Match a specific substring of a string.
 
     Examples::
 
-        the_actor.should(See.the(LastResponseBody(), ContainsTheKey("skeleton")))
+        the_actor.should(
+            See.the(Text.of_the(WELCOME_MESSAGE), ContainsTheText("Hello,"))
+        )
     """
 
+    @property
+    def text_to_log(self) -> str:
+        """Represent the text in a log-friendly way."""
+        return represent_prop(self.text)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"Containing the key {self.key_to_log}."
+        return f"Containing the text {self.text_to_log}."
 
-    @beat("... hoping it's a dict containing the key {key_to_log}.")
-    def resolve(self) -> Matcher[Mapping[K, Any]]:
+    @beat("... hoping it contains {text_to_log}.")
+    def resolve(self) -> Matcher[str]:
         """Produce the Matcher to make the assertion."""
-        return has_key(self.key)
+        return contains_string(self.text)
 
-    def __init__(self, key: K) -> None:
-        self.key = key
-        self.key_to_log = represent_prop(key)
+    def __init__(self, text: str) -> None:
+        self.text = text
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/contains_the_text.py` & `screenpy-4.2.5/screenpy/resolutions/reads_exactly.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-"""Matches a substring in a string."""
+"""Matches an exact string."""
 
-from hamcrest import contains_string
+from hamcrest import has_string
 from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
 
-class ContainsTheText:
-    """Match a specific substring of a string.
+class ReadsExactly:
+    """Match a specific string exactly.
 
     Examples::
 
         the_actor.should(
-            See.the(Text.of_the(WELCOME_MESSAGE), ContainsTheText("Hello,"))
+            See.the(Text.of_the(LOGIN_MESSAGE), ReadsExactly("Log in below."))
         )
     """
 
+    @property
+    def text_to_log(self) -> str:
+        """Represent the text in a log-friendly way."""
+        return represent_prop(self.text)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"Containing the text {self.text_to_log}."
+        return f"{self.text_to_log}, verbatim."
 
-    @beat("... hoping it contains {text_to_log}.")
-    def resolve(self) -> Matcher[str]:
+    @beat("... hoping it's {text_to_log}, verbatim.")
+    def resolve(self) -> Matcher[object]:
         """Produce the Matcher to make the assertion."""
-        return contains_string(self.text)
+        return has_string(self.text)
 
     def __init__(self, text: str) -> None:
         self.text = text
-        self.text_to_log = represent_prop(text)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/contains_the_value.py` & `screenpy-4.2.5/screenpy/resolutions/contains_the_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 """Matches a dictionary that contains a specific value."""
 
-from typing import Any, Generic, Mapping, TypeVar
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Generic, Mapping, TypeVar
 
 from hamcrest import has_value
-from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
+if TYPE_CHECKING:
+    from hamcrest.core.matcher import Matcher
+
 V = TypeVar("V")
 
 
 class ContainsTheValue(Generic[V]):
     """Match a dictionary containing a specific value.
 
     Examples::
 
         the_actor.should(
             See.the(Cookies(), ContainTheValue("pumpernickle"))
         )
     """
 
+    @property
+    def value_to_log(self) -> str | V:
+        """Represent the value in a log-friendly way."""
+        return represent_prop(self.value)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Containing the value {self.value_to_log}."
 
     @beat("... hoping it contains the value {value_to_log}.")
     def resolve(self) -> Matcher[Mapping[Any, V]]:
         """Produce the Matcher to form the assertion."""
         return has_value(self.value)
 
     def __init__(self, value: V) -> None:
         self.value = value
-        self.value_to_log = represent_prop(value)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/custom_matchers/is_in_bounds.py` & `screenpy-4.2.5/screenpy/resolutions/custom_matchers/is_in_bounds.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py` & `screenpy-4.2.5/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/ends_with.py` & `screenpy-4.2.5/screenpy/resolutions/ends_with.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,19 +13,23 @@
     Examples::
 
         the_actor.should(
             See.the(Text.of_the(LOGIN_ERROR), EndsWith("username or password."))
         )
     """
 
+    @property
+    def postfix_to_log(self) -> str:
+        """Represent the postfix in a log-friendly way."""
+        return represent_prop(self.postfix)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Ending with {self.postfix_to_log}."
 
     @beat("... hoping it ends with {postfix_to_log}.")
     def resolve(self) -> Matcher[str]:
         """Produce the Matcher to make the assertion."""
         return ends_with(self.postfix)
 
     def __init__(self, postfix: str) -> None:
         self.postfix = postfix
-        self.postfix_to_log = represent_prop(postfix)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/has_length.py` & `screenpy-4.2.5/screenpy/resolutions/has_length.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,19 +14,23 @@
     Examples::
 
         the_actor.should(
             See.the(Selected.options_from(INDUSTRIES), HasLength(5))
         )
     """
 
+    @property
+    def item_plural(self) -> str:
+        """Decide if we need "item" or "items" in the beat message."""
+        return "items" if self.length != 1 else "item"
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"{self.length} item{self.plural} long."
+        return f"{self.length} {self.item_plural} long."
 
-    @beat("... hoping it's a collection with {length} item{plural} in it.")
+    @beat("... hoping it's a collection with {length} {item_plural} in it.")
     def resolve(self) -> Matcher[Sized]:
         """Produce the Matcher to make the assertion."""
         return has_length(self.length)
 
     def __init__(self, length: int) -> None:
         self.length = length
-        self.plural = "s" if self.length != 1 else ""
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_close_to.py` & `screenpy-4.2.5/screenpy/resolutions/is_close_to.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_empty.py` & `screenpy-4.2.5/screenpy/resolutions/is_empty.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_greater_than.py` & `screenpy-4.2.5/screenpy/resolutions/is_greater_than.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """Matches a value greater than the given number."""
 
-from typing import Any
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
 
 from hamcrest import greater_than
-from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
+if TYPE_CHECKING:
+    from hamcrest.core.matcher import Matcher
+
 
 class IsGreaterThan:
     """Match on a number that is greater than the given number.
 
     Examples::
 
         the_actor.should(See.the(Number.of(COUPONS), IsGreaterThan(1)))
     """
 
+    @property
+    def number_to_log(self) -> str | float:
+        """Represent the number in a log-friendly way."""
+        return represent_prop(self.number)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Greater than {self.number_to_log}."
 
     @beat("... hoping it's greater than {number_to_log}.")
     def resolve(self) -> Matcher[Any]:
         """Produce the Matcher to make the assertion."""
         return greater_than(self.number)
 
     def __init__(self, number: float) -> None:
         self.number = number
-        self.number_to_log = represent_prop(number)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_greater_than_or_equal_to.py` & `screenpy-4.2.5/screenpy/resolutions/is_greater_than_or_equal_to.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 """Matches a value greater than the given number."""
 
-from typing import Any
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
 
 from hamcrest import greater_than_or_equal_to
-from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
+if TYPE_CHECKING:
+    from hamcrest.core.matcher import Matcher
+
 
 class IsGreaterThanOrEqualTo:
     """Match on a number that is greater than or equal to the given number.
 
     Examples::
 
         the_actor.should(
             See.the(Number.of(COUPONS), IsGreaterThanOrEqualTo(1))
         )
     """
 
+    @property
+    def number_to_log(self) -> str | float:
+        """Represent the number in a log-friendly way."""
+        return represent_prop(self.number)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Greater than or equal to {self.number_to_log}."
 
     @beat("... hoping it's greater than or equal to {number_to_log}.")
     def resolve(self) -> Matcher[Any]:
         """Produce the Matcher to make the assertion."""
         return greater_than_or_equal_to(self.number)
 
     def __init__(self, number: float) -> None:
         self.number = number
-        self.number_to_log = represent_prop(number)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_in_range.py` & `screenpy-4.2.5/screenpy/resolutions/is_in_range.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from screenpy.exceptions import UnableToFormResolution
 from screenpy.pacing import beat
+from screenpy.speech_tools import represent_prop
 
 from .custom_matchers.is_in_bounds import is_in_bounds
 
 if TYPE_CHECKING:
     from hamcrest.core.matcher import Matcher
 
 
@@ -30,26 +31,30 @@
         )
 
         the_actor.should(See.the(Number.of(PUPPY_PICTURES), IsInRange("1-5")))
 
         the_actor.should(See.the(Number.of(COOKIES), IsInRange("[1, 5)")))
     """
 
+    @property
+    def bounds_to_log(self) -> str | int:
+        """Represent the bounds in a log-friendly way."""
+        bounding_string = self.bounds[0]  # given bounding string
+        if len(self.bounds) == 2:  # noqa: PLR2004
+            # given bounding numbers
+            bounding_string = f"[{self.bounds[0]}, {self.bounds[1]}]"
+        return represent_prop(bounding_string)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
-        return f"In the range {self.bounding_string}."
+        return f"In the range {self.bounds_to_log}."
 
-    @beat("... hoping it's in the range {bounding_string}.")
+    @beat("... hoping it's in the range {bounds_to_log}.")
     def resolve(self) -> Matcher[float]:
         """Produce the Matcher to make the assertion."""
         return is_in_bounds(*self.bounds)
 
     def __init__(self, *bounds: int | str) -> None:
         if len(bounds) > 2:  # noqa: PLR2004
             msg = f"{self.__class__.__name__} was given too many arguments: {bounds}."
             raise UnableToFormResolution(msg)
-
         self.bounds = bounds
-        self.bounding_string = self.bounds[0]  # given bounding string
-        if len(self.bounds) == 2:  # noqa: PLR2004
-            # given bounding numbers
-            self.bounding_string = f"[{self.bounds[0]}, {self.bounds[1]}]"
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_less_than.py` & `screenpy-4.2.5/screenpy/resolutions/is_less_than.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 """Matches a value less than the given number."""
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from hamcrest import less_than
-from hamcrest.core.matcher import Matcher
 
 from screenpy.pacing import beat
 from screenpy.speech_tools import represent_prop
 
+if TYPE_CHECKING:
+    from hamcrest.core.matcher import Matcher
+
 
 class IsLessThan:
     """Match on a number that is less than the given number.
 
     Examples::
 
         the_actor.should(
             See.the(Number.of(ADVERTISEMENT_POPUPS), IsLessThan(1))
         )
     """
 
+    @property
+    def number_to_log(self) -> str | float:
+        """Represent the number in a log-friendly way."""
+        return represent_prop(self.number)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Less than {self.number_to_log}."
 
     @beat("... hoping it's less than {number_to_log}.")
     def resolve(self) -> Matcher[float]:
         """Produce the Matcher to make the assertion."""
         return less_than(self.number)
 
     def __init__(self, number: float) -> None:
         self.number = number
-        self.number_to_log = represent_prop(number)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/is_not.py` & `screenpy-4.2.5/screenpy/resolutions/is_not.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,19 +16,23 @@
     """Match a negated Resolution.
 
     Examples::
 
         the_actor.should(See.the(Element(WELCOME_BANNER), IsNot(Visible())))
     """
 
+    @property
+    def resolution_to_log(self) -> str:
+        """Represent the Resolution in a log-friendly way."""
+        return get_additive_description(self.resolution)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Not {self.resolution_to_log}."
 
     @beat("... hoping it's not {resolution_to_log}.")
     def resolve(self) -> Matcher[object]:
         """Produce the Matcher to make the assertion."""
         return is_not(self.resolution.resolve())
 
     def __init__(self, resolution: Resolvable) -> None:
         self.resolution = resolution
-        self.resolution_to_log = get_additive_description(self.resolution)
```

### Comparing `screenpy-4.2.4/screenpy/resolutions/starts_with.py` & `screenpy-4.2.5/screenpy/resolutions/starts_with.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,19 +13,23 @@
     Examples::
 
         the_actor.should(
             See.the(Text.of_the(WELCOME_MESSAGE), StartsWith("Welcome"))
         )
     """
 
+    @property
+    def prefix_to_log(self) -> str:
+        """Represent the prefix in a log-friendly way."""
+        return represent_prop(self.prefix)
+
     def describe(self) -> str:
         """Describe the Resolution's expectation."""
         return f"Starting with {self.prefix_to_log}."
 
     @beat("... hoping it starts with {prefix_to_log}.")
     def resolve(self) -> Matcher[str]:
         """Produce the Matcher to make the assertion."""
         return starts_with(self.prefix)
 
     def __init__(self, prefix: str) -> None:
         self.prefix = prefix
-        self.prefix_to_log = represent_prop(prefix)
```

### Comparing `screenpy-4.2.4/screenpy/speech_tools.py` & `screenpy-4.2.5/screenpy/speech_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """A grab-bag of useful language-massaging functions with broad applicability."""
 
 from __future__ import annotations
 
 import re
 from typing import TypeVar, overload
+from unittest import mock
 
 from hamcrest.core.helpers.hasmethod import hasmethod
-from hamcrest.core.helpers.ismock import ismock
 
 from screenpy.protocols import Answerable, Describable, Performable, Resolvable
 
 T = TypeVar("T")
 
 
 def get_additive_description(describable: Describable | T) -> str:
@@ -48,26 +48,28 @@
         # Neither Describable nor any other -able, must be a value.
         description = f"the {describable.__class__.__name__}"
 
     return description
 
 
 @overload
-def represent_prop(item: str) -> str: ...
+def represent_prop(item: mock.Mock) -> mock.Mock: ...
 
 
 @overload
-def represent_prop(item: T) -> T: ...
+def represent_prop(item: str | T) -> str: ...
 
 
-def represent_prop(item: str | T) -> str | T:
+def represent_prop(item: str | T | mock.Mock) -> str | mock.Mock:
     """Represent items in a manner suitable for the audience (logging)."""
-    if not ismock(item) and hasmethod(item, "describe_to"):
+    if isinstance(item, mock.Mock):
+        return item
+    if hasmethod(item, "describe_to"):
         return f"{item}"
     if isinstance(item, str):
         return repr(item)
 
     description = str(item)
-    if description[:1] == "<" and description[-1:] == ">":
-        return item
+    if description.startswith("<") and description.endswith(">"):
+        return description
 
     return f"<{item}>"
```

### Comparing `screenpy-4.2.4/PKG-INFO` & `screenpy-4.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenpy
-Version: 4.2.4
+Version: 4.2.5
 Summary: Screenplay pattern base for Python automated test suites.
 Home-page: https://github.com/ScreenPyHQ/screenpy
 License: MIT
 Author: Perry Goy
 Author-email: perry.goy@gmail.com
 Maintainer: Gabe Langton
 Requires-Python: >=3.8,<4.0
@@ -32,22 +32,23 @@
 Provides-Extra: requests
 Provides-Extra: selenium
 Provides-Extra: test
 Requires-Dist: PyHamcrest (>=2.0.0)
 Requires-Dist: autodoc-pydantic ; extra == "dev" or extra == "docs"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: coverage ; extra == "dev" or extra == "test"
+Requires-Dist: cruft ; extra == "dev"
 Requires-Dist: importlib_metadata ; python_version >= "3.8.dev0" and python_version < "3.9.dev0"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: pytest ; extra == "dev" or extra == "test"
 Requires-Dist: pytest-mock ; extra == "dev" or extra == "test"
-Requires-Dist: ruff (>=0.1.13) ; extra == "dev"
+Requires-Dist: ruff (>=0.2.0) ; extra == "dev"
 Requires-Dist: screenpy-adapter_allure (>=4.0.1,<5.0.0) ; extra == "allure"
 Requires-Dist: screenpy-appium ; extra == "appium"
 Requires-Dist: screenpy-playwright ; extra == "playwright"
 Requires-Dist: screenpy-pyotp (>=4.0.1,<5.0.0) ; extra == "pyotp"
 Requires-Dist: screenpy-requests (>=4.0.1,<5.0.0) ; extra == "requests"
 Requires-Dist: screenpy-selenium (>=4.0.3,<5.0.0) ; extra == "selenium"
 Requires-Dist: sphinx ; extra == "dev" or extra == "docs"
@@ -57,14 +58,15 @@
 Requires-Dist: typing_extensions (>=4.8.0)
 Project-URL: Documentation, https://screenpy-docs.readthedocs.io
 Project-URL: Repository, https://github.com/ScreenPyHQ/screenpy
 Description-Content-Type: text/markdown
 
 ScreenPy
 ========
+
 [![Build Status](../../actions/workflows/tests.yml/badge.svg)](../../actions/workflows/tests.yml)
 [![Build Status](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)
 
 [![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy.svg)](https://pypi.org/project/screenpy)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -110,26 +112,26 @@
 
 Installation
 ------------
     pip install screenpy
 
 
 Documentation
-----------
+-------------
 Please check out the [Read The Docs documentation](https://screenpy-docs.readthedocs.io/en/latest/) for the latest information about this module!
 
 
 Contributing
 ------------
 You want to contribute? Great! Here are the things you should do before submitting your PR:
 
 1. Fork the repo and git clone your fork.
 1. `dev` install the project package:
-   1. `pip install -e .[dev]` 
-   1. Optional (poetry users):
-      1. `poetry install --extras dev`
+    1. `pip install -e .[dev]`
+    1. Optional (poetry users):
+        1. `poetry install --extras dev`
 1. Run `pre-commit install` once.
 1. Run `tox` to perform tests frequently.
 1. Create pull-request from your branch.
 
 That's it! :)
```

