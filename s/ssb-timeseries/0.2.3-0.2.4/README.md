# Comparing `tmp/ssb_timeseries-0.2.3.tar.gz` & `tmp/ssb_timeseries-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_timeseries-0.2.3.tar", max compression
+gzip compressed data, was "ssb_timeseries-0.2.4.tar", max compression
```

## Comparing `ssb_timeseries-0.2.3.tar` & `ssb_timeseries-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2024-05-23 09:04:33.695865 ssb_timeseries-0.2.3/LICENSE
--rw-r--r--   0        0        0    10072 2024-05-23 09:04:33.695865 ssb_timeseries-0.2.3/README.md
--rw-r--r--   0        0        0     4508 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      452 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/__init__.py
--rw-r--r--   0        0        0      739 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/__main__.py
--rw-r--r--   0        0        0     9527 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/config.py
--rw-r--r--   0        0        0    36528 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/dataset.py
--rw-r--r--   0        0        0     8038 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/dates.py
--rw-r--r--   0        0        0     9053 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/fs.py
--rw-r--r--   0        0        0    15424 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/io.py
--rw-r--r--   0        0        0     4286 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/logging.py
--rw-r--r--   0        0        0    11842 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/meta.py
--rw-r--r--   0        0        0     5963 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/properties.py
--rw-r--r--   0        0        0        0 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/py.typed
--rw-r--r--   0        0        0     5786 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/sample_data.py
--rw-r--r--   0        0        0     1203 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/sample_metadata.py
--rw-r--r--   0        0        0     1451 2024-05-23 09:04:33.699865 ssb_timeseries-0.2.3/src/ssb_timeseries/setup.py
--rw-r--r--   0        0        0      253 2024-05-23 09:04:43.532018 ssb_timeseries-0.2.3/src/ssb_timeseries/types.py
--rw-r--r--   0        0        0    11240 1970-01-01 00:00:00.000000 ssb_timeseries-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-29 11:08:02.859722 ssb_timeseries-0.2.4/LICENSE
+-rw-r--r--   0        0        0     9495 2024-05-29 11:08:12.083769 ssb_timeseries-0.2.4/README.md
+-rw-r--r--   0        0        0     4508 2024-05-29 11:08:12.083769 ssb_timeseries-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      452 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/__main__.py
+-rw-r--r--   0        0        0     5682 2024-05-29 11:08:12.083769 ssb_timeseries-0.2.4/src/ssb_timeseries/config.py
+-rw-r--r--   0        0        0    37693 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/dataset.py
+-rw-r--r--   0        0        0     8038 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/dates.py
+-rw-r--r--   0        0        0    10098 2024-05-29 11:08:12.083769 ssb_timeseries-0.2.4/src/ssb_timeseries/fs.py
+-rw-r--r--   0        0        0    15112 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/io.py
+-rw-r--r--   0        0        0     4286 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/logging.py
+-rw-r--r--   0        0        0    11842 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/meta.py
+-rw-r--r--   0        0        0     5823 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/properties.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/py.typed
+-rw-r--r--   0        0        0     6041 2024-05-29 11:08:12.083769 ssb_timeseries-0.2.4/src/ssb_timeseries/sample_data.py
+-rw-r--r--   0        0        0     1203 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/sample_metadata.py
+-rw-r--r--   0        0        0     1451 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/setup.py
+-rw-r--r--   0        0        0      253 2024-05-29 11:08:02.863722 ssb_timeseries-0.2.4/src/ssb_timeseries/types.py
+-rw-r--r--   0        0        0    10663 1970-01-01 00:00:00.000000 ssb_timeseries-0.2.4/PKG-INFO
```

### Comparing `ssb_timeseries-0.2.3/LICENSE` & `ssb_timeseries-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/README.md` & `ssb_timeseries-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,79 +13,57 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)][poetry]
 
 [pypi status]: https://pypi.org/project/ssb-timeseries/
 [documentation]: https://statisticsnorway.github.io/ssb-timeseries
+[API reference]: https://statisticsnorway.github.io/ssb-timeseries/reference.html
 [tests]: https://github.com/statisticsnorway/ssb-timeseries/actions?workflow=Tests
 [sonarcov]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [sonarquality]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 [poetry]: https://python-poetry.org/
 
 ## Background
 
-Statistics Norway is building a new procuction system in the cloud.
+Statistics Norway is the national statistics agency in Norway. We are building a new procuction system in the cloud and moving towards a modern architecture based on open source technologies.
 
-Moving towards modern architecture, development methodology and open source technologies: Python and R are replacing SAS for statistics production code. Oracle databases and ODI for ETL are being replaced by a data lake architecture relying heavily on Parquet files.
+**Time series** play a key role in the statistics production process.
 
-Another big issue has been time series.Time series are essential to statistics production, so the decision to phase out FAME while not having landed precisely what should replace it has left a huge gap.
+Our mission comes with strict requirements for transparency and data quality. Some are mandated by law, others stem from commitment to international standards.
 
-A complete solution will touch several areas of functionality:
+The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are sometimes significant, they are far from extreme. Quality and reliability is by far more important than latency. This shifts the focus towards process and data control.
 
-- The core is storage with performant read and write, search and filtering
+This libarary came out of a PoC to demonstrate how key functionality could be provided in alignment with architecture decisions and process model requirements.
+
+- At the core is storage with performant read and write, search and filtering
 - Good descriptive metadata is key to findability
 - A wide selection of math and statistics libraries is key for calculations and models
 - Visualisation tools play a role both in ad hoc and routine inspection and quality control
 - Workflow integration with automation and process monitoring help keeping consistent quality
 - Data lineage and process metadata is essential for quality control
 
-In Statistics Norway strict requirements for transparency and data quality are mandated by law and commitment to international standards. The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are some times significant, they are far from extreme. This shifts the focus from performance towards process and data control.
-
-This project came out of a PoC to demonstrate how the key functionality may be provided with the core technologies Python and Parquet, in alignment with architecture decisions and process model requirements. Constructed to be an abstraction between the storage layer and the statistics production code, it provides a way forward while postponing some the technical choices.
-
-- Basic functionality for read/write, calculations, time aggregation and plotting was demonstrated December 2023.
-- Persisting snapshots in alignment with the process model, simple descriptive tagging and integrations with GCS buckets was added Q1 2024.
+It is constructed to be an abstraction between the storage and automation layers and the statistics production code. providing a way forward while postponing some technical choices.
 
 ## How to get started?
 
-See notebook files and tests, `demo.ipynb` and `tests/test_*.py` for examples of usage, and what works and in some cases what does not.
-
-Note that
-
-- The library is constructed to be platform independent, but top priority is making it work in a Linux environment.
 - Install by way of `poetry add ssb_timeseries`.
 - The library should work out of the box with default settings. Note that the defaults are for local testing, ie not be suitable for the production setting.
 - To apply custom settings: The environment variable TIMESERIES_CONFIG should point to a JSON file with configurations.
 - The command `poetry run timeseries-config <...>` can be run from a terminal in order to shift between defauls.
-- Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the Jupyter environment (or the equivalent running elsewhere.
-- The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`.
-- With the environment variable set and the configuration in place `poetry run pytest` should succeed.
+- Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the SSB Jupyter environment (or the equivalent running elsewhere).
+- The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared GCS bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`. Take appropriate steps to make sure you have access. The library does not attempt to facilitate that.
+- With the environment variable set and the configuration in place you should be all set. See the reference https://statisticsnorway.github.io/ssb-timeseries/reference.html
 
-While the library is in a workable state and should work both locally and in JupyterLab, it is still in an exploratory phase. There is a risk that fundamental choices are reversed and breaking changes introduced.
+**Note that** while the library is in a workable state and should work both locally and (for SSB users) in JupyterLab, it is still in early development. There is a risk that fundamental choices are reversed and breaking changes introduced.
 
-With that disclaimer, feel free to explore and experiment, and do not be shy about asking questions or giving feedback. At this stage, feedback is all important.
+With that disclaimer, feel free to explore and experiment, and do not be shy about asking questions or giving feedback.
 
-Assuming you have Python working with a standard SSB setup for git and poetry etc, the following should get you going:
-
-```bash
-# Get the poc package
-git clone https://github.com/statisticsnorway/arkitektur-poc-tidsserier.git
-
-# Run inside a poetry controlled venv:
-poetry shell
-## Create default config
-poetry run timeseries-config home
-# Run the tests to check that everything is OK:
-poetry run pytest
-# A couple of the test cases *are expected* fail when running for the first time in a new location.
-# They should create the structures they need and should succeed in subsequent runs.
-```
 
 ## Functionality overview
 
 The core of the library is the Dataset class. This is essentially a wrapper around a DataFrame (for now Pandas, later probably Polars) in the .data attribute.
 
 The .data attribute should comply to conventions implied by the underlying _information model_. These will start out as pure conventions and subject to evalutation. At a later stage they are likely to be enforced by Parquet schemas. Failing to obey them will cause some methods to fail.
 
@@ -113,30 +91,45 @@
 - The combination `<Dataset.name>.<Series.name>` will serve as a globally unique series identifier.
 - `<Dataset.name>` identifies a "directory", hence must be unique. (Caveat: Directories per type creates room for error.)
 - `<Series.name>` (.data column name) must be unique within the set.
 - Series names _should_ be related to (preferrably constructed from) codes or meta data in such a way that they can be mapped to "tags" via a format mask (and if needed a translation table).
 
 Yes, that _was_ the short version. The long version is still pending production.
 
-To be continued ...
 
-### Other sources of documentation:
+### Internal documentation:
 
 - https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3581313026/Statistikkproduksjon
 - https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3595665419/Lagring+av+tidsserier
 
 ## API-documentation
 
-The [documentation] is published on GitHub Pages. Se the Reference page for
-API-documentation.
+The [documentation] is published on GitHub Pages. See the [API reference]  for API-documentation.
 
 ## Contributing
 
 Contributions are very welcome.
-To learn more, see the [Contributor Guide].
+
+For SSB internals, assuming you have Python working with a standard SSB setup for git and poetry etc, the following should get you going:
+
+```bash
+# Get the poc package
+git clone https://github.com/statisticsnorway/arkitektur-poc-tidsserier.git
+
+# Run inside a poetry controlled venv:
+poetry shell
+## Create default config
+poetry run timeseries-config home
+# Run the tests to check that everything is OK:
+poetry run pytest
+# A couple of the test cases *are expected* fail when running for the first time in a new location.
+# They should create the structures they need and should succeed in subsequent runs.
+```
+
+See the [Contributor Guide] to learn more.
 
 ## License
 
 Distributed under the terms of the [MIT license][license],
 _SSB Timeseries_ is free and open source software.
 
 ## Issues
```

### Comparing `ssb_timeseries-0.2.3/pyproject.toml` & `ssb_timeseries-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-timeseries"
-version = "0.2.3"
+version = "0.2.4"
 description = "SSB Timeseries"
 authors = ["Bernhard Ryeng <bernhard.ryeng@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-timeseries"
 repository = "https://github.com/statisticsnorway/ssb-timeseries"
 documentation = "https://statisticsnorway.github.io/ssb-timeseries"
```

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/__main__.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/__main__.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/dataset.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,18 +392,46 @@
             raise TypeError("Dataset.filter() did not return a Dataset type.")
 
     def plot(self, *args: Any, **kwargs: Any) -> Any:
         """Plot dataset data.
 
         Convenience wrapper around Dataframe.plot() with sensible defaults.
         """
-        xlabels = self.datetime_columns()[0]
+        df = self.data.copy()
+
+        if self.data_type.temporality == properties.Temporality.FROM_TO:
+            interval_handling = kwargs.pop("interval_handling", "interval").lower()
+            match interval_handling:
+                case "interval":
+                    from_data = df
+                    to_data = df
+                    from_data["valid_to"] = from_data["valid_from"]
+                    df = pd.concat(
+                        [from_data, to_data],
+                        axis=0,
+                        ignore_index=True,
+                    ).sort_values(by=["valid_from", "valid_to"])
+                    df.drop(columns=["valid_to"], inplace=True)
+                    xlabels = "valid_from"
+                case "midpoint":
+                    xlabels = "midpoint"
+                    df["midpoint"] = df[self.datetime_columns()].median(axis=1)
+                    df.drop(columns=["valid_from", "valid_to"], inplace=True)
+
+                case _:
+                    raise ValueError(
+                        "Invalid option for interval_handling. Must be 'from', 'to', 'interval' or 'midpoint'."
+                    )
+        else:
+            xlabels = self.datetime_columns()[0]
+
         ts_logger.debug(f"DATASET.plot(): x labels = {xlabels}")
         ts_logger.debug(f"Dataset.plot({args!r}, {kwargs!r}) x-labels {xlabels}")
-        return self.data.plot(  # type: ignore[call-overload]
+
+        return df.plot(  # type: ignore[call-overload]
             xlabels,
             *args,
             legend=len(self.data.columns) < 9,
             title=self.name,
             figsize=(12, 4),
             **kwargs,
         )
```

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/dates.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/dates.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/fs.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/fs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,46 @@
+import functools
 import glob
 import json
 import os
 import shutil
 from pathlib import Path
 
 import pandas
 import pyarrow
 from dapla import FileClient
 
+from ssb_timeseries.types import F
 from ssb_timeseries.types import PathStr
 
-"""This is an abstraction that allows file based io regardless of whether involved file systems are local or gcs.
+"""
+This module allows file based io regardless of whether involved file systems are local or GCS.
 """
 
 # ruff: noqa: ANN002, ANN003
-# mypy: disable-error-code="arg-type, type-arg, no-any-return, no-untyped-def, import-untyped, attr-defined, type-var, index"
+# mypy: disable-error-code="arg-type, type-arg, no-any-return, no-untyped-def, import-untyped, attr-defined, type-var, index, return-value"
+
+
+def path_to_str(path: PathStr) -> PathStr:
+    """Normalise as strings.
+
+    This is a trick to make automated tests pass on Windows.
+    """
+    return str(Path(path)).replace("gs:/", "gs://")
+
+
+def wrap_return_as_str(func: F) -> F:
+    """Decorator to normalise outputs using path_to_str()."""
+
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        out = func(*args, **kwargs)
+        return path_to_str(out)
+
+    return wrapper
 
 
 def remove_prefix(path: PathStr) -> str:
     """Helper function to compensate for some os.* functions shorten gs://<path> to gs:/<path>."""
     return path.replace("//", "/").replace("gs:/", "")
 
 
@@ -47,51 +69,64 @@
     elif is_gcs(path):
         fs = FileClient.get_gcs_file_system()
         return fs.exists(path)
     else:
         return Path(path).exists()
 
 
-def existing_subpath(path: PathStr) -> str:
+@wrap_return_as_str
+def existing_subpath(path: PathStr) -> PathStr:
     """Return the existing part of a path on local or GCS file system."""
     if Path(path).exists():
         return str(path)
     else:
         p = Path(path).parent
         while not p.exists():
             p = Path(p).parent
-        return str(p)
+        return p
 
 
 def touch(path: PathStr) -> None:
     """Touch file regardless of wether the filesystem is local or GCS."""
     if is_gcs(path):
         fs = FileClient.get_gcs_file_system()
         fs.touch(path)
     else:
         mk_parent_dir(path)
         Path(path).touch()
 
 
+@wrap_return_as_str
+def path(*args: PathStr) -> str:
+    """Join args to form path. Make sure that gcs paths are begins with double slash: gs://..."""
+    p = Path(args[0]).joinpath(*args[1:])
+    return p
+    # .replace("gs:/", "gs://")
+    # Feels dirty. Could instead do something like:
+    # str(Path(args[0]).joinpath(*args[1:])).replace("gs:/{[a-z]}", "gs://{1}")
+
+
 def mkdir(path: PathStr) -> None:
     """Make directory regardless of filesystem is local or GCS."""
     # not good enough .. it is hard to distinguish between dirs and files that do not exist yet
     if is_local(path):
-        os.makedirs(path, exist_ok=True)
+        # os.makedirs(path, exist_ok=True)
+        Path(path).mkdir(parents=True, exist_ok=True)
     else:
         ...
 
 
 def mk_parent_dir(path: PathStr) -> None:
     """Ensure a parent directory exists. ... regardless of wether fielsystem is local or GCS."""
-    # wanted a mkdir that could work with both file and directory paths,
+    # wanted a mkdir that could work seamlessly with both file and directory paths,
     # but it is hard to distinguish between dirs and files that do not exist yet
     # --> use this to create parent directory for files, mkdir() when the last part of path is a directory
     if is_local(path):
-        os.makedirs(os.path.dirname(path), exist_ok=True)
+        # os.makedirs(os.path.dirname(path), exist_ok=True)
+        Path(path).parent.mkdir(parents=True, exist_ok=True)
     else:
         ...
 
 
 def file_count(path: PathStr, create: bool = False) -> int:
     """Count files in path. Should work regardless of wether source and target location is local fs or GCS to local."""
     return len(ls(path, create=create))
@@ -147,57 +182,56 @@
         case ("gcs", "local"):
             fs.get(from_path, to_path)
         case ("gcs", "gcs"):
             fs.move(from_path, to_path)
 
 
 def rm(path: PathStr) -> None:
-    """Remove file from local or GCS filesystem."""
+    """Remove file from local or GCS filesystem. Nonrecursive. For a recursive variant, see rmtree()."""
     if is_gcs(path):
-        ...
-        # TO DO: implement this (but recursive)
-        # fs = FileClient.get_gcs_file_system()
-        # fs.rm(path)
+        fs = FileClient.get_gcs_file_system()
+        fs.rm(path)
     else:
         os.remove(path)
 
 
 def rmtree(
     path: str,
 ) -> None:
-    """Remove all directory and all its files and subdirectories regardless of local or GCS filesystem."""
+    """Recursively remove a directory and all its subdirectories and files regardless of local or GCS filesystem."""
     if is_gcs(path):
         ...
         # TO DO: implement this (but recursive)
         # fs = FileClient.get_gcs_file_system()
         # fs.rm(path)
     else:
         shutil.rmtree(path)
 
 
+@wrap_return_as_str
 def same_path(*args) -> PathStr:
     """Return common part of path, for two or more files. Files must be on same file system, but the file system can be either local or GCS."""
     # TO DO: add support for Windows style paths?
     # ... regex along the lines of: [A-Z\:|\\\\]
     paths = [a.replace("gs:/", "") for a in args]
     return os.path.commonpath(paths)
 
 
 def find(
-    path: PathStr,
+    search_path: PathStr,
     pattern: str = "",
     full_path: bool = False,
     replace_root: bool = False,
 ) -> list[str]:
     """Find files and subdirectories with names matching pattern. Should work for both local and GCS filesystems."""
     if pattern:
         pattern = f"*{pattern}*"
     else:
         pattern = "*"
-    search_str = os.path.join(path, "*", pattern)
+    search_str = path(search_path, "*", pattern)
     if is_gcs(path):
         fs = FileClient.get_gcs_file_system()
         found = fs.glob(search_str)
     else:
         found = glob.glob(search_str)
 
     if replace_root:
```

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/io.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                 f"DATASET {self.set_name}: START: Reading metadata from file {self.metadata_fullpath}."
             )
             meta = fs.read_json(self.metadata_fullpath)
         return meta
 
     def write_metadata(self, meta: dict) -> None:
         """Write tags to the metadata file."""
-        os.makedirs(self.metadata_dir, exist_ok=True)
+        # no longer necessary: os.makedirs(self.metadata_dir, exist_ok=True)
         try:
             fs.write_json(self.metadata_fullpath, meta)
             ts_logger.info(
                 f"DATASET {self.set_name}: Writing metadata to file {self.metadata_fullpath}."
             )
         except Exception as e:
             ts_logger.exception(
@@ -237,15 +237,14 @@
             )
 
     def last_version(self, directory: str, pattern: str = "*.parquet") -> str:
         """Check directory and get max version number from files matching regex pattern."""
         files = fs.ls(directory, pattern=pattern)
         number_of_files = len(files)
 
-        # TODO: mypy --> error: Item "None" of "Match[str] | None" has no attribute "group"  [union-attr]
         vs = sorted([int(re.search("(_v)(\d+)(.parquet)", f).group(2)) for f in files])
         ts_logger.debug(
             f"DATASET {self.set_name}: io.last_version regex identified versions {vs} in {directory}."
         )
         if vs:
             read_from_filenames = max(vs)
             out = read_from_filenames
@@ -302,25 +301,20 @@
 
             #  to comply with the naming standard we need to know some things about the data
             ts_logger.debug(
                 f"DATASET last version {next_vs} from {period_from} to {period_to}.')"
             )
         return out
 
-    def sharing_directory(self, bucket: str, team: str = "") -> PathStr:
+    def sharing_directory(self, bucket: str) -> PathStr:
         """Get name of sharing directory based on dataset parameters and configuration.
 
         Creates the directory if it does not exist.
         """
-        fix_test_cases_before_taking_this_approach = False
-        if team and fix_test_cases_before_taking_this_approach:
-            # allowing this breaks tests! --> TODO: adapt test cases
-            directory = os.path.join(bucket, team, self.set_name)
-        else:
-            directory = os.path.join(bucket, self.set_name)
+        directory = os.path.join(bucket, self.set_name)
 
         ts_logger.warning(f"DATASET.IO.SHARING_DIRECTORY: {directory}")
         fs.mkdir(directory)
         return directory
 
     def snapshot(
         self,
@@ -360,21 +354,23 @@
         fs.cp(self.data_fullpath, data_publish_path)
         fs.cp(self.metadata_fullpath, meta_publish_path)
 
         if sharing:
             ts_logger.warning(f"Sharing configs: {sharing}")
             for s in sharing:
                 ts_logger.debug(f"Sharing: {s}")
+                if "team" not in s.keys():
+                    s["team"] = "no team specified"
                 fs.cp(
                     data_publish_path,
-                    self.sharing_directory(bucket=s["path"], team=s["team"]),
+                    self.sharing_directory(bucket=s["path"]),
                 )
                 fs.cp(
                     meta_publish_path,
-                    self.sharing_directory(bucket=s["path"], team=s["team"]),
+                    self.sharing_directory(bucket=s["path"]),
                 )
                 ts_logger.warning(
                     f"DATASET {self.set_name}: sharing with {s['team']}, snapshot copied to {s['path']}."
                 )
 
     @classmethod
     def dir(cls, *args: str, **kwargs: bool) -> str:
```

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/logging.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/logging.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/meta.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/meta.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/properties.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,24 @@
     def to_dict(cls) -> dict:
         """Returns a dictionary representation of the enum."""
         return {e.name: e.value for e in cls}
 
     @classmethod
     def keys(cls) -> list:
         """Returns a list of all the enum keys."""
-        # return cls._member_names_
         return [item.name for item in cls]
 
     @classmethod
     def values(cls) -> list:
         """Returns a list of all the enum values."""
-        # return list(cls._value2member_map_.keys)
         return [item.value[0] for item in cls]
 
     @classmethod
     def descriptions(cls) -> list:
         """Returns a list of descriptions for all enum values."""
-        # return list(cls._value2member_map_.keys())
         return [item.value[1] for item in cls]
 
     def __eq__(self, other: Self) -> bool:
         """Equality test."""
         return repr(self) == repr(other)
 
     def __repr__(self) -> str:
```

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/sample_data.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/sample_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import itertools
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 
-# mypy: disable-error-code="type-arg, import-untyped, unreachable"
+from ssb_timeseries.dates import date_utc
+
+# mypy: disable-error-code="arg-type, type-arg, import-untyped, unreachable, attr-defined"
 
 
 def series_names(*args: dict | str | list[str] | tuple, **kwargs: str) -> list[str]:
     """Return all permutations of the elements of multiple groups of strings.
 
     Args:
         *args (str | list | tuple | dict): Each arg in args should be a collection of names to be combined with the other.
@@ -27,15 +29,15 @@
         # TODO: fix mypy error: Statement is unreachable  [unreachable]
         return [value for value in args.values()]
 
     final_args = []
 
     for arg in args:
         if arg is None:
-            return ""
+            final_args.append([""])
         if isinstance(arg, str):
             final_args.append([arg])
         elif isinstance(arg, list):
             final_args.append(arg)
         elif isinstance(arg, tuple):
             final_args.append(list(arg))
         else:
@@ -96,29 +98,35 @@
     """
     # Handle start_date and end_date defaults
     if start_date is None:
         start_date = datetime.min  # Representing negative infinity
     if end_date is None:
         end_date = datetime.max  # Representing positive infinity
 
-    valid_at = pd.date_range(start=start_date, end=end_date, freq=f"{interval}{freq}")
-    valid_from = pd.date_range(start=start_date, end=end_date, freq=freq)
     # Add other frequencies as needed
     freq_lookup = {
         "Y": "years",
         "YS": "years",
         "M": "months",
         "ME": "months",
         "MS": "months",
         "D": "days",
         "H": "hours",
         "T": "minutes",
         "S": "seconds",
     }
-    valid_to = valid_from + pd.DateOffset(**{freq_lookup[freq]: interval})  # type: ignore
+    offset = pd.DateOffset(**{freq_lookup[freq]: interval})
+    valid_at = pd.date_range(start=start_date, end=end_date, freq=f"{interval}{freq}")
+    valid_from = valid_at
+    valid_to = pd.date_range(
+        start=date_utc(start_date) + offset,
+        end=date_utc(end_date) + offset,
+        freq=f"{interval}{freq}",
+    )
+    # ... valid_to = valid_from + pd.DateOffset(**{freq_lookup[freq]: interval})  # type: ignore
 
     # BUGFIX: If *lists receives strings, permutations will be over chars by chars
     # Kombiner listene til en enkelt liste av lister
     # list = list(lists)
 
     # name_parts = series_names(*lists)
     # Generer alle mulige kombinasjoner av listene med separator
```

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/sample_metadata.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/src/ssb_timeseries/setup.py` & `ssb_timeseries-0.2.4/src/ssb_timeseries/setup.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.3/PKG-INFO` & `ssb_timeseries-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-timeseries
-Version: 0.2.3
+Version: 0.2.4
 Summary: SSB Timeseries
 Home-page: https://github.com/statisticsnorway/ssb-timeseries
 License: MIT
 Author: Bernhard Ryeng
 Author-email: bernhard.ryeng@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -42,79 +42,57 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)][poetry]
 
 [pypi status]: https://pypi.org/project/ssb-timeseries/
 [documentation]: https://statisticsnorway.github.io/ssb-timeseries
+[API reference]: https://statisticsnorway.github.io/ssb-timeseries/reference.html
 [tests]: https://github.com/statisticsnorway/ssb-timeseries/actions?workflow=Tests
 [sonarcov]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [sonarquality]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 [poetry]: https://python-poetry.org/
 
 ## Background
 
-Statistics Norway is building a new procuction system in the cloud.
+Statistics Norway is the national statistics agency in Norway. We are building a new procuction system in the cloud and moving towards a modern architecture based on open source technologies.
 
-Moving towards modern architecture, development methodology and open source technologies: Python and R are replacing SAS for statistics production code. Oracle databases and ODI for ETL are being replaced by a data lake architecture relying heavily on Parquet files.
+**Time series** play a key role in the statistics production process.
 
-Another big issue has been time series.Time series are essential to statistics production, so the decision to phase out FAME while not having landed precisely what should replace it has left a huge gap.
+Our mission comes with strict requirements for transparency and data quality. Some are mandated by law, others stem from commitment to international standards.
 
-A complete solution will touch several areas of functionality:
+The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are sometimes significant, they are far from extreme. Quality and reliability is by far more important than latency. This shifts the focus towards process and data control.
 
-- The core is storage with performant read and write, search and filtering
+This libarary came out of a PoC to demonstrate how key functionality could be provided in alignment with architecture decisions and process model requirements.
+
+- At the core is storage with performant read and write, search and filtering
 - Good descriptive metadata is key to findability
 - A wide selection of math and statistics libraries is key for calculations and models
 - Visualisation tools play a role both in ad hoc and routine inspection and quality control
 - Workflow integration with automation and process monitoring help keeping consistent quality
 - Data lineage and process metadata is essential for quality control
 
-In Statistics Norway strict requirements for transparency and data quality are mandated by law and commitment to international standards. The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are some times significant, they are far from extreme. This shifts the focus from performance towards process and data control.
-
-This project came out of a PoC to demonstrate how the key functionality may be provided with the core technologies Python and Parquet, in alignment with architecture decisions and process model requirements. Constructed to be an abstraction between the storage layer and the statistics production code, it provides a way forward while postponing some the technical choices.
-
-- Basic functionality for read/write, calculations, time aggregation and plotting was demonstrated December 2023.
-- Persisting snapshots in alignment with the process model, simple descriptive tagging and integrations with GCS buckets was added Q1 2024.
+It is constructed to be an abstraction between the storage and automation layers and the statistics production code. providing a way forward while postponing some technical choices.
 
 ## How to get started?
 
-See notebook files and tests, `demo.ipynb` and `tests/test_*.py` for examples of usage, and what works and in some cases what does not.
-
-Note that
-
-- The library is constructed to be platform independent, but top priority is making it work in a Linux environment.
 - Install by way of `poetry add ssb_timeseries`.
 - The library should work out of the box with default settings. Note that the defaults are for local testing, ie not be suitable for the production setting.
 - To apply custom settings: The environment variable TIMESERIES_CONFIG should point to a JSON file with configurations.
 - The command `poetry run timeseries-config <...>` can be run from a terminal in order to shift between defauls.
-- Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the Jupyter environment (or the equivalent running elsewhere.
-- The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`.
-- With the environment variable set and the configuration in place `poetry run pytest` should succeed.
+- Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the SSB Jupyter environment (or the equivalent running elsewhere).
+- The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared GCS bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`. Take appropriate steps to make sure you have access. The library does not attempt to facilitate that.
+- With the environment variable set and the configuration in place you should be all set. See the reference https://statisticsnorway.github.io/ssb-timeseries/reference.html
 
-While the library is in a workable state and should work both locally and in JupyterLab, it is still in an exploratory phase. There is a risk that fundamental choices are reversed and breaking changes introduced.
+**Note that** while the library is in a workable state and should work both locally and (for SSB users) in JupyterLab, it is still in early development. There is a risk that fundamental choices are reversed and breaking changes introduced.
 
-With that disclaimer, feel free to explore and experiment, and do not be shy about asking questions or giving feedback. At this stage, feedback is all important.
+With that disclaimer, feel free to explore and experiment, and do not be shy about asking questions or giving feedback.
 
-Assuming you have Python working with a standard SSB setup for git and poetry etc, the following should get you going:
-
-```bash
-# Get the poc package
-git clone https://github.com/statisticsnorway/arkitektur-poc-tidsserier.git
-
-# Run inside a poetry controlled venv:
-poetry shell
-## Create default config
-poetry run timeseries-config home
-# Run the tests to check that everything is OK:
-poetry run pytest
-# A couple of the test cases *are expected* fail when running for the first time in a new location.
-# They should create the structures they need and should succeed in subsequent runs.
-```
 
 ## Functionality overview
 
 The core of the library is the Dataset class. This is essentially a wrapper around a DataFrame (for now Pandas, later probably Polars) in the .data attribute.
 
 The .data attribute should comply to conventions implied by the underlying _information model_. These will start out as pure conventions and subject to evalutation. At a later stage they are likely to be enforced by Parquet schemas. Failing to obey them will cause some methods to fail.
 
@@ -142,30 +120,45 @@
 - The combination `<Dataset.name>.<Series.name>` will serve as a globally unique series identifier.
 - `<Dataset.name>` identifies a "directory", hence must be unique. (Caveat: Directories per type creates room for error.)
 - `<Series.name>` (.data column name) must be unique within the set.
 - Series names _should_ be related to (preferrably constructed from) codes or meta data in such a way that they can be mapped to "tags" via a format mask (and if needed a translation table).
 
 Yes, that _was_ the short version. The long version is still pending production.
 
-To be continued ...
 
-### Other sources of documentation:
+### Internal documentation:
 
 - https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3581313026/Statistikkproduksjon
 - https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3595665419/Lagring+av+tidsserier
 
 ## API-documentation
 
-The [documentation] is published on GitHub Pages. Se the Reference page for
-API-documentation.
+The [documentation] is published on GitHub Pages. See the [API reference]  for API-documentation.
 
 ## Contributing
 
 Contributions are very welcome.
-To learn more, see the [Contributor Guide].
+
+For SSB internals, assuming you have Python working with a standard SSB setup for git and poetry etc, the following should get you going:
+
+```bash
+# Get the poc package
+git clone https://github.com/statisticsnorway/arkitektur-poc-tidsserier.git
+
+# Run inside a poetry controlled venv:
+poetry shell
+## Create default config
+poetry run timeseries-config home
+# Run the tests to check that everything is OK:
+poetry run pytest
+# A couple of the test cases *are expected* fail when running for the first time in a new location.
+# They should create the structures they need and should succeed in subsequent runs.
+```
+
+See the [Contributor Guide] to learn more.
 
 ## License
 
 Distributed under the terms of the [MIT license][license],
 _SSB Timeseries_ is free and open source software.
 
 ## Issues
```

