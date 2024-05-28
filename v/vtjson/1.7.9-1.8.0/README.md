# Comparing `tmp/vtjson-1.7.9.tar.gz` & `tmp/vtjson-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.7.9.tar", last modified: Sun Apr 28 06:37:06 2024, max compression
+gzip compressed data, was "vtjson-1.8.0.tar", last modified: Tue May 28 21:40:49 2024, max compression
```

## Comparing `vtjson-1.7.9.tar` & `vtjson-1.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:37:06.217266 vtjson-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-28 06:37:00.000000 vtjson-1.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 06:37:06.217266 vtjson-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19109 2024-04-28 06:37:00.000000 vtjson-1.7.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 06:37:00.000000 vtjson-1.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:37:06.217266 vtjson-1.7.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:37:06.217266 vtjson-1.7.9/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30777 2024-04-28 06:37:00.000000 vtjson-1.7.9/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:40:49.930052 vtjson-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-28 21:40:45.000000 vtjson-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-28 21:40:49.930052 vtjson-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-28 21:40:45.000000 vtjson-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 21:40:45.000000 vtjson-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:40:49.930052 vtjson-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:40:49.926052 vtjson-1.8.0/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-28 21:40:49.000000 vtjson-1.8.0/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 21:40:49.000000 vtjson-1.8.0/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:40:49.000000 vtjson-1.8.0/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 21:40:49.000000 vtjson-1.8.0/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 21:40:49.000000 vtjson-1.8.0/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35601 2024-05-28 21:40:45.000000 vtjson-1.8.0/vtjson.py
```

### Comparing `vtjson-1.7.9/LICENSE` & `vtjson-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.9/PKG-INFO` & `vtjson-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.9
+Version: 1.8.0
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -226,15 +226,14 @@
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
-- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
@@ -242,18 +241,23 @@
 - `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
 - `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
 - `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
 - `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
 - `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
-- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
-corresponding inequality is not checked.
-- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+- `interval(lb, ub, strict_lb=False, strict_ub=False)`. This checks if `lb <= object <= ub`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the corresponding inequality is not checked. The optional arguments `strict_lb`, `strict_ub` indicate whether the corresponding inequalities should be strict.
+- `gt(lb)`. This checks if `object > lb`.
+- `ge(lb)`. This checks if `object >= lb`.
+- `lt(ub)`. This checks if `object < ub`.
+- `le(ub)`. This checks if `object <= ub`.
+- `size(lowerbound, upperbound=None)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis). If `upperbound=None` then `upperbound` is set to `lowerbound`.
 - `fields({field1: schema1, field2: schema2, ..., fieldN: schemaN})`. Matches Python objects with attributes `field1, field2, ..., fieldN` whose corresponding values should validate against `schema1, schema2, ..., schemaN` respectively.
+- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
+- `filter(callable, schema, filter_name=None)`. Applies `callable` to the object and validates the result with `schema`. The optional argument `filter_name` is used in non-validation messages.
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
 An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
@@ -281,15 +285,15 @@
   ```python
   __compile__(_deferred_compiles=None)
   ```
   This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
-- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema.
+- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. If keys are not basic values such as instances of `bool`, `int`, `float`, `str`, etc... then they are automatically optional.
 - A `set`. A set validates an object, if one of its members does.
 - An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
 ## Creating types
 A cool feature of `vtjson` is that one can transform a schema into a genuine Python type via
 ```python
 t = make_type(schema)
 ```
```

### Comparing `vtjson-1.7.9/README.md` & `vtjson-1.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -208,15 +208,14 @@
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
-- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
@@ -224,18 +223,23 @@
 - `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
 - `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
 - `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
 - `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
 - `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
-- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
-corresponding inequality is not checked.
-- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+- `interval(lb, ub, strict_lb=False, strict_ub=False)`. This checks if `lb <= object <= ub`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the corresponding inequality is not checked. The optional arguments `strict_lb`, `strict_ub` indicate whether the corresponding inequalities should be strict.
+- `gt(lb)`. This checks if `object > lb`.
+- `ge(lb)`. This checks if `object >= lb`.
+- `lt(ub)`. This checks if `object < ub`.
+- `le(ub)`. This checks if `object <= ub`.
+- `size(lowerbound, upperbound=None)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis). If `upperbound=None` then `upperbound` is set to `lowerbound`.
 - `fields({field1: schema1, field2: schema2, ..., fieldN: schemaN})`. Matches Python objects with attributes `field1, field2, ..., fieldN` whose corresponding values should validate against `schema1, schema2, ..., schemaN` respectively.
+- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
+- `filter(callable, schema, filter_name=None)`. Applies `callable` to the object and validates the result with `schema`. The optional argument `filter_name` is used in non-validation messages.
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
 An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
@@ -263,15 +267,15 @@
   ```python
   __compile__(_deferred_compiles=None)
   ```
   This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
-- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema.
+- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. If keys are not basic values such as instances of `bool`, `int`, `float`, `str`, etc... then they are automatically optional.
 - A `set`. A set validates an object, if one of its members does.
 - An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
 ## Creating types
 A cool feature of `vtjson` is that one can transform a schema into a genuine Python type via
 ```python
 t = make_type(schema)
 ```
```

### Comparing `vtjson-1.7.9/pyproject.toml` & `vtjson-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.9/vtjson.egg-info/PKG-INFO` & `vtjson-1.8.0/vtjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.9
+Version: 1.8.0
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -226,15 +226,14 @@
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
-- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
@@ -242,18 +241,23 @@
 - `nothing`. Matches nothing.
 ## Mixins
 Mixins are built-ins that are usually combined with other schemas using `intersect`.
 - `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
 - `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
 - `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
 - `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
-- `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
-corresponding inequality is not checked.
-- `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+- `interval(lb, ub, strict_lb=False, strict_ub=False)`. This checks if `lb <= object <= ub`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the corresponding inequality is not checked. The optional arguments `strict_lb`, `strict_ub` indicate whether the corresponding inequalities should be strict.
+- `gt(lb)`. This checks if `object > lb`.
+- `ge(lb)`. This checks if `object >= lb`.
+- `lt(ub)`. This checks if `object < ub`.
+- `le(ub)`. This checks if `object <= ub`.
+- `size(lowerbound, upperbound=None)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis). If `upperbound=None` then `upperbound` is set to `lowerbound`.
 - `fields({field1: schema1, field2: schema2, ..., fieldN: schemaN})`. Matches Python objects with attributes `field1, field2, ..., fieldN` whose corresponding values should validate against `schema1, schema2, ..., schemaN` respectively.
+- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
+- `filter(callable, schema, filter_name=None)`. Applies `callable` to the object and validates the result with `schema`. The optional argument `filter_name` is used in non-validation messages.
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
 An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
@@ -281,15 +285,15 @@
   ```python
   __compile__(_deferred_compiles=None)
   ```
   This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
-- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema.
+- A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema. Keys can themselves be schemas. E.g. `{str: str}` represents a dictionary whose keys and values are both strings. If keys are not basic values such as instances of `bool`, `int`, `float`, `str`, etc... then they are automatically optional.
 - A `set`. A set validates an object, if one of its members does.
 - An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
 ## Creating types
 A cool feature of `vtjson` is that one can transform a schema into a genuine Python type via
 ```python
 t = make_type(schema)
 ```
```

### Comparing `vtjson-1.7.9/vtjson.py` & `vtjson-1.8.0/vtjson.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import collections
 import datetime
 import ipaddress
 import math
 import pathlib
 import re
 import urllib.parse
 
@@ -29,15 +28,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.7.9"
+__version__ = "1.8.0"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -71,30 +70,14 @@
 def _wrong_type_message(object, name, type_name, explanation=None):
     message = f"{name} (value:{_c(object)}) is not of type '{type_name}'"
     if explanation is not None:
         message += f": {explanation}"
     return message
 
 
-def _keys2(dict):
-    ret = set()
-    for k in dict:
-        if isinstance(k, optional_key):
-            ret.add((k.key, k, True))
-        elif isinstance(k, str) and len(k) > 0 and k[-1] == "?":
-            ret.add((k[:-1], k, True))
-        else:
-            ret.add((k, k, False))
-    return ret
-
-
-def _keys(dict):
-    return {k[0] for k in _keys2(dict)}
-
-
 class _validate_meta(type):
     def __instancecheck__(cls, object):
         valid = _validate(cls.__schema__, object, "object", strict=cls.__strict__)
         if cls.__debug__ and valid != "":
             print(f"DEBUG: {valid}")
         return valid == ""
 
@@ -365,97 +348,185 @@
             return _wrong_type_message(object, name, "int")
         elif (object - self.remainder) % self.divisor == 0:
             return ""
         else:
             return _wrong_type_message(object, name, self.__name__)
 
 
+class gt:
+    def __init__(self, lb):
+        try:
+            lb <= lb
+        except Exception:
+            raise SchemaError(
+                f"The lower bound {lb} does not support comparison"
+            ) from None
+        self.lb = lb
+
+    def message(self, name, object):
+        return f"{name} (value:{_c(object)}) is not strictly greater than {self.lb}"
+
+    def __validate__(self, object, name, strict):
+        try:
+            if self.lb < object:
+                return ""
+            else:
+                return self.message(name, object)
+        except Exception as e:
+            return f"{self.message(name, object)}: {str(e)}"
+
+
+class ge:
+    def __init__(self, lb):
+        try:
+            lb <= lb
+        except Exception:
+            raise SchemaError(
+                f"The lower bound {lb} does not support comparison"
+            ) from None
+        self.lb = lb
+
+    def message(self, name, object):
+        return f"{name} (value:{_c(object)}) is not greater than or equal to {self.lb}"
+
+    def __validate__(self, object, name, strict):
+        try:
+            if self.lb <= object:
+                return ""
+            else:
+                return self.message(name, object)
+        except Exception as e:
+            return f"{self.message(name, object)}: {str(e)}"
+
+
+class lt:
+    def __init__(self, ub):
+        try:
+            ub <= ub
+        except Exception:
+            raise SchemaError(
+                f"The upper bound {ub} does not support comparison"
+            ) from None
+        self.ub = ub
+
+    def message(self, name, object):
+        return f"{name} (value:{_c(object)}) is not strictly less than {self.ub}"
+
+    def __validate__(self, object, name, strict):
+        try:
+            if self.ub > object:
+                return ""
+            else:
+                return self.message(name, object)
+        except Exception as e:
+            return f"{self.message(name, object)}: {str(e)}"
+
+
+class le:
+    def __init__(self, ub):
+        try:
+            ub <= ub
+        except Exception:
+            raise SchemaError(
+                f"The upper bound {ub} does not support comparison"
+            ) from None
+        self.ub = ub
+
+    def message(self, name, object):
+        return f"{name} (value:{_c(object)}) is not less than or equal to {self.ub}"
+
+    def __validate__(self, object, name, strict):
+        try:
+            if self.ub >= object:
+                return ""
+            else:
+                return self.message(name, object)
+        except Exception as e:
+            return f"{self.message(name, object)}: {str(e)}"
+
+
 class interval:
-    def __init__(self, lb, ub):
+    def __init__(self, lb, ub, strict_lb=False, strict_ub=False):
         self.lb = lb
         self.ub = ub
+
         self.lb_s = "..." if lb == ... else repr(lb)
         self.ub_s = "..." if ub == ... else repr(ub)
 
+        ld = "]" if strict_lb else "["
+        ud = "[" if strict_ub else "]"
+
+        if lb is not ...:
+            if strict_lb:
+                lower = gt(lb)
+            else:
+                lower = ge(lb)
+
+        if ub is not ...:
+            if strict_ub:
+                upper = lt(ub)
+            else:
+                upper = le(ub)
+
         if lb is ... and ub is ...:
-            self.__validate__ = self.__validate_none__
+            self.__validate__ = anything().__validate__
         elif lb is ...:
             try:
                 ub <= ub
             except Exception:
                 raise SchemaError(
                     f"The upper bound in the interval"
-                    f" [{self.lb_s},{self.ub_s}] does not support comparison"
+                    f" {ld}{self.lb_s},{self.ub_s}{ud} does not support comparison"
                 ) from None
-            self.__validate__ = self.__validate_ub__
+            self.__validate__ = upper.__validate__
         elif ub is ...:
             try:
                 lb <= lb
             except Exception:
                 raise SchemaError(
                     f"The lower bound in the interval"
-                    f" [{self.lb_s},{self.ub_s}] does not support comparison"
+                    f" {ld}{self.lb_s},{self.ub_s}{ud} does not support comparison"
                 ) from None
-            self.__validate__ = self.__validate_lb__
+            self.__validate__ = lower.__validate__
         else:
             try:
                 lb <= ub
             except Exception:
                 raise SchemaError(
                     f"The upper and lower bound in the interval"
-                    f" [{self.lb_s},{self.ub_s}] are incomparable"
+                    f" {ld}{self.lb_s},{self.ub_s}{ud} are incomparable"
                 ) from None
+            self.__validate__ = _intersect((lower, upper)).__validate__
 
-    def message(self, name, object):
-        return (
-            f"{name} (value:{_c(object)}) is not in the interval "
-            f"[{self.lb_s},{self.ub_s}]"
-        )
-
+    # Not used but necessary for the protocol
     def __validate__(self, object, name, strict):
-        try:
-            if self.lb <= object <= self.ub:
-                return ""
-            else:
-                return self.message(name, object)
-        except Exception as e:
-            return f"{self.message(name, object)}: {str(e)}"
-
-    def __validate_ub__(self, object, name, strict):
-        try:
-            if object <= self.ub:
-                return ""
-            else:
-                return self.message(name, object)
-        except Exception as e:
-            return f"{self.message(name, object)}: {str(e)}"
-
-    def __validate_lb__(self, object, name, strict):
-        try:
-            if object >= self.lb:
-                return ""
-            else:
-                return self.message(name, object)
-        except Exception as e:
-            return f"{self.message(name, object)}: {str(e)}"
-
-    def __validate_none__(self, object, name, strict):
         return ""
 
 
 class size:
-    def __init__(self, lb, ub):
+    def __init__(self, lb, ub=None):
+        if ub is None:
+            ub = lb
         if not isinstance(lb, int):
-            raise SchemaError(f"{repr(lb)} is not of type 'int'")
-        if lb < -0:
-            raise SchemaError(f"{repr(lb)} is not >= 0")
+            raise SchemaError(
+                f"the lower size bound (value: {repr(lb)}) is not of type 'int'"
+            )
+        if lb < 0:
+            raise SchemaError(
+                f"the lower size bound (value: {repr(lb)}) is smaller than 0"
+            )
         if not isinstance(ub, int) and ub != ...:
-            raise SchemaError(f"{repr(ub)} is not of type 'int'")
+            raise SchemaError(
+                f"the upper size bound (value:{repr(ub)}) is not of type 'int'"
+            )
         if isinstance(ub, int) and ub < lb:
-            raise SchemaError(f"{repr(ub)} is not >= {repr(lb)}")
+            raise SchemaError(
+                f"the lower size bound (value: {repr(lb)}) is bigger "
+                f"than the upper bound (value: {repr(ub)})"
+            )
         self.interval = interval(lb, ub)
 
     def __validate__(self, object, name, strict):
         try:
             L = len(object)
         except Exception:
             return f"{name} (value:{_c(object)}) has no len()"
@@ -829,45 +900,57 @@
                 raise SchemaError(f"key {repr(k)} in {repr(d)} is not a string")
         self.d = d
 
     def __compile__(self, _deferred_compiles=None):
         return _fields(self.d, _deferred_compiles=_deferred_compiles)
 
 
-class _dict:
-    def __init__(self, schema, _deferred_compiles=None):
-        self.schema = collections.OrderedDict()
-        for k, v in schema.items():
-            self.schema[k] = compile(v, _deferred_compiles=_deferred_compiles)
-        self.keys = _keys(self.schema)
-        self.keys2 = _keys2(self.schema)
+class _filter:
+    def __init__(self, filter, schema, filter_name=None, _deferred_compiles=None):
+        self.filter = filter
+        self.schema = compile(schema, _deferred_compiles=_deferred_compiles)
+        if filter_name is not None:
+            self.filter_name = filter_name
+        else:
+            try:
+                self.filter_name = self.filter.__name__
+            except Exception:
+                self.filter_name = "filter"
+            if self.filter_name == "<lambda>":
+                self.filter_name = "filter"
 
     def __validate__(self, object, name, strict):
-        if not isinstance(object, dict):
-            return _wrong_type_message(object, name, "dict")
-        for k_, k, o in self.keys2:
-            # (k_,k,o)=(normalized key, key, optional)
-            name_ = f"{name}['{k_}']"
-            if k_ not in object:
-                if o:
-                    continue
-                else:
-                    return f"{name_} is missing"
-            else:
-                ret = self.schema[k].__validate__(object[k_], name=name_, strict=strict)
-                if ret != "":
-                    return ret
-        if strict:
-            for x in object:
-                if x not in self.keys:
-                    return f"{name}['{x}'] is not in the schema"
-        return ""
+        try:
+            object = self.filter(object)
+        except Exception as e:
+            return (
+                f"Applying {self.filter_name} to {name} "
+                f"(value: {_c(object)}) failed: {str(e)}"
+            )
+        name = f"{self.filter_name}({name})"
+        return self.schema.__validate__(object, name, strict)
 
-    def __str__(self):
-        return str(self.schema)
+
+class filter:
+    def __init__(self, filter, schema, filter_name=None):
+        if filter_name is not None and not isinstance(filter_name, str):
+            raise SchemaError("The filter name is not a string")
+        if not callable(filter):
+            raise SchemaError("The filter is not callable")
+        self.filter = filter
+        self.schema = schema
+        self.filter_name = filter_name
+
+    def __compile__(self, _deferred_compiles=None):
+        return _filter(
+            self.filter,
+            self.schema,
+            filter_name=self.filter_name,
+            _deferred_compiles=None,
+        )
 
 
 class _type:
     def __init__(self, schema):
         self.schema = schema
         if isinstance(schema, _GenericAlias):
             raise SchemaError("Parametrized generics are not supported!")
@@ -986,7 +1069,79 @@
             else:
                 return _wrong_type_message(object, name, self.__name__)
         except Exception as e:
             return _wrong_type_message(object, name, self.__name__, str(e))
 
     def __str__(self):
         return str(self.schema)
+
+
+def is_object(obj):
+    return (
+        not callable(obj)
+        and not hasattr(obj, "__validate__")
+        and not hasattr(obj, "__compile__")
+    )
+
+
+class _dict:
+    def __init__(self, schema, _deferred_compiles=None):
+        self.min_keys = set()
+        self.object_keys = set()
+        self.other_keys = set()
+        self.schema = {}
+        for k in schema:
+            compiled_schema = compile(schema[k], _deferred_compiles=_deferred_compiles)
+            optional = True
+            if isinstance(k, optional_key):
+                key = k.key
+            elif isinstance(k, str) and len(k) > 0 and k[-1] == "?":
+                key = k[:-1]
+            else:
+                optional = False
+                key = k
+            c = compile(key, _deferred_compiles=_deferred_compiles)
+            if is_object(key):
+                if not optional:
+                    self.min_keys.add(key)
+                self.object_keys.add(key)
+                self.schema[key] = compiled_schema
+            else:
+                self.other_keys.add(c)
+                self.schema[c] = compiled_schema
+
+    def __validate__(self, object, name, strict):
+        if not isinstance(object, dict):
+            return _wrong_type_message(object, name, "dict")
+
+        for k in self.min_keys:
+            name_ = f"{name}['{k}']"
+            if k not in object:
+                return f"{name_} is missing"
+
+        for k in object:
+            name_ = f"{name}['{k}']"
+            if k in self.object_keys:
+                val = self.schema[k].__validate__(object[k], name=name_, strict=strict)
+                if val != "":
+                    return val
+                continue
+            else:
+                match = False
+                for kk in self.other_keys:
+                    if kk.__validate__(k, name="key", strict=strict) == "":
+                        val = self.schema[kk].__validate__(
+                            object[k], name=name_, strict=strict
+                        )
+                        if val != "":
+                            return val
+                        else:
+                            match = True
+                            break
+                if match:
+                    continue
+            if strict:
+                return f"{name_} is not in the schema"
+        return ""
+
+    def __str__(self):
+        return str(self.schema)
```

