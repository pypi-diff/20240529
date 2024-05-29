# Comparing `tmp/arrow_odbc-7.0.3.tar.gz` & `tmp/arrow_odbc-7.0.4.tar.gz`

## Comparing `arrow_odbc-7.0.3.tar` & `arrow_odbc-7.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.3/Cargo.toml
--rw-r--r--   0      501       20      136 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/.gitattributes
--rw-r--r--   0      501       20      213 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/.github/dependabot.yml
--rw-r--r--   0      501       20     1762 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/.github/workflows/test.yml
--rw-r--r--   0      501       20     2652 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/.gitignore
--rw-r--r--   0      501       20      841 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/.readthedocs.yaml
--rw-r--r--   0      501       20    12116 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/Changelog.md
--rw-r--r--   0      501       20     1954 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/Contributing.md
--rw-r--r--   0      501       20     1069 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/LICENSE
--rw-r--r--   0      501       20     8040 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/README.md
--rw-r--r--   0      501       20       14 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/cbindgen.toml
--rw-r--r--   0      501       20      623 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/conftest.py
--rw-r--r--   0      501       20      638 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/Makefile
--rw-r--r--   0      501       20      804 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/make.bat
--rw-r--r--   0      501       20       16 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/requirements.txt
--rw-r--r--   0      501       20      155 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/source/conf.py
--rw-r--r--   0      501       20      458 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/source/index.rst
--rw-r--r--   0      501       20       67 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/docker-compose.yml
--rw-r--r--   0      501       20      564 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      446 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1885 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      788 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      578 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    25240 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9625 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/error.rs
--rw-r--r--   0      501       20     3434 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/lib.rs
--rw-r--r--   0      501       20      655 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/logging.rs
--rw-r--r--   0      501       20     1239 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/parameter.rs
--rw-r--r--   0      501       20      421 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/pool.rs
--rw-r--r--   0      501       20     8757 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20    12865 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/reader.rs
--rw-r--r--   0      501       20     3545 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/src/writer.rs
--rw-r--r--   0      501       20   274432 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/temp_db.duckdb
--rw-r--r--   0      501       20        0 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/tests/__init__.py
--rw-r--r--   0      501       20     4115 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/tests/iris.csv
--rw-r--r--   0      501       20     2413 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/tests/iris.parquet
--rw-r--r--   0      501       20    29032 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    42700 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/Cargo.lock
--rw-r--r--   0      501       20      825 2024-05-29 07:03:23.000000 arrow_odbc-7.0.3/pyproject.toml
--rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.3/PKG-INFO
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.4/Cargo.toml
+-rw-r--r--   0      501       20      136 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/.gitattributes
+-rw-r--r--   0      501       20      213 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/.github/dependabot.yml
+-rw-r--r--   0      501       20     1762 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/.github/workflows/test.yml
+-rw-r--r--   0      501       20     2650 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/.gitignore
+-rw-r--r--   0      501       20      841 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/.readthedocs.yaml
+-rw-r--r--   0      501       20    12116 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/Changelog.md
+-rw-r--r--   0      501       20     1954 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/Contributing.md
+-rw-r--r--   0      501       20     1069 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/LICENSE
+-rw-r--r--   0      501       20     8040 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/README.md
+-rw-r--r--   0      501       20       14 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/cbindgen.toml
+-rw-r--r--   0      501       20      623 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/conftest.py
+-rw-r--r--   0      501       20      638 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/Makefile
+-rw-r--r--   0      501       20      804 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/make.bat
+-rw-r--r--   0      501       20       16 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/docker-compose.yml
+-rw-r--r--   0      501       20      564 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      446 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1885 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      788 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      578 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    25240 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9625 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/error.rs
+-rw-r--r--   0      501       20     3434 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/lib.rs
+-rw-r--r--   0      501       20      655 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/logging.rs
+-rw-r--r--   0      501       20     1239 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/parameter.rs
+-rw-r--r--   0      501       20      421 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/pool.rs
+-rw-r--r--   0      501       20     8757 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20    12865 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/reader.rs
+-rw-r--r--   0      501       20     3545 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/src/writer.rs
+-rw-r--r--   0      501       20   274432 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/temp_db.duckdb
+-rw-r--r--   0      501       20        0 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/tests/iris.parquet
+-rw-r--r--   0      501       20    29032 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    42700 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/Cargo.lock
+-rw-r--r--   0      501       20      825 2024-05-29 07:15:19.000000 arrow_odbc-7.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.4/PKG-INFO
```

### Comparing `arrow_odbc-7.0.3/Cargo.toml` & `arrow_odbc-7.0.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/.github/workflows/test.yml` & `arrow_odbc-7.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/.github/workflows/wheel.yml` & `arrow_odbc-7.0.4/.github/workflows/wheel.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
         
   macos-x86-wheel:
-    runs-on: osx_13_x86
+    runs-on: macos-12
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Publish package
```

### Comparing `arrow_odbc-7.0.3/.readthedocs.yaml` & `arrow_odbc-7.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/Changelog.md` & `arrow_odbc-7.0.4/Changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog
 
-## 7.0.1-3
+## 7.0.1-4
 
 - Build wheel for MacOS 13 x86
 
 ## 7.0.0
 
 - unsigned TinyInt is now mapped to `UInt8`.
```

### Comparing `arrow_odbc-7.0.3/Contributing.md` & `arrow_odbc-7.0.4/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/LICENSE` & `arrow_odbc-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/README.md` & `arrow_odbc-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/conftest.py` & `arrow_odbc-7.0.4/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/doc/Makefile` & `arrow_odbc-7.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/doc/make.bat` & `arrow_odbc-7.0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/doc/source/conf.py` & `arrow_odbc-7.0.4/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "7.0.3"
+release = "7.0.4"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-7.0.3/manylinux/Dockerfile` & `arrow_odbc-7.0.4/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/manylinux/build_wheel.sh` & `arrow_odbc-7.0.4/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/python/arrow_odbc/connect.py` & `arrow_odbc-7.0.4/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/python/arrow_odbc/error.py` & `arrow_odbc-7.0.4/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/python/arrow_odbc/log.py` & `arrow_odbc-7.0.4/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/python/arrow_odbc/pool.py` & `arrow_odbc-7.0.4/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/python/arrow_odbc/reader.py` & `arrow_odbc-7.0.4/python/arrow_odbc/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/python/arrow_odbc/writer.py` & `arrow_odbc-7.0.4/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/error.rs` & `arrow_odbc-7.0.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/lib.rs` & `arrow_odbc-7.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/logging.rs` & `arrow_odbc-7.0.4/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/parameter.rs` & `arrow_odbc-7.0.4/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-7.0.4/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/reader.rs` & `arrow_odbc-7.0.4/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/src/writer.rs` & `arrow_odbc-7.0.4/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/temp_db.duckdb` & `arrow_odbc-7.0.4/temp_db.duckdb`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/tests/iris.csv` & `arrow_odbc-7.0.4/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/tests/iris.parquet` & `arrow_odbc-7.0.4/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/tests/test_arrow_odbc.py` & `arrow_odbc-7.0.4/tests/test_arrow_odbc.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/Cargo.lock` & `arrow_odbc-7.0.4/Cargo.lock`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.3/pyproject.toml` & `arrow_odbc-7.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "7.0.3"
+version = "7.0.4"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0", "pyodbc", "duckdb"]
```

### Comparing `arrow_odbc-7.0.3/PKG-INFO` & `arrow_odbc-7.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arrow-odbc
-Version: 7.0.3
+Version: 7.0.4
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Requires-Dist: pyodbc ; extra == 'test'
 Requires-Dist: duckdb ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
```

