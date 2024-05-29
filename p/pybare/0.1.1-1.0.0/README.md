# Comparing `tmp/pybare-0.1.1.tar.gz` & `tmp/pybare-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybare-0.1.1.tar", last modified: Thu Sep 24 01:43:59 2020, max compression
+gzip compressed data, was "pybare-1.0.0.tar", last modified: Wed May 29 03:23:52 2024, max compression
```

## Comparing `pybare-0.1.1.tar` & `pybare-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-sr-x   0 noah      (1000) noah      (1000)        0 2020-09-24 01:43:59.880000 pybare-0.1.1/
--rw-r--r--   0 noah      (1000) noah      (1000)     4870 2020-09-24 01:43:59.880000 pybare-0.1.1/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)     3383 2020-08-24 03:10:18.000000 pybare-0.1.1/README.md
-drwxr-sr-x   0 noah      (1000) noah      (1000)        0 2020-09-24 01:43:59.880000 pybare-0.1.1/bare/
--rw-r--r--   0 noah      (1000) noah      (1000)      588 2020-08-23 22:31:25.000000 pybare-0.1.1/bare/__init__.py
--rw-r--r--   0 noah      (1000) noah      (1000)    22456 2020-09-11 03:18:48.000000 pybare-0.1.1/bare/encoder.py
--rw-r--r--   0 noah      (1000) noah      (1000)     7791 2020-09-11 03:18:48.000000 pybare-0.1.1/bare/test_encoder.py
--rw-r--r--   0 noah      (1000) noah      (1000)    11076 2020-09-24 01:37:20.000000 pybare-0.1.1/bare/types.py
-drwxr-sr-x   0 noah      (1000) noah      (1000)        0 2020-09-24 01:43:59.880000 pybare-0.1.1/pybare.egg-info/
--rw-r--r--   0 noah      (1000) noah      (1000)     4870 2020-09-24 01:43:59.000000 pybare-0.1.1/pybare.egg-info/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)      206 2020-09-24 01:43:59.000000 pybare-0.1.1/pybare.egg-info/SOURCES.txt
--rw-r--r--   0 noah      (1000) noah      (1000)        1 2020-09-24 01:43:59.000000 pybare-0.1.1/pybare.egg-info/dependency_links.txt
--rw-r--r--   0 noah      (1000) noah      (1000)        5 2020-09-24 01:43:59.000000 pybare-0.1.1/pybare.egg-info/top_level.txt
--rw-r--r--   0 noah      (1000) noah      (1000)       38 2020-09-24 01:43:59.880000 pybare-0.1.1/setup.cfg
--rw-r--r--   0 noah      (1000) noah      (1000)      788 2020-09-24 01:42:35.000000 pybare-0.1.1/setup.py
+drwxr-xr-x   0 noah      (1000) users      (100)        0 2024-05-29 03:23:52.419556 pybare-1.0.0/
+-rw-r--r--   0 noah      (1000) users      (100)     1053 2024-05-24 01:30:00.000000 pybare-1.0.0/LICENSE
+-rw-r--r--   0 noah      (1000) users      (100)     2639 2024-05-29 03:23:52.419556 pybare-1.0.0/PKG-INFO
+-rw-r--r--   0 noah      (1000) users      (100)     2145 2024-05-29 02:02:09.000000 pybare-1.0.0/README.md
+drwxr-xr-x   0 noah      (1000) users      (100)        0 2024-05-29 03:23:52.419556 pybare-1.0.0/bare/
+-rw-r--r--   0 noah      (1000) users      (100)      788 2024-05-29 03:17:56.000000 pybare-1.0.0/bare/__init__.py
+-rw-r--r--   0 noah      (1000) users      (100)     4674 2024-05-29 03:20:16.000000 pybare-1.0.0/bare/barearray.py
+-rw-r--r--   0 noah      (1000) users      (100)     3738 2024-05-29 03:18:36.000000 pybare-1.0.0/bare/barestruct.py
+-rw-r--r--   0 noah      (1000) users      (100)      671 2024-05-29 01:42:58.000000 pybare-1.0.0/bare/baretype.py
+-rw-r--r--   0 noah      (1000) users      (100)     2348 2024-05-29 02:24:31.000000 pybare-1.0.0/bare/data.py
+-rw-r--r--   0 noah      (1000) users      (100)     3565 2024-05-29 03:17:30.000000 pybare-1.0.0/bare/map.py
+-rw-r--r--   0 noah      (1000) users      (100)     3318 2024-05-29 03:14:56.000000 pybare-1.0.0/bare/misc.py
+-rw-r--r--   0 noah      (1000) users      (100)     8788 2024-05-29 03:07:19.000000 pybare-1.0.0/bare/number.py
+-rw-r--r--   0 noah      (1000) users      (100)     8272 2024-05-29 03:20:18.000000 pybare-1.0.0/bare/test_encoder.py
+-rw-r--r--   0 noah      (1000) users      (100)     6175 2024-05-29 03:18:02.000000 pybare-1.0.0/bare/union.py
+-rw-r--r--   0 noah      (1000) users      (100)     1281 2024-05-29 03:17:44.000000 pybare-1.0.0/bare/util.py
+drwxr-xr-x   0 noah      (1000) users      (100)        0 2024-05-29 03:23:52.419556 pybare-1.0.0/pybare.egg-info/
+-rw-r--r--   0 noah      (1000) users      (100)     2639 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/PKG-INFO
+-rw-r--r--   0 noah      (1000) users      (100)      318 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/SOURCES.txt
+-rw-r--r--   0 noah      (1000) users      (100)        1 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/dependency_links.txt
+-rw-r--r--   0 noah      (1000) users      (100)        5 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/top_level.txt
+-rw-r--r--   0 noah      (1000) users      (100)       38 2024-05-29 03:23:52.419556 pybare-1.0.0/setup.cfg
+-rw-r--r--   0 noah      (1000) users      (100)      742 2024-05-29 03:22:55.000000 pybare-1.0.0/setup.py
```

### Comparing `pybare-0.1.1/README.md` & `pybare-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+Metadata-Version: 2.1
+Name: pybare
+Version: 1.0.0
+Summary: A declarative implementation of BARE for Python
+Home-page: https://sr.ht/~chiefnoah/PyBARE/
+Author: Noah Pederson
+Author-email: noah@packetlost.dev
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyBARE
 [![builds.sr.ht status](https://builds.sr.ht/~chiefnoah/pybare.svg)](https://builds.sr.ht/~chiefnoah/pybare?)
 
 An declarative implementation of the [BARE](https://baremessages.org/) message
-format for Python 3.6+
+format for Python 3.11+
 
 ---
 
 pybare is a general purpose library for strongly typed primitives in Python that
 supports serializing to and from BARE messages.
 
 ```shell
@@ -14,102 +29,63 @@
 ```
 
 ## Goals
 
 * Provide a declarative structure for defining types
 * Validation on value updates
 * Support streaming messages
-* Codegen based on `.schema` files
 
 ## Status
 
 pybare fully implements all BARE types for both encoding and decoding. This
 includes reading multiple messages from the same `BinaryIO` stream.
 
 ### TODO
 
-- [  ] Codegen based on `.schema` files
-- [  ] Better documentation
-- [  ] More tests
-- [  ] Fast C implementation for encoding
+- [ ] Codegen based on `.schema` files
+- [ ] Better documentation
+- [ ] More tests
+- [ ] Fast C implementation for encoding
 
 ## Examples
 
 pybare currently requires you define your structures by hand. Examples can be
 found in the
 [tests](https://git.sr.ht/~chiefnoah/pybare/tree/master/bare/test_encoder.py).
 
 ### Quickstart
 
 ```python
-from bare import Struct, Map, Str, UInt, Optional, DataFixed
+from bare import Struct, map, Str, UInt, optional, data, array, Void
 
-# Alternatively, DataFixed(length=64)
-class PubKey(DataFixed):
-    _length = 64 # 512 bits
+# Alternatively, class Data(size=64): ...
+PubKey = data(64) # 512 bits
 
 class User(Struct):
-    username = Str()
-    userid = Int()
-    email = Optional(Str)
-    keys = Map(Str, PubKey)
-    repos = Array(Str) # variable length array
+    username = Filed(Str)
+    userid = Field(Int)
+    email = Field(optional(Str))
+    keys = Field(map(Str, PubKey))
+    repos = Field(array(Str)) # variable length array
 
 
-noah = User(username="chiefnoah", userid=1)
-noah.username == 'chiefnoah' # True
+noah = User(username="chiefnoah", userid=1, email=Void(), keys={}, repos=[])
+noah.username == 'chiefnoah'
 noah.username = 'someoneelse'
-noah.username == 'someoneelse' # True
+noah.username == 'someoneelse'
 noah.userid == 1 # True
 noah.username = 1 # raise: bare.ValidationError
 noah.keys # {} (empty dict)
 noah.keys['my key'] = bytes(64) #\x00\x00...
 noah.keys['oops'] = bytes(1) # raise: bare.ValidationError
-noah.email is None: # True
+noah.email == Void() # True
 noah.email = 12345 # raise: bare.ValidationError
 noah.pack() # \x00\x01 ... (binary data)
 ```
 
-#### 'Magic' values
-
-pybare primitive types (refered to by their baseclass `Field`) and their
-subclasses implement the
-[descriptor protocol](https://docs.python.org/3/howto/descriptor.html) to get
-their 'magic' behavior. When an _instance_ is declared as a _class field_, the
-type can be treated as it's underlying value (ie. `noah.username` is just the
-`str` "chiefnoah" instead of `bare.Str`), while also providing validation and the
-ability to "pack" the values into their corresponding bare primitives.
-
-Note: in order to be treated as `Struct` members, fields _must_ be declared as
-instances, not just their types.
-
-For example:
-
-```python
-class User(Struct):
-    username = Str # this is ignored!
-    email = Str() # this isn't!
-```
-`Struct` and it's subclasses do not implement the descriptor protocol, as they
-are container types. On instances of `Struct`s (or any other object that declares
-a `Field` type as a class field), the underlying value is stored as the class
-field name prefixed with `_`.
-
-Example:
-```python
-u = User(username="noah")
-u.username # "noah"
-u._username # "noah"
-```
-
-You *can* modify this 'internal' value directly to bypass any validation imposed
-by the `Field` type (but why would you want to do that).
-
-Despite all of this, it's generally safe to include functions and other data on
-subclasses of `Field`s. Again, only fields that have been declared on the class
-will be serialized with `pack`.
-
-
+Note, you **must** wrap the desired type in a `Field` to get its 'magic' behavior.
+Class or instance fields that are not wrapped in a `Field` will be ignored by the `pack`
+and `unpack` methods.
 
 ---
 
 To contribute, send patches to [~chiefnoah/inbox@lists.sr.ht](mailto:~chiefnoah/inbox@lists.sr.ht)
```

### Comparing `pybare-0.1.1/bare/test_encoder.py` & `pybare-1.0.0/bare/test_encoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,70 @@
-from .types import *
-
 # TODO: fix import structure, structs should be somewhere else
-from .encoder import Struct, Map, Array, _ValidatedMap, ValidationError, Optional, Union
-from collections import OrderedDict
-import pytest
 import enum
+import inspect
 import io
 import os
-import inspect
+
+import pytest
+
+from bare import (I32, I64, U8, Array, Data, Enum, Field, Int, Map, Str,
+                  Struct, UInt, Union, Void, array, data, map, optional,
+                  union, UnionVariant)
 
 
 class Nested(Struct):
-    s = Str()
-    # a = Array(Int(), 3)
+    s = Field(Str)
 
 
 class Example(Struct):
-
-    testint = Int()
-    teststr = Str()
-    testuint = U8()
-    n = Nested()
+    testint = Field(Int)
+    teststr = Field(Str)
+    testuint = Field(U8)
+    n = Field(Nested)
+    # m = Field(Map(Str, UInt))
 
 
 def test_example_struct():
     n = Nested(s="nested")
-    ex = Example(testint=11, teststr="a test", m={"test": 1}, n=n)
+    ex = Example(testint=11, teststr="a test", n=n)
     assert hasattr(ex, "testint")
     assert hasattr(ex, "teststr")
     assert hasattr(ex, "n")
     assert hasattr(ex.n, "s")
     assert ex.testint == 11
     assert ex.teststr == "a test"
     assert ex.n.s == "nested"
     ex2 = Example(testint=12, teststr="another test")
     assert ex2.testint == 12
     assert ex2.teststr == "another test"
     # Check that the values in the original instance haven't been modified
     assert ex.testint == 11
     assert ex.teststr == "a test"
 
-class C():
-    s = Str()
+
+class C:
+    s = Field(Str)
+
 
 def test_assign_value():
     o = C()
     o.s = "some string"
-    assert getattr(o, 's') == 'some string'
-    assert isinstance(inspect.getmembers(C)[-1][1], Str)
-
-class ExampleMap(Map):
-    _keytype = Str
-    _valuetype = Str
+    assert getattr(o, "s") == "some string"
+    # assert isinstance(inspect.getmembers(C)[-1][1], Str)
+    assert C.__dict__["s"].ty is Str
 
 
 class ExampleMapStruct(Struct):
-    m = Map(Str, Int)
-    m2 = Map(Int, Str)
-    m3 = ExampleMap()
+    m = Field(map(Str, Int))
+    m2 = Field(map(Int, Str))
+    m3 = Field(map(Str, Str))
 
 
 def test_map():
-    ex = ExampleMapStruct()
+    ex = ExampleMapStruct(m={}, m2={}, m3={})
     ex.m["test"] = 2
     ex.m2 = {0: "test"}
     ex.m3 = {"test": "test"}
     assert isinstance(ex.m, _ValidatedMap)
     assert isinstance(ex.m2, _ValidatedMap)
     assert isinstance(ex.m3, _ValidatedMap)
     assert ex.m2[0] == "test"
@@ -80,168 +79,170 @@
     map = Map(Str(), Str(), value={"test": "test"})
     assert map.value["test"] == "test"
     map2 = Map(Str, Str)
     map2.value["another"] = "test"
     assert map2.value["another"] == "test"
 
 
+class MyArray(Array, inner=Int):
+    ...
+
 class ArrayTest(Struct):
-    a = Array(Int)
-    n = Array(Nested, length=1)
+    a = Field(MyArray)
+    n = Field(array(Nested, size=1))
 
 
 def test_array_struct():
     ex = ArrayTest()
     ex.a = [1, 2, 3]
     ex.n = [Nested(s="test")]
     assert ex.a == [1, 2, 3]
-    with pytest.raises(ValidationError):
+    with pytest.raises(TypeError):
         ex.a = ["a", "b", "c"]
-    Array(Int).validate([1, 2, 3])
+    array(Int).validate([1, 2, -3])
 
 
 class OptionalStruct(Struct):
-    i = Int()
-    s = Optional(Str)
-    nested = Optional(Nested)
+    i = Field(Int)
+    s = Field(optional(Str))
+    nested = Field(optional(Nested))
 
 
 def test_optional():
-    ex = OptionalStruct(i=1, s=None)
-    assert ex.s is None
-    assert ex.nested is None
-    ex.s = "test"
+    ex = OptionalStruct(i=1, s=Void(), nested=Void())
+    assert ex.s == Void()
+    assert ex.nested == Void()
+    ex.s = Str("test")
     assert ex.s == "test"
-    with pytest.raises(ValidationError):
-        ex.s = 1
-    ex.s = None
-    assert ex.s is None
+    with pytest.raises(TypeError):
+        ex.s = 1  # type: ignore
+    ex.s = Void()
+    assert isinstance(ex.s, Void)
 
     ex.nested = Nested(s="test")
     assert ex.nested.s == "test"
-    with pytest.raises(ValidationError):
+    with pytest.raises(TypeError):
         ex.nested = "test"
 
 
-class ExampleUnion(Union):
-    _members = (Str, Int)
+class ExampleUnion(Union, variants=(Str, Int)):
+    ...
 
 
 class UnionTest(Struct):
-    e = ExampleUnion()
-    b = Union(members=(Str, Int))
-    c = Union(members=(OptionalStruct, ArrayTest))
+    e = Field(ExampleUnion)
+    b = Field(union(Str, Int))
+    c = Field(union(OptionalStruct, ArrayTest))
 
 
 def test_union():
     ex = UnionTest(
-        e=1, b="test", c=ArrayTest(a=[1], n=[Nested(s="s")])
+        e=Int(1), b=Str("test"), c=ArrayTest(a=[1], n=[Nested(s="s")])
     )  # MUST specify values for union types when creating an object
     assert ex.e == 1
-    ex.e = "1"
+    ex.e = Str("1")
     assert ex.e == "1"
-    with pytest.raises(ValidationError):
+    with pytest.raises(TypeError):
         ex.e = {"test": "test"}
-    b = ex.pack()
+    b = io.BytesIO(ex.pack())
     ex2 = UnionTest.unpack(b)
     assert ex.e == ex.e
     assert ex.b == ex.b
-    assert ex.c.a == [1]
-    assert ex.c.n[0].s == "s"
-    assert ex.c.a == [1]
+    assert ex.c.value.a.value == [1]
+    assert ex.c.value.n[0].s == "s"
+    assert ex.c.value.a.value == [1]
 
 
-class EnumTest(enum.Enum):
+class EnumTest(Enum):
     TEST = 0
     TEST2 = 1
 
 
 class EnumTestStruct(Struct):
-    e = Enum(EnumTest)
+    e = Field(EnumTest)
 
 
 def test_enum():
     ex = EnumTestStruct(e=0)
     assert ex.e == 0
-    with pytest.raises(ValidationError):
+    with pytest.raises(TypeError):
         ex.e = 100
 
 
-class PublicKey(DataFixed):
-    _length = 128
+PublicKey = data(128)
 
 
 class Time(Str):
     pass
 
 
-class Department(enum.Enum):
+class Department(Enum):
     ACCOUNTING = 0
     ADMINISTRATION = 1
     CUSTOMER_SERVICE = 2
     DEVELOPMENT = 3
 
     JSMITH = 99
 
 
 class Address(Struct):
-    address = Array(Str, length=4)
-    city = Str()
-    state = Str()
-    country = Str()
+    address = Field(array(Str, size=4))
+    city = Field(Str)
+    state = Field(Str)
+    country = Field(Str)
 
 
 class Order(Struct):
-    orderID = I64()
-    quantity = I32()
+    orderID = Field(I64)
+    quantity = Field(I32)
 
 
 class Customer(Struct):
-    name = Str()
-    email = Str()
-    address = Address()
-    orders = Array(Order)
-    metadata = Map(Str, Data)
+    name = Field(Str)
+    email = Field(Str)
+    address = Field(Address)
+    orders = Field(array(Order))
+    metadata = Field(map(Str, Data))
 
 
 class Employee(Struct):
-    name = Str()
-    email = Str()
-    address = Address()
-    department = Enum(Department)
-    hireDate = Time()
-    publicKey = Optional(PublicKey)
-    metadata = Map(Str, Data)
+    name = Field(Str)
+    email = Field(Str)
+    address = Field(Address)
+    department = Field(Department)
+    hireDate = Field(Time)
+    publicKey = Field(optional(PublicKey))
+    metadata = Field(map(Str, Data))
 
 
 class TerminatedEmployee(Void):
     pass
 
 
-class Person(Union):
-    _members = (Customer, Employee, TerminatedEmployee)
+class Person(Union, variants=(Customer, Employee, TerminatedEmployee)):
+    ...
 
 
 @pytest.mark.parametrize(
     "file", ["customer.bin", "employee.bin", "people.bin", "terminated.bin"]
 )
 def test_people(file):
     with open(os.path.join(os.path.dirname(__file__), "_examples", file), "br") as f:
         people = []
         while True:
             try:
-                p = Person().unpack(f)
+                p = Person.unpack(f)
                 people.append(p)
             except RuntimeError:
                 break
         f.seek(0)
         f = f.read()
         buf = io.BytesIO()
         for person in people:
-            person.pack(buf)
+            buf.write(person.pack())
         assert buf.getvalue() == f
 
 
 def test_varint():
     expected = b"\x18"
     i = Int(value=12)
     assert i.pack() == expected
@@ -268,62 +269,70 @@
     assert s.pack() == b"\x00"
 
 
 @pytest.mark.parametrize(
     "value",
     [
         (
-            Str(value="a test string"),
+            Str("a test string"),
             b"\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67",
         ),
         (
-            Int(value=12345678),
+            Int(12345678),
             b"\x9c\x85\xe3\x0b\x9c\x85\xe3\x0b\x9c\x85\xe3\x0b\x9c\x85\xe3\x0b",
         ),
     ],
 )
 def test_fixed_array(value):
-    a = Array(type=value[0].__class__, length=4, values=[value[0]] * 4)
+    a = array(value[0].__class__, size=4)([value[0]] * 4)
     assert a.pack() == value[1]
 
 
 @pytest.mark.parametrize(
     "value",
     [
         (
-            Str(value="a test string"),
+            Str("a test string"),
             b"\x04\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67",
         ),
-        (Int(value=123456), b"\x04\x80\x89\x0f\x80\x89\x0f\x80\x89\x0f\x80\x89\x0f"),
+        (Int(123456), b"\x04\x80\x89\x0f\x80\x89\x0f\x80\x89\x0f\x80\x89\x0f"),
     ],
 )
 def test_array(value):
-    a = Array(type=value[0].__class__, values=[value[0]] * 4)
+    a = array(value[0].__class__)([value[0]] * 4)
     packed = a.pack()
-    assert a.pack() == value[1]
+    assert bytes(a.pack()) == value[1]
     buf = io.BytesIO(packed)
     unpacked = a.unpack(buf)
-    assert unpacked.to_dict() == a.to_dict()
+    assert unpacked == a
 
 
 class B(Struct):
-    c = Int()
-
+    c = Field(Int)
 
 class X(Struct):
-    a = Str()
-    b = B()
+    a = Field(Str)
+    b = Field(B)
 
 
 def test_struct():
     s = X(a="a test string", b=B(c=12345))
     expected = b"\x0d\x61\x20\x74\x65\x73\x74\x20\x73\x74\x72\x69\x6e\x67\xf2\xc0\x01"
     assert s.pack() == expected
     buf = io.BytesIO(expected)
     unpacked = s.unpack(buf)
-    assert unpacked.to_dict() == s.to_dict()
+    assert unpacked == s
 
 
 def test_map():
     expected = b"\x02\x04\x74\x65\x73\x74\x04\x74\x65\x73\x74\x07\x61\x6e\x6f\x74\x68\x65\x72\x04\x63\x61\x73\x65"
-    m = Map(Str, Str, value={"test": "test", "another": "case"})
+    anon_map = map(Str, Str)
+    m = anon_map({"test": "test", "another": "case"})
     assert m.pack() == expected
+
+def test_union_variant():
+    MyUnion = union(UnionVariant(Str, 2), UInt)
+    x = MyUnion(Str("hello"))
+    fp = io.BytesIO(x.pack())
+    assert fp.getbuffer()[0] == 0x2
+    y = MyUnion.unpack(fp)
+    assert y.value == Str("hello")
```

### Comparing `pybare-0.1.1/setup.py` & `pybare-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybare", # Replace with your own username
-    version="0.1.1",
+    version="1.0.0",
     author="Noah Pederson",
     author_email="noah@packetlost.dev",
     description="A declarative implementation of BARE for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sr.ht/~chiefnoah/PyBARE/",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.11',
 )
```

