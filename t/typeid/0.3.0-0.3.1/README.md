# Comparing `tmp/typeid-0.3.0.tar.gz` & `tmp/typeid-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeid-0.3.0.tar", max compression
+gzip compressed data, was "typeid-0.3.1.tar", max compression
```

## Comparing `typeid-0.3.0.tar` & `typeid-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 11:53:12.620224 typeid-0.3.0/LICENSE
--rw-r--r--   0        0        0     2239 2024-05-23 10:16:53.746492 typeid-0.3.0/README.md
--rw-r--r--   0        0        0      509 2024-05-23 10:19:06.232956 typeid-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4905 2024-05-23 10:07:43.860496 typeid-0.3.0/typeid/__init__.py
--rw-r--r--   0        0        0     1283 2024-05-22 15:35:58.509544 typeid-0.3.0/typeid/sqla.py
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 typeid-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-29 09:07:33.103697 typeid-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2239 2024-05-29 09:07:33.103697 typeid-0.3.1/README.md
+-rw-r--r--   0        0        0      509 2024-05-29 09:30:40.134278 typeid-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5471 2024-05-29 09:07:33.107030 typeid-0.3.1/typeid/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-29 09:07:33.107030 typeid-0.3.1/typeid/sqla.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 typeid-0.3.1/PKG-INFO
```

### Comparing `typeid-0.3.0/LICENSE` & `typeid-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typeid-0.3.0/README.md` & `typeid-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `typeid-0.3.0/typeid/__init__.py` & `typeid-0.3.1/typeid/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,63 +17,78 @@
     >>> assert str(typeids.ApikeyId(uuid7().hex)).startswith("apikey_")
     >>> assert (typeids.UserId("user_nnv5rr3rfk3hgry6xrygr").hex
     ...    == "0664c4135ed83faabd4bc0dc33839c9f")
     >>> extra_types = generate("admin", suffix="IdUseWithCare")
     >>> assert str(extra_types.AdminIdUseWithCare(uuid7().hex)).startswith("admin_")
 """
 
-from typing import Dict, Optional, Callable
+from typing import Optional, Callable
 from base58 import b58encode, b58decode
 from uuid import UUID
 
 
 class BaseId(UUID):
     """BaseID implementation that does the lifting of a UUID into a typed UUID
     and formats it more nicely.
 
     :param _prefix: The internal _prefix is filled in the generate() method
     """
 
     #: This class variable will be filled in by type() later own
     _prefix: str = ""
     _generator: Optional[Callable] = None
+    _encode = staticmethod(b58encode)
+    _decode = staticmethod(b58decode)
 
     def __init__(self, id: Optional[UUID | str | bytes] = None) -> None:
         if id is None and callable(self._generator):
             generator = getattr(self, "_generator")
             id = generator()
 
         if isinstance(id, UUID):
+            # Load from a UUID using the hex representation
             super().__init__(id.hex)
-        elif isinstance(id, bytes):
+
+        elif isinstance(id, bytes) and len(id) == 16:
+            # forward the hex content of a bytes array
             super().__init__(id.hex())
+
         elif isinstance(id, str):
-            if id.startswith(self._prefix):
+            # Load from string
+            # NOTE: we need to make a distinction if it starts with our prefix
+            # or not
+
+            if id.startswith(f"{self._prefix}_"):
+                # uses our prefix
                 prefix_free_id = id[len(self._prefix) + 1 :]
-                uid: bytes = b58decode(prefix_free_id)
+                uid: bytes = self._decode(prefix_free_id.encode("ascii"))
                 super().__init__(uid.hex())
+
             elif "_" in id:
+                # does not use our prefix but has a _ in the string!
                 found_prefix = id[: id.index("_")]
                 raise ValueError(
                     f"Wrong prefix, got {found_prefix}, expected {self._prefix}"
                 )
+
             else:
+                # most probably a hex string
                 super().__init__(id)
         else:
             raise NotImplementedError(
                 "Incorrect argument type. Requries, UUID, hex, bytes or string."
             )
 
     def __str__(self) -> str:
         """Prefix and base58 encode the id
 
         :return: encoded and prefixed id as string
         """
         prefix = str(self._prefix)
-        id = b58encode(self.bytes).decode("ascii").lower()
+        id = self._encode(self.bytes).decode("ascii")
         return f"{prefix}_{id}"
 
 
 class AttrDict(dict):
     """This class enables us to access the return values of generate() as
     attributes."""
 
@@ -83,15 +98,15 @@
 
 
 def generate(
     *args: str,
     suffix: str = "Id",
     enable_sqla: bool = False,
     generator: Callable = None,
-) -> Dict[str, BaseId]:
+) -> AttrDict:
     """Generate types based on a list of arguments. Each argument will result in
     a new type named after the argument (camel-cased) with the defined suffix at the end.
 
     :param *args: list of strings for which to generate typed Id classes
     :param suffix: (Id) suffix used in the classes
     :param enable_sqla: (False) If true, also generates classes (suffix "SQLA" to be used for sqlalchemy)
     :param generator: (None) Allows to provide a generator for new instances
@@ -105,14 +120,15 @@
     >>> typed_ids = generate(
     ...     "user",
     ...     "apikey",
     ...     generator=lambda: uuid7().hex
     ... )
     >>> user_id = str(typed_ids.UserId())
     >>> # user_id = user_nnv5rr3rfk3hgry6xrygr
+    >>> u_id_typed = typed_ids.userId("user_nnv5rr3rfk3hgry6xrygr")
     """
     ret = {}
     for _type in args:
         name = f"{_type.capitalize()}{suffix}"
         typeid_class = type(
             name, (BaseId,), dict(_prefix=_type, _generator=staticmethod(generator))
         )
```

### Comparing `typeid-0.3.0/typeid/sqla.py` & `typeid-0.3.1/typeid/sqla.py`

 * *Files identical despite different names*

### Comparing `typeid-0.3.0/PKG-INFO` & `typeid-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeid
-Version: 0.3.0
+Version: 0.3.1
 Summary: UUID-compatible Typed IDs with prefixes
 License: MIT
 Author: Fabian Schuh
 Author-email: info@chainsquad.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

