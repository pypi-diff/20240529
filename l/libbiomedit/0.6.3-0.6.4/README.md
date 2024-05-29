# Comparing `tmp/libbiomedit-0.6.3.tar.gz` & `tmp/libbiomedit-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbiomedit-0.6.3.tar", last modified: Mon Oct 31 10:02:36 2022, max compression
+gzip compressed data, was "libbiomedit-0.6.4.tar", last modified: Wed May 29 07:08:11 2024, max compression
```

## Comparing `libbiomedit-0.6.3.tar` & `libbiomedit-0.6.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 10:02:36.005174 libbiomedit-0.6.3/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1800 2022-10-31 10:02:36.006174 libbiomedit-0.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      786 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 10:02:35.998174 libbiomedit-0.6.3/libbiomedit/
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3009 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/archive.py
--rw-rw-rw-   0 root         (0) root         (0)    13445 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/crypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 10:02:36.003174 libbiomedit-0.6.3/libbiomedit/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/lib/classify.py
--rw-rw-rw-   0 root         (0) root         (0)    11718 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/lib/deserialize.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/lib/secret.py
--rw-rw-rw-   0 root         (0) root         (0)     3518 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    10401 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/portal.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/py.typed
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/libbiomedit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 10:02:36.002174 libbiomedit-0.6.3/libbiomedit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1800 2022-10-31 10:02:35.000000 libbiomedit-0.6.3/libbiomedit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      650 2022-10-31 10:02:35.000000 libbiomedit-0.6.3/libbiomedit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-31 10:02:35.000000 libbiomedit-0.6.3/libbiomedit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-31 10:02:34.000000 libbiomedit-0.6.3/libbiomedit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2022-10-31 10:02:35.000000 libbiomedit-0.6.3/libbiomedit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-10-31 10:02:35.000000 libbiomedit-0.6.3/libbiomedit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      961 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1216 2022-10-31 10:02:36.006174 libbiomedit-0.6.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 10:02:36.005174 libbiomedit-0.6.3/test/
--rw-rw-rw-   0 root         (0) root         (0)     3279 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/test/test_archive.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/test/test_classify.py
--rw-rw-rw-   0 root         (0) root         (0)    22805 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/test/test_crypt.py
--rw-rw-rw-   0 root         (0) root         (0)     6790 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/test/test_deserialize.py
--rw-rw-rw-   0 root         (0) root         (0)     3808 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/test/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13362 2022-10-31 10:02:24.000000 libbiomedit-0.6.3/test/test_portal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.696083 libbiomedit-0.6.4/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-29 07:08:11.696083 libbiomedit-0.6.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.691083 libbiomedit-0.6.4/libbiomedit/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2916 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)    13317 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/crypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.693083 libbiomedit-0.6.4/libbiomedit/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 07:07:59.000000 libbiomedit-0.6.4/libbiomedit/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/lib/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    11817 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/lib/deserialize.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/lib/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/portal.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 07:07:59.000000 libbiomedit-0.6.4/libbiomedit/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.694083 libbiomedit-0.6.4/libbiomedit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:08:10.000000 libbiomedit-0.6.4/libbiomedit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-29 07:08:11.696083 libbiomedit-0.6.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.694083 libbiomedit-0.6.4/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    22832 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_deserialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13310 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_portal.py
```

### Comparing `libbiomedit-0.6.3/LICENSE` & `libbiomedit-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.3/PKG-INFO` & `libbiomedit-0.6.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: libbiomedit
-Version: 0.6.3
+Version: 0.6.4
 Summary: Shared library for arround biomedit data transfer
 Home-page: https://gitlab.com/biomedit/libbiomedit
 Author: Robin Engler, Jarosław Surkont, Riccardo Muri, Gerhard Bräunlich, Christian Ribeaud, François Martin
 Author-email: Robin.Engler@sib.swiss, riccardo.murri@id.ethz.ch, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, christian.ribeaud@karakun.com, francois.martin@karakun.com
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: gpg-lite>=0.12.3
+Provides-Extra: dev
+Requires-Dist: mypy==1.8.0; extra == "dev"
+Requires-Dist: pytest==8.0.0; extra == "dev"
+Requires-Dist: ruff==0.2.0; extra == "dev"
+Requires-Dist: bandit==1.7.7; extra == "dev"
+Requires-Dist: types-pkg_resources; extra == "dev"
 
-[![pipeline status](https://gitlab.com/biomedit/libbiomedit/badges/master/pipeline.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/libbiomedit/badges/master/coverage.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/master)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pipeline status](https://gitlab.com/biomedit/libbiomedit/badges/main/pipeline.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/libbiomedit/badges/main/coverage.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/main)
+[![Code style: ruff](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://astral.sh/ruff)
 [![python version](https://img.shields.io/pypi/pyversions/libbiomedit.svg)](https://pypi.org/project/libbiomedit)
 [![license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![latest version](https://img.shields.io/pypi/v/libbiomedit.svg)](https://pypi.org/project/libbiomedit)
 
 # libbiomedit
 
-Shared library for biomedIT projects.
+Shared library for BioMedIT projects.
```

### Comparing `libbiomedit-0.6.3/README.md` & `libbiomedit-0.6.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![pipeline status](https://gitlab.com/biomedit/libbiomedit/badges/master/pipeline.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/libbiomedit/badges/master/coverage.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/master)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pipeline status](https://gitlab.com/biomedit/libbiomedit/badges/main/pipeline.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/libbiomedit/badges/main/coverage.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/main)
+[![Code style: ruff](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://astral.sh/ruff)
 [![python version](https://img.shields.io/pypi/pyversions/libbiomedit.svg)](https://pypi.org/project/libbiomedit)
 [![license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![latest version](https://img.shields.io/pypi/v/libbiomedit.svg)](https://pypi.org/project/libbiomedit)
 
 # libbiomedit
 
-Shared library for biomedIT projects.
+Shared library for BioMedIT projects.
```

### Comparing `libbiomedit-0.6.3/libbiomedit/archive.py` & `libbiomedit-0.6.4/libbiomedit/archive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import tarfile
 import zipfile
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 
-# TODO: remove pylint disable, once we require python >= 3.9
-from os import PathLike  # pylint: disable=unused-import
+from os import PathLike
 from typing import IO, List, Union, Generator
 
 from . import unwrap
 
 
 class ArchiveReaderInterface(ABC):
     @classmethod
@@ -73,15 +72,15 @@
             return unwrap(self.extractfile(name))
         except (KeyError, ValueError) as e:
             raise KeyError(f"File object {name} not found in {str(self.name)}") from e
 
 
 @contextmanager
 def archive_reader(
-    path: Union[str, "PathLike[str]"]
+    path: Union[str, "PathLike[str]"],
 ) -> Generator[Union[ZipReader, TarReader], None, None]:
     if ZipReader.is_valid_type(path):
         with ZipReader.opener(path) as zip_reader:
             yield zip_reader
     elif TarReader.is_valid_type(path):
         with TarReader.opener(path) as tar_reader:
             yield tar_reader
```

### Comparing `libbiomedit-0.6.3/libbiomedit/crypt.py` & `libbiomedit-0.6.4/libbiomedit/crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 import warnings
 import functools
 import json
 
-# TODO: remove pylint disable, once we require python >= 3.9
-from os import PathLike  # pylint: disable=unused-import
+from os import PathLike
 from typing import Iterable, Iterator, Optional, Union
 
 import gpg_lite as gpg
 
 from .archive import archive_reader
 from .metadata import METADATA_FILE_SIG, METADATA_FILE, MetaData
 
@@ -194,15 +193,14 @@
         for identifier in key_identifiers
     )
 
 
 # TODO: remove signee_fingerprint argument in the next major release.
 #       This argument is not doing anything anymore, and is only kept to
 #       avoid creating a breaking change.
-# pylint: disable=too-many-locals
 def verify_metadata_signature(
     tar_file: Union[
         str, "PathLike[str]"
     ],  # TODO: unquote type-hint, once we require python >= 3.9
     gpg_store: gpg.GPGStore,
     signee_fingerprint: Optional[str] = None,
     keyserver_url: Optional[str] = None,
```

### Comparing `libbiomedit-0.6.3/libbiomedit/lib/classify.py` & `libbiomedit-0.6.4/libbiomedit/lib/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Union, Tuple, Any, Dict, Optional, Sequence, Callable, Type
+from typing import Union, Tuple, Any, Dict, Optional, Sequence, Callable, Type, ClassVar
 from enum import Enum
 import collections.abc
 from abc import ABC
 
 import dataclasses
 
 from .secret import Secret
@@ -12,16 +12,16 @@
 # Starting with python 3.7, the typing module has a new API
 __origin_attr__ = "__extra__" if sys.version_info < (3, 7) else "__origin__"
 
 _classifiers = []
 
 
 class IsDataclass(type):
-    __dataclass_fields__: Dict[
-        str, "dataclasses.Field[Any]"
+    __dataclass_fields__: ClassVar[
+        Dict[str, "dataclasses.Field[Any]"]
     ]  # TODO: unquote typehint, once we require python >= 3.9
 
 
 class IsTypingType(ABC):
     __args__: Tuple[type, ...]
```

### Comparing `libbiomedit-0.6.3/libbiomedit/lib/deserialize.py` & `libbiomedit-0.6.4/libbiomedit/lib/deserialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,25 +81,25 @@
 
 
 _deserializers = {}
 _serializers = {}
 
 
 def _deserializer(
-    T: Union[type, object]
+    T: Union[type, object],
 ) -> Callable[[TransformFactory[Any]], TransformFactory[Any]]:
     def decorator(f: TransformFactory[Any]) -> TransformFactory[Any]:
         _deserializers[T] = f
         return f
 
     return decorator
 
 
 def _serializer(
-    T: Union[type, object]
+    T: Union[type, object],
 ) -> Callable[[TransformFactory[Any]], TransformFactory[Any]]:
     def decorator(f: TransformFactory[Any]) -> TransformFactory[Any]:
         _serializers[T] = f
         return f
 
     return decorator
 
@@ -155,15 +155,16 @@
 ) -> Callable[[IsTypingType], Transform]:
     def _transform_tuple(T: IsTypingType) -> Transform:
         item_types: Tuple[AbstractType, ...] = T.__args__
         if transform is serialize and any(
             is_secret(item_type) for item_type in item_types
         ):
             raise ValueError(
-                "Serializing tuples containing Secret is not supported. Try using Optional[Secret]"
+                "Serializing tuples containing Secret is not supported. "
+                "Try using Optional[Secret]"
             )
 
         if len(item_types) == 2 and cast(Any, item_types[1]) is ...:
             inner_transform = transform(item_types[0])
 
             def _transform_ellipsis(data: Tuple[Any, ...]) -> Tuple[Any, ...]:
                 return tuple(inner_transform(item) for item in data)
@@ -200,15 +201,16 @@
             item_type = T.__args__[0]
         except AttributeError as e:
             raise ValueError(
                 f"Sequence of type {seq_type.__name__} without item type"
             ) from e
         if transform is serialize and is_secret(item_type):
             raise ValueError(
-                "Serializing sequences of Secret is not supported. try using Optional[Secret]"
+                "Serializing sequences of Secret is not supported. "
+                "Try using Optional[Secret]"
             )
         if seq_type is collections.abc.Sequence:
             seq_type = list
 
         def _transform(data: Sequence[Any]) -> Sequence[Any]:
             return seq_type(map(transform(item_type), data))
 
@@ -238,15 +240,16 @@
 
 
 @_serializer(IsDataclass)
 def serialize_dataclass(T: IsDataclass) -> Transform:
     serializers_by_name = prepare_serializers(T, serialize)
     if any(is_secret(f.type) for f in dataclasses.fields(T)):
         raise ValueError(
-            "Serializing dataclasses with Secret values are not supported. Try using Optional[Secret]."
+            "Serializing dataclasses with Secret values are not supported. "
+            "Try using Optional[Secret]."
         )
 
     def _serialize(obj: Any) -> Dict[str, Any]:
         converted_data = {
             f_name: serializer(getattr(obj, f_name))
             for f_name, serializer in serializers_by_name
         }
@@ -291,15 +294,16 @@
         t for t in T.__args__ if not (isinstance(t, type) and isinstance(None, t))
     )
 
 
 @_deserializer(Union)
 def deserialize_union(T: IsTypingType) -> Transform:
     """Deserializes Unions of dataclasses.
-    The variants are assumed to be adjacently tagged by its type ("type" and "value")."""
+    The variants are assumed to be adjacently tagged by its type ("type" and "value").
+    """
     types = T.__args__
     if not all(dataclasses.is_dataclass(t) for t in types):
         raise ValueError("Currently, only Unions of dataclasses are supported")
     transform_by_name: Dict[str, Transform] = {
         t.__name__: deserialize(t) for t in types
     }
 
@@ -331,30 +335,32 @@
 
     def _serialize(data: Any) -> Dict[str, Any]:
         inner_type = type(data)
         inner_serialize = transform_by_type.get(inner_type)
         if inner_serialize is None:
             variants = ", ".join(t.__name__ for t in transform_by_type)
             raise ValueError(
-                f"{data}: Could associate {inner_type.__name__} to one of the variants {variants}"
+                f"{data}: Could associate {inner_type.__name__} to one of the "
+                f"variants {variants}"
             )
         return {"type": inner_type.__name__, "value": inner_serialize(data)}
 
     return _serialize
 
 
 def transform_dict(
     transform: TransformFactory[Any],
 ) -> TransformFactory[IsTypingType]:
     def _transform_dict(T: IsTypingType) -> Callable[[Dict[Any, Any]], Dict[Any, Any]]:
         key_type, val_type = T.__args__
 
         if transform is serialize and is_secret(val_type):
             raise ValueError(
-                "Serializing dicts with Secret values is not supported. Use Optional[Secret]."
+                "Serializing dicts with Secret values is not supported. "
+                "Use Optional[Secret]."
             )
 
         key_transform = transform(key_type)
         val_transform = transform(val_type)
 
         def _transform(data: Dict[Any, Any]) -> Dict[Any, Any]:
             return {key_transform(key): val_transform(val) for key, val in data.items()}
```

### Comparing `libbiomedit-0.6.3/libbiomedit/lib/secret.py` & `libbiomedit-0.6.4/libbiomedit/lib/secret.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.3/libbiomedit/metadata.py` & `libbiomedit-0.6.4/libbiomedit/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,28 +82,39 @@
 class HexStr256(ValidatedStr):
     validator = hex_str(256, normalize=str.lower)
 
 
 DATE_FMT = "%Y-%m-%dT%H:%M:%S%z"
 
 
+# TODO: use `datetime.fromisoformat` when support for Python <= 3.10 is dropped
+def _datetime_from_isoformat(s: str) -> datetime:
+    try:
+        # try to parse the date with the default format (without milliseconds)
+        return datetime.strptime(s, DATE_FMT)
+    except ValueError:
+        # as a fallback, try using the default format extended with milliseconds
+        # (note the `.%f` part)
+        return datetime.strptime(s, "%Y-%m-%dT%H:%M:%S.%f%z")
+
+
 class Purpose(Enum):
     PRODUCTION = "PRODUCTION"
     TEST = "TEST"
 
 
 @dataclass(frozen=True)
 class MetaData:
     sender: HexStr1024
     recipients: List[HexStr1024]
     checksum: HexStr256
     timestamp: datetime = field(
         metadata={
-            "deserialize": lambda s: datetime.strptime(s, DATE_FMT),
-            "serialize": lambda d: datetime.strftime(d, DATE_FMT),
+            "deserialize": _datetime_from_isoformat,
+            "serialize": lambda d: datetime.strftime(d, DATE_FMT),  # type: ignore
         },
         default_factory=lambda: datetime.now().astimezone(),
     )
     version: str = "0.7.1"
     checksum_algorithm: str = "SHA256"
     compression_algorithm: str = "gzip"
     transfer_id: Optional[int] = None
```

### Comparing `libbiomedit-0.6.3/libbiomedit/portal.py` & `libbiomedit-0.6.4/libbiomedit/portal.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.3/libbiomedit.egg-info/PKG-INFO` & `libbiomedit-0.6.4/libbiomedit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: libbiomedit
-Version: 0.6.3
+Version: 0.6.4
 Summary: Shared library for arround biomedit data transfer
 Home-page: https://gitlab.com/biomedit/libbiomedit
 Author: Robin Engler, Jarosław Surkont, Riccardo Muri, Gerhard Bräunlich, Christian Ribeaud, François Martin
 Author-email: Robin.Engler@sib.swiss, riccardo.murri@id.ethz.ch, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, christian.ribeaud@karakun.com, francois.martin@karakun.com
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: gpg-lite>=0.12.3
+Provides-Extra: dev
+Requires-Dist: mypy==1.8.0; extra == "dev"
+Requires-Dist: pytest==8.0.0; extra == "dev"
+Requires-Dist: ruff==0.2.0; extra == "dev"
+Requires-Dist: bandit==1.7.7; extra == "dev"
+Requires-Dist: types-pkg_resources; extra == "dev"
 
-[![pipeline status](https://gitlab.com/biomedit/libbiomedit/badges/master/pipeline.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/libbiomedit/badges/master/coverage.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/master)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pipeline status](https://gitlab.com/biomedit/libbiomedit/badges/main/pipeline.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/libbiomedit/badges/main/coverage.svg)](https://gitlab.com/biomedit/libbiomedit/-/commits/main)
+[![Code style: ruff](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://astral.sh/ruff)
 [![python version](https://img.shields.io/pypi/pyversions/libbiomedit.svg)](https://pypi.org/project/libbiomedit)
 [![license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![latest version](https://img.shields.io/pypi/v/libbiomedit.svg)](https://pypi.org/project/libbiomedit)
 
 # libbiomedit
 
-Shared library for biomedIT projects.
+Shared library for BioMedIT projects.
```

### Comparing `libbiomedit-0.6.3/libbiomedit.egg-info/SOURCES.txt` & `libbiomedit-0.6.4/libbiomedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.3/pyproject.toml` & `libbiomedit-0.6.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 40.6.0", "wheel"]
 
-[tool.pylint.MAIN]
-jobs = 2
-load-plugins = ["biomedit_lints"]
-
-[tool.pylint.'MESSAGES CONTROL']
-disable = "line-too-long,invalid-name,too-few-public-methods,too-many-instance-attributes,too-many-arguments,missing-docstring,fixme"
-output-format = "text"
-reports = "no"
-
 [tool.coverage.run]
 branch = true
 source = ["libbiomedit"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{37,38,39,310,311},report
+envlist = py{37,38,39,310,311,312},report
 isolated_build = true
 
 [testenv]
 setenv =
-    py{37,38,39,310,311}: COVERAGE_FILE = .coverage.{envname}
+    py{37,38,39,310,311,312}: COVERAGE_FILE = .coverage.{envname}
 depends =
-    report: py{37,38,39,310,311}
+    report: py{37,38,39,310,311,312}
 deps =
     pytest
     pytest-cov
     coverage[toml]
 commands =
     pytest {posargs: --cov --cov-report=}
 
@@ -41,7 +32,12 @@
     coverage combine
     coverage report
 """
 
 [tool.mypy]
 files = ["libbiomedit", "test"]
 strict = true
+
+[tool.ruff.lint]
+# Enable the pycodestyle (`E`) and Pyflakes (`F`) default rules.
+# Additionally, add flake8-unused-arguments (ARG)
+select = ["E", "F", "ARG"]
```

### Comparing `libbiomedit-0.6.3/setup.cfg` & `libbiomedit-0.6.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,35 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Operating System :: OS Independent
 
 [options]
 install_requires = 
 	gpg-lite>=0.12.3
 packages = find:
 zip_safe = False
 python_requires = >=3.7
 
 [options.package_data]
 libbiomedit = py.typed
 
 [options.extras_require]
-test = pytest
+dev = 
+	mypy==1.8.0
+	pytest==8.0.0
+	ruff==0.2.0
+	bandit==1.7.7
+	types-pkg_resources
 
 [options.packages.find]
 exclude = 
 	test
 	test.*
 
 [egg_info]
```

### Comparing `libbiomedit-0.6.3/test/test_archive.py` & `libbiomedit-0.6.4/test/test_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
                         )
                         # Missing file
                         missing_file_name = "missing.json"
                         with self.assertRaises(KeyError) as cm:
                             archive.extract_member(missing_file_name)
                         self.assertEqual(
                             str(cm.exception),
-                            f"'File object {missing_file_name} not found in {tmp.name}'",
+                            f"'File object {missing_file_name} not found in "
+                            f"{tmp.name}'",
                         )
 
             with self.subTest("Not at file"):
                 name = "not_a_file"
                 with tarfile.open(tmp.name, mode="w") as tar:
                     t_info = tarfile.TarInfo(name)
                     t_info.type = tarfile.DIRTYPE
```

### Comparing `libbiomedit-0.6.3/test/test_classify.py` & `libbiomedit-0.6.4/test/test_classify.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.3/test/test_crypt.py` & `libbiomedit-0.6.4/test/test_crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,39 +36,40 @@
 C_UID = gpg.Uid(full_name="Sgt Hartmann", email=CN_EMAIL)
 D_UID = gpg.Uid(full_name="Doug", email=CN_EMAIL)
 A_FINGERPRINT = "A" * 40
 B_FINGERPRINT = "B" * 40
 C_FINGERPRINT = "C" * 40
 D_FINGERPRINT = "D" * 40
 
+
 # Base data to generate default "user" PGP keys.
 def mock_key(**kwargs: Any) -> gpg.Key:
     """Generate a mock PGP key."""
 
-    mock_data = dict(
-        key_id=CN_FINGERPRINT[-16:],
-        fingerprint=CN_FINGERPRINT,
-        validity=gpg.Validity.ultimately_valid,
-        key_length=4096,
-        pub_key_algorithm=1,
-        creation_date="1550241679",
-        uids=(CN_UID,),
-        owner_trust="u",
-        key_type=gpg.KeyType.public,
-        origin=KEYSERVER,
-        signatures=(CN_SIGNATURE,),
-        key_capabilities=frozenset(
+    mock_data = {
+        "key_id": CN_FINGERPRINT[-16:],
+        "fingerprint": CN_FINGERPRINT,
+        "validity": gpg.Validity.ultimately_valid,
+        "key_length": 4096,
+        "pub_key_algorithm": 1,
+        "creation_date": "1550241679",
+        "uids": (CN_UID,),
+        "owner_trust": "u",
+        "key_type": gpg.KeyType.public,
+        "origin": KEYSERVER,
+        "signatures": (CN_SIGNATURE,),
+        "key_capabilities": frozenset(
             (
                 gpg.KeyCapability.sign,
                 gpg.KeyCapability.certify,
                 gpg.KeyCapability.encrypt,
             )
         ),
-        sub_keys=(),
-    )
+        "sub_keys": (),
+    }
 
     return gpg.Key(**cast(Dict[str, Any], {**mock_data, **kwargs}))
 
 
 def mock_subkey(fingerprint: str) -> gpg.SubKey:
     return gpg.SubKey(
         key_type=gpg.KeyType.public,
@@ -120,15 +121,15 @@
         self.keyserver_keys = keyserver_keys
         self.download_count = 0
         self.detached_sig_signee = detached_sig_signee
 
     def list_pub_keys(
         self,
         search_terms: Iterable[str],
-        sigs: bool = True,  # pylint: disable=unused-argument
+        sigs: bool = True,  # noqa: ARG002 unused-method-argument
     ) -> Sequence[gpg.Key]:
         """Return the list of local keys where the search term matches either
         the email, the fingerprint of the key ID.
         """
         # Make sure that a valid search term was passed.
         for x in search_terms:
             if "@" not in x and len(x) != 40 and len(x) != 16:
@@ -148,15 +149,15 @@
             )
         ]
 
     def vks_recv_key(
         self,
         identifier: str,
         keyserver: str,
-        url_opener: crypt.URL_OPENER_TYPE = crypt.DEFAULT_URL_OPENER,  # pylint: disable=unused-argument
+        url_opener: crypt.URL_OPENER_TYPE = crypt.DEFAULT_URL_OPENER,  # noqa: ARG002 unused-method-argument
     ) -> None:
         """Add the requested keys to the local keys if they are present in
         the keyserver_keys list. This simulates key download.
         """
         received_keys = [
             key for key in self.keyserver_keys if key.fingerprint == identifier
         ]
@@ -174,27 +175,27 @@
     def import_file(self, *args: Any, **kwargs: Any) -> None:
         pass
 
     def vks_get_key_by_fingerprint(
         self,
         keyserver: str,
         fingerprint: str,
-        url_opener: crypt.URL_OPENER_TYPE = crypt.DEFAULT_URL_OPENER,  # pylint: disable=unused-argument
+        url_opener: crypt.URL_OPENER_TYPE = crypt.DEFAULT_URL_OPENER,  # noqa: ARG002 unused-method-argument
     ) -> mock.Mock:
         """Wrapper around vks_recv_key that only download keys specified
         via their fingerprint.
         """
         if len(fingerprint) < 40:
             raise RuntimeError("Not a valid PGP fingerprint")
         self.vks_recv_key(identifier=fingerprint, keyserver=keyserver)
         return mock.Mock()
 
     def verify_detached_sig(
         self,
-        src: bytes,  # pylint: disable=unused-argument
+        src: bytes,  # noqa: ARG002 unused-method-argument
         sig: bytes,
     ) -> str:
         """If the signature is valid, return the signee's fingerprint."""
         if sig != b"valid":
             raise gpg.GPGError("Invalid signature")
         return self.detached_sig_signee
 
@@ -313,15 +314,14 @@
         ],
     ],
 )
 def test_download_key_by_fingerprint(
     fingerprint_to_download: str,
     expectation: Any,
 ) -> None:
-
     # Create a fake GPGStore object (a local keyring).
     local_keys = [KEY_CN]
     keyserver_keys = [KEY_A, KEY_B]
     gpg_store = MockGPGStore(local_keys, keyserver_keys)
 
     # Test function.
     with mock.patch(
@@ -519,15 +519,14 @@
             raise RuntimeError("Not a valid PGP fingerprint")
         gpg_store.vks_recv_key(identifier=fingerprint, keyserver=keyserver)
         return mock.Mock()
 
     with mock.patch(
         "gpg_lite.keyserver.vks_get_key_by_fingerprint", mock_vks_get_key_by_fingerprint
     ):
-
         with expectation, warning:
             refreshed_keys = crypt.retrieve_and_refresh_keys(
                 key_identifiers=key_identifiers,
                 gpg_store=gpg_store,
                 keyserver_url=keyserver_url,
                 allow_key_download=allow_download,
             )
@@ -638,24 +637,25 @@
     detached_sig_signee: str,
     expectation: Any,
 ) -> None:
     """Verify that data package metadata are signed as expected."""
 
     @contextlib.contextmanager
     def mock_archive_reader_init(f: Any) -> Generator[mock.Mock, None, None]:
-        yield mock_archive_open_obj(f)  # pylint: disable=cell-var-from-loop
+        yield mock_archive_open_obj(f)
 
     # Special case: simulate the scenario where the metadata file is missing.
     if metadata_content is None:
         metadata_file_content = b"no metadata file"
     # Regular case: a metadata file is present.
     else:
         test_metadata = {
             "recipients": [CN_FINGERPRINT, A_FINGERPRINT, B_FINGERPRINT],
-            "checksum": "fade655fd178c7fd03d8b52f9350cae9076b532622bc0794f147418a289b7cad",
+            "checksum": "fade655fd178c7fd03d8b52f9350cae9076b532622bc0794f147418"
+            "a289b7cad",
             "timestamp": "2022-02-01T14:13:45+0100",
             "version": "0.7.1",
             "checksum_algorithm": "SHA256",
             "compression_algorithm": "gzip",
             "transfer_id": 7,
             "purpose": "TEST",
         }
```

### Comparing `libbiomedit-0.6.3/test/test_deserialize.py` & `libbiomedit-0.6.4/test/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.3/test/test_portal.py` & `libbiomedit-0.6.4/test/test_portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 TEST_METADATA = MetaData.from_dict(TEST_METADATA_DICT)
 TEST_FILE_NAME = "20220816T090807.zip"
 TEST_FILE_SIZE = 5 << 30  # 5 GB
 
 
 def mock_key_status_response(
     data: str,
-    url: str,  # pylint: disable=unused-argument
+    url: str,  # noqa: ARG001 unused-function-argument
 ) -> str:
     """Mock function that emulates the response from the key status
     portal API endpoint.
     """
     fingerprints = json.loads(data)["fingerprints"]
     return json.dumps(
         [
@@ -105,17 +105,15 @@
             return server_response
 
     mock_urlopen = mock.MagicMock()
     mock_urlopen.return_value.__enter__.return_value = MockHTTPResponse()
 
     portal_api = PortalApi()
     with mock.patch.object(portal_api, "urlopen", mock_urlopen):
-        response = portal_api._post(  # pylint: disable=protected-access
-            url="https://example.com/endpoint", data=b"..."
-        )
+        response = portal_api._post(url="https://example.com/endpoint", data=b"...")
         assert response == server_response
 
 
 @pytest.mark.parametrize("endpoint_name", ["pgpkey_status", "dpkg_check", "dpkg_log"])
 def test_endpoint_url(endpoint_name: str) -> None:
     """Test the PortalApi's properties dedicated to provide endpoint URLs."""
```

