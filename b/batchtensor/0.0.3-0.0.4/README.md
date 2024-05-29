# Comparing `tmp/batchtensor-0.0.3.tar.gz` & `tmp/batchtensor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchtensor-0.0.3.tar", max compression
+gzip compressed data, was "batchtensor-0.0.4.tar", max compression
```

## Comparing `batchtensor-0.0.3.tar` & `batchtensor-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1501 2024-03-18 06:43:56.330048 batchtensor-0.0.3/LICENSE
--rw-r--r--   0        0        0     7539 2024-03-18 06:43:56.330048 batchtensor-0.0.3/README.md
--rw-r--r--   0        0        0     6256 2024-03-18 06:43:56.330048 batchtensor-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       21 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/__init__.py
--rw-r--r--   0        0        0      128 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/constants.py
--rw-r--r--   0        0        0     3204 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/__init__.py
--rw-r--r--   0        0        0     6658 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/comparison.py
--rw-r--r--   0        0        0     3525 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/conversion.py
--rw-r--r--   0        0        0     2847 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/indexing.py
--rw-r--r--   0        0        0     4101 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/joining.py
--rw-r--r--   0        0        0     4133 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/math.py
--rw-r--r--   0        0        0      984 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/misc.py
--rw-r--r--   0        0        0     5237 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/permutation.py
--rw-r--r--   0        0        0     6876 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/pointwise.py
--rw-r--r--   0        0        0    23852 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/reduction.py
--rw-r--r--   0        0        0    10503 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/slicing.py
--rw-r--r--   0        0        0     7449 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/nested/trigo.py
--rw-r--r--   0        0        0      633 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/__init__.py
--rw-r--r--   0        0        0     3500 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/applier.py
--rw-r--r--   0        0        0     1183 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/apply.py
--rw-r--r--   0        0        0      914 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/base.py
--rw-r--r--   0        0        0      919 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/default.py
--rw-r--r--   0        0        0     1216 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/mapping.py
--rw-r--r--   0        0        0     1264 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/sequence.py
--rw-r--r--   0        0        0      541 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/recursive/state.py
--rw-r--r--   0        0        0     2476 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/__init__.py
--rw-r--r--   0        0        0     5294 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/comparison.py
--rw-r--r--   0        0        0     2583 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/indexing.py
--rw-r--r--   0        0        0     3025 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/joining.py
--rw-r--r--   0        0        0     3345 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/math.py
--rw-r--r--   0        0        0     4485 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/permutation.py
--rw-r--r--   0        0        0    19223 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/reduction.py
--rw-r--r--   0        0        0     7880 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/tensor/slicing.py
--rw-r--r--   0        0        0      201 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/utils/__init__.py
--rw-r--r--   0        0        0     7014 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/utils/bfs.py
--rw-r--r--   0        0        0     7149 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/utils/dfs.py
--rw-r--r--   0        0        0     2324 2024-03-18 06:43:56.330048 batchtensor-0.0.3/src/batchtensor/utils/seed.py
--rw-r--r--   0        0        0     8823 1970-01-01 00:00:00.000000 batchtensor-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-29 04:16:32.679293 batchtensor-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7758 2024-05-29 04:16:32.679293 batchtensor-0.0.4/README.md
+-rw-r--r--   0        0        0     6563 2024-05-29 04:16:32.683293 batchtensor-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/constants.py
+-rw-r--r--   0        0        0     3204 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/__init__.py
+-rw-r--r--   0        0        0     6662 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/comparison.py
+-rw-r--r--   0        0        0     3542 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/conversion.py
+-rw-r--r--   0        0        0     2932 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/indexing.py
+-rw-r--r--   0        0        0     4115 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/joining.py
+-rw-r--r--   0        0        0     4185 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/math.py
+-rw-r--r--   0        0        0     1047 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/misc.py
+-rw-r--r--   0        0        0     5352 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/permutation.py
+-rw-r--r--   0        0        0     6885 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/pointwise.py
+-rw-r--r--   0        0        0    24369 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/reduction.py
+-rw-r--r--   0        0        0    10678 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/slicing.py
+-rw-r--r--   0        0        0     7461 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/nested/trigo.py
+-rw-r--r--   0        0        0      642 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/__init__.py
+-rw-r--r--   0        0        0     3739 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/auto.py
+-rw-r--r--   0        0        0      884 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/base.py
+-rw-r--r--   0        0        0      941 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/default.py
+-rw-r--r--   0        0        0      933 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/interface.py
+-rw-r--r--   0        0        0     1223 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/mapping.py
+-rw-r--r--   0        0        0     1270 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/sequence.py
+-rw-r--r--   0        0        0      541 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/recursive/state.py
+-rw-r--r--   0        0        0     2476 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/__init__.py
+-rw-r--r--   0        0        0     5298 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/comparison.py
+-rw-r--r--   0        0        0     2633 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/indexing.py
+-rw-r--r--   0        0        0     3019 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/joining.py
+-rw-r--r--   0        0        0     3397 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/math.py
+-rw-r--r--   0        0        0     4565 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/permutation.py
+-rw-r--r--   0        0        0    19705 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/reduction.py
+-rw-r--r--   0        0        0     7999 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/tensor/slicing.py
+-rw-r--r--   0        0        0      201 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/utils/__init__.py
+-rw-r--r--   0        0        0     6985 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/utils/bfs.py
+-rw-r--r--   0        0        0     7151 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/utils/dfs.py
+-rw-r--r--   0        0        0     2280 2024-05-29 04:16:32.683293 batchtensor-0.0.4/src/batchtensor/utils/seed.py
+-rw-r--r--   0        0        0     9136 1970-01-01 00:00:00.000000 batchtensor-0.0.4/PKG-INFO
```

### Comparing `batchtensor-0.0.3/LICENSE` & `batchtensor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `batchtensor-0.0.3/README.md` & `batchtensor-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -140,20 +140,21 @@
 pip install batchtensor[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/batchtensor/get_started) to see how
 to install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `batchtensor` versions and tested dependencies.
 
-| `batchtensor` | `coola`      | `torch`       | `python`      |
-|---------------|--------------|---------------|---------------|
-| `main`        | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` |
-| `0.0.3`       | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` |
-| `0.0.2`       | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` |
-| `0.0.1`       | `>=0.1,<0.4` | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `batchtensor` | `coola`      | `numpy`<sup>*</sup> | `torch`       | `python`      |
+|---------------|--------------|---------------------|---------------|---------------|
+| `main`        | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.4`       | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.3`       | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.2`       | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.1`       | `>=0.1,<0.4` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
 
 <sup>*</sup> indicates an optional dependency
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -43,21 +43,23 @@
 command: ```shell pip install batchtensor ``` To make the package as slim as
 possible, only the minimal packages required to use `batchtensor` are
 installed. To include all the dependencies, you can use the following command:
 ```shell pip install batchtensor[all] ``` Please check the [get started page]
 (https://durandtibo.github.io/batchtensor/get_started) to see how to install
 only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `batchtensor` versions and tested
-dependencies. | `batchtensor` | `coola` | `torch` | `python` | |---------------
-|--------------|---------------|---------------| | `main` | `>=0.1,<1.0` |
-`>=1.11,<3.0` | `>=3.9,<3.13` | | `0.0.3` | `>=0.1,<1.0` | `>=1.11,<3.0` |
-`>=3.9,<3.13` | | `0.0.2` | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
-`0.0.1` | `>=0.1,<0.4` | `>=1.11,<3.0` | `>=3.9,<3.13` | * indicates an
-optional dependency ## Contributing Please check the instructions in
-[CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions and Communication
+dependencies. | `batchtensor` | `coola` | `numpy`* | `torch` | `python` | |----
+-----------|--------------|---------------------|---------------|--------------
+-| | `main` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.4` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.3` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.2` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.1` | `>=0.1,<0.4` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | *
+indicates an optional dependency ## Contributing Please check the instructions
+in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions and Communication
 Everyone is welcome to contribute to the community. If you have any questions
 or suggestions, you can submit [Github Issues](https://github.com/durandtibo/
 batchtensor/issues). We will reply to you as soon as possible. Thank you very
 much. ## API stability :warning: While `batchtensor` is in development stage,
 no API is guaranteed to be stable from one release to the next. In fact, it is
 very likely that the API will change multiple times before a stable 1.0.0
 release. In practice, this means that upgrading `batchtensor` to a new version
```

### Comparing `batchtensor-0.0.3/pyproject.toml` & `batchtensor-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batchtensor"
-version = "0.0.3"
+version = "0.0.4"
 description = "Functions to manipulate batches of PyTorch tensors"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/batchtensor"
 repository = "https://github.com/durandtibo/batchtensor"
 keywords = [
     "batch",
@@ -34,41 +34,44 @@
     { include = "batchtensor", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
 coola = ">=0.1,<1.0"
 python = ">=3.9,<3.13"
-torch = ">=1.11,<3.0"
+torch = [
+    { version = ">=1.11,<2.3", markers="sys_platform == 'darwin' and platform_machine != 'arm64'" },
+    { version = ">=1.11,<3.0" }
+]
 
 # Optional dependencies
 numpy = { version = ">=1.21,<2.0", optional = true }
 
 [tool.poetry.extras]
 all = ['numpy']
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mike = "^2.0"
+mike = "^2.1"
 mkdocs-material = "^9.5"
-mkdocstrings = { extras = ["python"], version = "^0.24" }
+mkdocstrings = { extras = ["python"], version = "^0.25" }
 
 [tool.poetry.group.dev.dependencies]
-black = ">=24.3"
-coverage = { extras = ["toml"], version = "^7.4" }
+black = ">=24.4"
+coverage = { extras = ["toml"], version = "^7.5" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 feu = ">=0.0.2,<0.1"
-pre-commit = "^3.6"
-pygments = "^2.17"
-pytest = "^8.1"
-pytest-cov = "^4.1"
+pre-commit = "^3.7"
+pygments = "^2.18"
+pytest = "^8.2"
+pytest-cov = "^5.0"
 pytest-timeout = "^2.3"
-ruff = ">=0.3.0,<1.0"
+ruff = ">=0.4.0,<1.0"
 xdoctest = "^1.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -92,15 +95,15 @@
 log_level = "DEBUG"
 addopts = "--color yes --durations 10 -rf"
 # Configuration of the short test summary info
 # https://docs.pytest.org/en/stable/usage.html#detailed-summary-report
 
 [tool.black]
 line-length = 100
-target-version = ["py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 include = '\.pyi?$'
 
 [tool.pylint.FORMAT]
 max-line-length = 100
 
 [tool.isort]
 profile = "black"
@@ -112,20 +115,23 @@
 syntax = "google"
 
 [tool.ruff]
 # List of rules: https://docs.astral.sh/ruff/rules/
 lint.select = [
     "A", # builtins
     "ANN", # annotations
+    "ARG", # flake8-unused-arguments
     "B", # bugbear
     "BLE", # flake8-blind-except
     "C4", # flake8-comprehensions
     "D", # pydocstyle
+    "DTZ", # flake8-datetimez
     "E", # pycodestyle (Error)
     "EM", # flake8-errmsg
+    "EXE", # flake8-executable
     "F", # pyflakes
     "FA", # flake8-future-annotations
     "FURB", # refurb
     "ICN", # flake8-import-conventions
     "INP", # flake8-no-pep420
     "ISC", # flake8-implicit-str-concat
     "LOG", # logging
@@ -137,14 +143,15 @@
     "PL", # Pylint
     "PT", # flake8-pytest-style
     "PTH", # pathlib
     "PYI", # flake8-pyi
     "Q", # flake8-quotes
     "RET", # flake8-return
     "RSE", # flake8-raise
+    "RUF", # Ruff-specific rules
     "S", # flake8-bandit
     "SIM", # flake8-simplify
     "T20", # flake8-print
     "TCH", # flake8-type-checking
     "TD", # flake8-todos
     "TID", # flake8-tidy-imports
     "TRY", # tryceratops
@@ -170,20 +177,23 @@
     "D209", # Multi-line docstring closing quotes should be on a separate line
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 lint.fixable = [
     "A",
     "ANN",
+    "ARG",
     "B",
     "BLE",
     "C4",
     "D",
+    "DTZ",
     "E",
     "EM",
+    "EXE",
     "F",
     "FA",
     "FURB",
     "ICN",
     "INP",
     "ISC",
     "LOG",
@@ -194,14 +204,15 @@
     "PL",
     "PT",
     "PTH",
     "PYI",
     "Q",
     "RET",
     "RSE",
+    "RUF",
     "S",
     "SIM",
     "T20",
     "TCH",
     "TD",
     "TID",
     "TRY",
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/__init__.py` & `batchtensor-0.0.4/src/batchtensor/nested/__init__.py`

 * *Files identical despite different names*

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/comparison.py` & `batchtensor-0.0.4/src/batchtensor/nested/comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     Returns:
         The indices that sort each tensor along the batch dimension
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import argsort_along_batch
     >>> data = {
     ...     "a": torch.tensor([[2, 6], [0, 3], [4, 9], [8, 1], [5, 7]]),
     ...     "b": torch.tensor([4, 3, 2, 1, 0]),
     ... }
     >>> out = argsort_along_batch(data)
@@ -67,14 +68,15 @@
 
     Returns:
         The indices that sort each tensor along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import argsort_along_seq
     >>> data = {'a': torch.tensor([[7, 3, 0, 8, 5], [1, 9, 6, 4, 2]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = argsort_along_seq(data)
     >>> out
     {'a': tensor([[2, 1, 4, 0, 3], [0, 4, 3, 2, 1]]), 'b': tensor([[4, 3, 2, 1, 0]])}
     >>> out = argsort_along_seq(data, descending=True)
@@ -106,14 +108,15 @@
             of (values, indices), where the values are the sorted
             values and indices are the indices of the elements in the
             original input tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import sort_along_batch
     >>> data = {
     ...     "a": torch.tensor([[2, 6], [0, 3], [4, 9], [8, 1], [5, 7]]),
     ...     "b": torch.tensor([4, 3, 2, 1, 0]),
     ... }
     >>> out = sort_along_batch(data)
@@ -158,14 +161,15 @@
             of (values, indices), where the values are the sorted
             values and indices are the indices of the elements in the
             original input tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import sort_along_seq
     >>> data = {'a': torch.tensor([[7, 3, 0, 8, 5], [1, 9, 6, 4, 2]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = sort_along_seq(data)
     >>> out
     {'a': torch.return_types.sort(
     values=tensor([[0, 3, 5, 7, 8], [1, 2, 4, 6, 9]]),
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/conversion.py` & `batchtensor-0.0.4/src/batchtensor/nested/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Returns:
         A nested data structure with ``torch.Tensor``s. The output data
             has the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import numpy as np
     >>> from batchtensor.nested import as_tensor
     >>> data = {"a": np.ones((2, 5), dtype=np.float32), "b": np.arange(5), "c": 42}
     >>> out = as_tensor(data)
     >>> out
     {'a': tensor([[1., 1., 1., 1., 1.], [1., 1., 1., 1., 1.]]),
      'b': tensor([0, 1, 2, 3, 4]),
@@ -64,14 +65,15 @@
         A nested data structure with ``torch.Tensor``s instead of
             ``numpy.ndarray``s. The output data has the same structure
             as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import numpy as np
     >>> from batchtensor.nested import from_numpy
     >>> data = {"a": np.ones((2, 5), dtype=np.float32), "b": np.arange(5)}
     >>> out = from_numpy(data)
     >>> out
     {'a': tensor([[1., 1., 1., 1., 1.], [1., 1., 1., 1., 1.]]), 'b': tensor([0, 1, 2, 3, 4])}
 
@@ -96,17 +98,18 @@
         A nested data structure with ``numpy.ndarray``s instead of
             ``torch.Tensor``s. The output data has the same structure
             as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import numpy as np
     >>> from batchtensor.nested import to_numpy
-    >>> data = {"a": torch.ones(2, 5), "b": torch.arange(5)}
+    >>> data = {"a": torch.ones(2, 5), "b": torch.tensor([0, 1, 2, 3, 4])}
     >>> out = to_numpy(data)
     >>> out
     {'a': array([[1., 1., 1., 1., 1.], [1., 1., 1., 1., 1.]], dtype=float32), 'b': array([0, 1, 2, 3, 4])}
 
     ```
     """
     return recursive_apply(data, lambda tensor: tensor.numpy())
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/indexing.py` & `batchtensor-0.0.4/src/batchtensor/nested/indexing.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,17 +33,21 @@
 
     Returns:
         The indexed tensors along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import index_select_along_batch
-    >>> tensors = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> tensors = {
+    ...     "a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]),
+    ...     "b": torch.tensor([4, 3, 2, 1, 0]),
+    ... }
     >>> out = index_select_along_batch(tensors, torch.tensor([2, 4]))
     >>> out
     {'a': tensor([[4, 5], [8, 9]]), 'b': tensor([2, 0])}
     >>> out = index_select_along_batch(tensors, torch.tensor([4, 3, 2, 1, 0]))
     >>> out
     {'a': tensor([[8, 9], [6, 7], [4, 5], [2, 3], [0, 1]]), 'b': tensor([0, 1, 2, 3, 4])}
 
@@ -68,17 +72,18 @@
 
     Returns:
         The indexed tensors along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import index_select_along_seq
-    >>> tensors = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> tensors = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = index_select_along_seq(tensors, torch.tensor([2, 4]))
     >>> out
     {'a': tensor([[2, 4], [7, 9]]), 'b': tensor([[2, 0]])}
     >>> out = index_select_along_seq(tensors, torch.tensor([4, 3, 2, 1, 0]))
     >>> out
     {'a': tensor([[4, 3, 2, 1, 0], [9, 8, 7, 6, 5]]), 'b': tensor([[0, 1, 2, 3, 4]])}
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/joining.py` & `batchtensor-0.0.4/src/batchtensor/nested/joining.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     Returns:
         The concatenated tensors along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cat_along_batch
     >>> data = [
     ...     {
     ...         "a": torch.tensor([[0, 1, 2], [4, 5, 6]]),
     ...         "b": torch.tensor([[10, 11, 12], [13, 14, 15]]),
     ...     },
@@ -76,14 +77,15 @@
 
     Returns:
         The concatenated tensors along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cat_along_seq
     >>> data = [
     ...     {
     ...         "a": torch.tensor([[0, 1, 2], [4, 5, 6]]),
     ...         "b": torch.tensor([[10, 11, 12], [13, 14, 15]]),
     ...     },
@@ -108,26 +110,27 @@
     Note:
         This function assumes the sequence dimension is the second
             dimension of the tensors. All the tensors should have the
             same sequence size.
 
     Args:
         data: The input data. Each item must be a tensor.
-        repeats: Specifies the number of times to repeat
+        repeats: The number of times to repeat
             the data along the sequence dimension.
 
     Returns:
         The tensors repeated along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import repeat_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = repeat_along_seq(data, 2)
     >>> out
     {'a': tensor([[0, 1, 2, 3, 4, 0, 1, 2, 3, 4], [5, 6, 7, 8, 9, 5, 6, 7, 8, 9]]),
      'b': tensor([[4, 3, 2, 1, 0, 4, 3, 2, 1, 0]])}
 
     ```
     """
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/math.py` & `batchtensor-0.0.4/src/batchtensor/nested/math.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Returns:
         The cumulative product of elements of input in the batch
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cumprod_along_batch
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([4, 3, 2, 1, 0]),
     ... }
     >>> out = cumprod_along_batch(data)
@@ -65,14 +66,15 @@
     Returns:
         The cumulative product of elements of input in the sequence
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cumprod_along_seq
     >>> data = {"a": torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]]), "b": torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = cumprod_along_seq(data)
     >>> out
     {'a': tensor([[    1,     2,     6,    24,   120], [    6,    42,   336,  3024, 30240]]), 'b': tensor([[ 4, 12, 24, 24,  0]])}
 
@@ -97,17 +99,18 @@
     Returns:
         The cumulative sum of elements of input in the batch
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cumsum_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = cumsum_along_batch(data)
     >>> out
     {'a': tensor([[ 0,  1], [ 2,  4], [ 6,  9], [12, 16], [20, 25]]), 'b': tensor([ 4,  7,  9, 10, 10])}
 
     ```
     """
     return recursive_apply(data, partial(bt.cumsum_along_batch))
@@ -128,17 +131,18 @@
     Returns:
         The cumulative sum of elements of input in the sequence
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cumsum_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = cumsum_along_seq(data)
     >>> out
     {'a': tensor([[ 0,  1,  3,  6, 10], [ 5, 11, 18, 26, 35]]), 'b': tensor([[ 4,  7,  9, 10, 10]])}
 
     ```
     """
     return recursive_apply(data, partial(bt.cumsum_along_seq))
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/misc.py` & `batchtensor-0.0.4/src/batchtensor/nested/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,17 +19,21 @@
 
     Returns:
         The data after conversion.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import to
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {
+    ...     "a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]),
+    ...     "b": torch.tensor([4, 3, 2, 1, 0]),
+    ... }
     >>> out = to(data, dtype=torch.float)
     >>> out
     {'a': tensor([[0., 1.], [2., 3.], [4., 5.], [6., 7.], [8., 9.]]),
      'b': tensor([4., 3., 2., 1., 0.])}
 
     ```
     """
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/permutation.py` & `batchtensor-0.0.4/src/batchtensor/nested/permutation.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,21 @@
     Raises:
         RuntimeError: if the shape of the permutation does not match
             the batch dimension of the tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import permute_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {
+    ...     "a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]),
+    ...     "b": torch.tensor([4, 3, 2, 1, 0]),
+    ... }
     >>> out = permute_along_batch(data, torch.tensor([2, 1, 3, 0, 4]))
     >>> out
     {'a': tensor([[4, 5], [2, 3], [6, 7], [0, 1], [8, 9]]), 'b': tensor([2, 3, 1, 4, 0])}
 
     ```
     """
     return recursive_apply(data, partial(tensor.permute_along_batch, permutation=permutation))
@@ -74,17 +78,18 @@
     Raises:
         RuntimeError: if the shape of the permutation does not match
             the sequence dimension of the tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import permute_along_seq
-    >>> data = {"a": torch.arange(10).view(2, 5), "b": torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {"a": torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), "b": torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = permute_along_seq(data, torch.tensor([2, 1, 3, 0, 4]))
     >>> out
     {'a': tensor([[2, 1, 3, 0, 4], [7, 6, 8, 5, 9]]), 'b': tensor([[2, 3, 1, 4, 0]])}
 
     ```
     """
     return recursive_apply(data, partial(tensor.permute_along_seq, permutation=permutation))
@@ -96,26 +101,27 @@
     Note:
         This function assumes the batch dimension is the first
             dimension of the tensors. All the tensors should have the
             same batch size.
 
     Args:
         data: The input data. Each item must be a tensor.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         The data with shuffled tensors along the sequence dimension.
             The output data has the same structure as the input data.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import shuffle_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = shuffle_along_batch(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
     ```
     """
     value = next(dfs_tensor(data))
@@ -131,26 +137,27 @@
     Note:
         This function assumes the sequence dimension is the second
             dimension of the tensors. All the tensors should have the
             same sequence size.
 
     Args:
         data: The input data. Each item must be a tensor.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         The data with shuffled tensors along the sequence dimension.
             The output data has the same structure as the input data.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import shuffle_along_seq
-    >>> data = {"a": torch.arange(10).view(2, 5), "b": torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {"a": torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), "b": torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = shuffle_along_seq(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([[...]])}
 
     ```
     """
     value = next(dfs_tensor(data))
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/pointwise.py` & `batchtensor-0.0.4/src/batchtensor/nested/pointwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Returns:
         The absolute value of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import abs
     >>> data = {
     ...     "a": torch.tensor([[-4, -3], [-2, -1], [0, 1], [2, 3], [4, 5]]),
     ...     "b": torch.tensor([2, 1, 0, -1, -2]),
     ... }
     >>> out = abs(data)
@@ -61,14 +62,15 @@
     Returns:
         The clamp value of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import clamp
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = clamp(data, min=1, max=5)
@@ -89,14 +91,15 @@
     Returns:
         The exponential of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import exp
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = exp(data)
@@ -117,14 +120,15 @@
     Returns:
         The base two exponential of the elements. The output has the
             same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import exp2
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = exp2(data)
@@ -145,14 +149,15 @@
     Returns:
         The exponential of the elements minus 1. The output has the
             same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import expm1
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = expm1(data)
@@ -173,14 +178,15 @@
     Returns:
         The natural logarithm of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import log
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = log(data)
@@ -202,14 +208,15 @@
     Returns:
         The logarithm to the base 2 of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import log2
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = log2(data)
@@ -231,14 +238,15 @@
     Returns:
         The with the logarithm to the base 10 of the elements. The
             output has the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import log10
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = log10(data)
@@ -259,14 +267,15 @@
     Returns:
         The natural logarithm of ``(1 + input)``. The output has the
             same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import log1p
     >>> data = {
     ...     "a": torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
     ...     "b": torch.tensor([5, 4, 3, 2, 1]),
     ... }
     >>> out = log1p(data)
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/reduction.py` & `batchtensor-0.0.4/src/batchtensor/nested/reduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,17 +46,21 @@
 
     Returns:
         The maximum of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import amax_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {
+    ...     "a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]),
+    ...     "b": torch.tensor([4, 3, 2, 1, 0]),
+    ... }
     >>> out = amax_along_batch(data)
     >>> out
     {'a': tensor([8, 9]), 'b': tensor(4)}
     >>> out = amax_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[8, 9]]), 'b': tensor([4])}
 
@@ -79,17 +83,18 @@
 
     Returns:
         The maximum of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import amax_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = amax_along_seq(data)
     >>> out
     {'a': tensor([4, 9]), 'b': tensor([4])}
     >>> out = amax_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[4], [9]]), 'b': tensor([[4]])}
 
@@ -112,17 +117,18 @@
 
     Returns:
         The minimum of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import amin_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = amin_along_batch(data)
     >>> out
     {'a': tensor([0, 1]), 'b': tensor(0)}
     >>> out = amin_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[0, 1]]), 'b': tensor([0])}
 
@@ -145,17 +151,18 @@
 
     Returns:
         The minimum of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import amin_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = amin_along_seq(data)
     >>> out
     {'a': tensor([0, 5]), 'b': tensor([0])}
     >>> out = amin_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[0], [5]]), 'b': tensor([[0]])}
 
@@ -180,17 +187,18 @@
     Returns:
         The indices of the maximum value of all elements along the
             batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import argmax_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = argmax_along_batch(data)
     >>> out
     {'a': tensor([4, 4]), 'b': tensor(0)}
     >>> out = argmax_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[4, 4]]), 'b': tensor([0])}
 
@@ -215,17 +223,18 @@
     Returns:
         The indices of the maximum value of all elements along the
             sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import argmax_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = argmax_along_seq(data)
     >>> out
     {'a': tensor([4, 4]), 'b': tensor([0])}
     >>> out = argmax_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[4], [4]]), 'b': tensor([[0]])}
 
@@ -250,17 +259,18 @@
     Returns:
         The indices of the minimum value of all elements along the
             batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import argmin_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = argmin_along_batch(data)
     >>> out
     {'a': tensor([0, 0]), 'b': tensor(4)}
     >>> out = argmin_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[0, 0]]), 'b': tensor([4])}
 
@@ -285,17 +295,18 @@
     Returns:
         The indices of the minimum value of all elements along the
             sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import argmin_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = argmin_along_seq(data)
     >>> out
     {'a': tensor([0, 0]), 'b': tensor([4])}
     >>> out = argmin_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[0], [0]]), 'b': tensor([[4]])}
 
@@ -320,17 +331,18 @@
         The first tensor will be populated with the maximum values and
              the second tensor, which must have dtype long, with their
              indices in the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import max_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = max_along_batch(data)
     >>> out
     {'a': torch.return_types.max(
     values=tensor([8, 9]),
     indices=tensor([4, 4])),
     'b': torch.return_types.max(
     values=tensor(4),
@@ -365,17 +377,18 @@
         The first tensor will be populated with the maximum values and
             the second tensor, which must have dtype long, with their
             indices in the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import max_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = max_along_seq(data)
     >>> out
     {'a': torch.return_types.max(
     values=tensor([4, 9]),
     indices=tensor([4, 4])),
     'b': torch.return_types.max(
     values=tensor([4]),
@@ -408,17 +421,18 @@
 
     Returns:
         The mean of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import mean_along_batch
-    >>> data = {"a": torch.arange(10, dtype=torch.float).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0], dtype=torch.float)}
+    >>> data = {"a": torch.tensor([[0., 1.], [2., 3.], [4., 5.], [6., 7.], [8., 9.]]), "b": torch.tensor([4, 3, 2, 1, 0], dtype=torch.float)}
     >>> out = mean_along_batch(data)
     >>> out
     {'a': tensor([4., 5.]), 'b': tensor(2.)}
     >>> out = mean_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[4., 5.]]), 'b': tensor([2.])}
 
@@ -442,17 +456,18 @@
         This function assumes the sequence dimension is the second
             dimension of the tensors. All the tensors should have the
             same sequence size.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import mean_along_seq
-    >>> data = {'a': torch.arange(10, dtype=torch.float).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]], dtype=torch.float)}
+    >>> data = {'a': torch.tensor([[0., 1., 2., 3., 4.], [5., 6., 7., 8., 9.]]), 'b': torch.tensor([[4, 3, 2, 1, 0]], dtype=torch.float)}
     >>> out = mean_along_seq(data)
     >>> out
     {'a': tensor([2., 7.]), 'b': tensor([2.])}
     >>> out = mean_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[2.], [7.]]), 'b': tensor([[2.]])}
 
@@ -477,17 +492,18 @@
         The first tensor will be populated with the median values and
             the second tensor, which must have dtype long, with their
             indices in the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import median_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = median_along_batch(data)
     >>> out
     {'a': torch.return_types.median(
     values=tensor([4, 5]),
     indices=tensor([2, 2])),
     'b': torch.return_types.median(
     values=tensor(2),
@@ -522,17 +538,18 @@
         The first tensor will be populated with the median values and
             the second tensor, which must have dtype long, with their
             indices in the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import median_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = median_along_seq(data)
     >>> out
     {'a': torch.return_types.median(
     values=tensor([2, 7]),
     indices=tensor([2, 2])),
     'b': torch.return_types.median(
     values=tensor([2]),
@@ -567,17 +584,18 @@
         The first tensor will be populated with the minimum values and
             the second tensor, which must have dtype long, with their
             indices in the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import min_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = min_along_batch(data)
     >>> out
     {'a': torch.return_types.min(
     values=tensor([0, 1]),
     indices=tensor([0, 0])),
     'b': torch.return_types.min(
     values=tensor(0),
@@ -612,17 +630,18 @@
         The first tensor will be populated with the minimum values and
             the second tensor, which must have dtype long, with their
             indices in the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import min_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = min_along_seq(data)
     >>> out
     {'a': torch.return_types.min(
     values=tensor([0, 5]),
     indices=tensor([0, 0])),
     'b': torch.return_types.min(
     values=tensor([0]),
@@ -655,17 +674,18 @@
 
     Returns:
         The product of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import prod_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([5, 4, 3, 2, 1])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([5, 4, 3, 2, 1])}
     >>> out = prod_along_batch(data)
     >>> out
     {'a': tensor([  0, 945]), 'b': tensor(120)}
     >>> out = prod_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[  0, 945]]), 'b': tensor([120])}
 
@@ -688,17 +708,18 @@
 
     Returns:
         The product of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import prod_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[5, 4, 3, 2, 1]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[5, 4, 3, 2, 1]])}
     >>> out = prod_along_seq(data)
     >>> out
     {'a': tensor([    0, 15120]), 'b': tensor([120])}
     >>> out = prod_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[    0], [15120]]), 'b': tensor([[120]])}
 
@@ -721,17 +742,18 @@
 
     Returns:
         The sum of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import sum_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = sum_along_batch(data)
     >>> out
     {'a': tensor([20, 25]), 'b': tensor(10)}
     >>> out = sum_along_batch(data, keepdim=True)
     >>> out
     {'a': tensor([[20, 25]]), 'b': tensor([10])}
 
@@ -754,17 +776,18 @@
 
     Returns:
         The sum of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import sum_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = sum_along_seq(data)
     >>> out
     {'a': tensor([10, 35]), 'b': tensor([10])}
     >>> out = sum_along_seq(data, keepdim=True)
     >>> out
     {'a': tensor([[10], [35]]), 'b': tensor([[10]])}
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/slicing.py` & `batchtensor-0.0.4/src/batchtensor/nested/slicing.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,17 +43,21 @@
 
     Returns:
         The data chuncks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import chunk_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {
+    ...     "a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]),
+    ...     "b": torch.tensor([4, 3, 2, 1, 0]),
+    ... }
     >>> outputs = chunk_along_batch(data, chunks=3)
     >>> outputs
     ({'a': tensor([[0, 1], [2, 3]]), 'b': tensor([4, 3])},
      {'a': tensor([[4, 5], [6, 7]]), 'b': tensor([2, 1])},
      {'a': tensor([[8, 9]]), 'b': tensor([0])})
 
     ```
@@ -85,17 +89,18 @@
 
     Returns:
         The data chuncks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import chunk_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> outputs = chunk_along_seq(data, chunks=3)
     >>> outputs
     ({'a': tensor([[0, 1], [5, 6]]), 'b': tensor([[4, 3]])},
      {'a': tensor([[2, 3], [7, 8]]), 'b': tensor([[2, 1]])},
      {'a': tensor([[4], [9]]), 'b': tensor([[0]])})
 
     ```
@@ -126,17 +131,18 @@
 
     Returns:
         The sliced tensors along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import select_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = select_along_batch(data, index=2)
     >>> out
     {'a': tensor([4, 5]), 'b': tensor(2)}
 
     ```
     """
     return recursive_apply(data, partial(bt.select_along_batch, index=index))
@@ -160,17 +166,18 @@
 
     Returns:
         The sliced tensors along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import select_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = select_along_seq(data, index=2)
     >>> out
     {'a': tensor([2, 7]), 'b': tensor([2])}
 
     ```
     """
     return recursive_apply(data, partial(bt.select_along_seq, index=index))
@@ -182,28 +189,29 @@
     Note:
         This function assumes the batch dimension is the first
             dimension of the tensors. All the tensors should have the
             same batch size.
 
     Args:
         data: The input data. Each item must be a tensor.
-        start: Specifies the index where the slicing of object starts.
-        stop: Specifies the index where the slicing of object stops.
+        start: The index where the slicing of object starts.
+        stop: The index where the slicing of object stops.
             ``None`` means last.
-        step: Specifies the increment between each index for slicing.
+        step: The increment between each index for slicing.
 
     Returns:
         The sliced tensor along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import slice_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> out = slice_along_batch(data, start=2)
     >>> out
     {'a': tensor([[4, 5], [6, 7], [8, 9]]), 'b': tensor([2, 1, 0])}
     >>> out = slice_along_batch(data, stop=3)
     >>> out
     {'a': tensor([[0, 1], [2, 3], [4, 5]]), 'b': tensor([4, 3, 2])}
     >>> out = slice_along_batch(data, step=2)
@@ -221,28 +229,29 @@
     Note:
         This function assumes the sequence dimension is the second
             dimension of the tensors. All the tensors should have the
             same sequence size.
 
     Args:
         data: The input data. Each item must be a tensor.
-        start: Specifies the index where the slicing of object starts.
-        stop: Specifies the index where the slicing of object stops.
+        start: The index where the slicing of object starts.
+        stop: The index where the slicing of object stops.
             ``None`` means last.
-        step: Specifies the increment between each index for slicing.
+        step: The increment between each index for slicing.
 
     Returns:
         The sliced tensor along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import slice_along_seq
-    >>> data = {'a': torch.arange(10).view(2, 5), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {'a': torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), 'b': torch.tensor([[4, 3, 2, 1, 0]])}
     >>> out = slice_along_seq(data, start=2)
     >>> out
     {'a': tensor([[2, 3, 4], [7, 8, 9]]), 'b': tensor([[2, 1, 0]])}
     >>> out = slice_along_seq(data, stop=3)
     >>> out
     {'a': tensor([[0, 1, 2], [5, 6, 7]]), 'b': tensor([[4, 3, 2]])}
     >>> out = slice_along_seq(data, step=2)
@@ -273,17 +282,18 @@
 
     Returns:
         The data chuncks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import split_along_batch
-    >>> data = {"a": torch.arange(10).view(5, 2), "b": torch.tensor([4, 3, 2, 1, 0])}
+    >>> data = {"a": torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]), "b": torch.tensor([4, 3, 2, 1, 0])}
     >>> outputs = split_along_batch(data, split_size_or_sections=2)
     >>> outputs
     ({'a': tensor([[0, 1], [2, 3]]), 'b': tensor([4, 3])},
      {'a': tensor([[4, 5], [6, 7]]), 'b': tensor([2, 1])},
      {'a': tensor([[8, 9]]), 'b': tensor([0])})
 
     ```
@@ -318,17 +328,18 @@
 
     Returns:
         The data chuncks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import split_along_seq
-    >>> data = {"a": torch.arange(10).view(2, 5), "b": torch.tensor([[4, 3, 2, 1, 0]])}
+    >>> data = {"a": torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]]), "b": torch.tensor([[4, 3, 2, 1, 0]])}
     >>> outputs = split_along_seq(data, split_size_or_sections=2)
     >>> outputs
     ({'a': tensor([[0, 1], [5, 6]]), 'b': tensor([[4, 3]])},
      {'a': tensor([[2, 3], [7, 8]]), 'b': tensor([[2, 1]])},
      {'a': tensor([[4], [9]]), 'b': tensor([[0]])})
 
     ```
```

### Comparing `batchtensor-0.0.3/src/batchtensor/nested/trigo.py` & `batchtensor-0.0.4/src/batchtensor/nested/trigo.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     Returns:
         The inverse cosine of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import acos
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = acos(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -59,14 +60,15 @@
     Returns:
         The inverse hyperbolic cosine of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import acosh
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = acosh(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -84,14 +86,15 @@
     Returns:
         The arcsine of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import asin
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = asin(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -110,14 +113,15 @@
     Returns:
         The inverse hyperbolic sine of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import asinh
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = asinh(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -135,14 +139,15 @@
     Returns:
         The arctangent of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import atan
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = atan(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -161,14 +166,15 @@
     Returns:
         The inverse hyperbolic tangent of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import atanh
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = atanh(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -186,14 +192,15 @@
     Returns:
         The cosine of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cos
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = cos(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -211,14 +218,15 @@
     Returns:
         The inverse cosine of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import cosh
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = cosh(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -236,14 +244,15 @@
     Returns:
         The sine of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import sin
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = sin(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -261,14 +270,15 @@
     Returns:
         The hyperbolic sine of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import sinh
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = sinh(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -286,14 +296,15 @@
     Returns:
         The tangent of the elements. The output has the same
             structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import tan
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = tan(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
 
@@ -311,14 +322,15 @@
     Returns:
         The hyperbolic tangent of the elements. The output has
             the same structure as the input.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.nested import tanh
     >>> data = {"a": torch.randn(5, 2), "b": torch.rand(5)}
     >>> out = tanh(data)
     >>> out
     {'a': tensor([[...]]), 'b': tensor([...])}
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/__init__.py` & `batchtensor-0.0.4/src/batchtensor/recursive/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 r"""Contain features to easily work on nested objects."""
 
 from __future__ import annotations
 
 __all__ = [
-    "Applier",
+    "AutoApplier",
     "ApplyState",
     "BaseApplier",
     "DefaultApplier",
     "MappingApplier",
     "SequenceApplier",
     "recursive_apply",
 ]
 
-from batchtensor.recursive.applier import Applier
-from batchtensor.recursive.apply import recursive_apply
+from batchtensor.recursive.auto import AutoApplier
 from batchtensor.recursive.base import BaseApplier
 from batchtensor.recursive.default import DefaultApplier
+from batchtensor.recursive.interface import recursive_apply
 from batchtensor.recursive.mapping import MappingApplier
 from batchtensor.recursive.sequence import SequenceApplier
 from batchtensor.recursive.state import ApplyState
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/applier.py` & `batchtensor-0.0.4/src/batchtensor/recursive/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-r"""Contain the main applier that call other appliers."""
+r"""Contain an applier that can automatically call other appliers based
+on the data type."""
 
 from __future__ import annotations
 
-__all__ = ["Applier"]
+__all__ = ["AutoApplier"]
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from coola.utils import str_indent, str_mapping
 
 from batchtensor.recursive.base import BaseApplier
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Mapping
 
     from batchtensor.recursive import ApplyState
 
 
-class Applier(BaseApplier[Any]):
-    """Implement the default equality tester."""
+class AutoApplier(BaseApplier[Any]):
+    """Implement an applier that can automatically call other appliers
+    based on the data type."""
 
-    registry: dict[type, BaseApplier] = {}
+    registry: ClassVar[dict[type, BaseApplier]] = {}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(\n  {str_indent(str_mapping(self.registry))}\n)"
 
     @classmethod
     def add_applier(cls, data_type: type, applier: BaseApplier, exist_ok: bool = False) -> None:
         r"""Add an applier for a given data type.
 
         Args:
-            data_type: Specifies the data type for this test.
-            applier: Specifies the applier object.
+            data_type: The data type for this test.
+            applier: The applier object.
             exist_ok: If ``False``, ``RuntimeError`` is raised if the
                 data type already exists. This parameter should be set
                 to ``True`` to overwrite the applier for a type.
 
         Raises:
             RuntimeError: if a applier is already registered for the
                 data type and ``exist_ok=False``.
 
         Example usage:
 
         ```pycon
-        >>> from batchtensor.recursive import Applier, SequenceApplier
-        >>> Applier.add_applier(list, SequenceApplier(), exist_ok=True)
+        >>> from batchtensor.recursive import AutoApplier, SequenceApplier
+        >>> AutoApplier.add_applier(list, SequenceApplier(), exist_ok=True)
 
         ```
         """
         if data_type in cls.registry and not exist_ok:
             msg = (
                 f"An applier ({cls.registry[data_type]}) is already registered for the data "
                 f"type {data_type}. Please use `exist_ok=True` if you want to overwrite the "
@@ -60,56 +62,61 @@
         return self.find_applier(type(data)).apply(data, func, state)
 
     @classmethod
     def has_applier(cls, data_type: type) -> bool:
         r"""Indicate if an applier is registered for the given data type.
 
         Args:
-            data_type: Specifies the data type to check.
+            data_type: The data type to check.
 
         Returns:
             ``True`` if an applier is registered, otherwise ``False``.
 
         Example usage:
 
         ```pycon
-        >>> from batchtensor.recursive import Applier
-        >>> Applier.has_applier(list)
+        >>> from batchtensor.recursive import AutoApplier
+        >>> AutoApplier.has_applier(list)
         True
-        >>> Applier.has_applier(str)
+        >>> AutoApplier.has_applier(str)
         False
 
         ```
         """
         return data_type in cls.registry
 
     @classmethod
     def find_applier(cls, data_type: Any) -> BaseApplier:
         r"""Find the applier associated to an object.
 
         Args:
-            data_type: Specifies the data type to get.
+            data_type: The data type to get.
 
         Returns:
             The applier associated to the data type.
 
         Example usage:
 
         ```pycon
-        >>> from batchtensor.recursive import Applier
-        >>> Applier.find_applier(list)
+        >>> from batchtensor.recursive import AutoApplier
+        >>> AutoApplier.find_applier(list)
         SequenceApplier()
 
         ```
         """
         for object_type in data_type.__mro__:
             applier = cls.registry.get(object_type, None)
             if applier is not None:
                 return applier
         msg = f"Incorrect data type: {data_type}"
         raise TypeError(msg)
 
 
 def register_appliers(mapping: Mapping[type, BaseApplier]) -> None:
+    r"""Register some appliers to ``AutoApplier``.
+
+    Args:
+        mapping: The mapping of data types and appliers.
+    """
     for typ, op in mapping.items():
-        if not Applier.has_applier(typ):  # pragma: no cover
-            Applier.add_applier(typ, op)
+        if not AutoApplier.has_applier(typ):  # pragma: no cover
+            AutoApplier.add_applier(typ, op)
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/apply.py` & `batchtensor-0.0.4/src/batchtensor/recursive/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-r"""Contain the main function to recursively apply a function on nested
-data."""
+r"""Contain the main public functions to recursively apply a function on
+nested data."""
 
 from __future__ import annotations
 
 __all__ = ["recursive_apply"]
 
 
 from typing import TYPE_CHECKING, Any
 
-from batchtensor.recursive.applier import Applier
+from batchtensor.recursive.auto import AutoApplier
 from batchtensor.recursive.state import ApplyState
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
-    from batchtensor.recursive import BaseApplier
 
+_applier = AutoApplier()
 
-_applier = Applier()
 
-
-def recursive_apply(data: Any, func: Callable, applier: BaseApplier | None = None) -> Any:
+def recursive_apply(data: Any, func: Callable) -> Any:
     r"""Recursively apply a function on all the items in a nested data.
 
     Args:
-        data: Specifies the input data.
-        func: Specifies the function to apply on each item.
-        applier: Specifies an optional ``BaseApplier`` to customize the
-            logic. By default, ``Applier`` is used.
+        data: The input data.
+        func: The function to apply on each item.
 
     Returns:
         The transformed data.
 
      Example usage:
 
     ```pycon
+
     >>> from batchtensor.recursive import recursive_apply
     >>> out = recursive_apply({"a": 1, "b": "abc"}, str)
     >>> out
     {'a': '1', 'b': 'abc'}
 
     ```
     """
-    applier = applier or _applier
-    return _applier.apply(data=data, func=func, state=ApplyState(applier))
+    return _applier.apply(data=data, func=func, state=ApplyState(_applier))
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/base.py` & `batchtensor-0.0.4/src/batchtensor/recursive/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
     @abstractmethod
     def apply(self, data: T, func: Callable, state: ApplyState) -> T:
         r"""Recursively apply a function on all the items in a nested
         data.
 
         Args:
-            data: Specifies the input data.
-            func: Specifies the function to apply on each item.
-            state: Specifies the current state.
+            data: The input data.
+            func: The function to apply on each item.
+            state: The current state.
 
         Returns:
             The transformed data.
         """
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/default.py` & `batchtensor-0.0.4/src/batchtensor/recursive/default.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 from __future__ import annotations
 
 __all__ = ["DefaultApplier"]
 
 
 from typing import TYPE_CHECKING, Any
 
-from batchtensor.recursive.applier import register_appliers
+from batchtensor.recursive.auto import register_appliers
 from batchtensor.recursive.base import BaseApplier
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from batchtensor.recursive import ApplyState
 
 
 class DefaultApplier(BaseApplier[Any]):
     r"""Define the default applier.
 
     Example usage:
 
     ```pycon
-    >>> from batchtensor.recursive import DefaultApplier, Applier, ApplyState
-    >>> state = ApplyState(applier=Applier())
+
+    >>> from batchtensor.recursive import DefaultApplier, AutoApplier, ApplyState
+    >>> state = ApplyState(applier=AutoApplier())
     >>> applier = DefaultApplier()
     >>> applier
     DefaultApplier()
     >>> out = applier.apply([1, "abc"], str, state)
     >>> out
     "[1, 'abc']"
 
     ```
     """
 
-    def apply(self, data: Any, func: Callable, state: ApplyState) -> Any:
+    def apply(self, data: Any, func: Callable, state: ApplyState) -> Any:  # noqa: ARG002
         return func(data)
 
 
 register_appliers({object: DefaultApplier()})
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/mapping.py` & `batchtensor-0.0.4/src/batchtensor/recursive/mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 from __future__ import annotations
 
 __all__ = ["MappingApplier"]
 
 from collections.abc import Mapping
 from typing import TYPE_CHECKING, TypeVar
 
-from batchtensor.recursive.applier import register_appliers
+from batchtensor.recursive.auto import register_appliers
 from batchtensor.recursive.base import BaseApplier
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from batchtensor.recursive import ApplyState
 
 T = TypeVar("T", Mapping, dict)
 
 
 class MappingApplier(BaseApplier[T]):
-    r"""Define a applier for mappings/dictionaries.
+    r"""Define an applier for mappings/dictionaries.
 
     Example usage:
 
     ```pycon
-    >>> from batchtensor.recursive import MappingApplier, Applier, ApplyState
-    >>> state = ApplyState(applier=Applier())
+
+    >>> from batchtensor.recursive import MappingApplier, AutoApplier, ApplyState
+    >>> state = ApplyState(applier=AutoApplier())
     >>> applier = MappingApplier()
     >>> applier
     MappingApplier()
     >>> out = applier.apply({"a": 1, "b": "abc"}, str, state)
     >>> out
     {'a': '1', 'b': 'abc'}
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/sequence.py` & `batchtensor-0.0.4/src/batchtensor/recursive/sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 __all__ = ["SequenceApplier"]
 
 from collections.abc import Sequence
 from typing import TYPE_CHECKING, TypeVar
 
-from batchtensor.recursive.applier import register_appliers
+from batchtensor.recursive.auto import register_appliers
 from batchtensor.recursive.base import BaseApplier
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from batchtensor.recursive import ApplyState
 
@@ -20,16 +20,17 @@
 
 class SequenceApplier(BaseApplier[T]):
     r"""Define a applier for sequences/lists/tuples.
 
     Example usage:
 
     ```pycon
-    >>> from batchtensor.recursive import SequenceApplier, Applier, ApplyState
-    >>> state = ApplyState(applier=Applier())
+
+    >>> from batchtensor.recursive import SequenceApplier, AutoApplier, ApplyState
+    >>> state = ApplyState(applier=AutoApplier())
     >>> applier = SequenceApplier()
     >>> applier
     SequenceApplier()
     >>> out = applier.apply([1, "abc"], str, state)
     >>> out
     ['1', 'abc']
```

### Comparing `batchtensor-0.0.3/src/batchtensor/recursive/state.py` & `batchtensor-0.0.4/src/batchtensor/recursive/state.py`

 * *Files identical despite different names*

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/__init__.py` & `batchtensor-0.0.4/src/batchtensor/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/comparison.py` & `batchtensor-0.0.4/src/batchtensor/tensor/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     Returns:
         The indices that sort a tensor along the batch dimension
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import argsort_along_batch
     >>> tensor = torch.tensor([[2, 6], [0, 3], [4, 9], [8, 1], [5, 7]])
     >>> out = argsort_along_batch(tensor)
     >>> out
     tensor([[1, 3], [0, 1], [2, 0], [4, 4], [3, 2]])
     >>> out = argsort_along_batch(tensor, descending=True)
@@ -66,14 +67,15 @@
 
     Returns:
         The indices that sort a tensor along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import argsort_along_seq
     >>> tensor = torch.tensor([[7, 3, 0, 8, 5], [1, 9, 6, 4, 2]])
     >>> out = argsort_along_seq(tensor)
     >>> out
     tensor([[2, 1, 4, 0, 3],
             [0, 4, 3, 2, 1]])
@@ -107,14 +109,15 @@
         A namedtuple of (values, indices), where the values are the
             sorted values and indices are the indices of the elements
             in the original input tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import sort_along_batch
     >>> tensor = torch.tensor([[2, 6], [0, 3], [4, 9], [8, 1], [5, 7]])
     >>> out = sort_along_batch(tensor)
     >>> out
     torch.return_types.sort(
     values=tensor([[0, 1], [2, 3], [4, 6], [5, 7], [8, 9]]),
@@ -150,14 +153,15 @@
         A namedtuple of (values, indices), where the values are the
             sorted values and indices are the indices of the elements
             in the original input tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import sort_along_seq
     >>> tensor = torch.tensor([[7, 3, 0, 8, 5], [1, 9, 6, 4, 2]])
     >>> out = sort_along_seq(tensor)
     >>> out
     torch.return_types.sort(
     values=tensor([[0, 3, 5, 7, 8], [1, 2, 4, 6, 9]]),
```

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/indexing.py` & `batchtensor-0.0.4/src/batchtensor/tensor/indexing.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 
     Returns:
         The indexed tensor along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import index_select_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = index_select_along_batch(tensor, torch.tensor([2, 4]))
     >>> out
     tensor([[4, 5],
             [8, 9]])
     >>> out = index_select_along_batch(tensor, torch.tensor([4, 3, 2, 1, 0]))
     >>> out
     tensor([[8, 9],
@@ -64,17 +65,18 @@
 
     Returns:
         The indexed tensor along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import index_select_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = index_select_along_seq(tensor, torch.tensor([2, 4]))
     >>> out
     tensor([[2, 4],
             [7, 9]])
     >>> out = index_select_along_seq(tensor, torch.tensor([4, 3, 2, 1, 0]))
     >>> out
     tensor([[4, 3, 2, 1, 0],
```

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/joining.py` & `batchtensor-0.0.4/src/batchtensor/tensor/joining.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     in the concatenating dimension) or be empty.
 
     Note:
         This function assumes the batch dimension is the first
             dimension.
 
     Args:
-        tensors: Specifies the batches to concatenate.
+        tensors: The tensors to concatenate.
 
     Returns:
         The concatenated tensors along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import cat_along_batch
     >>> tensors = [
     ...     torch.tensor([[0, 1, 2], [4, 5, 6]]),
     ...     torch.tensor([[10, 11, 12], [13, 14, 15]]),
     ... ]
     >>> out = cat_along_batch(tensors)
@@ -54,22 +55,23 @@
     in the concatenating dimension) or be empty.
 
     Note:
         This function assumes the sequence dimension is the second
             dimension.
 
     Args:
-        tensors: Specifies the batches to concatenate.
+        tensors: The tensors to concatenate.
 
     Returns:
         The concatenated tensors along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import cat_along_seq
     >>> tensors = [
     ...     torch.tensor([[0, 1, 2], [4, 5, 6]]),
     ...     torch.tensor([[10, 11], [12, 13]]),
     ... ]
     >>> out = cat_along_seq(tensors)
@@ -87,27 +89,28 @@
 
     Note:
         This function assumes the sequence dimension is the second
             dimension.
 
     Args:
         tensor: The input tensor.
-        repeats: Specifies the number of times to repeat
-            the data along the sequence dimension.
+        repeats: The number of times to repeat the data along the
+            sequence dimension.
 
     Returns:
         A new tensor with the data repeated along the sequence
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import repeat_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = repeat_along_seq(tensor, 2)
     >>> out
     tensor([[0, 1, 2, 3, 4, 0, 1, 2, 3, 4],
             [5, 6, 7, 8, 9, 5, 6, 7, 8, 9]])
 
     ```
     """
```

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/math.py` & `batchtensor-0.0.4/src/batchtensor/tensor/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Returns:
         The cumulative product of elements of input in the batch
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import cumprod_along_batch
     >>> tensor = torch.tensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]])
     >>> out = cumprod_along_batch(tensor)
     >>> out
     tensor([[   1,    2], [   3,    8], [  15,   48], [ 105,  384], [ 945, 3840]])
 
@@ -61,14 +62,15 @@
     Returns:
         The cumulative product of elements of input in the sequence
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import cumprod_along_seq
     >>> tensor = torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])
     >>> out = cumprod_along_seq(tensor)
     >>> out
     tensor([[    1,     2,     6,    24,   120],
             [    6,    42,   336,  3024, 30240]])
@@ -92,17 +94,18 @@
     Returns:
         The cumulative sum of elements of input in the batch
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import cumsum_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = cumsum_along_batch(tensor)
     >>> out
     tensor([[ 0,  1], [ 2,  4], [ 6,  9], [12, 16], [20, 25]])
 
     ```
     """
     return tensor.cumsum(dim=BATCH_DIM)
@@ -122,17 +125,18 @@
     Returns:
         The cumulative sum of elements of input in the sequence
             dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import cumsum_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = cumsum_along_seq(tensor)
     >>> out
     tensor([[ 0,  1,  3,  6, 10],
             [ 5, 11, 18, 26, 35]])
 
     ```
     """
```

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/permutation.py` & `batchtensor-0.0.4/src/batchtensor/tensor/permutation.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,17 +29,18 @@
     Raises:
         RuntimeError: if the shape of the permutation does not match
             the batch dimension of the tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import permute_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = permute_along_batch(tensor, torch.tensor([2, 1, 3, 0, 4]))
     >>> out
     tensor([[4, 5],
             [2, 3],
             [6, 7],
             [0, 1],
             [8, 9]])
@@ -74,17 +75,18 @@
     Raises:
         RuntimeError: if the shape of the permutation does not match
             the sequence dimension of the tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import permute_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = permute_along_seq(tensor, torch.tensor([2, 1, 3, 0, 4]))
     >>> out
     tensor([[2, 1, 3, 0, 4],
             [7, 6, 8, 5, 9]])
 
     ```
     """
@@ -104,25 +106,26 @@
 
     Note:
         This function assumes the batch dimension is the first
             dimension.
 
     Args:
         tensor: The tensor to split.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         The shuffled tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import shuffle_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = shuffle_along_batch(tensor)
     >>> out
     tensor([[...]])
 
     ```
     """
     return permute_along_batch(
@@ -138,25 +141,26 @@
 
     Note:
         This function assumes the sequence dimension is the second
             dimension.
 
     Args:
         tensor: The tensor to split.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         The shuffled tensor.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import shuffle_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = shuffle_along_seq(tensor)
     >>> out
     tensor([[...]])
 
     ```
     """
     return permute_along_seq(
```

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/reduction.py` & `batchtensor-0.0.4/src/batchtensor/tensor/reduction.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,17 +44,18 @@
 
     Returns:
         The maximum of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import amax_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = amax_along_batch(tensor)
     >>> out
     tensor([8, 9])
     >>> out = amax_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[8, 9]])
 
@@ -76,17 +77,18 @@
 
     Returns:
         The maximum of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import amax_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = amax_along_seq(tensor)
     >>> out
     tensor([4, 9])
     >>> out = amax_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[4], [9]])
 
@@ -108,17 +110,18 @@
 
     Returns:
         The minimum of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import amin_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = amin_along_batch(tensor)
     >>> out
     tensor([0, 1])
     >>> out = amin_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[0, 1]])
 
@@ -140,17 +143,18 @@
 
     Returns:
         The minimum of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import amin_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = amin_along_seq(tensor)
     >>> out
     tensor([0, 5])
     >>> out = amin_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[0], [5]])
 
@@ -174,17 +178,18 @@
     Returns:
         The indices of the maximum value of all elements along the
             batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import argmax_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = argmax_along_batch(tensor)
     >>> out
     tensor([4, 4])
     >>> out = argmax_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[4, 4]])
 
@@ -208,17 +213,18 @@
     Returns:
         The indices of the maximum value of all elements along the
             sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import argmax_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = argmax_along_seq(tensor)
     >>> out
     tensor([4, 4])
     >>> out = argmax_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[4], [4]])
 
@@ -242,17 +248,18 @@
     Returns:
         The indices of the minimum value of all elements along the
             batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import argmin_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = argmin_along_batch(tensor)
     >>> out
     tensor([0, 0])
     >>> out = argmin_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[0, 0]])
 
@@ -276,17 +283,18 @@
     Returns:
         The indices of the minimum value of all elements along the
             sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import argmin_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = argmin_along_seq(tensor)
     >>> out
     tensor([0, 0])
     >>> out = argmin_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[0], [0]])
 
@@ -310,17 +318,18 @@
         The first tensor will be populated with the maximum values and
             the second tensor, which must have dtype long, with their
             indices in the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import max_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = max_along_batch(tensor)
     >>> out
     torch.return_types.max(
     values=tensor([8, 9]),
     indices=tensor([4, 4]))
     >>> out = max_along_batch(tensor, keepdim=True)
     >>> out
@@ -348,17 +357,18 @@
         The first tensor will be populated with the maximum values and
             the second tensor, which must have dtype long, with their
             indices in the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import max_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = max_along_seq(tensor)
     >>> out
     torch.return_types.max(
     values=tensor([4, 9]),
     indices=tensor([4, 4]))
     >>> out = max_along_seq(tensor, keepdim=True)
     >>> out
@@ -384,17 +394,18 @@
 
     Returns:
         The mean of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import mean_along_batch
-    >>> tensor = torch.arange(10, dtype=torch.float).view(5, 2)
+    >>> tensor = torch.tensor([[0., 1.], [2., 3.], [4., 5.], [6., 7.], [8., 9.]])
     >>> out = mean_along_batch(tensor)
     >>> out
     tensor([4., 5.])
     >>> out = mean_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[4., 5.]])
 
@@ -416,17 +427,18 @@
 
     Returns:
         The mean of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import mean_along_seq
-    >>> tensor = torch.arange(10, dtype=torch.float).view(2, 5)
+    >>> tensor = torch.tensor([[0., 1., 2., 3., 4.], [5., 6., 7., 8., 9.]])
     >>> out = mean_along_seq(tensor)
     >>> out
     tensor([2., 7.])
     >>> out = mean_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[2.], [7.]])
 
@@ -450,17 +462,18 @@
         The first tensor will be populated with the median values and
             the second tensor, which must have dtype long, with their
             indices in the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import median_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = median_along_batch(tensor)
     >>> out
     torch.return_types.median(
     values=tensor([4, 5]),
     indices=tensor([2, 2]))
     >>> out = median_along_batch(tensor, keepdim=True)
     >>> out
@@ -488,17 +501,18 @@
         The first tensor will be populated with the median values and
             the second tensor, which must have dtype long, with their
             indices in the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import median_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = median_along_seq(tensor)
     >>> out
     torch.return_types.median(
     values=tensor([2, 7]),
     indices=tensor([2, 2]))
     >>> out = median_along_seq(tensor, keepdim=True)
     >>> out
@@ -526,17 +540,18 @@
         The first tensor will be populated with the minimum values and
             the second tensor, which must have dtype long, with their
             indices in the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import min_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = min_along_batch(tensor)
     >>> out
     torch.return_types.min(
     values=tensor([0, 1]),
     indices=tensor([0, 0]))
     >>> out = min_along_batch(tensor, keepdim=True)
     >>> out
@@ -564,17 +579,18 @@
         The first tensor will be populated with the minimum values and
             the second tensor, which must have dtype long, with their
             indices in the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import min_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = min_along_seq(tensor)
     >>> out
     torch.return_types.min(
     values=tensor([0, 5]),
     indices=tensor([0, 0]))
     >>> out = min_along_seq(tensor, keepdim=True)
     >>> out
@@ -600,17 +616,18 @@
 
     Returns:
         The product of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import prod_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = prod_along_batch(tensor)
     >>> out
     tensor([  0, 945])
     >>> out = prod_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[  0, 945]])
 
@@ -632,17 +649,18 @@
 
     Returns:
         The product of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import prod_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = prod_along_seq(tensor)
     >>> out
     tensor([    0, 15120])
     >>> out = prod_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[    0], [15120]])
 
@@ -664,17 +682,18 @@
 
     Returns:
         The sum of all elements along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import sum_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = sum_along_batch(tensor)
     >>> out
     tensor([20, 25])
     >>> out = sum_along_batch(tensor, keepdim=True)
     >>> out
     tensor([[20, 25]])
 
@@ -696,17 +715,18 @@
 
     Returns:
         The sum of all elements along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import sum_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = sum_along_seq(tensor)
     >>> out
     tensor([10, 35])
     >>> out = sum_along_seq(tensor, keepdim=True)
     >>> out
     tensor([[10], [35]])
```

### Comparing `batchtensor-0.0.3/src/batchtensor/tensor/slicing.py` & `batchtensor-0.0.4/src/batchtensor/tensor/slicing.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 
     Returns:
         The tensor chunks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import chunk_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> outputs = chunk_along_batch(tensor, chunks=3)
     >>> outputs
     (tensor([[0, 1], [2, 3]]),
      tensor([[4, 5], [6, 7]]),
      tensor([[8, 9]]))
 
     ```
@@ -72,17 +73,18 @@
 
     Returns:
         The tensor chunks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import chunk_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> outputs = chunk_along_seq(tensor, chunks=3)
     >>> outputs
     (tensor([[0, 1], [5, 6]]),
      tensor([[2, 3], [7, 8]]),
      tensor([[4], [9]]))
 
     ```
@@ -106,17 +108,18 @@
 
     Returns:
         The sliced tensor along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import select_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = select_along_batch(tensor, index=2)
     >>> out
     tensor([4, 5])
 
     ```
     """
     return tensor[index]
@@ -138,17 +141,18 @@
 
     Returns:
         The sliced tensor along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import select_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> out = select_along_seq(tensor, index=2)
     >>> out
     tensor([2, 7])
 
     ```
     """
     return tensor[:, index]
@@ -161,28 +165,29 @@
 
     Note:
         This function assumes the batch dimension is the first
             dimension.
 
     Args:
         tensor: The input tensor.
-        start: Specifies the index where the slicing of object starts.
-        stop: Specifies the index where the slicing of object stops.
+        start: The index where the slicing of object starts.
+        stop: The index where the slicing of object stops.
             ``None`` means last.
-        step: Specifies the increment between each index for slicing.
+        step: The increment between each index for slicing.
 
     Returns:
         The sliced tensor along the batch dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import slice_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> out = slice_along_batch(tensor, start=2)
     >>> out
     tensor([[4, 5],
             [6, 7],
             [8, 9]])
     >>> out = slice_along_batch(tensor, stop=3)
     >>> out
@@ -207,25 +212,26 @@
 
     Note:
         This function assumes the sequence dimension is the second
             dimension.
 
     Args:
         tensor: The input tensor.
-        start: Specifies the index where the slicing of object starts.
-        stop: Specifies the index where the slicing of object stops.
+        start: The index where the slicing of object starts.
+        stop: The index where the slicing of object stops.
             ``None`` means last.
-        step: Specifies the increment between each index for slicing.
+        step: The increment between each index for slicing.
 
     Returns:
         The sliced tensor along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import slice_along_seq
     >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [9, 8, 7, 6, 5]])
     >>> out = slice_along_seq(tensor, start=2)
     >>> out
     tensor([[2, 3, 4],
             [7, 6, 5]])
@@ -261,17 +267,18 @@
 
     Returns:
         The tensor chunks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import split_along_batch
-    >>> tensor = torch.arange(10).view(5, 2)
+    >>> tensor = torch.tensor([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]])
     >>> outputs = split_along_batch(tensor, split_size_or_sections=2)
     >>> outputs
     (tensor([[0, 1], [2, 3]]),
      tensor([[4, 5], [6, 7]]),
      tensor([[8, 9]]))
 
     ```
@@ -297,17 +304,18 @@
 
     Returns:
         The tensor chunks.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.tensor import split_along_seq
-    >>> tensor = torch.arange(10).view(2, 5)
+    >>> tensor = torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]])
     >>> outputs = split_along_seq(tensor, split_size_or_sections=2)
     >>> outputs
     (tensor([[0, 1], [5, 6]]),
      tensor([[2, 3], [7, 8]]),
      tensor([[4], [9]]))
 
     ```
```

### Comparing `batchtensor-0.0.3/src/batchtensor/utils/bfs.py` & `batchtensor-0.0.4/src/batchtensor/utils/bfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "register_default_iterators",
 ]
 
 import logging
 from collections import deque
 from collections.abc import Generator, Iterable, Mapping
 from dataclasses import dataclass
-from typing import Any, Generic, TypeVar
+from typing import Any, ClassVar, Generic, TypeVar
 
 import torch
 from coola.utils import str_indent, str_mapping
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
@@ -32,25 +32,26 @@
     r"""Implement a Breadth-First Search (BFS) iterator over the
     ``torch.Tensor``s.
 
     This function assumes the underlying data has a tree-like
     structure.
 
     Args:
-        data: Specifies the data to iterate on.
+        data: The data to iterate on.
 
     Yields:
         The next ``torch.Tensor`` in the data.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.utils.bfs import bfs_tensor
-    >>> list(bfs_tensor(["abc", torch.ones(2, 3), 42, torch.arange(5)]))
+    >>> list(bfs_tensor(["abc", torch.ones(2, 3), 42, torch.tensor([0, 1, 2, 3, 4])]))
     [tensor([[1., 1., 1.], [1., 1., 1.]]), tensor([0, 1, 2, 3, 4])]
 
     ```
     """
     state = IteratorState(iterator=TensorIterator(), queue=deque([data]))
     while state.queue:
         item = state.queue.popleft()
@@ -72,27 +73,27 @@
     r"""Define the base class to iterate over the data to find the
     tensors with a Breadth-First Search (BFS) strategy."""
 
     def iterate(self, data: T, state: IteratorState) -> None:
         r"""Iterate over the data and add the items to the queue.
 
         Args:
-            data: Specifies the data to iterate on.
-            state: Specifies the current state, which include the
+            data: The data to iterate on.
+            state: The current state, which include the
                 queue.
         """
 
 
 class DefaultTensorIterator(BaseTensorIterator[Any]):
     r"""Implement the default tensor iterator."""
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}()"
 
-    def iterate(self, data: Any, state: IteratorState) -> None:
+    def iterate(self, data: Any, state: IteratorState) -> None:  # noqa: ARG002
         return
 
 
 class IterableTensorIterator(BaseTensorIterator[Iterable]):
     r"""Implement the tensor iterator for iterable objects."""
 
     def __repr__(self) -> str:
@@ -113,28 +114,28 @@
         for item in data.values():
             state.queue.append(item)
 
 
 class TensorIterator(BaseTensorIterator[Any]):
     """Implement a tensor iterator."""
 
-    registry: dict[type, BaseTensorIterator] = {}
+    registry: ClassVar[dict[type, BaseTensorIterator]] = {}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(\n  {str_indent(str_mapping(self.registry))}\n)"
 
     @classmethod
     def add_iterator(
         cls, data_type: type, iterator: BaseTensorIterator, exist_ok: bool = False
     ) -> None:
         r"""Add an iterator for a given data type.
 
         Args:
-            data_type: Specifies the data type for this test.
-            iterator: Specifies the iterator object.
+            data_type: The data type for this test.
+            iterator: The iterator object.
             exist_ok: If ``False``, ``RuntimeError`` is raised if the
                 data type already exists. This parameter should be set
                 to ``True`` to overwrite the iterator for a type.
 
         Raises:
             RuntimeError: if an iterator is already registered for the
                 data type and ``exist_ok=False``.
@@ -161,15 +162,15 @@
 
     @classmethod
     def has_iterator(cls, data_type: type) -> bool:
         r"""Indicate if an iterator is registered for the given data
         type.
 
         Args:
-            data_type: Specifies the data type to check.
+            data_type: The data type to check.
 
         Returns:
             ``True`` if an iterator is registered, otherwise ``False``.
 
         Example usage:
 
         ```pycon
@@ -184,15 +185,15 @@
         return data_type in cls.registry
 
     @classmethod
     def find_iterator(cls, data_type: Any) -> BaseTensorIterator:
         r"""Find the iterator associated to an object.
 
         Args:
-            data_type: Specifies the data type to get.
+            data_type: The data type to get.
 
         Returns:
             The iterator associated to the data type.
 
         Example usage:
 
         ```pycon
@@ -210,15 +211,15 @@
         raise TypeError(msg)
 
 
 def register_iterators(mapping: Mapping[type, BaseTensorIterator]) -> None:
     r"""Register some iterators.
 
     Args:
-        mapping: Specifies the iterators to register.
+        mapping: The iterators to register.
     """
     for typ, op in mapping.items():
         if not TensorIterator.has_iterator(typ):  # pragma: no cover
             TensorIterator.add_iterator(typ, op)
 
 
 def register_default_iterators() -> None:
```

### Comparing `batchtensor-0.0.3/src/batchtensor/utils/dfs.py` & `batchtensor-0.0.4/src/batchtensor/utils/dfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "register_default_iterators",
 ]
 
 import logging
 from collections import deque
 from collections.abc import Generator, Iterable, Mapping
 from dataclasses import dataclass
-from typing import Any, Generic, TypeVar
+from typing import Any, ClassVar, Generic, TypeVar
 
 import torch
 from coola.utils import str_indent, str_mapping
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
@@ -32,25 +32,26 @@
     r"""Implement a Depth-First Search (DFS) iterator over the
     ``torch.Tensor``s.
 
     This function assumes the underlying data has a tree-like
     structure.
 
     Args:
-        data: Specifies the data to iterate on.
+        data: The data to iterate on.
 
     Yields:
         The next ``torch.Tensor`` in the data.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.utils.dfs import dfs_tensor
-    >>> list(dfs_tensor(["abc", torch.ones(2, 3), 42, torch.arange(5)]))
+    >>> list(dfs_tensor(["abc", torch.ones(2, 3), 42, torch.tensor([0, 1, 2, 3, 4])]))
     [tensor([[1., 1., 1.], [1., 1., 1.]]), tensor([0, 1, 2, 3, 4])]
 
     ```
     """
     state = IteratorState(iterator=TensorIterator())
     yield from state.iterator.iterate(data, state)
 
@@ -66,30 +67,34 @@
     r"""Define the base class to iterate over the data to find the
     tensors with a Depth-First Search (DFS) strategy."""
 
     def iterate(self, data: T, state: IteratorState) -> Generator[torch.Tensor, None, None]:
         r"""Iterate over the data and add the items to the queue.
 
         Args:
-            data: Specifies the data to iterate on.
-            state: Specifies the current state, which include the
+            data: The data to iterate on.
+            state: The current state, which include the
                 queue.
 
         Yields:
             The next ``torch.Tensor`` in the data.
         """
 
 
 class DefaultTensorIterator(BaseTensorIterator[Any]):
     r"""Implement the default tensor iterator."""
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}()"
 
-    def iterate(self, data: Any, state: IteratorState) -> Generator[torch.Tensor, None, None]:
+    def iterate(
+        self,
+        data: Any,
+        state: IteratorState,  # noqa: ARG002
+    ) -> Generator[torch.Tensor, None, None]:
         if torch.is_tensor(data):
             yield data
 
 
 class IterableTensorIterator(BaseTensorIterator[Iterable]):
     r"""Implement the tensor iterator for iterable objects."""
 
@@ -111,28 +116,28 @@
         for item in data.values():
             yield from state.iterator.iterate(item, state)
 
 
 class TensorIterator(BaseTensorIterator[Any]):
     """Implement a tensor iterator."""
 
-    registry: dict[type, BaseTensorIterator] = {}
+    registry: ClassVar[dict[type, BaseTensorIterator]] = {}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(\n  {str_indent(str_mapping(self.registry))}\n)"
 
     @classmethod
     def add_iterator(
         cls, data_type: type, iterator: BaseTensorIterator, exist_ok: bool = False
     ) -> None:
         r"""Add an iterator for a given data type.
 
         Args:
-            data_type: Specifies the data type for this test.
-            iterator: Specifies the iterator object.
+            data_type: The data type for this test.
+            iterator: The iterator object.
             exist_ok: If ``False``, ``RuntimeError`` is raised if the
                 data type already exists. This parameter should be set
                 to ``True`` to overwrite the iterator for a type.
 
         Raises:
             RuntimeError: if an iterator is already registered for the
                 data type and ``exist_ok=False``.
@@ -159,15 +164,15 @@
 
     @classmethod
     def has_iterator(cls, data_type: type) -> bool:
         r"""Indicate if an iterator is registered for the given data
         type.
 
         Args:
-            data_type: Specifies the data type to check.
+            data_type: The data type to check.
 
         Returns:
             ``True`` if an iterator is registered, otherwise ``False``.
 
         Example usage:
 
         ```pycon
@@ -182,15 +187,15 @@
         return data_type in cls.registry
 
     @classmethod
     def find_iterator(cls, data_type: Any) -> BaseTensorIterator:
         r"""Find the iterator associated to an object.
 
         Args:
-            data_type: Specifies the data type to get.
+            data_type: The data type to get.
 
         Returns:
             The iterator associated to the data type.
 
         Example usage:
 
         ```pycon
@@ -208,15 +213,15 @@
         raise TypeError(msg)
 
 
 def register_iterators(mapping: Mapping[type, BaseTensorIterator]) -> None:
     r"""Register some iterators.
 
     Args:
-        mapping: Specifies the iterators to register.
+        mapping: The iterators to register.
     """
     for typ, op in mapping.items():
         if not TensorIterator.has_iterator(typ):  # pragma: no cover
             TensorIterator.add_iterator(typ, op)
 
 
 def register_default_iterators() -> None:
```

### Comparing `batchtensor-0.0.3/src/batchtensor/utils/seed.py` & `batchtensor-0.0.4/src/batchtensor/utils/seed.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import torch
 
 
 def get_random_seed(seed: int) -> int:
     r"""Get a random seed.
 
     Args:
-        seed: Specifies a random seed to make the process
-            reproducible.
+        seed: A random seed to make the process reproducible.
 
     Returns:
-        int: A random seed. The value is between ``-2 ** 63`` and
+        A random seed. The value is between ``-2 ** 63`` and
             ``2 ** 63 - 1``.
 
     Example usage:
 
     ```pycon
+
     >>> from batchtensor.utils.seed import get_random_seed
     >>> get_random_seed(44)
     6176747449835261347
 
     ```
     """
     return torch.randint(-(2**63), 2**63 - 1, size=(1,), generator=get_torch_generator(seed)).item()
@@ -33,23 +33,24 @@
 
 def get_torch_generator(
     random_seed: int = 1, device: torch.device | str | None = "cpu"
 ) -> torch.Generator:
     r"""Create a ``torch.Generator`` initialized with a given seed.
 
     Args:
-        random_seed: Specifies a random seed.
-        device: Specifies the desired device for the generator.
+        random_seed: A random seed.
+        device: The desired device for the generator.
 
     Returns:
-        ``torch.Generator``
+        A ``torch.Generator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from batchtensor.utils.seed import get_torch_generator
     >>> generator = get_torch_generator(42)
     >>> torch.rand(2, 4, generator=generator)
     tensor([[0.8823, 0.9150, 0.3829, 0.9593],
             [0.3904, 0.6009, 0.2566, 0.7936]])
     >>> generator = get_torch_generator(42)
@@ -64,23 +65,24 @@
     return generator
 
 
 def setup_torch_generator(generator_or_seed: int | torch.Generator) -> torch.Generator:
     r"""Set up a ``torch.Generator`` object.
 
     Args:
-        generator_or_seed: Specifies a ``torch.Generator`` object or
-            a random seed.
+        generator_or_seed: A ``torch.Generator`` object or a random
+            seed.
 
     Returns:
         A ``torch.Generator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from batchtensor.utils.seed import setup_torch_generator
     >>> generator = setup_torch_generator(42)
     >>> generator
     <torch._C.Generator object at 0x...>
 
     ```
     """
```

### Comparing `batchtensor-0.0.3/PKG-INFO` & `batchtensor-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchtensor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions to manipulate batches of PyTorch tensors
 Home-page: https://github.com/durandtibo/batchtensor
 License: BSD-3-Clause
 Keywords: batch,sequence,pytorch,tensor
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: coola (>=0.1,<1.0)
 Requires-Dist: numpy (>=1.21,<2.0) ; extra == "all"
+Requires-Dist: torch (>=1.11,<2.3) ; sys_platform == "darwin" and platform_machine != "arm64"
 Requires-Dist: torch (>=1.11,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/batchtensor
 Description-Content-Type: text/markdown
 
 # batchtensor
 
 <p align="center">
@@ -171,20 +172,21 @@
 pip install batchtensor[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/batchtensor/get_started) to see how
 to install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `batchtensor` versions and tested dependencies.
 
-| `batchtensor` | `coola`      | `torch`       | `python`      |
-|---------------|--------------|---------------|---------------|
-| `main`        | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` |
-| `0.0.3`       | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` |
-| `0.0.2`       | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` |
-| `0.0.1`       | `>=0.1,<0.4` | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `batchtensor` | `coola`      | `numpy`<sup>*</sup> | `torch`       | `python`      |
+|---------------|--------------|---------------------|---------------|---------------|
+| `main`        | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.4`       | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.3`       | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.2`       | `>=0.1,<1.0` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
+| `0.0.1`       | `>=0.1,<0.4` | `>=1.21,<2.0`       | `>=1.11,<3.0` | `>=3.9,<3.13` |
 
 <sup>*</sup> indicates an optional dependency
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: batchtensor Version: 0.0.3 Summary: Functions to
+Metadata-Version: 2.1 Name: batchtensor Version: 0.0.4 Summary: Functions to
 manipulate batches of PyTorch tensors Home-page: https://github.com/durandtibo/
 batchtensor License: BSD-3-Clause Keywords: batch,sequence,pytorch,tensor
 Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com Requires-Python:
 >=3.9,<3.13 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries Provides-Extra: all
 Requires-Dist: coola (>=0.1,<1.0) Requires-Dist: numpy (>=1.21,<2.0) ; extra ==
-"all" Requires-Dist: torch (>=1.11,<3.0) Project-URL: Repository, https://
-github.com/durandtibo/batchtensor Description-Content-Type: text/markdown #
-batchtensor
+"all" Requires-Dist: torch (>=1.11,<2.3) ; sys_platform == "darwin" and
+platform_machine != "arm64" Requires-Dist: torch (>=1.11,<3.0) Project-URL:
+Repository, https://github.com/durandtibo/batchtensor Description-Content-Type:
+text/markdown # batchtensor
                   _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
                         _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_1_4_8_e_d_c_2_6_a_d_d_1_3_8_d_0_4_9_2_8_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_1_4_8_e_d_c_2_6_a_d_d_1_3_8_d_0_4_9_2_8_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
@@ -60,21 +61,23 @@
 command: ```shell pip install batchtensor ``` To make the package as slim as
 possible, only the minimal packages required to use `batchtensor` are
 installed. To include all the dependencies, you can use the following command:
 ```shell pip install batchtensor[all] ``` Please check the [get started page]
 (https://durandtibo.github.io/batchtensor/get_started) to see how to install
 only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `batchtensor` versions and tested
-dependencies. | `batchtensor` | `coola` | `torch` | `python` | |---------------
-|--------------|---------------|---------------| | `main` | `>=0.1,<1.0` |
-`>=1.11,<3.0` | `>=3.9,<3.13` | | `0.0.3` | `>=0.1,<1.0` | `>=1.11,<3.0` |
-`>=3.9,<3.13` | | `0.0.2` | `>=0.1,<1.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
-`0.0.1` | `>=0.1,<0.4` | `>=1.11,<3.0` | `>=3.9,<3.13` | * indicates an
-optional dependency ## Contributing Please check the instructions in
-[CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions and Communication
+dependencies. | `batchtensor` | `coola` | `numpy`* | `torch` | `python` | |----
+-----------|--------------|---------------------|---------------|--------------
+-| | `main` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.4` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.3` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.2` | `>=0.1,<1.0` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | |
+`0.0.1` | `>=0.1,<0.4` | `>=1.21,<2.0` | `>=1.11,<3.0` | `>=3.9,<3.13` | *
+indicates an optional dependency ## Contributing Please check the instructions
+in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions and Communication
 Everyone is welcome to contribute to the community. If you have any questions
 or suggestions, you can submit [Github Issues](https://github.com/durandtibo/
 batchtensor/issues). We will reply to you as soon as possible. Thank you very
 much. ## API stability :warning: While `batchtensor` is in development stage,
 no API is guaranteed to be stable from one release to the next. In fact, it is
 very likely that the API will change multiple times before a stable 1.0.0
 release. In practice, this means that upgrading `batchtensor` to a new version
```

