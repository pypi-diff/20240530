# Comparing `tmp/typegraph3-0.1.1.tar.gz` & `tmp/typegraph3-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph3-0.1.1.tar", last modified: Wed May 29 10:37:25 2024, max compression
+gzip compressed data, was "typegraph3-0.1.2rc1.tar", last modified: Thu May 30 12:52:29 2024, max compression
```

## Comparing `typegraph3-0.1.1.tar` & `typegraph3-0.1.2rc1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-05-29 10:37:12.909791 typegraph3-0.1.1/LICENSE
--rw-r--r--   0        0        0     6326 2024-05-29 10:37:12.909791 typegraph3-0.1.1/README.md
--rw-r--r--   0        0        0      512 2024-05-29 10:37:25.121916 typegraph3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      111 2024-05-29 10:37:12.909791 typegraph3-0.1.1/src/typegraph/__init__.py
--rw-r--r--   0        0        0    24100 2024-05-29 10:37:12.909791 typegraph3-0.1.1/src/typegraph/core.py
--rw-r--r--   0        0        0     4416 2024-05-29 10:37:12.909791 typegraph3-0.1.1/src/typegraph/type_utils.py
--rw-r--r--   0        0        0        0 2024-05-29 10:37:12.909791 typegraph3-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0    16886 2024-05-29 10:37:12.909791 typegraph3-0.1.1/tests/test_switch.py
--rw-r--r--   0        0        0     6625 1970-01-01 00:00:00.000000 typegraph3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/LICENSE
+-rw-r--r--   0        0        0     6378 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/README.md
+-rw-r--r--   0        0        0      515 2024-05-30 12:52:29.061537 typegraph3-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/converter/__init__.py
+-rw-r--r--   0        0        0    20373 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/converter/base.py
+-rw-r--r--   0        0        0     7807 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/converter/typevar.py
+-rw-r--r--   0        0        0     4916 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/type_utils.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/tests/__init__.py
+-rw-r--r--   0        0        0    17209 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/tests/test_switch.py
+-rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 typegraph3-0.1.2rc1/PKG-INFO
```

### Comparing `typegraph3-0.1.1/LICENSE` & `typegraph3-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `typegraph3-0.1.1/README.md` & `typegraph3-0.1.2rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 
 # TypeGraph
 
 _**TypeGraph** is a Python library designed for type conversion between various types, including custom types, built-in types, and structural types (such as lists, sets, and dictionaries). It supports both synchronous and asynchronous conversion methods._
 
-> 人间总有一两风，填我十万八千梦
+> 蓦然回首，那人却在灯火阑珊处
 
  [![CodeFactor](https://www.codefactor.io/repository/github/luxuncang/typegraph/badge)](https://www.codefactor.io/repository/github/luxuncang/typegraph)
  [![GitHub](https://img.shields.io/github/license/luxuncang/typegraph)](https://github.com/luxuncang/typegraph/blob/master/LICENSE)
  [![CodeQL](https://github.com/luxuncang/typegraph/workflows/CodeQL/badge.svg)](https://github.com/luxuncang/typegraph/blob/master/.github/workflows/codeql.yml)
 
 English | [简体中文](./README-zh.md)
 
@@ -135,14 +135,15 @@
 
 @t.auto_convert()
 def test(a: str):
     return a
 
 d = {"name": "John", "phone": "123", "address": "123"}
 
+t.convert([d], list[str], debug=True, protocol=True)
 ```
 
 `t.show_mermaid_graph()`
 
 ```mermaid
 graph TD;
 dict-->PersonDict
@@ -159,17 +160,17 @@
 dict-->A
 dict-->B
 Person-->str
 A-.->Person
 ```
 
 ```bash
-Converting dict[str, str] to <class 'str'> using [<class 'dict'>, <class '__main__.A'>, <class '__main__.Person'>, <class 'str'>], <function TypeConverter.get_converter.<locals>.<lambda>.<locals>.<lambda> at 0x7fb9c8a948b0>
+Converting dict[str, str] to <class 'str'> using [<class 'dict'>, <class '__main__.A'>, <class '__main__.Person'>, <class 'str'>], <function TypeConverter.get_converter.<locals>.<lambda>.<locals>.<lambda> at 0x7f1f3306fac0>
 
-'John 123 123'
+['John 123 123']
 ```
 
 ### Auto-Convert Decorator
 Automatically convert function arguments based on type annotations:
 
 #### Synchronous
 
@@ -273,15 +274,15 @@
 
 - [X] Subclass type
 - [X] Union type
 - [X] Annotated type
 - [X] Structural type
 - [X] Protocol type (input types only)
 - [X] TypedDict type
-- [ ] Generic type
+- [X] Generic type
 
 ## License
 This project is licensed under the MIT License.
 
 ## Contributing
 Contributions are welcome! Please open an issue or submit a pull request for any changes.
```

### Comparing `typegraph3-0.1.1/pyproject.toml` & `typegraph3-0.1.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typegraph3"
-version = "0.1.1"
+version = "0.1.2rc1"
 description = "Type Auto Switch"
 authors = [
     { name = "luxuncang", email = "luxuncang@qq.com" },
 ]
 dependencies = [
     "typing-inspect>=0.9.0",
     "networkx>=3.3",
```

### Comparing `typegraph3-0.1.1/src/typegraph/type_utils.py` & `typegraph3-0.1.2rc1/src/typegraph/type_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 import types
 import typing
-import inspect
 
 from typing import (
-    TypeVar,
-    Generic,
     Union,
-    Annotated,
     List,
-    Dict,
     Callable,
     Any,
     runtime_checkable,
-    Protocol,
     Type,
 )
 from typing_extensions import get_type_hints
-from typing_inspect import is_generic_type, get_generic_type
+from typing_inspect import get_generic_type
 
 
 def get_origin(tp):
     """Get the unsubscripted version of a type.
 
     This supports generic types, Callable, Tuple, Union, Literal, Final, ClassVar
     and Annotated. Return None for unsupported types. Examples::
@@ -39,15 +33,15 @@
     if isinstance(tp, typing._GenericAlias):  # type: ignore
         if isinstance(tp._name, str) and getattr(typing, tp._name, None):
             return getattr(typing, tp._name)
         return tp.__origin__
     if isinstance(
         tp,
         (
-            typing._BaseGenericAlias,
+            typing._BaseGenericAlias, # type: ignore
             typing.GenericAlias,  # type: ignore
             typing.ParamSpecArgs,
             typing.ParamSpecKwargs,
         ),
     ):
         return tp.__origin__
     if tp is typing.Generic:
@@ -139,7 +133,26 @@
 
 def check_protocol_type(tp, expected_type, *, strict: bool = True):
     if not is_protocol_type(expected_type):
         raise TypeError(f"{expected_type} is not a protocol type")
     if strict:
         return attribute_check(tp, expected_type) and method_check(tp, expected_type)
     return issubclass(tp, runtime_checkable(expected_type))
+
+
+def generate_type(generic: Type[Any], instance: List[Type[Any]]):
+    if types.UnionType == generic:
+        return Union[tuple(instance)]  # type: ignore
+    elif Callable == generic:
+        if len(instance) == 2:
+            return generic[instance[0], instance[1]]
+        return generic
+    elif len(instance) == 0:
+        return generic
+    return generic[tuple(instance)]
+
+
+def get_subclass_types(cls: Type):
+    if hasattr(cls, "__subclasses__"):
+        for subclass in cls.__subclasses__():
+            yield subclass
+            yield from get_subclass_types(subclass)
```

### Comparing `typegraph3-0.1.1/tests/test_switch.py` & `typegraph3-0.1.2rc1/tests/test_switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from __future__ import annotations
+
 import unittest
 import asyncio
-from typing import Protocol
+from typing import TypeVar
+
+from typegraph.converter.base import TypeConverter
 
-from typegraph.core import TypeConverter
+K = TypeVar("K")
+V = TypeVar("V")
 
 
 class TypeConverterTests(unittest.TestCase):
     def setUp(self):
         self.converter = TypeConverter()
 
     def test_register_converter(self):
@@ -220,14 +225,18 @@
 
         class Test:
             def __init__(self, t):
                 self.t = t
 
         class Test2(int): ...
 
+        class Test3: ...
+
+        class Test4: ...
+
         @t.register_converter(str, int)
         def str_to_int(input_value):
             return int(input_value)
 
         @t.register_converter(int, str)
         def int_to_str(input_value):
             return str(input_value)
@@ -250,15 +259,19 @@
         def Test_to_float(input_value):
             return float(input_value.t)
 
         @t.register_converter(str, float)
         def str_to_float(input_value):
             return float(input_value)
 
-        @self.converter.auto_convert()
+        @self.converter.async_register_converter(dict[K,V], dict[V,K])
+        async def reverse_dict(d: dict[K,V]) -> dict[V,K]:
+            return {v: k for k, v in d.items()}
+
+        @self.converter.auto_convert(localns=locals())
         def test_float_to_str(x: Test):
             return x.t
 
         @self.converter.auto_convert(sub_class=True)
         def test_switch(x: str):
             return x
 
@@ -270,18 +283,22 @@
         def test_union(x: list | float):
             return x
 
         @self.converter.auto_convert(sub_class=True)
         def test_structural(x: list[str]):
             return x
 
-        @self.converter.auto_convert(sub_class=True)
+        @self.converter.auto_convert()
         def test_next_structural(x: list[dict[str, int]]):
             return x
 
+        @self.converter.auto_convert()
+        def test_structural_dict(x: list[dict[str, int]]):
+            return x
+
         result = test_float_to_str("10")
         self.assertEqual(result, "10")
 
         result = test_switch(Test("10.0"))
         self.assertEqual(result, "10.0")
 
         result = add_one(10)
@@ -298,27 +315,27 @@
 
         result = test_structural([1, 2, 3])
         self.assertEqual(result, ["1", "2", "3"])
 
         result = test_next_structural([{1: "1"}, {2: "2"}, {3: "3"}])
         self.assertEqual(result, [{'1': 1}, {'2': 2}, {'3': 3}])
 
+
     def test_auto_convert_protocol(self):
         from typing import Protocol, TypedDict
         from dataclasses import dataclass
 
         t = self.converter
 
         class Person(Protocol):
             name: str
             phone: str
             address: str
 
-            def get_name(self) -> str:
-                ...
+            def get_name(self) -> str: ...
 
         class PersonDict(TypedDict):
             name: str
             phone: str
             address: str
 
         class A:
@@ -339,35 +356,33 @@
             name: str
             phone: str
             address: str
 
         @t.register_converter(dict, PersonDict)
         def convert_dict_to_persondict(data: dict):
             return PersonDict(
-                name=data["name"],
-                phone=data["phone"],
-                address=data["address"]
+                name=data["name"], phone=data["phone"], address=data["address"]
             )
 
         @t.register_converter(Person, str)
         def convert_person_to_str(data: Person):
             return f"{data.name} {data.phone} {data.address}"
 
         @t.register_converter(dict, A)
         def convert_dict_to_a(data: dict):
             return A(data["name"], data["phone"], data["address"])
 
         @t.register_converter(dict, B)
         def convert_dict_to_b(data: dict):
             return B(data["name"], data["phone"], data["address"])
-        
+
         @t.auto_convert(protocol=True)
         def test(a: str):
             return a
-        
+
         @t.auto_convert(protocol=True)
         def tests(a: list[str]):
             return a
 
         d = {"name": "John", "phone": "123", "address": "123"}
 
         result = test(d)
@@ -411,15 +426,15 @@
         def Test_to_float(input_value):
             return float(input_value.t)
 
         @t.register_converter(str, float)
         def str_to_float(input_value):
             return float(input_value)
 
-        @self.converter.async_auto_convert()
+        @self.converter.async_auto_convert(localns=locals())
         async def test_float_to_str(x: Test):
             return x.t
 
         @self.converter.async_auto_convert(sub_class=True)
         async def test_switch(x: str):
             return x
 
@@ -458,31 +473,30 @@
             result = await test_switch(Test2(10))
             self.assertEqual(result, "10")
 
             result = await test_structural([1, 2, 3])
             self.assertEqual(result, ["1", "2", "3"])
 
             result = await test_next_structural([{1: "1"}, {2: "2"}, {3: "3"}])
-            self.assertEqual(result, [{'1': 1}, {'2': 2}, {'3': 3}])
+            self.assertEqual(result, [{"1": 1}, {"2": 2}, {"3": 3}])
 
         asyncio.run(test_async_conversion())
 
     def test_async_auto_convert_protocol(self):
         from typing import Protocol, TypedDict
         from dataclasses import dataclass
 
         t = self.converter
 
         class Person(Protocol):
             name: str
             phone: str
             address: str
 
-            def get_name(self) -> str:
-                ...
+            def get_name(self) -> str: ...
 
         class PersonDict(TypedDict):
             name: str
             phone: str
             address: str
 
         class A:
@@ -503,35 +517,33 @@
             name: str
             phone: str
             address: str
 
         @t.register_converter(dict, PersonDict)
         def convert_dict_to_persondict(data: dict):
             return PersonDict(
-                name=data["name"],
-                phone=data["phone"],
-                address=data["address"]
+                name=data["name"], phone=data["phone"], address=data["address"]
             )
 
         @t.register_converter(Person, str)
         def convert_person_to_str(data: Person):
             return f"{data.name} {data.phone} {data.address}"
 
         @t.register_converter(dict, A)
         def convert_dict_to_a(data: dict):
             return A(data["name"], data["phone"], data["address"])
 
         @t.register_converter(dict, B)
         def convert_dict_to_b(data: dict):
             return B(data["name"], data["phone"], data["address"])
-        
+
         @t.auto_convert(protocol=True)
         async def test(a: str):
             return a
-        
+
         @t.auto_convert(protocol=True)
         async def tests(a: list[str]):
             return a
 
         async def test_async_conversion_protocol():
             d = {"name": "John", "phone": "123", "address": "123"}
 
@@ -539,9 +551,10 @@
             self.assertEqual(result, "John 123 123")
 
             result = await tests([d])
             self.assertEqual(result, ["John 123 123"])
 
         asyncio.run(test_async_conversion_protocol())
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `typegraph3-0.1.1/PKG-INFO` & `typegraph3-0.1.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegraph3
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: Type Auto Switch
 Author-Email: luxuncang <luxuncang@qq.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: typing-inspect>=0.9.0
 Requires-Dist: networkx>=3.3
 Requires-Dist: typeguard>=4.3.0
@@ -12,15 +12,15 @@
 
 <div align="center">
 
 # TypeGraph
 
 _**TypeGraph** is a Python library designed for type conversion between various types, including custom types, built-in types, and structural types (such as lists, sets, and dictionaries). It supports both synchronous and asynchronous conversion methods._
 
-> 人间总有一两风，填我十万八千梦
+> 蓦然回首，那人却在灯火阑珊处
 
  [![CodeFactor](https://www.codefactor.io/repository/github/luxuncang/typegraph/badge)](https://www.codefactor.io/repository/github/luxuncang/typegraph)
  [![GitHub](https://img.shields.io/github/license/luxuncang/typegraph)](https://github.com/luxuncang/typegraph/blob/master/LICENSE)
  [![CodeQL](https://github.com/luxuncang/typegraph/workflows/CodeQL/badge.svg)](https://github.com/luxuncang/typegraph/blob/master/.github/workflows/codeql.yml)
 
 English | [简体中文](./README-zh.md)
 
@@ -147,14 +147,15 @@
 
 @t.auto_convert()
 def test(a: str):
     return a
 
 d = {"name": "John", "phone": "123", "address": "123"}
 
+t.convert([d], list[str], debug=True, protocol=True)
 ```
 
 `t.show_mermaid_graph()`
 
 ```mermaid
 graph TD;
 dict-->PersonDict
@@ -171,17 +172,17 @@
 dict-->A
 dict-->B
 Person-->str
 A-.->Person
 ```
 
 ```bash
-Converting dict[str, str] to <class 'str'> using [<class 'dict'>, <class '__main__.A'>, <class '__main__.Person'>, <class 'str'>], <function TypeConverter.get_converter.<locals>.<lambda>.<locals>.<lambda> at 0x7fb9c8a948b0>
+Converting dict[str, str] to <class 'str'> using [<class 'dict'>, <class '__main__.A'>, <class '__main__.Person'>, <class 'str'>], <function TypeConverter.get_converter.<locals>.<lambda>.<locals>.<lambda> at 0x7f1f3306fac0>
 
-'John 123 123'
+['John 123 123']
 ```
 
 ### Auto-Convert Decorator
 Automatically convert function arguments based on type annotations:
 
 #### Synchronous
 
@@ -285,15 +286,15 @@
 
 - [X] Subclass type
 - [X] Union type
 - [X] Annotated type
 - [X] Structural type
 - [X] Protocol type (input types only)
 - [X] TypedDict type
-- [ ] Generic type
+- [X] Generic type
 
 ## License
 This project is licensed under the MIT License.
 
 ## Contributing
 Contributions are welcome! Please open an issue or submit a pull request for any changes.
```

