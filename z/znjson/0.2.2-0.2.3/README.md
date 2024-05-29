# Comparing `tmp/znjson-0.2.2.tar.gz` & `tmp/znjson-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znjson-0.2.2.tar", max compression
+gzip compressed data, was "znjson-0.2.3.tar", max compression
```

## Comparing `znjson-0.2.2.tar` & `znjson-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    13576 2023-03-10 10:38:56.946490 znjson-0.2.2/LICENSE
--rw-r--r--   0        0        0     2838 2023-03-10 10:38:56.946490 znjson-0.2.2/README.md
--rw-r--r--   0        0        0      934 2023-03-10 10:50:38.548749 znjson-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      889 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/__init__.py
--rw-r--r--   0        0        0     3998 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/base.py
--rw-r--r--   0        0        0     2884 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/config.py
--rw-r--r--   0        0        0      680 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/converter/__init__.py
--rw-r--r--   0        0        0      862 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/converter/class_converter.py
--rw-r--r--   0        0        0      580 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/converter/numpy_converter_base64.py
--rw-r--r--   0        0        0      550 2023-03-10 10:50:38.558749 znjson-0.2.2/znjson/converter/numpy_converter_small.py
--rw-r--r--   0        0        0      807 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/converter/old_converters.py
--rw-r--r--   0        0        0      374 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/converter/pathlib_converter.py
--rw-r--r--   0        0        0      148 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/exceptions/__init__.py
--rw-r--r--   0        0        0     2772 2023-03-10 10:38:56.966490 znjson-0.2.2/znjson/main.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 znjson-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    13576 2024-02-28 13:30:59.424610 znjson-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2838 2024-02-28 13:30:59.424703 znjson-0.2.3/README.md
+-rw-r--r--   0        0        0      673 2024-05-29 13:33:52.218573 znjson-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      957 2024-05-29 13:33:52.219356 znjson-0.2.3/znjson/__init__.py
+-rw-r--r--   0        0        0     3999 2024-05-29 13:33:52.219502 znjson-0.2.3/znjson/base.py
+-rw-r--r--   0        0        0     2885 2024-05-29 13:33:52.219643 znjson-0.2.3/znjson/config.py
+-rw-r--r--   0        0        0      681 2024-05-29 13:33:52.219784 znjson-0.2.3/znjson/converter/__init__.py
+-rw-r--r--   0        0        0      863 2024-05-29 13:33:52.219932 znjson-0.2.3/znjson/converter/class_converter.py
+-rw-r--r--   0        0        0      581 2024-05-29 13:33:52.220076 znjson-0.2.3/znjson/converter/numpy_converter_base64.py
+-rw-r--r--   0        0        0      551 2024-05-29 13:33:52.220221 znjson-0.2.3/znjson/converter/numpy_converter_small.py
+-rw-r--r--   0        0        0      807 2024-05-29 13:33:52.220369 znjson-0.2.3/znjson/converter/old_converters.py
+-rw-r--r--   0        0        0      375 2024-05-29 13:33:52.220577 znjson-0.2.3/znjson/converter/pathlib_converter.py
+-rw-r--r--   0        0        0      148 2024-02-28 13:30:59.427688 znjson-0.2.3/znjson/exceptions/__init__.py
+-rw-r--r--   0        0        0     3149 2024-05-29 13:33:52.220715 znjson-0.2.3/znjson/main.py
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 znjson-0.2.3/PKG-INFO
```

### Comparing `znjson-0.2.2/LICENSE` & `znjson-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `znjson-0.2.2/README.md` & `znjson-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `znjson-0.2.2/znjson/__init__.py` & `znjson-0.2.3/znjson/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 """The ZnJSON serializing module
 
 https://github.com/zincware/ZnJSON
 """
+
 import importlib.metadata
 import logging
 import sys
 
 from znjson import converter
 from znjson.base import ConverterBase
 from znjson.config import config, deregister, register
-from znjson.main import ZnDecoder, ZnEncoder
+from znjson.main import ZnDecoder, ZnEncoder, dumps, loads
 
-__all__ = ["ConverterBase", "ZnDecoder", "ZnEncoder", "config", "register", "deregister"]
+__all__ = [
+    "ConverterBase",
+    "ZnDecoder",
+    "ZnEncoder",
+    "config",
+    "register",
+    "deregister",
+    "loads",
+    "dumps",
+]
 __all__ += converter.__all__
 
 __version__ = importlib.metadata.version("znjson")
 
 config.register()
 
 logger = logging.getLogger(__name__)
```

### Comparing `znjson-0.2.2/znjson/base.py` & `znjson-0.2.3/znjson/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ZnJSON converter parent class"""
+
 from __future__ import annotations
 
 import abc
 import base64
 import functools
 import io
 import logging
```

### Comparing `znjson-0.2.2/znjson/config.py` & `znjson-0.2.3/znjson/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ZnJSON global configuration file"""
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass, field
 from typing import List, Tuple, Type, Union
 
 from znjson import converter
```

### Comparing `znjson-0.2.2/znjson/converter/__init__.py` & `znjson-0.2.3/znjson/converter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manage Converter Inputs based on available moduls"""
+
 from znjson.converter.class_converter import ClassConverter
 from znjson.converter.pathlib_converter import PathlibConverter
 
 __all__ = ["PathlibConverter", "ClassConverter"]
 
 try:
     from znjson.converter.numpy_converter_base64 import NumpyConverter
```

### Comparing `znjson-0.2.2/znjson/converter/class_converter.py` & `znjson-0.2.3/znjson/converter/class_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Use pickle to serialize arbitrary classes"""
+
 import functools
 import importlib
 import pickle
 
 from znjson.base import ConverterBase
```

### Comparing `znjson-0.2.2/znjson/converter/numpy_converter_base64.py` & `znjson-0.2.3/znjson/converter/numpy_converter_base64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Use base64 encoding to ASCII for large numpy arrays"""
+
 import functools
 
 import numpy as np
 
 from znjson.base import ConverterBase
```

### Comparing `znjson-0.2.2/znjson/converter/numpy_converter_small.py` & `znjson-0.2.3/znjson/converter/numpy_converter_small.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convert small numpy arrays to lists"""
+
 import numpy as np
 
 from znjson.base import ConverterBase
 
 
 class NumpyConverterSmall(ConverterBase):
     """Convert small numpy arrays to lists"""
```

### Comparing `znjson-0.2.2/znjson/converter/old_converters.py` & `znjson-0.2.3/znjson/converter/old_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Converters that should not be used anymore but are
- still available for backwards compatibility."""
+still available for backwards compatibility."""
+
 import io
 
 import numpy as np
 
 from znjson.converter.numpy_converter_base64 import NumpyConverter
```

### Comparing `znjson-0.2.2/znjson/main.py` & `znjson-0.2.3/znjson/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 """ZnJSON main Encoder / Decoder classes to use with the default json library"""
+
+import functools
 import json
 from typing import Any
 
 from znjson.config import config
 
 
+@functools.wraps(json.loads)
+def loads(data: str, cls=None, **kwargs):
+    """Load a string with ZnJSON decoding"""
+    return json.loads(data, cls=cls or ZnDecoder, **kwargs)
+
+
+@functools.wraps(json.dumps)
+def dumps(data: Any, cls=None, **kwargs) -> str:
+    """Dump data with ZnJSON encoding"""
+    return json.dumps(data, cls=cls or ZnEncoder, **kwargs)
+
+
 class SelectConverters:
     """Mixin to manipulate to converters in use"""
 
     _active_converters = None
 
     @classmethod
     def from_converters(cls, converter, add_default=False):
```

### Comparing `znjson-0.2.2/PKG-INFO` & `znjson-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: znjson
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python Package to Encode/Decode some common file formats to json
 License: Apache-2.0
 Keywords: json,zntrack,jsonpickle,serialization,deserialization
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: repository, https://github.com/zincware/ZnJSON
 Description-Content-Type: text/markdown
 
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnJSON/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnJSON?branch=main)
 [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Tests](https://github.com/zincware/ZnJSON/actions/workflows/pytest.yaml/badge.svg)](https://coveralls.io/github/zincware/ZnJSON?branch=main)
 [![PyPI version](https://badge.fury.io/py/znjson.svg)](https://badge.fury.io/py/znjson)
```

