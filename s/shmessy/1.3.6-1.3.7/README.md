# Comparing `tmp/shmessy-1.3.6.tar.gz` & `tmp/shmessy-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shmessy-1.3.6.tar", max compression
+gzip compressed data, was "shmessy-1.3.7.tar", max compression
```

## Comparing `shmessy-1.3.6.tar` & `shmessy-1.3.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1073 2024-05-26 10:44:36.899494 shmessy-1.3.6/LICENSE
--rw-r--r--   0        0        0     5669 2024-05-26 10:44:36.899494 shmessy-1.3.6/README.md
--rw-r--r--   0        0        0      863 2024-05-26 10:45:03.647499 shmessy-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     5701 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/exceptions.py
--rw-r--r--   0        0        0      395 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/schema.py
--rw-r--r--   0        0        0        0 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/types/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/types/base.py
--rw-r--r--   0        0        0     2226 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/types/boolean.py
--rw-r--r--   0        0        0     2566 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/types/date.py
--rw-r--r--   0        0        0     3128 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/types/datetime_.py
--rw-r--r--   0        0        0     1016 2024-05-26 10:44:36.899494 shmessy-1.3.6/src/shmessy/types/email.py
--rw-r--r--   0        0        0     1550 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/types/float.py
--rw-r--r--   0        0        0     1256 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/types/integer.py
--rw-r--r--   0        0        0     1272 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/types/ipv4_address.py
--rw-r--r--   0        0        0      991 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/types/string.py
--rw-r--r--   0        0        0     3188 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/types/unix_timestamp.py
--rw-r--r--   0        0        0     7381 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/types_handler.py
--rw-r--r--   0        0        0     1848 2024-05-26 10:44:36.903494 shmessy-1.3.6/src/shmessy/utils.py
--rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-28 13:24:38.294172 shmessy-1.3.7/LICENSE
+-rw-r--r--   0        0        0     5669 2024-05-28 13:24:38.294172 shmessy-1.3.7/README.md
+-rw-r--r--   0        0        0      863 2024-05-28 13:25:12.789351 shmessy-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5701 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/__init__.py
+-rw-r--r--   0        0        0     1559 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/date_utils.py
+-rw-r--r--   0        0        0     2023 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/exceptions.py
+-rw-r--r--   0        0        0      395 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/schema.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/__init__.py
+-rw-r--r--   0        0        0     1090 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/base.py
+-rw-r--r--   0        0        0     2226 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/boolean.py
+-rw-r--r--   0        0        0     1732 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/date.py
+-rw-r--r--   0        0        0     2041 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/datetime_.py
+-rw-r--r--   0        0        0     1016 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/email.py
+-rw-r--r--   0        0        0     1550 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/float.py
+-rw-r--r--   0        0        0     1256 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/integer.py
+-rw-r--r--   0        0        0     1272 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/ipv4_address.py
+-rw-r--r--   0        0        0      991 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/string.py
+-rw-r--r--   0        0        0     3188 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types/unix_timestamp.py
+-rw-r--r--   0        0        0     7381 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/types_handler.py
+-rw-r--r--   0        0        0     1848 2024-05-28 13:24:38.298172 shmessy-1.3.7/src/shmessy/utils.py
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.7/PKG-INFO
```

### Comparing `shmessy-1.3.6/LICENSE` & `shmessy-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/README.md` & `shmessy-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/pyproject.toml` & `shmessy-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shmessy"
-version = "v1.3.6"
+version = "v1.3.7"
 description = "If your data is messy - Use Shmessy!"
 readme = "README.md"
 authors = ["Ohad Mata <ohadmata@gmail.com>"]
 homepage = "https://github.com/ohadmata/shmessy"
 repository = "https://github.com/ohadmata/shmessy"
 packages = [
     { include = "shmessy", from = "src" },
```

### Comparing `shmessy-1.3.6/src/shmessy/__init__.py` & `shmessy-1.3.7/src/shmessy/__init__.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/exceptions.py` & `shmessy-1.3.7/src/shmessy/exceptions.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types/base.py` & `shmessy-1.3.7/src/shmessy/types/string.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-import math
-from abc import ABC, abstractmethod
+import logging
 from typing import Any, Optional, Tuple
 
 from numpy import ndarray
 from pandas import Series
 
 from ..schema import InferredField
+from .base import BaseType
 
+logger = logging.getLogger(__name__)
 
-class BaseType(ABC):
-    weight: int = 0
 
-    @abstractmethod
-    def validate(self, data: ndarray) -> Optional[InferredField]:
-        pass
-
-    @abstractmethod
-    def cast_value(self, value: Any, pattern: Optional[Any] = None) -> Optional[Any]:
-        pass
-
-    @abstractmethod
-    def cast_column(
-        self, column: Series, inferred_field: InferredField
-    ) -> Optional[Any]:
-        pass
-
-    @abstractmethod
-    def ignore_cast_for_types(self) -> Tuple[Any]:
-        pass
+class StringType(BaseType):
+    weight = 9
 
-    @property
-    def name(self) -> str:
-        return str(self.__class__.__name__.replace("Type", ""))
+    def validate(self, data: ndarray) -> Optional[InferredField]:
+        for value in data:
+            try:
+                str(value)
+            except Exception:  # noqa
+                logger.debug(f"Cannot cast the value '{value}' to {self.name}")
+                return None
+        return InferredField(inferred_type=self.name)
 
     @property
     def prefer_column_casting(self) -> bool:
-        return False
+        return True
+
+    def cast_column(self, column: Series, inferred_field: InferredField) -> Series:
+        return column.apply(lambda x: str(x))
 
-    @staticmethod
-    def is_empty_value(value: Any) -> bool:
-        if value is None or (isinstance(value, float) and math.isnan(value)):
-            return True
-        return False
+    def cast_value(self, value: Any, pattern: Optional[Any] = None) -> Optional[Any]:
+        return str(value)
+
+    def ignore_cast_for_types(self) -> Tuple[Any]:
+        return tuple()
```

### Comparing `shmessy-1.3.6/src/shmessy/types/boolean.py` & `shmessy-1.3.7/src/shmessy/types/boolean.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types/email.py` & `shmessy-1.3.7/src/shmessy/types/email.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types/float.py` & `shmessy-1.3.7/src/shmessy/types/float.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types/integer.py` & `shmessy-1.3.7/src/shmessy/types/integer.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types/ipv4_address.py` & `shmessy-1.3.7/src/shmessy/types/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types/unix_timestamp.py` & `shmessy-1.3.7/src/shmessy/types/unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/types_handler.py` & `shmessy-1.3.7/src/shmessy/types_handler.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/src/shmessy/utils.py` & `shmessy-1.3.7/src/shmessy/utils.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.6/PKG-INFO` & `shmessy-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shmessy
-Version: 1.3.6
+Version: 1.3.7
 Summary: If your data is messy - Use Shmessy!
 Home-page: https://github.com/ohadmata/shmessy
 Author: Ohad Mata
 Author-email: ohadmata@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

