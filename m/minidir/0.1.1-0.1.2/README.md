# Comparing `tmp/minidir-0.1.1.tar.gz` & `tmp/minidir-0.1.2.tar.gz`

## Comparing `minidir-0.1.1.tar` & `minidir-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 minidir-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 minidir-0.1.1/minidir.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 minidir-0.1.1/tests/test_minidir.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 minidir-0.1.1/.gitignore
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 minidir-0.1.1/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 minidir-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 minidir-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 minidir-0.1.2/minidir/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minidir-0.1.2/minidir/py.typed
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 minidir-0.1.2/tests/test_minidir.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 minidir-0.1.2/.gitignore
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 minidir-0.1.2/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 minidir-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 minidir-0.1.2/PKG-INFO
```

### Comparing `minidir-0.1.1/minidir.py` & `minidir-0.1.2/minidir/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,52 @@
-import typing
-import pathlib
 import os
+import pathlib
+import typing
 
 
 class NotFound(Exception):
     """NotFound is the error that there is no file for some path."""
 
-    pass
-
 
 class NameCollision(Exception):
     """NameCollision is the error that try to create a file with invalid path."""
 
-    pass
-
 
 class File(typing.Protocol):
     """File is a interface that can read and write content."""
 
-    def read(self) -> bytes:
-        pass
+    def read(self) -> bytes: ...
 
-    def write(self, content: bytes) -> None:
-        pass
+    def write(self, content: bytes) -> None: ...
 
 
 class Path(typing.Protocol):
     """Path is a interface that represent the path and name of some file."""
 
-    def __hash__(self) -> int:
-        pass
+    def __hash__(self) -> int: ...
 
-    def __eq__(self, other) -> bool:
-        pass
+    def __eq__(self, other) -> bool: ...
 
-    def __str__(self) -> str:
-        pass
+    def __str__(self) -> str: ...
 
-    def parent(self) -> str:
-        pass
+    def parent(self) -> str: ...
 
-    def base(self) -> str:
-        pass
+    def base(self) -> str: ...
 
 
 class Directory(typing.Protocol):
     """Directory is a interface that can add, remove and iterate files"""
 
-    def __iter__(self) -> typing.Iterator[Path]:
-        pass
+    def __iter__(self) -> typing.Iterator[Path]: ...
 
-    def create(self, path: Path) -> File:
-        pass
+    def create(self, path: Path) -> File: ...
 
-    def remove(self, path: Path) -> None:
-        pass
+    def remove(self, path: Path) -> None: ...
 
-    def get(self, path: Path) -> File:
-        pass
+    def get(self, path: Path) -> File: ...
 
 
 class FakeDirectory:
     """FakeDirectory implements Directory protocol in memory."""
 
     _dir: typing.Dict[str, bytes]
```

### Comparing `minidir-0.1.1/tests/test_minidir.py` & `minidir-0.1.2/tests/test_minidir.py`

 * *Files identical despite different names*

### Comparing `minidir-0.1.1/.gitignore` & `minidir-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `minidir-0.1.1/pyproject.toml` & `minidir-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "minidir"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Weida Hong", email="wdhongtw@gmail.com" },
 ]
-description = " Minimal directory interface and some implementations"
+description = "Minimal directory interface and some implementations"
 keywords = [
   "filesystem",
   "directory",
   "fake",
   "testing",
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Testing",
+    "Typing :: Typed",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/wdhongtw/minidir"
 
 [tool.hatch.build]
 sources = ["src"]
```

### Comparing `minidir-0.1.1/PKG-INFO` & `minidir-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: minidir
-Version: 0.1.1
-Summary:  Minimal directory interface and some implementations
+Version: 0.1.2
+Summary: Minimal directory interface and some implementations
 Project-URL: Homepage, https://github.com/wdhongtw/minidir
 Author-email: Weida Hong <wdhongtw@gmail.com>
 Keywords: directory,fake,filesystem,testing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # minidir: Minimal directory interface and implementation
 
 The minimal interface for directories and files and
 two implementations: in-memory and real file system versions.
@@ -20,7 +21,19 @@
 ## Development
 
 Local (editable) installation is required before running tests.
 
 ```shell
 pip install -e .
 ```
+
+
+---
+
+## Create API token for CLI upload
+
+- Goto <https://pypi.org/manage/account/token/>
+- Create token
+- Save token in `$HOME/.pypirc`
+    - username: `__token__`
+    - password: `pypi-some-token`
+
```

