# Comparing `tmp/ddeutil_io-0.1.7.tar.gz` & `tmp/ddeutil_io-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_io-0.1.7.tar", last modified: Wed May 22 02:05:18 2024, max compression
+gzip compressed data, was "ddeutil_io-0.1.8.tar", last modified: Wed May 29 01:49:37 2024, max compression
```

## Comparing `ddeutil_io-0.1.7.tar` & `ddeutil_io-0.1.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/ddeutil/io/__base/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/__regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/param.py
--rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_register_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.268420 ddeutil_io-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-29 01:49:37.268420 ddeutil_io-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:49:37.268420 ddeutil_io-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.264420 ddeutil_io-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.264420 ddeutil_io-0.1.8/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.264420 ddeutil_io-0.1.8/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.268420 ddeutil_io-0.1.8/src/ddeutil/io/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__base/__regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.268420 ddeutil_io-0.1.8/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-29 01:49:37.000000 ddeutil_io-0.1.8/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 01:49:37.000000 ddeutil_io-0.1.8/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:49:37.000000 ddeutil_io-0.1.8/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 01:49:37.000000 ddeutil_io-0.1.8/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 01:49:37.000000 ddeutil_io-0.1.8/src/ddeutil_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:37.268420 ddeutil_io-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_base_rw_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_base_rw_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_base_rw_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_base_rw_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_config_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-29 01:49:32.000000 ddeutil_io-0.1.8/tests/test_register_deploy.py
```

### Comparing `ddeutil_io-0.1.7/LICENSE` & `ddeutil_io-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/PKG-INFO` & `ddeutil_io-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ddeutil
 Requires-Dist: fmtutil
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: deepdiff==7.0.1
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: toml==0.10.2
 
 # Data Utility Package: _IO_
 
 [![test](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml)
 [![python support version](https://img.shields.io/pypi/pyversions/ddeutil-io)](https://pypi.org/project/ddeutil-io/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/ddeutil-io)](https://github.com/korawica/ddeutil-io)
```

### Comparing `ddeutil_io-0.1.7/README.md` & `ddeutil_io-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/pyproject.toml` & `ddeutil_io-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 requires-python = ">=3.9.13"
 dependencies = [
     "ddeutil",
     "fmtutil",
     "pydantic==2.7.1",
     "deepdiff==7.0.1",
     "pyyaml==6.0.1",
+    "toml==0.10.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/korawica/ddeutil-io/"
 "Source Code" = "https://github.com/korawica/ddeutil-io/"
 
@@ -61,15 +62,18 @@
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 console_output_style = "count"
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
-filterwarnings = ["error"]
+filterwarnings = [
+    "error",
+    "ignore::DeprecationWarning",
+]
 
 [tool.mypy]
 python_version = "3.9"
 files = ["ddeutil"]
 show_error_codes = true
 pretty = true
 strict = true
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/__base/__init__.py` & `ddeutil_io-0.1.8/src/ddeutil/io/__base/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# ------------------------------------------------------------------------------
+# Copyright (c) 2022 Korawich Anuttra. All rights reserved.
+# Licensed under the MIT License. See LICENSE in the project root for
+# license information.
+# ------------------------------------------------------------------------------
 from __future__ import annotations
 
 import fnmatch
 import os
 import shutil
 from pathlib import Path
 from typing import (
@@ -14,14 +19,16 @@
     CsvPipeFl,
     EnvFl,
     Fl,
     JsonEnvFl,
     JsonFl,
     MarshalFl,
     PickleFl,
+    TomlEnvFl,
+    TomlFl,
     YamlEnvFl,
     YamlFl,
 )
 from .utils import (
     add_newline,
     search_env_replace,
 )
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/__base/__regex.py` & `ddeutil_io-0.1.8/src/ddeutil/io/__base/__regex.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/__base/files.py` & `ddeutil_io-0.1.8/src/ddeutil/io/__base/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,37 +23,40 @@
 import logging
 import marshal
 import mmap
 import os
 import pickle
 from contextlib import contextmanager
 from pathlib import Path
+from tarfile import TarFile
 from typing import (
     IO,
     Any,
     AnyStr,
     Callable,
     ClassVar,
     Literal,
     Optional,
     Protocol,
     Union,
     get_args,
 )
 
+import toml
+
 # NOTE: import msgpack
 import yaml
+from ddeutil.core import must_split
 
 try:
     from yaml import CSafeLoader as SafeLoader
     from yaml import CUnsafeLoader as UnsafeLoader
 except ImportError:
     from yaml import SafeLoader, UnsafeLoader
 
-from .__regex import RegexConf
 from .utils import search_env, search_env_replace
 
 FileCompressType = Literal["gzip", "gz", "xz", "bz2"]
 DirCompressType = Literal["zip", "rar", "tar", "h5", "hdf5", "fits"]
 
 
 def compress_lib(compress: str) -> CompressProtocol:
@@ -104,20 +107,20 @@
 
     def __init__(
         self,
         path: Union[str, Path],
         *,
         encoding: Optional[str] = None,
         compress: Optional[FileCompressType] = None,
-    ):
+    ) -> None:
         self.path: Path = Path(path) if isinstance(path, str) else path
         self.encoding: str = encoding or "utf-8"
         self.compress: Optional[FileCompressType] = compress
 
-        # Action anything after set up attributes.
+        # NOTE: Action anything after set up attributes.
         self.after_set_attrs()
 
     def after_set_attrs(self) -> None: ...
 
     def __call__(self, *args, **kwargs) -> IO:
         return self.open(*args, **kwargs)
 
@@ -177,59 +180,76 @@
             if str(err) != "cannot mmap an empty file":
                 raise err
             yield file
             logging.error("Does not open file with memory mode")
         finally:
             file.close()
 
-    def read(self, *args, **kwargs):
-        raise NotImplementedError
 
-    def write(self, *args, **kwargs):
-        raise NotImplementedError
+class OpenDirProtocol(Protocol):
+
+    def write(self, name, arcname): ...
+
+    def extractall(self, path): ...
+
+
+class CustomTarFile(TarFile):
+
+    def write(self, name, arcname=None):
+        return self.add(name, arcname)
 
 
 class Dir:
     """Open File Object"""
 
     def __init__(
         self,
         path: Union[str, Path],
         *,
-        compress: Optional[DirCompressType] = None,
-    ):
+        compress: str,
+    ) -> None:
         self.path: Path = Path(path) if isinstance(path, str) else path
-        self.compress = compress
-        # Action anything after set up attributes.
+        _compress, sub = must_split(compress, ":", maxsplit=1)
+        self.compress: DirCompressType = _compress
+        self.sub_compress: str = sub or "_"
+
+        # NOTE: Action anything after set up attributes.
         self.after_set_attrs()
 
     def after_set_attrs(self) -> None: ...
 
-    def open(self, *, mode: str, **kwargs):
-        if not self.compress:
-            return ""
-        elif self.compress in {"zip"}:
+    def open(self, *, mode: str, **kwargs) -> OpenDirProtocol:
+        """Open dir"""
+        if self.compress in {"zip"}:
             import zipfile
 
+            ZIP_COMPRESS: dict[str, Any] = {
+                "_": zipfile.ZIP_DEFLATED,
+                "bz2": zipfile.ZIP_BZIP2,
+            }
+
             return zipfile.ZipFile(
                 self.path,
                 mode=mode,
-                compression=zipfile.ZIP_DEFLATED,
+                compression=ZIP_COMPRESS[self.sub_compress],
                 **kwargs,
             )
         elif self.compress in {"tar"}:
-            import tarfile
+            TAR_COMPRESS: dict[str, str] = {
+                "_": "gz",
+                "gz": "gz",
+                "bz2": "bz2",
+                "xz": "xz",
+            }
 
-            # TODO: Wrapped tar module with change some methods like,
-            #   - add --> write
-            return tarfile.open(
+            return CustomTarFile.open(
                 self.path,
-                mode=f"{mode}:gz",  # w:bz2
+                mode=f"{mode}:{TAR_COMPRESS[self.sub_compress]}",
             )
-        return NotImplementedError
+        raise NotImplementedError
 
 
 class EnvFl(Fl, FlAbc):
     """Env object which mapping search engine"""
 
     keep_newline: ClassVar[bool] = False
     default: ClassVar[str] = ""
@@ -329,15 +349,15 @@
     @staticmethod
     def prepare(x: str) -> str:
         return x
 
     def read(self, safe: bool = True) -> dict[str, Any]:
         with self.open(mode="r") as _r:
             _env_replace: str = search_env_replace(
-                RegexConf.RE_YAML_COMMENT.sub("", _r.read()),
+                yaml.dump(yaml.load(_r.read(), UnsafeLoader)),
                 raise_if_default_not_exists=self.raise_if_not_default,
                 default=self.default,
                 escape=self.escape,
                 caller=self.prepare,
             )
             if _result := yaml.load(
                 _env_replace,
@@ -467,37 +487,69 @@
                 _w.write(json.dumps(data))
             else:
                 json.dump(data, _w, indent=indent)
 
 
 class JsonEnvFl(JsonFl):
     raise_if_not_default: bool = False
-    default: str = "N/A"
-    escape: str = "ESC"
+    default: str = "null"
+    escape: str = "<ESCAPE>"
 
     @staticmethod
     def prepare(x: str) -> str:
         return x
 
     def read(self) -> Union[dict[Any, Any], list[Any]]:
-        with self.open(mode="r") as _r:
+        with self.open(mode="rt") as _r:
             return json.loads(
                 search_env_replace(
                     _r.read(),
                     raise_if_default_not_exists=self.raise_if_not_default,
                     default=self.default,
                     escape=self.escape,
                     caller=self.prepare,
                 )
             )
 
     def write(self, data, *, indent: int = 4) -> None:
         raise NotImplementedError
 
 
+class TomlFl(Fl, FlAbc):
+    def read(self):
+        with self.open(mode="rt") as _r:
+            return toml.loads(_r.read())
+
+    def write(self, data: Any) -> None:
+        with self.open(mode="wt") as _w:
+            toml.dump(data, _w)
+
+
+class TomlEnvFl(TomlFl):
+    raise_if_not_default: bool = False
+    default: str = "null"
+    escape: str = "<ESCAPE>"
+
+    @staticmethod
+    def prepare(x: str) -> str:
+        return x
+
+    def read(self):
+        with self.open(mode="rt") as _r:
+            return toml.loads(
+                search_env_replace(
+                    _r.read(),
+                    raise_if_default_not_exists=self.raise_if_not_default,
+                    default=self.default,
+                    escape=self.escape,
+                    caller=self.prepare,
+                )
+            )
+
+
 class PickleFl(Fl, FlAbc):
     def read(self):
         with self.open(mode="rb") as _r:
             return pickle.loads(_r.read())
 
     def write(self, data):
         with self.open(mode="wb") as _w:
@@ -520,10 +572,12 @@
     "JsonFl",
     "JsonEnvFl",
     "YamlFl",
     "YamlFlResolve",
     "YamlEnvFl",
     "CsvFl",
     "CsvPipeFl",
+    "TomlFl",
+    "TomlEnvFl",
     "MarshalFl",
     "PickleFl",
 )
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/__base/utils.py` & `ddeutil_io-0.1.8/src/ddeutil/io/__base/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# ------------------------------------------------------------------------------
+# Copyright (c) 2022 Korawich Anuttra. All rights reserved.
+# Licensed under the MIT License. See LICENSE in the project root for
+# license information.
+# ------------------------------------------------------------------------------
 from __future__ import annotations
 
 import os
 from typing import (
     Callable,
     Optional,
 )
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/__init__.py` & `ddeutil_io-0.1.8/src/ddeutil/io/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     CsvPipeFl,
     EnvFl,
     Fl,
     JsonEnvFl,
     JsonFl,
     MarshalFl,
     PickleFl,
+    TomlEnvFl,
+    TomlFl,
     YamlEnvFl,
     YamlFl,
     YamlFlResolve,
 )
 from .__base.utils import (
     search_env,
     search_env_replace,
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/config.py` & `ddeutil_io-0.1.8/src/ddeutil/io/config.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.8/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/param.py` & `ddeutil_io-0.1.8/src/ddeutil/io/param.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/register.py` & `ddeutil_io-0.1.8/src/ddeutil/io/register.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.8/src/ddeutil/io/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,16 @@
 
 def map_func(value: T, fn: Callable[[str], str]) -> T:
     """Map any function from input argument to configuration data.
 
     Examples:
         >>> map_func({"foo": "bar"}, lambda x: x + "!")
         {'foo': 'bar!'}
+        >>> map_func(("foo", "bar"), lambda x: x + "!")
+        ('foo!', 'bar!')
     """
     if isinstance(value, dict):
         return {k: map_func(value[k], fn) for k in value}
     elif isinstance(value, (list, tuple)):
         return type(value)([map_func(i, fn) for i in value])
     elif not isinstance(value, str):
         return value
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil_io.egg-info/PKG-INFO` & `ddeutil_io-0.1.8/src/ddeutil_io.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ddeutil
 Requires-Dist: fmtutil
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: deepdiff==7.0.1
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: toml==0.10.2
 
 # Data Utility Package: _IO_
 
 [![test](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml)
 [![python support version](https://img.shields.io/pypi/pyversions/ddeutil-io)](https://pypi.org/project/ddeutil-io/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/ddeutil-io)](https://github.com/korawica/ddeutil-io)
```

### Comparing `ddeutil_io-0.1.7/src/ddeutil_io.egg-info/SOURCES.txt` & `ddeutil_io-0.1.8/src/ddeutil_io.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 src/ddeutil/io/__base/files.py
 src/ddeutil/io/__base/utils.py
 src/ddeutil_io.egg-info/PKG-INFO
 src/ddeutil_io.egg-info/SOURCES.txt
 src/ddeutil_io.egg-info/dependency_links.txt
 src/ddeutil_io.egg-info/requires.txt
 src/ddeutil_io.egg-info/top_level.txt
-tests/test_base_csv.py
 tests/test_base_dir.py
-tests/test_base_env.py
 tests/test_base_file.py
-tests/test_base_yaml.py
+tests/test_base_rw_csv.py
+tests/test_base_rw_env.py
+tests/test_base_rw_toml.py
+tests/test_base_rw_yaml.py
 tests/test_config_file.py
 tests/test_config_sqlite.py
 tests/test_param.py
 tests/test_register.py
 tests/test_register_deploy.py
```

### Comparing `ddeutil_io-0.1.7/tests/test_base_csv.py` & `ddeutil_io-0.1.8/tests/test_base_rw_csv.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_base_env.py` & `ddeutil_io-0.1.8/tests/test_base_rw_env.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_base_file.py` & `ddeutil_io-0.1.8/tests/test_base_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_base_yaml.py` & `ddeutil_io-0.1.8/tests/test_base_rw_yaml.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
 import shutil
-import unittest
-import warnings
 from collections.abc import Generator
 from pathlib import Path
 from textwrap import dedent
 from typing import Any
 
 import ddeutil.io.__base.files as fl
 import pytest
@@ -29,28 +27,35 @@
     main_key:
         sub_key:
             string: 'test ${DEMO_ENV_VALUE} value'
             int: 0.001
             bool: false
             list: ['i1', 'i2', 'i3']
             str2bool: on
+            statement: |
+                # Comment ${DEMO_ENV_VALUE}
+                This is a long statement with comment above
     """
     ).strip()
 
 
 @pytest.fixture(scope="module")
 def yaml_data_safe() -> dict[str, Any]:
     return {
         "main_key": {
             "sub_key": {
                 "string": "test ${DEMO_ENV_VALUE} value",
                 "int": 0.001,
                 "bool": False,
                 "list": ["i1", "i2", "i3"],
                 "str2bool": True,
+                "statement": (
+                    "# Comment ${DEMO_ENV_VALUE}\n"
+                    "This is a long statement with comment above"
+                ),
             }
         }
     }
 
 
 def test_write_yaml_file_with_safe(target_path, yaml_str_safe, yaml_data_safe):
     yaml_path: Path = target_path / "test_write_file.yaml"
@@ -61,14 +66,18 @@
 def test_read_yaml_resolve_file(target_path, yaml_str_safe, yaml_data_safe):
     yaml_path: Path = target_path / "test_read_file_resolve.yaml"
     with open(yaml_path, mode="w", encoding="utf-8") as f:
         f.write(yaml_str_safe)
 
     data = fl.YamlFlResolve(path=yaml_path).read(safe=False)
     assert "on" == data["main_key"]["sub_key"]["str2bool"]
+    assert (
+        "# Comment ${DEMO_ENV_VALUE}\n"
+        "This is a long statement with comment above"
+    ) == data["main_key"]["sub_key"]["statement"]
 
 
 def test_read_yaml_file_with_safe(target_path, yaml_str_safe, yaml_data_safe):
     yaml_path: Path = target_path / "test_read_file_safe.yaml"
     with open(yaml_path, mode="w", encoding="utf-8") as f:
         yaml.dump(yaml.safe_load(yaml_str_safe), f)
 
@@ -81,120 +90,121 @@
     with open(yaml_path, mode="w", encoding="utf-8") as f:
         f.write(yaml_str_safe)
 
     data = fl.YamlFl(path=yaml_path).read(safe=False)
     assert yaml_data_safe == data
 
 
-class YamlEnvFileTestCase(unittest.TestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        cls.root_path: str = os.path.dirname(os.path.abspath(__file__)).replace(
-            os.sep, "/"
-        )
-
-    def setUp(self) -> None:
-        self.maxDiff = None
-        warnings.simplefilter("ignore", category=ResourceWarning)
-        self.yaml_str: str = dedent(
-            """
-        main_key:
-            sub_key:
-                key01: 'test ${DEMO_ENV_VALUE} value'
-                key02: $1 This is escape with number
-                key03: $$ESCAPE This is escape with $
-                key04: ['i1', 'i2', '${DEMO_ENV_VALUE}']
-                key05: ${DEMO_ENV_VALUE_EMPTY:default}
-                key06: $${DEMO_ENV_VALUE}
-                key07: This ${DEMO_ENV_VALUE} ${{DEMO_ENV_VALUE}}
+@pytest.fixture(scope="module")
+def yaml_str_env_safe() -> str:
+    return dedent(
         """
-        ).strip()
-        self.yaml_data: dict = {
-            "main_key": {
-                "sub_key": {
-                    "key01": "test demo value",
-                    "key02": "$1 This is escape with number",
-                    "key03": "$ESCAPE This is escape with $",
-                    "key04": ["i1", "i2", "demo"],
-                    "key05": "default",
-                    "key06": "${DEMO_ENV_VALUE}",
-                    "key07": "This demo ${{DEMO_ENV_VALUE}}",
-                }
-            }
-        }
+    main_key:
+        sub_key:
+            key01: 'test ${DEMO_ENV_VALUE} value'
+            key02: $1 This is escape with number
+            key03: $$ESCAPE This is escape with $
+            key04: ['i1', 'i2', '${DEMO_ENV_VALUE}']
+            key05: ${DEMO_ENV_VALUE_EMPTY:default}
+            key06: $${DEMO_ENV_VALUE}
+            key07: This ${DEMO_ENV_VALUE} ${{DEMO_ENV_VALUE}}
+            key08: |
+                # Comment
+                statement ${DEMO_ENV_VALUE}
+    """
+    ).strip()
 
-    def test_read_yaml_file_with_safe_mode(self):
-        yaml_path: str = f"{self.root_path}/test_read_file_env.yaml"
 
-        with open(yaml_path, mode="w", encoding="utf-8") as f:
-            yaml.dump(yaml.safe_load(self.yaml_str), f)
+@pytest.fixture(scope="module")
+def yaml_data_env_safe() -> dict[str, Any]:
+    return {
+        "main_key": {
+            "sub_key": {
+                "key01": "test demo value",
+                "key02": "$1 This is escape with number",
+                "key03": "$ESCAPE This is escape with $",
+                "key04": ["i1", "i2", "demo"],
+                "key05": "default",
+                "key06": "${DEMO_ENV_VALUE}",
+                "key07": "This demo ${{DEMO_ENV_VALUE}}",
+                "key08": "# Comment\nstatement demo",
+            },
+        },
+    }
 
-        os.environ["DEMO_ENV_VALUE"] = "demo"
 
-        data = fl.YamlEnvFl(path=yaml_path).read()
-        self.assertDictEqual(self.yaml_data, data)
-
-        os.remove(yaml_path)
-
-    def test_read_yaml_file_with_safe_mode_and_prepare(self):
-        yaml_path: str = f"{self.root_path}/test_read_file_env_prepare.yaml"
-
-        with open(yaml_path, mode="w", encoding="utf-8") as f:
-            yaml.dump(yaml.safe_load(self.yaml_str), f)
-
-        os.environ["DEMO_ENV_VALUE"] = "demo"
-
-        yml_loader = fl.YamlEnvFl(path=yaml_path)
-        yml_loader.prepare = lambda x: f"{x}!!"
-        data = yml_loader.read()
-        self.assertDictEqual(
-            {
-                "main_key": {
-                    "sub_key": {
-                        "key01": "test demo!! value",
-                        "key02": "$1 This is escape with number",
-                        "key03": "$ESCAPE This is escape with $",
-                        "key04": ["i1", "i2", "demo!!"],
-                        "key05": "default!!",
-                        "key06": "${DEMO_ENV_VALUE}",
-                        "key07": "This demo!! ${{DEMO_ENV_VALUE}}",
-                    }
-                }
-            },
-            data,
-        )
+def test_read_yaml_file_with_safe_mode(
+    yaml_str_env_safe,
+    yaml_data_env_safe,
+    target_path,
+):
+    yaml_path: str = target_path / "test_read_file_env.yaml"
 
-        os.remove(yaml_path)
+    with open(yaml_path, mode="w", encoding="utf-8") as f:
+        yaml.dump(yaml.safe_load(yaml_str_env_safe), f)
 
-    def test_read_yaml_file_with_safe_mode_and_prepare_2(self):
-        yaml_path: str = f"{self.root_path}/test_read_file_env_prepare_2.yaml"
+    os.environ["DEMO_ENV_VALUE"] = "demo"
 
-        with open(yaml_path, mode="w", encoding="utf-8") as f:
-            yaml.dump(yaml.safe_load(self.yaml_str), f)
-
-        os.environ["DEMO_ENV_VALUE"] = "P@ssW0rd"
-
-        import urllib.parse
-
-        yml_loader = fl.YamlEnvFl
-        yml_loader.prepare = staticmethod(
-            lambda x: urllib.parse.quote_plus(str(x))
-        )
-        data = yml_loader(path=yaml_path).read()
-        self.assertDictEqual(
-            {
-                "main_key": {
-                    "sub_key": {
-                        "key01": "test P%40ssW0rd value",
-                        "key02": "$1 This is escape with number",
-                        "key03": "$ESCAPE This is escape with $",
-                        "key04": ["i1", "i2", "P%40ssW0rd"],
-                        "key05": "default",
-                        "key06": "${DEMO_ENV_VALUE}",
-                        "key07": "This P%40ssW0rd ${{DEMO_ENV_VALUE}}",
-                    }
-                }
-            },
-            data,
-        )
+    data = fl.YamlEnvFl(path=yaml_path).read()
+    assert yaml_data_env_safe == data
+
+
+def test_read_yaml_file_with_safe_mode_and_prepare(
+    target_path,
+    yaml_str_env_safe,
+):
+    yaml_path: str = target_path / "test_read_file_env_prepare.yaml"
 
-        os.remove(yaml_path)
+    with open(yaml_path, mode="w", encoding="utf-8") as f:
+        yaml.dump(yaml.safe_load(yaml_str_env_safe), f)
+
+    os.environ["DEMO_ENV_VALUE"] = "demo"
+
+    yml_loader = fl.YamlEnvFl(path=yaml_path)
+    yml_loader.prepare = lambda x: f"{x}!!"
+    data = yml_loader.read()
+    assert {
+        "main_key": {
+            "sub_key": {
+                "key01": "test demo!! value",
+                "key02": "$1 This is escape with number",
+                "key03": "$ESCAPE This is escape with $",
+                "key04": ["i1", "i2", "demo!!"],
+                "key05": "default!!",
+                "key06": "${DEMO_ENV_VALUE}",
+                "key07": "This demo!! ${{DEMO_ENV_VALUE}}",
+                "key08": "# Comment\nstatement demo!!",
+            }
+        }
+    } == data
+
+
+def test_read_yaml_file_with_safe_mode_and_prepare_2(
+    target_path,
+    yaml_str_env_safe,
+):
+    yaml_path: str = target_path / "test_read_file_env_prepare_2.yaml"
+
+    with open(yaml_path, mode="w", encoding="utf-8") as f:
+        yaml.dump(yaml.safe_load(yaml_str_env_safe), f)
+
+    os.environ["DEMO_ENV_VALUE"] = "P@ssW0rd"
+
+    import urllib.parse
+
+    yml_loader = fl.YamlEnvFl
+    yml_loader.prepare = staticmethod(lambda x: urllib.parse.quote_plus(str(x)))
+    data = yml_loader(path=yaml_path).read()
+    assert {
+        "main_key": {
+            "sub_key": {
+                "key01": "test P%40ssW0rd value",
+                "key02": "$1 This is escape with number",
+                "key03": "$ESCAPE This is escape with $",
+                "key04": ["i1", "i2", "P%40ssW0rd"],
+                "key05": "default",
+                "key06": "${DEMO_ENV_VALUE}",
+                "key07": "This P%40ssW0rd ${{DEMO_ENV_VALUE}}",
+                "key08": "# Comment\nstatement P%40ssW0rd",
+            }
+        }
+    } == data
```

### Comparing `ddeutil_io-0.1.7/tests/test_config_file.py` & `ddeutil_io-0.1.8/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_config_sqlite.py` & `ddeutil_io-0.1.8/tests/test_config_sqlite.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_param.py` & `ddeutil_io-0.1.8/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_register.py` & `ddeutil_io-0.1.8/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.7/tests/test_register_deploy.py` & `ddeutil_io-0.1.8/tests/test_register_deploy.py`

 * *Files identical despite different names*

