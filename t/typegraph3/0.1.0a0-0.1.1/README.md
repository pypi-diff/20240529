# Comparing `tmp/typegraph3-0.1.0a0.tar.gz` & `tmp/typegraph3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph3-0.1.0a0.tar", last modified: Tue May 28 12:41:11 2024, max compression
+gzip compressed data, was "typegraph3-0.1.1.tar", last modified: Wed May 29 10:37:25 2024, max compression
```

## Comparing `typegraph3-0.1.0a0.tar` & `typegraph3-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     4887 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/README.md
--rw-r--r--   0        0        0      517 2024-05-28 12:41:11.222243 typegraph3-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      111 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/src/typegraph/__init__.py
--rw-r--r--   0        0        0    21661 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/src/typegraph/core.py
--rw-r--r--   0        0        0     3302 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/src/typegraph/type_utils.py
--rw-r--r--   0        0        0        0 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0    13207 2024-05-28 12:40:53.074265 typegraph3-0.1.0a0/tests/test_switch.py
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 typegraph3-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-29 10:37:12.909791 typegraph3-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6326 2024-05-29 10:37:12.909791 typegraph3-0.1.1/README.md
+-rw-r--r--   0        0        0      512 2024-05-29 10:37:25.121916 typegraph3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-05-29 10:37:12.909791 typegraph3-0.1.1/src/typegraph/__init__.py
+-rw-r--r--   0        0        0    24100 2024-05-29 10:37:12.909791 typegraph3-0.1.1/src/typegraph/core.py
+-rw-r--r--   0        0        0     4416 2024-05-29 10:37:12.909791 typegraph3-0.1.1/src/typegraph/type_utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:37:12.909791 typegraph3-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    16886 2024-05-29 10:37:12.909791 typegraph3-0.1.1/tests/test_switch.py
+-rw-r--r--   0        0        0     6625 1970-01-01 00:00:00.000000 typegraph3-0.1.1/PKG-INFO
```

### Comparing `typegraph3-0.1.0a0/LICENSE` & `typegraph3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typegraph3-0.1.0a0/README.md` & `typegraph3-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,62 @@
+<div align="center">
+
 # TypeGraph
 
-## 概述
-**TypeGraph** 是一个 Python 库，用于在不同类型之间进行类型转换，包括自定义类型、内置类型和结构类型（如列表、集合和字典）。它支持同步和异步的转换方法。
+_**TypeGraph** is a Python library designed for type conversion between various types, including custom types, built-in types, and structural types (such as lists, sets, and dictionaries). It supports both synchronous and asynchronous conversion methods._
+
+> 人间总有一两风，填我十万八千梦
+
+ [![CodeFactor](https://www.codefactor.io/repository/github/luxuncang/typegraph/badge)](https://www.codefactor.io/repository/github/luxuncang/typegraph)
+ [![GitHub](https://img.shields.io/github/license/luxuncang/typegraph)](https://github.com/luxuncang/typegraph/blob/master/LICENSE)
+ [![CodeQL](https://github.com/luxuncang/typegraph/workflows/CodeQL/badge.svg)](https://github.com/luxuncang/typegraph/blob/master/.github/workflows/codeql.yml)
+
+English | [简体中文](./README-zh.md)
 
-## 功能
-- 注册同步和异步函数的类型转换器。
-- 根据类型注解自动转换函数参数。
-- 支持子类、联合类型和结构类型的转换。
-- 使用 mermaid 语法可视化转换图。
+</div>
 
-## 安装
-使用以下命令安装运行该库所需的依赖项：
+## Features
+- Register type converters for synchronous and asynchronous functions.
+- Automatically convert function arguments based on type annotations.
+- Support for subclass, union types, and structural types conversion.
+- Visualize the conversion graph using mermaid syntax.
+
+## Installation
+Install the required dependencies with the following command:
 
 ```sh
 pip install typegraph3
 ```
 
-## 入门指南
+Or
 
-### 示例：同步转换器
-注册同步转换器并使用：
+```sh
+pdm add typegraph3
+```
+
+## Getting Started
+
+### Example: Synchronous Converter
+Register and use a synchronous converter:
 
 ```python
 from typegraph import TypeConverter
 
 converter = TypeConverter()
 
 @converter.register_converter(int, str)
 def int_to_str(value: int) -> str:
     return str(value)
 
 result = converter.convert(10, str)  # "10"
 print(result)
 ```
 
-### 示例：异步转换器
-注册异步转换器并使用：
+### Example: Asynchronous Converter
+Register and use an asynchronous converter:
 
 ```python
 import asyncio
 from typegraph import TypeConverter
 
 converter = TypeConverter()
 
@@ -50,45 +67,64 @@
 async def test_async_conversion():
     result = await converter.async_convert("10", int)  # 10
     print(result)
 
 asyncio.run(test_async_conversion())
 ```
 
-### 实例：协议类型
+### Example: Protocol Types
 
 ```python
-from typing import Protocol
+from typing import Protocol, TypedDict, runtime_checkable
 from dataclasses import dataclass
 
 from typegraph import TypeConverter
 
 t = TypeConverter()
 
 class Person(Protocol):
     name: str
     phone: str
     address: str
 
+    def get_name(self) -> str:
+        ...
+
+class PersonDict(TypedDict):
+    name: str
+    phone: str
+    address: str
+
 class A:
     name: str
     phone: str
     address: str
 
     def __init__(self, name: str, phone: str, address: str):
         self.name = name
         self.phone = phone
         self.address = address
 
+    def get_name(self) -> str:
+        return self.name
+
 @dataclass
 class B:
     name: str
     phone: str
     address: str
 
+@t.register_converter(dict, PersonDict)
+def convert_dict_to_persondict(data: dict):
+    return PersonDict(
+        name=data["name"],
+        phone=data["phone"],
+        address=data["address"]
+    )
+
 @t.register_converter(Person, str)
 def convert_person_to_str(data: Person):
     return f"{data.name} {data.phone} {data.address}"
 
 @t.register_converter(dict, A)
 def convert_dict_to_a(data: dict):
     return A(data["name"], data["phone"], data["address"])
@@ -99,34 +135,47 @@
 
 @t.auto_convert()
 def test(a: str):
     return a
 
 d = {"name": "John", "phone": "123", "address": "123"}
 
-t.convert(d, A, debug=True)
 ```
 
+`t.show_mermaid_graph()`
+
 ```mermaid
 graph TD;
+dict-->PersonDict
+dict-->A
+dict-->B
 Person-->str
+```
+
+`t.show_mermaid_graph(protocol=True)`
+
+```mermaid
+graph TD;
+dict-->PersonDict
 dict-->A
 dict-->B
+Person-->str
+A-.->Person
 ```
 
 ```bash
-Converting dict[str, str] to <class '__main__.A'> using [<class 'dict'>, <class '__main__.A'>], <function convert_dict_to_a at 0x7f66025cc040>
+Converting dict[str, str] to <class 'str'> using [<class 'dict'>, <class '__main__.A'>, <class '__main__.Person'>, <class 'str'>], <function TypeConverter.get_converter.<locals>.<lambda>.<locals>.<lambda> at 0x7fb9c8a948b0>
 
-<__main__.A at 0x7f6602841e10>
+'John 123 123'
 ```
 
-### 自动转换装饰器
-根据类型注解自动转换函数参数：
+### Auto-Convert Decorator
+Automatically convert function arguments based on type annotations:
 
-#### 同步
+#### Synchronous
 
 ```python
 from typegraph import TypeConverter
 
 converter = TypeConverter()
 
 @converter.register_converter(str, int)
@@ -137,15 +186,15 @@
 def add_one(x: int) -> int:
     return x + 1
 
 result = add_one("10")  # 11
 print(result)
 ```
 
-#### 异步
+#### Asynchronous
 
 ```python
 from typegraph import TypeConverter
 import asyncio
 
 converter = TypeConverter()
 
@@ -160,31 +209,31 @@
 async def test_async():
     result = await add_one("10")  # 11
     print(result)
 
 asyncio.run(test_async())
 ```
 
-## 测试
+## Testing
 
-提供了单元测试，以确保库的正确功能。运行测试：
+Unit tests are provided to ensure the library functions correctly. Run the tests:
 
 ```bash
 pytest test_switch.py
 ```
 
-测试覆盖了：
-- 同步转换器的注册与执行。
-- 异步转换器的注册与执行。
-- 转换能力检查。
-- 函数参数的自动转换（同步和异步）。
+Tests cover:
+- Registration and execution of synchronous converters.
+- Registration and execution of asynchronous converters.
+- Conversion capability checks.
+- Automatic conversion of function arguments (both synchronous and asynchronous).
 
-## 可视化
+## Visualization
 
-您可以可视化类型转换图：
+You can visualize the type conversion graph:
 
 ```python
 from typegraph import TypeConverter
 
 t = TypeConverter()
 
 class Test:
@@ -203,39 +252,38 @@
 def B_to_float(input_value):
     return float(input_value.t)
 
 @t.register_converter(float, str)
 async def float_to_str(input_value):
     return str(input_value)
 
-t.show_mermaid_graph()
+t.show_mermaid_graph(subclass=True)
 ```
 
-
 ```mermaid
 graph TD;
 float-->Test
 float-->str
 Test-->float
 TestFloat-.->float
 ```
 
-图将使用 mermaid 语法显示，您可以在线渲染或在支持的环境中（如 Jupyter Notebooks）进行渲染。
+The graph will be displayed using mermaid syntax, which can be rendered online or in supported environments like Jupyter Notebooks.
 
-## 支持的类型
+## Supported Types
 
-- [X] 子类类型 (SubClass type)
-- [X] 联合类型 (Union type)
-- [X] 注解类型 (Annotated type)
-- [X] 结构类型 (Structural type)
-- [X] 协议类型 (Protocol type) (只支持输入类型)
-- [X] 字典类型 (TypedDict type)
-- [ ] 泛型类型 (Generic type)
+- [X] Subclass type
+- [X] Union type
+- [X] Annotated type
+- [X] Structural type
+- [X] Protocol type (input types only)
+- [X] TypedDict type
+- [ ] Generic type
 
-## 许可
-此项目使用 MIT 许可证。
+## License
+This project is licensed under the MIT License.
 
-## 贡献
-欢迎贡献！请提出 issue 或提交 pull request 来进行更改。
+## Contributing
+Contributions are welcome! Please open an issue or submit a pull request for any changes.
 
-## 联系方式
-如果您有任何问题或疑问，请在此仓库中提出 issue。
+## Contact
+If you have any questions or concerns, please open an issue in this repository.
```

### Comparing `typegraph3-0.1.0a0/pyproject.toml` & `typegraph3-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typegraph3"
-version = "0.1.0alpha"
+version = "0.1.1"
 description = "Type Auto Switch"
 authors = [
     { name = "luxuncang", email = "luxuncang@qq.com" },
 ]
 dependencies = [
     "typing-inspect>=0.9.0",
     "networkx>=3.3",
```

### Comparing `typegraph3-0.1.0a0/src/typegraph/core.py` & `typegraph3-0.1.1/src/typegraph/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,52 +24,88 @@
 
 import networkx as nx
 from typing_extensions import get_args, get_origin
 from typing_inspect import is_union_type, is_typevar, get_generic_type
 from typeguard import check_type, TypeCheckError, CollectionCheckStrategy
 
 
-from .type_utils import get_origin as get_real_origin, is_structural_type, deep_type
+from .type_utils import (
+    get_origin as get_real_origin,
+    is_structural_type,
+    deep_type,
+    is_protocol_type,
+    check_protocol_type,
+)
 
 
 T = TypeVar("T")
 In = TypeVar("In", contravariant=True)
 Out = TypeVar("Out")
 P = ParamSpec("P")
 
 
-def get_all_subclasses(cls):
-    if hasattr(cls, "__subclasses__"):
-        for subclass in cls.__subclasses__():
-            yield subclass
-            yield from get_all_subclasses(subclass)
-
-
 def generate_type(generic: Type[Any], instance: List[Type[Any]]):
     if types.UnionType == generic:
         return Union[tuple(instance)]  # type: ignore
     return generic[tuple(instance)]
 
 
 class TypeConverter:
     instances: List["TypeConverter"] = []
 
     def __init__(self):
         self.G = nx.DiGraph()
-        self.vG = nx.DiGraph()
-        self.gG = nx.DiGraph()
+        self.sG = nx.DiGraph()
+        self.pG = nx.DiGraph()
+        self.pmG = nx.DiGraph()
         TypeConverter.instances.append(self)
 
+    def get_graph(self, sub_class: bool = False, protocol: bool = False):
+        if sub_class and protocol:
+            return nx.compose_all([self.G, self.sG, self.pG])
+        elif sub_class:
+            return nx.compose(self.G, self.sG)
+        elif protocol:
+            return nx.compose(self.G, self.pG)
+        return self.G
+
     def _gen_edge(
         self, in_type: Type[In], out_type: Type[Out], converter: Callable[P, Out]
     ):
         self.G.add_edge(in_type, out_type, converter=converter, line=True)
-        self.vG.add_edge(in_type, out_type, converter=converter, line=True)
-        for sub_in_type in get_all_subclasses(in_type):
-            self.vG.add_edge(sub_in_type, out_type, converter=converter, line=False)
+        for sub_in_type in self.get_subclass_types(in_type):
+            self.sG.add_edge(
+                sub_in_type,
+                out_type,
+                converter=converter,
+                line=False,
+                metadata={"sub_class": True},
+            )
+        if is_protocol_type(in_type):
+            self.pmG.add_node(in_type)
+        if is_protocol_type(out_type):
+            self.pmG.add_node(out_type)
+        for p_type in self.get_protocol_types(in_type):
+            self.pG.add_edge(
+                in_type,
+                p_type,
+                converter=lambda x: x,
+                line=False,
+                metadata={"protocol": True},
+            )
+        for p_type in self.get_protocol_types(out_type):
+            if out_type == str:
+                print(p_type, in_type, out_type, converter)
+            self.pG.add_edge(
+                out_type,
+                p_type,
+                converter=lambda x: x,
+                line=False,
+                metadata={"protocol": True},
+            )
 
     def register_converter(self, input_type: Type[In], out_type: Type[Out]):
         def decorator(func: Callable[P, T]) -> Callable[P, Out]:
             self._gen_edge(input_type, out_type, func)
             return cast(Callable[P, Out], func)
 
         return decorator
@@ -78,148 +114,115 @@
         def decorator(func: Callable[P, Awaitable[Out]]):
             self._gen_edge(input_type, out_type, func)
             return func
 
         return decorator
 
     def can_convert(
-        self, in_type: Type[In], out_type: Type[Out], full: bool = False
+        self, in_type: Type[In], out_type: Type[Out], sub_class=False, protocol=False
     ) -> bool:
         try:
-            if full:
-                nx.has_path(self.vG, in_type, out_type)
-            else:
-                nx.has_path(self.G, in_type, out_type)
+            nx.has_path(
+                self.get_graph(sub_class=sub_class, protocol=protocol),
+                in_type,
+                out_type,
+            )
             res = True
         except nx.NodeNotFound:
             res = False
         return res
 
-    def get_protocol_type(
-        self,
-        input_value,
-        sub_class: bool = False,
-    ):
-        nodes = set()
-
-        if sub_class:
-            for edge in self.vG.edges():
-                if edge[0] in nodes:
-                    continue
-                nodes.add(edge[0])
-                try:
-                    check_type(
-                        input_value,
-                        edge[0],
-                        collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
-                    )
-                except TypeCheckError:
-                    continue
-                yield edge[0]
-        else:
-            for edge in self.G.edges():
-                if edge[0] in nodes:
-                    continue
-                nodes.add(edge[0])
-                try:
-                    check_type(
-                        input_value,
-                        edge[0],
-                        collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
-                    )
-                except TypeCheckError:
-                    continue
-                yield edge[0]
-
     def get_converter(
         self,
         in_type: Type[In],
         out_type: Type[Out],
-        sub_class: bool = False,
+        sub_class=False,
+        protocol=False,
         input_value: Any = None,
     ):
         """
         [X] SubClass type
         [X] Union type
         [X] Annotated type
         [X] Structural type
         [ ] Generic type
         """
 
-        if self.can_convert(in_type, out_type, full=sub_class):
+        for path, converters in self.get_all_paths(
+            in_type, out_type, sub_class=sub_class, protocol=protocol
+        ):
+            func = reduce(lambda f, g: lambda x: g(f(x)), converters)
+            yield path, func
+        for p_type in self.get_protocol_types_by_value(
+            input_value, sub_class=sub_class, protocol=protocol
+        ):
             for path, converters in self.get_all_paths(
-                in_type, out_type, full=sub_class
+                p_type, out_type, sub_class=sub_class, protocol=protocol
             ):
                 func = reduce(lambda f, g: lambda x: g(f(x)), converters)
                 yield path, func
-        for p_type in self.get_protocol_type(input_value, sub_class=sub_class):
-            if self.can_convert(p_type, out_type, full=sub_class):
+        if is_union_type(out_type):
+            for out_type in get_args(out_type):
                 for path, converters in self.get_all_paths(
-                    p_type, out_type, full=sub_class
+                    in_type, out_type, sub_class=sub_class, protocol=protocol
                 ):
                     func = reduce(lambda f, g: lambda x: g(f(x)), converters)
                     yield path, func
-        if is_union_type(out_type):
-            for out_type in get_args(out_type):
-                if self.can_convert(in_type, out_type, full=sub_class):
+                for p_type in self.get_protocol_types_by_value(
+                    input_value, sub_class=sub_class, protocol=protocol
+                ):
                     for path, converters in self.get_all_paths(
-                        in_type, out_type, full=sub_class
+                        p_type, out_type, sub_class=sub_class, protocol=protocol
                     ):
                         func = reduce(lambda f, g: lambda x: g(f(x)), converters)
                         yield path, func
-                for p_type in self.get_protocol_type(input_value, sub_class=sub_class):
-                    if self.can_convert(p_type, out_type, full=sub_class):
-                        for path, converters in self.get_all_paths(
-                            p_type, out_type, full=sub_class
-                        ):
-                            func = reduce(lambda f, g: lambda x: g(f(x)), converters)
-                            yield path, func
 
     async def async_get_converter(
         self,
         in_type: Type[In],
         out_type: Type[Out],
         sub_class: bool = False,
+        protocol: bool = False,
         input_value=None,
     ):
         def async_wrapper(converters):
             async def async_converter(input_value):
                 for converter in converters:
                     if inspect.iscoroutinefunction(converter):
                         input_value = await converter(input_value)
                     else:
                         input_value = converter(input_value)
                 return input_value
 
             return async_converter
 
-        if self.can_convert(in_type, out_type, full=sub_class):
+        for path, converters in self.get_all_paths(
+            in_type, out_type, sub_class=sub_class, protocol=protocol
+        ):
+            yield path, async_wrapper(converters)
+        for p_type in self.get_protocol_types_by_value(
+            input_value, sub_class=sub_class, protocol=protocol
+        ):
             for path, converters in self.get_all_paths(
-                in_type, out_type, full=sub_class
+                p_type, out_type, sub_class=sub_class, protocol=protocol
             ):
                 yield path, async_wrapper(converters)
-        for p_type in self.get_protocol_type(input_value, sub_class=sub_class):
-            if self.can_convert(p_type, out_type, full=sub_class):
+        if is_union_type(out_type):
+            for out_type in get_args(out_type):
                 for path, converters in self.get_all_paths(
-                    p_type, out_type, full=sub_class
+                    in_type, out_type, sub_class=sub_class, protocol=protocol
                 ):
                     yield path, async_wrapper(converters)
-        if is_union_type(out_type):
-            for out_type in get_args(out_type):
-                if self.can_convert(in_type, out_type, full=sub_class):
+                for p_type in self.get_protocol_types_by_value(
+                    input_value, sub_class=sub_class
+                ):
                     for path, converters in self.get_all_paths(
-                        in_type, out_type, full=sub_class
+                        p_type, out_type, sub_class=sub_class, protocol=protocol
                     ):
                         yield path, async_wrapper(converters)
-                for p_type in self.get_protocol_type(input_value, sub_class=sub_class):
-                    if self.can_convert(p_type, out_type, full=sub_class):
-                        for path, converters in self.get_all_paths(
-                            p_type, out_type, full=sub_class
-                        ):
-                            yield path, async_wrapper(converters)
 
     def _apply_converters(self, input_value, converters):
         for converter in converters:
             input_value = converter(input_value)
         return input_value
 
     def _get_obj_type(
@@ -230,50 +233,66 @@
         return get_generic_type(obj)
 
     def convert(
         self,
         input_value,
         out_type: Type[Out],
         sub_class: bool = False,
+        protocol: bool = False,
         debug: bool = False,
     ) -> Out:
         input_type = self._get_obj_type(input_value, full=True)
         for sub_input_type in iter_deep_type(input_type):
             all_converters = self.get_converter(
                 sub_input_type,  # type: ignore
                 out_type,
-                sub_class,
-                input_value,
+                sub_class=sub_class,
+                protocol=protocol,
+                input_value=input_value,
             )
             if all_converters is not None:
                 for path, converter in all_converters:
                     try:
                         if debug:
                             print(
                                 f"Converting {sub_input_type} to {out_type} using {path}, {converter}"
                             )
                         return converter(input_value)
                     except Exception:
-                        continue
+                        ...
         if is_structural_type(input_type) and is_structural_type(out_type):
             in_origin = get_origin(input_type)
             out_origin = get_origin(out_type)
             if in_origin == out_origin:
                 out_args = get_args(out_type)
 
                 def _iter_func(item):
                     return self.convert(
-                        item, out_args[0], sub_class=sub_class, debug=debug
+                        item,
+                        out_args[0],
+                        sub_class=sub_class,
+                        protocol=protocol,
+                        debug=debug,
                     )
 
                 def __iter_func_dict(item):
                     k, v = item
                     return self.convert(
-                        k, out_args[0], sub_class=sub_class, debug=debug
-                    ), self.convert(v, out_args[1], sub_class=sub_class, debug=debug)
+                        k,
+                        out_args[0],
+                        sub_class=sub_class,
+                        protocol=protocol,
+                        debug=debug,
+                    ), self.convert(
+                        v,
+                        out_args[1],
+                        sub_class=sub_class,
+                        protocol=protocol,
+                        debug=debug,
+                    )
 
                 if in_origin == list or out_origin == List:
                     res = list(map(_iter_func, input_value))
                 elif in_origin == tuple or out_origin == Tuple:
                     res = tuple(map(_iter_func, input_value))
                 elif in_origin == set or out_origin == Set:
                     res = set(map(_iter_func, input_value))
@@ -290,51 +309,65 @@
         raise ValueError(f"No converter registered for {input_type} to {out_type}")
 
     async def async_convert(
         self,
         input_value,
         out_type: Type[Out],
         sub_class: bool = False,
+        protocol: bool = False,
         debug: bool = False,
     ) -> Out:
         input_type = self._get_obj_type(input_value, full=True)
         for sub_input_type in iter_deep_type(input_type):
             all_converters = self.async_get_converter(
-                sub_input_type, # type: ignore
+                sub_input_type,  # type: ignore
                 out_type,
-                sub_class,
-                input_value,
+                sub_class=sub_class,
+                protocol=protocol,
+                input_value=input_value,
             )
             if all_converters is not None:
                 async for path, converter in all_converters:
                     try:
                         if debug:
                             print(
                                 f"Converting {sub_input_type} to {out_type} using {path}, {converter}"
                             )
                         return await converter(input_value)
                     except Exception:
-                        continue
+                        ...
         if is_structural_type(input_type) and is_structural_type(out_type):
             in_origin = get_origin(input_type)
             out_origin = get_origin(out_type)
             if in_origin == out_origin:
                 out_args = get_args(out_type)
 
                 async def _iter_func(item):
                     return await self.async_convert(
-                        item, out_args[0], sub_class=sub_class, debug=debug
+                        item,
+                        out_args[0],
+                        sub_class=sub_class,
+                        protocol=protocol,
+                        debug=debug,
                     )
 
                 async def __iter_func_dict(item):
                     k, v = item
                     return await self.async_convert(
-                        k, out_args[0], sub_class=sub_class, debug=debug
+                        k,
+                        out_args[0],
+                        sub_class=sub_class,
+                        protocol=protocol,
+                        debug=debug,
                     ), await self.async_convert(
-                        v, out_args[1], sub_class=sub_class, debug=debug
+                        v,
+                        out_args[1],
+                        sub_class=sub_class,
+                        protocol=protocol,
+                        debug=debug,
                     )
 
                 if in_origin == list or out_origin == List:
                     res = await asyncio.gather(*map(_iter_func, input_value))
                 elif in_origin == tuple or out_origin == Tuple:
                     res = tuple(await asyncio.gather(*map(_iter_func, input_value)))
                 elif in_origin == set or out_origin == Set:
@@ -349,102 +382,160 @@
                 else:
                     raise ValueError(
                         f"Unsupported structural_type {input_type} to {out_type}"
                     )
                 return cast(Out, res)
         raise ValueError(f"No converter registered for {input_type} to {out_type}")
 
-    def auto_convert(self, sub_class: bool = False, ignore_error: bool = False):
+    def auto_convert(
+        self,
+        sub_class: bool = False,
+        protocol: bool = False,
+        ignore_error: bool = False,
+    ):
         def decorator(func: Callable[P, T]):
             sig = inspect.signature(func)
 
             @wraps(func)
             def wrapper(*args, **kwargs) -> T:
                 bound = sig.bind(*args, **kwargs)
                 for name, value in bound.arguments.items():
                     param = sig.parameters[name]
                     if param.annotation is not inspect.Parameter.empty:
                         try:
                             bound.arguments[name] = self.convert(
-                                value, param.annotation, sub_class=sub_class
+                                value,
+                                param.annotation,
+                                sub_class=sub_class,
+                                protocol=protocol,
                             )
                         except Exception as e:
                             if ignore_error:
                                 continue
                             raise e
                 return func(*bound.args, **bound.kwargs)
 
             return wrapper
 
         return decorator
 
-    def async_auto_convert(self, sub_class: bool = False, ignore_error: bool = False):
+    def async_auto_convert(
+        self,
+        sub_class: bool = False,
+        protocol: bool = False,
+        ignore_error: bool = False,
+    ):
         def decorator(func: Callable[P, Awaitable[T]]):
             sig = inspect.signature(func)
 
             @wraps(func)
             async def wrapper(*args, **kwargs) -> T:
                 bound = sig.bind(*args, **kwargs)
                 for name, value in bound.arguments.items():
                     param = sig.parameters[name]
                     if param.annotation is not inspect.Parameter.empty:
                         try:
                             bound.arguments[name] = await self.async_convert(
-                                value, param.annotation, sub_class=sub_class
+                                value,
+                                param.annotation,
+                                sub_class=sub_class,
+                                protocol=protocol,
                             )
                         except Exception as e:
                             if ignore_error:
                                 continue
                             raise e
                 return await func(*bound.args, **bound.kwargs)
 
             return wrapper
 
         return decorator
 
-    def get_edges(self, full: bool = False):
-        if not full:
-            for edge in self.G.edges(data=True):
-                yield edge
-        else:
-            for edge in self.vG.edges(data=True):
-                yield edge
+    def get_edges(self, sub_class: bool = False, protocol: bool = False):
+        for edge in self.get_graph(sub_class=sub_class, protocol=protocol).edges(
+            data=True
+        ):
+            yield edge
 
-    def show_mermaid_graph(self, full: bool = False):
+    def show_mermaid_graph(self, sub_class: bool = False, protocol: bool = False):
         from IPython.display import display, Markdown
 
         text = "```mermaid\ngraph TD;\n"
-        for edge in self.get_edges(full=full):
+        for edge in self.get_edges(sub_class=sub_class, protocol=protocol):
             line_style = "--" if edge[2]["line"] else "-.-"
             text += f"{edge[0].__name__}{line_style}>{edge[1].__name__}\n"
         text += "```"
 
         display(Markdown(text))
         return text
 
-    def get_all_paths(self, in_type: Type[In], out_type: Type[Out], full: bool = False):
-        if full:
-            G = self.vG
-        else:
-            G = self.G
+    def get_all_paths(
+        self,
+        in_type: Type[In],
+        out_type: Type[Out],
+        sub_class: bool = False,
+        protocol: bool = False,
+    ):
+        G = self.get_graph(sub_class=sub_class, protocol=protocol)
 
-        if self.can_convert(in_type, out_type, full=full):
+        if self.can_convert(in_type, out_type, sub_class=sub_class, protocol=protocol):
             try:
                 for path in nx.shortest_simple_paths(G, in_type, out_type):
                     converters = [
                         G.get_edge_data(path[i], path[i + 1])["converter"]
                         for i in range(len(path) - 1)
                     ]
                     if len(path) == 1 and len(converters) == 0:
                         yield path * 2, [lambda x: x]
                     else:
                         yield path, converters
             except nx.NetworkXNoPath:
                 ...
 
+    def get_subclass_types(self, cls: Type):
+        if hasattr(cls, "__subclasses__"):
+            for subclass in cls.__subclasses__():
+                yield subclass
+                yield from self.get_subclass_types(subclass)
+
+    def get_protocol_types(self, cls: Type, strict: bool = True):
+        nodes = set()
+        for node in list(self.pmG.nodes()):
+            if node in nodes:
+                continue
+            nodes.add(node)
+            try:
+                if not check_protocol_type(cls, node, strict=strict):
+                    continue
+            except TypeError:
+                continue
+            if cls != node:
+                yield node
+
+    def get_protocol_types_by_value(
+        self, input_value, sub_class: bool = False, protocol: bool = False
+    ):
+        nodes = set()
+        G = self.get_graph(sub_class=sub_class, protocol=protocol)
+
+        for edge in G.edges():
+            if edge[0] in nodes:
+                continue
+            nodes.add(edge[0])
+            try:
+                check_type(
+                    input_value,
+                    edge[0],
+                    collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
+                )
+            except TypeCheckError:
+                continue
+            yield edge[0]
+
+
 @dataclass
 class TypeVarModel:
     origin: Any
     args: Optional[List["TypeVarModel" | List["TypeVarModel"]]] = None
 
     def to_dict(self):
         return {
```

### Comparing `typegraph3-0.1.0a0/tests/test_switch.py` & `typegraph3-0.1.1/tests/test_switch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import unittest
 import asyncio
+from typing import Protocol
+
 from typegraph.core import TypeConverter
 
 
 class TypeConverterTests(unittest.TestCase):
     def setUp(self):
         self.converter = TypeConverter()
 
@@ -36,15 +38,15 @@
         self.assertTrue(self.converter.can_convert(int, str))
         self.assertTrue(self.converter.can_convert(str, int))
 
         self.assertFalse(self.converter.can_convert(int, Test))
         self.assertFalse(self.converter.can_convert(Test, int))
 
         self.assertFalse(self.converter.can_convert(Test, str))
-        self.assertTrue(self.converter.can_convert(Test, str, full=True))
+        self.assertTrue(self.converter.can_convert(Test, str, sub_class=True))
 
         self.assertFalse(self.converter.can_convert(str, float | int))
         self.assertFalse(self.converter.can_convert(int, float))
 
     def test_get_converter(self):
         class Test(int): ...
 
@@ -70,26 +72,14 @@
         self.assertEqual(result[0][1](10), "10")
 
         # Test Subclass
         result = list(self.converter.get_converter(Test, str, sub_class=True))
         self.assertEqual(result[0][0], [Test, str])
         self.assertEqual(result[0][1](10), "10")
 
-        # Test Structural
-        # result = list(self.converter.get_converter(list[int], list[float | str]))
-        # self.assertEqual(result[0][0], [int, str])
-        # self.assertEqual(result[0][1]([10]), ["10"])
-
-        # Test Nest Structural
-        # result = list(self.converter.get_converter(list[list[int]], list[list[float | str]]))
-        # print(result)
-        # self.assertEqual(result[0][0], [int, str])
-        # print(result[0][1]([[10]]))
-        # self.assertEqual(result[0][1]([[10]]), [["10"]])
-
     def test_convert(self):
         class Test(int): ...
 
         self.converter.register_converter(int, str)(str)
         self.converter.register_converter(str, int)(int)
 
         result = self.converter.convert(10, str)
@@ -308,14 +298,88 @@
 
         result = test_structural([1, 2, 3])
         self.assertEqual(result, ["1", "2", "3"])
 
         result = test_next_structural([{1: "1"}, {2: "2"}, {3: "3"}])
         self.assertEqual(result, [{'1': 1}, {'2': 2}, {'3': 3}])
 
+    def test_auto_convert_protocol(self):
+        from typing import Protocol, TypedDict
+        from dataclasses import dataclass
+
+        t = self.converter
+
+        class Person(Protocol):
+            name: str
+            phone: str
+            address: str
+
+            def get_name(self) -> str:
+                ...
+
+        class PersonDict(TypedDict):
+            name: str
+            phone: str
+            address: str
+
+        class A:
+            name: str
+            phone: str
+            address: str
+
+            def __init__(self, name: str, phone: str, address: str):
+                self.name = name
+                self.phone = phone
+                self.address = address
+
+            def get_name(self) -> str:
+                return self.name
+
+        @dataclass
+        class B:
+            name: str
+            phone: str
+            address: str
+
+        @t.register_converter(dict, PersonDict)
+        def convert_dict_to_persondict(data: dict):
+            return PersonDict(
+                name=data["name"],
+                phone=data["phone"],
+                address=data["address"]
+            )
+
+        @t.register_converter(Person, str)
+        def convert_person_to_str(data: Person):
+            return f"{data.name} {data.phone} {data.address}"
+
+        @t.register_converter(dict, A)
+        def convert_dict_to_a(data: dict):
+            return A(data["name"], data["phone"], data["address"])
+
+        @t.register_converter(dict, B)
+        def convert_dict_to_b(data: dict):
+            return B(data["name"], data["phone"], data["address"])
+        
+        @t.auto_convert(protocol=True)
+        def test(a: str):
+            return a
+        
+        @t.auto_convert(protocol=True)
+        def tests(a: list[str]):
+            return a
+
+        d = {"name": "John", "phone": "123", "address": "123"}
+
+        result = test(d)
+        self.assertEqual(result, "John 123 123")
+
+        result = tests([d])
+        self.assertEqual(result, ["John 123 123"])
+
     def test_async_auto_convert(self):
         t = self.converter
 
         class Test:
             def __init__(self, t):
                 self.t = t
 
@@ -398,10 +462,86 @@
             self.assertEqual(result, ["1", "2", "3"])
 
             result = await test_next_structural([{1: "1"}, {2: "2"}, {3: "3"}])
             self.assertEqual(result, [{'1': 1}, {'2': 2}, {'3': 3}])
 
         asyncio.run(test_async_conversion())
 
+    def test_async_auto_convert_protocol(self):
+        from typing import Protocol, TypedDict
+        from dataclasses import dataclass
+
+        t = self.converter
+
+        class Person(Protocol):
+            name: str
+            phone: str
+            address: str
+
+            def get_name(self) -> str:
+                ...
+
+        class PersonDict(TypedDict):
+            name: str
+            phone: str
+            address: str
+
+        class A:
+            name: str
+            phone: str
+            address: str
+
+            def __init__(self, name: str, phone: str, address: str):
+                self.name = name
+                self.phone = phone
+                self.address = address
+
+            def get_name(self) -> str:
+                return self.name
+
+        @dataclass
+        class B:
+            name: str
+            phone: str
+            address: str
+
+        @t.register_converter(dict, PersonDict)
+        def convert_dict_to_persondict(data: dict):
+            return PersonDict(
+                name=data["name"],
+                phone=data["phone"],
+                address=data["address"]
+            )
+
+        @t.register_converter(Person, str)
+        def convert_person_to_str(data: Person):
+            return f"{data.name} {data.phone} {data.address}"
+
+        @t.register_converter(dict, A)
+        def convert_dict_to_a(data: dict):
+            return A(data["name"], data["phone"], data["address"])
+
+        @t.register_converter(dict, B)
+        def convert_dict_to_b(data: dict):
+            return B(data["name"], data["phone"], data["address"])
+        
+        @t.auto_convert(protocol=True)
+        async def test(a: str):
+            return a
+        
+        @t.auto_convert(protocol=True)
+        async def tests(a: list[str]):
+            return a
+
+        async def test_async_conversion_protocol():
+            d = {"name": "John", "phone": "123", "address": "123"}
+
+            result = await test(d)
+            self.assertEqual(result, "John 123 123")
+
+            result = await tests([d])
+            self.assertEqual(result, ["John 123 123"])
+
+        asyncio.run(test_async_conversion_protocol())
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `typegraph3-0.1.0a0/PKG-INFO` & `typegraph3-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 Metadata-Version: 2.1
 Name: typegraph3
-Version: 0.1.0a0
+Version: 0.1.1
 Summary: Type Auto Switch
 Author-Email: luxuncang <luxuncang@qq.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: typing-inspect>=0.9.0
 Requires-Dist: networkx>=3.3
 Requires-Dist: typeguard>=4.3.0
 Description-Content-Type: text/markdown
 
+<div align="center">
+
 # TypeGraph
 
-## 概述
-**TypeGraph** 是一个 Python 库，用于在不同类型之间进行类型转换，包括自定义类型、内置类型和结构类型（如列表、集合和字典）。它支持同步和异步的转换方法。
+_**TypeGraph** is a Python library designed for type conversion between various types, including custom types, built-in types, and structural types (such as lists, sets, and dictionaries). It supports both synchronous and asynchronous conversion methods._
+
+> 人间总有一两风，填我十万八千梦
+
+ [![CodeFactor](https://www.codefactor.io/repository/github/luxuncang/typegraph/badge)](https://www.codefactor.io/repository/github/luxuncang/typegraph)
+ [![GitHub](https://img.shields.io/github/license/luxuncang/typegraph)](https://github.com/luxuncang/typegraph/blob/master/LICENSE)
+ [![CodeQL](https://github.com/luxuncang/typegraph/workflows/CodeQL/badge.svg)](https://github.com/luxuncang/typegraph/blob/master/.github/workflows/codeql.yml)
+
+English | [简体中文](./README-zh.md)
 
-## 功能
-- 注册同步和异步函数的类型转换器。
-- 根据类型注解自动转换函数参数。
-- 支持子类、联合类型和结构类型的转换。
-- 使用 mermaid 语法可视化转换图。
+</div>
 
-## 安装
-使用以下命令安装运行该库所需的依赖项：
+## Features
+- Register type converters for synchronous and asynchronous functions.
+- Automatically convert function arguments based on type annotations.
+- Support for subclass, union types, and structural types conversion.
+- Visualize the conversion graph using mermaid syntax.
+
+## Installation
+Install the required dependencies with the following command:
 
 ```sh
 pip install typegraph3
 ```
 
-## 入门指南
+Or
 
-### 示例：同步转换器
-注册同步转换器并使用：
+```sh
+pdm add typegraph3
+```
+
+## Getting Started
+
+### Example: Synchronous Converter
+Register and use a synchronous converter:
 
 ```python
 from typegraph import TypeConverter
 
 converter = TypeConverter()
 
 @converter.register_converter(int, str)
 def int_to_str(value: int) -> str:
     return str(value)
 
 result = converter.convert(10, str)  # "10"
 print(result)
 ```
 
-### 示例：异步转换器
-注册异步转换器并使用：
+### Example: Asynchronous Converter
+Register and use an asynchronous converter:
 
 ```python
 import asyncio
 from typegraph import TypeConverter
 
 converter = TypeConverter()
 
@@ -62,45 +79,64 @@
 async def test_async_conversion():
     result = await converter.async_convert("10", int)  # 10
     print(result)
 
 asyncio.run(test_async_conversion())
 ```
 
-### 实例：协议类型
+### Example: Protocol Types
 
 ```python
-from typing import Protocol
+from typing import Protocol, TypedDict, runtime_checkable
 from dataclasses import dataclass
 
 from typegraph import TypeConverter
 
 t = TypeConverter()
 
 class Person(Protocol):
     name: str
     phone: str
     address: str
 
+    def get_name(self) -> str:
+        ...
+
+class PersonDict(TypedDict):
+    name: str
+    phone: str
+    address: str
+
 class A:
     name: str
     phone: str
     address: str
 
     def __init__(self, name: str, phone: str, address: str):
         self.name = name
         self.phone = phone
         self.address = address
 
+    def get_name(self) -> str:
+        return self.name
+
 @dataclass
 class B:
     name: str
     phone: str
     address: str
 
+@t.register_converter(dict, PersonDict)
+def convert_dict_to_persondict(data: dict):
+    return PersonDict(
+        name=data["name"],
+        phone=data["phone"],
+        address=data["address"]
+    )
+
 @t.register_converter(Person, str)
 def convert_person_to_str(data: Person):
     return f"{data.name} {data.phone} {data.address}"
 
 @t.register_converter(dict, A)
 def convert_dict_to_a(data: dict):
     return A(data["name"], data["phone"], data["address"])
@@ -111,34 +147,47 @@
 
 @t.auto_convert()
 def test(a: str):
     return a
 
 d = {"name": "John", "phone": "123", "address": "123"}
 
-t.convert(d, A, debug=True)
 ```
 
+`t.show_mermaid_graph()`
+
 ```mermaid
 graph TD;
+dict-->PersonDict
+dict-->A
+dict-->B
 Person-->str
+```
+
+`t.show_mermaid_graph(protocol=True)`
+
+```mermaid
+graph TD;
+dict-->PersonDict
 dict-->A
 dict-->B
+Person-->str
+A-.->Person
 ```
 
 ```bash
-Converting dict[str, str] to <class '__main__.A'> using [<class 'dict'>, <class '__main__.A'>], <function convert_dict_to_a at 0x7f66025cc040>
+Converting dict[str, str] to <class 'str'> using [<class 'dict'>, <class '__main__.A'>, <class '__main__.Person'>, <class 'str'>], <function TypeConverter.get_converter.<locals>.<lambda>.<locals>.<lambda> at 0x7fb9c8a948b0>
 
-<__main__.A at 0x7f6602841e10>
+'John 123 123'
 ```
 
-### 自动转换装饰器
-根据类型注解自动转换函数参数：
+### Auto-Convert Decorator
+Automatically convert function arguments based on type annotations:
 
-#### 同步
+#### Synchronous
 
 ```python
 from typegraph import TypeConverter
 
 converter = TypeConverter()
 
 @converter.register_converter(str, int)
@@ -149,15 +198,15 @@
 def add_one(x: int) -> int:
     return x + 1
 
 result = add_one("10")  # 11
 print(result)
 ```
 
-#### 异步
+#### Asynchronous
 
 ```python
 from typegraph import TypeConverter
 import asyncio
 
 converter = TypeConverter()
 
@@ -172,31 +221,31 @@
 async def test_async():
     result = await add_one("10")  # 11
     print(result)
 
 asyncio.run(test_async())
 ```
 
-## 测试
+## Testing
 
-提供了单元测试，以确保库的正确功能。运行测试：
+Unit tests are provided to ensure the library functions correctly. Run the tests:
 
 ```bash
 pytest test_switch.py
 ```
 
-测试覆盖了：
-- 同步转换器的注册与执行。
-- 异步转换器的注册与执行。
-- 转换能力检查。
-- 函数参数的自动转换（同步和异步）。
+Tests cover:
+- Registration and execution of synchronous converters.
+- Registration and execution of asynchronous converters.
+- Conversion capability checks.
+- Automatic conversion of function arguments (both synchronous and asynchronous).
 
-## 可视化
+## Visualization
 
-您可以可视化类型转换图：
+You can visualize the type conversion graph:
 
 ```python
 from typegraph import TypeConverter
 
 t = TypeConverter()
 
 class Test:
@@ -215,39 +264,38 @@
 def B_to_float(input_value):
     return float(input_value.t)
 
 @t.register_converter(float, str)
 async def float_to_str(input_value):
     return str(input_value)
 
-t.show_mermaid_graph()
+t.show_mermaid_graph(subclass=True)
 ```
 
-
 ```mermaid
 graph TD;
 float-->Test
 float-->str
 Test-->float
 TestFloat-.->float
 ```
 
-图将使用 mermaid 语法显示，您可以在线渲染或在支持的环境中（如 Jupyter Notebooks）进行渲染。
+The graph will be displayed using mermaid syntax, which can be rendered online or in supported environments like Jupyter Notebooks.
 
-## 支持的类型
+## Supported Types
 
-- [X] 子类类型 (SubClass type)
-- [X] 联合类型 (Union type)
-- [X] 注解类型 (Annotated type)
-- [X] 结构类型 (Structural type)
-- [X] 协议类型 (Protocol type) (只支持输入类型)
-- [X] 字典类型 (TypedDict type)
-- [ ] 泛型类型 (Generic type)
+- [X] Subclass type
+- [X] Union type
+- [X] Annotated type
+- [X] Structural type
+- [X] Protocol type (input types only)
+- [X] TypedDict type
+- [ ] Generic type
 
-## 许可
-此项目使用 MIT 许可证。
+## License
+This project is licensed under the MIT License.
 
-## 贡献
-欢迎贡献！请提出 issue 或提交 pull request 来进行更改。
+## Contributing
+Contributions are welcome! Please open an issue or submit a pull request for any changes.
 
-## 联系方式
-如果您有任何问题或疑问，请在此仓库中提出 issue。
+## Contact
+If you have any questions or concerns, please open an issue in this repository.
```

