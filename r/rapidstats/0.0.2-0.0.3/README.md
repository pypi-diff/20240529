# Comparing `tmp/rapidstats-0.0.2.tar.gz` & `tmp/rapidstats-0.0.3.tar.gz`

## Comparing `rapidstats-0.0.2.tar` & `rapidstats-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 rapidstats-0.0.2/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-05-29 00:30:56.000000 rapidstats-0.0.2/.github/workflows/CI.yaml
--rw-r--r--   0     1001      127      666 2024-05-29 00:30:56.000000 rapidstats-0.0.2/.github/workflows/tests.yaml
--rw-r--r--   0     1001      127     1504 2024-05-29 00:30:56.000000 rapidstats-0.0.2/.gitignore
--rw-r--r--   0     1001      127      701 2024-05-29 00:30:56.000000 rapidstats-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1078 2024-05-29 00:30:56.000000 rapidstats-0.0.2/LICENSE
--rw-r--r--   0     1001      127     1027 2024-05-29 00:30:56.000000 rapidstats-0.0.2/README.md
--rw-r--r--   0     1001      127    84498 2024-05-29 00:30:56.000000 rapidstats-0.0.2/benchmarks/analyze_benchmarks.ipynb
--rw-r--r--   0     1001      127     2495 2024-05-29 00:30:56.000000 rapidstats-0.0.2/benchmarks/benchmark.py
--rw-r--r--   0     1001      127      101 2024-05-29 00:30:56.000000 rapidstats-0.0.2/python/rapidstats/__init__.py
--rw-r--r--   0     1001      127     3806 2024-05-29 00:30:56.000000 rapidstats-0.0.2/python/rapidstats/_bootstrap.py
--rw-r--r--   0     1001      127     1499 2024-05-29 00:30:56.000000 rapidstats-0.0.2/python/rapidstats/_metrics.py
--rw-r--r--   0     1001      127      628 2024-05-29 00:30:56.000000 rapidstats-0.0.2/python/rapidstats/_rustystats.pyi
--rw-r--r--   0     1001      127     1184 2024-05-29 00:30:56.000000 rapidstats-0.0.2/python/rapidstats/_utils.py
--rw-r--r--   0     1001      127        0 2024-05-29 00:30:56.000000 rapidstats-0.0.2/python/rapidstats/py.typed
--rw-r--r--   0     1001      127      845 2024-05-29 00:30:56.000000 rapidstats-0.0.2/release.py
--rw-r--r--   0     1001      127     1058 2024-05-29 00:30:56.000000 rapidstats-0.0.2/requirements_dev.txt
--rw-r--r--   0     1001      127      906 2024-05-29 00:30:56.000000 rapidstats-0.0.2/src/bootstrap.rs
--rw-r--r--   0     1001      127     1871 2024-05-29 00:30:56.000000 rapidstats-0.0.2/src/lib.rs
--rw-r--r--   0     1001      127     7122 2024-05-29 00:30:56.000000 rapidstats-0.0.2/src/metrics.rs
--rw-r--r--   0     1001      127        0 2024-05-29 00:30:56.000000 rapidstats-0.0.2/src/rustystats.rs
--rw-r--r--   0     1001      127     3166 2024-05-29 00:30:56.000000 rapidstats-0.0.2/tests/test_rapidstats.py
--rw-r--r--   0     1001      127      308 2024-05-29 00:30:56.000000 rapidstats-0.0.2/tox.ini
--rw-r--r--   0     1001      127    45588 2024-05-29 00:30:56.000000 rapidstats-0.0.2/Cargo.lock
--rw-r--r--   0     1001      127     1083 2024-05-29 00:30:56.000000 rapidstats-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 rapidstats-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 rapidstats-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-05-29 01:43:24.000000 rapidstats-0.0.3/.github/workflows/CI.yaml
+-rw-r--r--   0     1001      127      666 2024-05-29 01:43:24.000000 rapidstats-0.0.3/.github/workflows/tests.yaml
+-rw-r--r--   0     1001      127     1504 2024-05-29 01:43:24.000000 rapidstats-0.0.3/.gitignore
+-rw-r--r--   0     1001      127      701 2024-05-29 01:43:24.000000 rapidstats-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1078 2024-05-29 01:43:24.000000 rapidstats-0.0.3/LICENSE
+-rw-r--r--   0     1001      127     1027 2024-05-29 01:43:24.000000 rapidstats-0.0.3/README.md
+-rw-r--r--   0     1001      127    84498 2024-05-29 01:43:24.000000 rapidstats-0.0.3/benchmarks/analyze_benchmarks.ipynb
+-rw-r--r--   0     1001      127     2495 2024-05-29 01:43:24.000000 rapidstats-0.0.3/benchmarks/benchmark.py
+-rw-r--r--   0     1001      127      101 2024-05-29 01:43:24.000000 rapidstats-0.0.3/python/rapidstats/__init__.py
+-rw-r--r--   0     1001      127     3806 2024-05-29 01:43:24.000000 rapidstats-0.0.3/python/rapidstats/_bootstrap.py
+-rw-r--r--   0     1001      127     1499 2024-05-29 01:43:24.000000 rapidstats-0.0.3/python/rapidstats/_metrics.py
+-rw-r--r--   0     1001      127      628 2024-05-29 01:43:24.000000 rapidstats-0.0.3/python/rapidstats/_rustystats.pyi
+-rw-r--r--   0     1001      127     1184 2024-05-29 01:43:24.000000 rapidstats-0.0.3/python/rapidstats/_utils.py
+-rw-r--r--   0     1001      127        0 2024-05-29 01:43:24.000000 rapidstats-0.0.3/python/rapidstats/py.typed
+-rw-r--r--   0     1001      127      845 2024-05-29 01:43:24.000000 rapidstats-0.0.3/release.py
+-rw-r--r--   0     1001      127     1092 2024-05-29 01:43:24.000000 rapidstats-0.0.3/requirements_dev.txt
+-rw-r--r--   0     1001      127      906 2024-05-29 01:43:24.000000 rapidstats-0.0.3/src/bootstrap.rs
+-rw-r--r--   0     1001      127     1871 2024-05-29 01:43:24.000000 rapidstats-0.0.3/src/lib.rs
+-rw-r--r--   0     1001      127     7122 2024-05-29 01:43:24.000000 rapidstats-0.0.3/src/metrics.rs
+-rw-r--r--   0     1001      127        0 2024-05-29 01:43:24.000000 rapidstats-0.0.3/src/rustystats.rs
+-rw-r--r--   0     1001      127     3166 2024-05-29 01:43:24.000000 rapidstats-0.0.3/tests/test_rapidstats.py
+-rw-r--r--   0     1001      127      308 2024-05-29 01:43:24.000000 rapidstats-0.0.3/tox.ini
+-rw-r--r--   0     1001      127    45588 2024-05-29 01:43:24.000000 rapidstats-0.0.3/Cargo.lock
+-rw-r--r--   0     1001      127     1065 2024-05-29 01:43:24.000000 rapidstats-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 rapidstats-0.0.3/PKG-INFO
```

### Comparing `rapidstats-0.0.2/.github/workflows/CI.yaml` & `rapidstats-0.0.3/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/.github/workflows/tests.yaml` & `rapidstats-0.0.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/.gitignore` & `rapidstats-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/.pre-commit-config.yaml` & `rapidstats-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/LICENSE` & `rapidstats-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/README.md` & `rapidstats-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/benchmarks/analyze_benchmarks.ipynb` & `rapidstats-0.0.3/benchmarks/analyze_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/benchmarks/benchmark.py` & `rapidstats-0.0.3/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/python/rapidstats/_bootstrap.py` & `rapidstats-0.0.3/python/rapidstats/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/python/rapidstats/_metrics.py` & `rapidstats-0.0.3/python/rapidstats/_metrics.py`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/python/rapidstats/_rustystats.pyi` & `rapidstats-0.0.3/python/rapidstats/_rustystats.pyi`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/python/rapidstats/_utils.py` & `rapidstats-0.0.3/python/rapidstats/_utils.py`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/release.py` & `rapidstats-0.0.3/release.py`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/requirements_dev.txt` & `rapidstats-0.0.3/requirements_dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 isort==5.13.2
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
 jaraco.functools==4.0.1
 jeepney==0.8.0
 keyring==25.2.1
 markdown-it-py==3.0.0
+maturin==1.5.1
 mdurl==0.1.2
 more-itertools==10.2.0
 mypy==1.10.0
 mypy-extensions==1.0.0
 nh3==0.2.17
 nodeenv==1.8.0
 numpy==1.26.4
 packaging==24.0
+patchelf==0.17.2.1
 pathspec==0.12.1
 pkginfo==1.10.0
 platformdirs==4.2.2
 pluggy==1.5.0
 pre-commit==3.7.1
 pycparser==2.22
 Pygments==2.18.0
```

### Comparing `rapidstats-0.0.2/src/bootstrap.rs` & `rapidstats-0.0.3/src/bootstrap.rs`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/src/lib.rs` & `rapidstats-0.0.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/src/metrics.rs` & `rapidstats-0.0.3/src/metrics.rs`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/tests/test_rapidstats.py` & `rapidstats-0.0.3/tests/test_rapidstats.py`

 * *Files identical despite different names*

### Comparing `rapidstats-0.0.2/Cargo.lock` & `rapidstats-0.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1229,15 +1229,15 @@
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
 name = "rapidstats"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "ndarray",
  "polars",
  "pyo3",
  "pyo3-polars",
  "rayon",
 ]
```

### Comparing `rapidstats-0.0.2/pyproject.toml` & `rapidstats-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [project]
-license = { file = "LICENSE" }
 name = "rapidstats"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library that implements fast statistical routines"
+license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "Cangyuan Li", email = "everest229@gmail.com" }]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "polars==0.20.30",
     "scipy==1.13.1",
     "tqdm==4.66.4",
     "pyarrow==16.1.0",
 ]
-dynamic = ["version"]
 
 [project.urls]
-"Homepage" = "https://github.com/CangyuanLi/faststats"
-"Source" = "https://github.com/CangyuanLi/faststats"
-"Bug Reports" = "https://github.com/CangyuanLi/faststats/issues"
+"Homepage" = "https://github.com/CangyuanLi/rapidstats"
+"Source" = "https://github.com/CangyuanLi/rapidstats"
+"Bug Reports" = "https://github.com/CangyuanLi/rapidstats/issues"
 
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
-module-name = "faststats._rustystats"
+module-name = "rapidstats._rustystats"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.mypy]
 mypy_path = "src"
 ignore_missing_imports = true
```

### Comparing `rapidstats-0.0.2/PKG-INFO` & `rapidstats-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: rapidstats
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: polars ==0.20.30
 Requires-Dist: scipy ==1.13.1
 Requires-Dist: tqdm ==4.66.4
 Requires-Dist: pyarrow ==16.1.0
 License-File: LICENSE
 Summary: A library that implements fast statistical routines
 Author-email: Cangyuan Li <everest229@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/CangyuanLi/faststats
-Project-URL: Source, https://github.com/CangyuanLi/faststats
-Project-URL: Bug Reports, https://github.com/CangyuanLi/faststats/issues
+Project-URL: Homepage, https://github.com/CangyuanLi/rapidstats
+Project-URL: Source, https://github.com/CangyuanLi/rapidstats
+Project-URL: Bug Reports, https://github.com/CangyuanLi/rapidstats/issues
 
 # faststats:
 [![PyPI version](https://badge.fury.io/py/faststats.svg)](https://badge.fury.io/py/faststats)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/faststats)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Tests](https://github.com/CangyuanLi/faststats/actions/workflows/tests.yml/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

