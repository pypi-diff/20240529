# Comparing `tmp/vtjson-1.8.2.tar.gz` & `tmp/vtjson-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.8.2.tar", last modified: Wed May 29 02:06:14 2024, max compression
+gzip compressed data, was "vtjson-1.8.3.tar", last modified: Wed May 29 17:34:27 2024, max compression
```

## Comparing `vtjson-1.8.2.tar` & `vtjson-1.8.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:06:14.041240 vtjson-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-29 02:06:03.000000 vtjson-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-29 02:06:14.041240 vtjson-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-29 02:06:03.000000 vtjson-1.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-29 02:06:03.000000 vtjson-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:06:14.041240 vtjson-1.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:06:14.041240 vtjson-1.8.2/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35776 2024-05-29 02:06:03.000000 vtjson-1.8.2/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:34:27.480576 vtjson-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-29 17:34:21.000000 vtjson-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-05-29 17:34:27.480576 vtjson-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21224 2024-05-29 17:34:21.000000 vtjson-1.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-29 17:34:21.000000 vtjson-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:34:27.480576 vtjson-1.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:34:27.480576 vtjson-1.8.3/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-05-29 17:34:27.000000 vtjson-1.8.3/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 17:34:27.000000 vtjson-1.8.3/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:34:27.000000 vtjson-1.8.3/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 17:34:27.000000 vtjson-1.8.3/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 17:34:27.000000 vtjson-1.8.3/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35515 2024-05-29 17:34:21.000000 vtjson-1.8.3/vtjson.py
```

### Comparing `vtjson-1.8.2/LICENSE` & `vtjson-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.8.2/PKG-INFO` & `vtjson-1.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.8.2
+Version: 1.8.3
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -285,17 +285,30 @@
   ```python
   __compile__(_deferred_compiles=None)
   ```
   This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
-- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. If keys are not basic values such as instances of `bool`, `int`, `float`, `str`, etc... then they are automatically optional.
+- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding values of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. A more elaborate discussion of validation of dictionaries is given below.
 - A `set`. A set validates an object, if one of its members does.
-- An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
+- An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used. Below we call
+such an object a `const schema`.
+## Validation of dictionaries
+In most cases the interpretation of a dictionary schema is obvious. Therefore the following description of the algorithm for validating an object against a dictionary schema is only needed for understanding obscure corner cases. 
+- First we verify that the object is also a dictionary. If not then validation fails.
+- Let us call a `const key` a key of the schema which is a const schema (see above). We verify that all non-optional const keys of the schema are also keys of the object. If this is not the
+case then validation fails.
+- Now we make a list of the keys of the schema (both optional and non-optional).
+- The object will pass validation if all its keys pass validation. We next discuss how to validate a particular key.
+- If none of the entries of the key list validate the given key and `strict=True` (the default) then the key fails validation. Otherwise it validates.
+- We now match the given key against all entries of the key list. If it matches an entry and the corresponding value also validates then the key is validated. Otherwise we keep going through the key list.
+- If the entire key list is consumed then validation of the key fails.
+
+**Note** A consequence of this algorithm is that non-const keys are automatically optional. The wrapper `optional_key` has no effect on them.
 ## Creating types
 A cool feature of `vtjson` is that one can transform a schema into a genuine Python type via
 ```python
 t = make_type(schema)
 ```
 so that validation can be done via
 ```python
```

### Comparing `vtjson-1.8.2/README.md` & `vtjson-1.8.3/vtjson.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: vtjson
+Version: 1.8.3
+Summary: A lightweight package for validating JSON like Python objects
+Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
+Project-URL: Homepage, https://github.com/vdbergh/vtjson
+Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: dnspython
+Requires-Dist: email_validator
+Requires-Dist: idna
+Requires-Dist: python-magic
+
 # vtjson
 A lightweight package for validating JSON like Python objects.
 
 ## Schemas
 
 Validation of JSON like Python objects is done according to a `schema` which is somewhat inspired by a typescript type. The format of a schema is more or less self explanatory as the following example shows.
 
@@ -267,17 +285,30 @@
   ```python
   __compile__(_deferred_compiles=None)
   ```
   This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
-- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. If keys are not basic values such as instances of `bool`, `int`, `float`, `str`, etc... then they are automatically optional.
+- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding values of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. A more elaborate discussion of validation of dictionaries is given below.
 - A `set`. A set validates an object, if one of its members does.
-- An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
+- An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used. Below we call
+such an object a `const schema`.
+## Validation of dictionaries
+In most cases the interpretation of a dictionary schema is obvious. Therefore the following description of the algorithm for validating an object against a dictionary schema is only needed for understanding obscure corner cases. 
+- First we verify that the object is also a dictionary. If not then validation fails.
+- Let us call a `const key` a key of the schema which is a const schema (see above). We verify that all non-optional const keys of the schema are also keys of the object. If this is not the
+case then validation fails.
+- Now we make a list of the keys of the schema (both optional and non-optional).
+- The object will pass validation if all its keys pass validation. We next discuss how to validate a particular key.
+- If none of the entries of the key list validate the given key and `strict=True` (the default) then the key fails validation. Otherwise it validates.
+- We now match the given key against all entries of the key list. If it matches an entry and the corresponding value also validates then the key is validated. Otherwise we keep going through the key list.
+- If the entire key list is consumed then validation of the key fails.
+
+**Note** A consequence of this algorithm is that non-const keys are automatically optional. The wrapper `optional_key` has no effect on them.
 ## Creating types
 A cool feature of `vtjson` is that one can transform a schema into a genuine Python type via
 ```python
 t = make_type(schema)
 ```
 so that validation can be done via
 ```python
```

### Comparing `vtjson-1.8.2/pyproject.toml` & `vtjson-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.8.2/vtjson.egg-info/PKG-INFO` & `vtjson-1.8.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: vtjson
-Version: 1.8.2
-Summary: A lightweight package for validating JSON like Python objects
-Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
-Project-URL: Homepage, https://github.com/vdbergh/vtjson
-Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dnspython
-Requires-Dist: email_validator
-Requires-Dist: idna
-Requires-Dist: python-magic
-
 # vtjson
 A lightweight package for validating JSON like Python objects.
 
 ## Schemas
 
 Validation of JSON like Python objects is done according to a `schema` which is somewhat inspired by a typescript type. The format of a schema is more or less self explanatory as the following example shows.
 
@@ -285,17 +267,30 @@
   ```python
   __compile__(_deferred_compiles=None)
   ```
   This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
-- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. If keys are not basic values such as instances of `bool`, `int`, `float`, `str`, etc... then they are automatically optional.
+- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding values of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. A more elaborate discussion of validation of dictionaries is given below.
 - A `set`. A set validates an object, if one of its members does.
-- An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
+- An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used. Below we call
+such an object a `const schema`.
+## Validation of dictionaries
+In most cases the interpretation of a dictionary schema is obvious. Therefore the following description of the algorithm for validating an object against a dictionary schema is only needed for understanding obscure corner cases. 
+- First we verify that the object is also a dictionary. If not then validation fails.
+- Let us call a `const key` a key of the schema which is a const schema (see above). We verify that all non-optional const keys of the schema are also keys of the object. If this is not the
+case then validation fails.
+- Now we make a list of the keys of the schema (both optional and non-optional).
+- The object will pass validation if all its keys pass validation. We next discuss how to validate a particular key.
+- If none of the entries of the key list validate the given key and `strict=True` (the default) then the key fails validation. Otherwise it validates.
+- We now match the given key against all entries of the key list. If it matches an entry and the corresponding value also validates then the key is validated. Otherwise we keep going through the key list.
+- If the entire key list is consumed then validation of the key fails.
+
+**Note** A consequence of this algorithm is that non-const keys are automatically optional. The wrapper `optional_key` has no effect on them.
 ## Creating types
 A cool feature of `vtjson` is that one can transform a schema into a genuine Python type via
 ```python
 t = make_type(schema)
 ```
 so that validation can be done via
 ```python
```

### Comparing `vtjson-1.8.2/vtjson.py` & `vtjson-1.8.3/vtjson.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.8.2"
+__version__ = "1.8.3"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -201,15 +201,15 @@
 
     def __compile__(self, _deferred_compiles=None):
         return _strict(self.schema, _deferred_compiles=_deferred_compiles)
 
 
 class quote:
     def __init__(self, schema):
-        self.schema = _object(schema)
+        self.schema = _const(schema)
 
     def __validate__(self, object, name, strict):
         return self.schema.__validate__(object, name, strict)
 
 
 class _set_name:
     def __init__(self, schema, name, _deferred_compiles=None):
@@ -591,15 +591,15 @@
     elif isinstance(schema, tuple) or isinstance(schema, list):
         ret = _sequence(schema, _deferred_compiles=_deferred_compiles)
     elif isinstance(schema, dict):
         ret = _dict(schema, _deferred_compiles=_deferred_compiles)
     elif isinstance(schema, set):
         ret = _union(schema, _deferred_compiles=_deferred_compiles)
     else:
-        ret = _object(schema)
+        ret = _const(schema)
 
     # back to updating the cache
     if _deferred_compiles[schema].in_use:
         _deferred_compiles[schema] = ret
     else:
         del _deferred_compiles[schema]
     return ret
@@ -1020,15 +1020,15 @@
                 return ret
         return ""
 
     def __str__(self):
         return str(self.schema)
 
 
-class _object:
+class _const:
     def __init__(self, schema):
         self.schema = schema
         if isinstance(schema, float):
             self.__validate__ = self.__validate_float__
 
     def message(self, name, object):
         return f"{name} (value:{_c(object)}) is not equal to {repr(self.schema)}"
@@ -1071,22 +1071,14 @@
         except Exception as e:
             return _wrong_type_message(object, name, self.__name__, str(e))
 
     def __str__(self):
         return str(self.schema)
 
 
-def is_object(obj):
-    return (
-        not callable(obj)
-        and not hasattr(obj, "__validate__")
-        and not hasattr(obj, "__compile__")
-    )
-
-
 class _dict:
     def __init__(self, schema, _deferred_compiles=None):
         self.min_keys = set()
         self.object_keys = set()
         self.other_keys = set()
         self.schema = {}
         for k in schema:
@@ -1096,15 +1088,15 @@
                 key = k.key
             elif isinstance(k, str) and len(k) > 0 and k[-1] == "?":
                 key = k[:-1]
             else:
                 optional = False
                 key = k
             c = compile(key, _deferred_compiles=_deferred_compiles)
-            if is_object(key):
+            if isinstance(c, _const):
                 if not optional:
                     self.min_keys.add(key)
                 self.object_keys.add(key)
                 self.schema[key] = compiled_schema
             else:
                 self.other_keys.add(c)
                 self.schema[c] = compiled_schema
@@ -1146,12 +1138,7 @@
                 return " and ".join(vals)
             if strict:
                 return f"{name_} is not in the schema"
         return ""
 
     def __str__(self):
         return str(self.schema)
-
-
-# schema = {regex("[a-z]+"): "lc", regex("[A-Z]+"): "UC"}
-# object = {11: "lc"}
-# validate(schema, object)
```

