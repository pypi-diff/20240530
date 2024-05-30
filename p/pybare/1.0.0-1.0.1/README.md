# Comparing `tmp/pybare-1.0.0.tar.gz` & `tmp/pybare-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybare-1.0.0.tar", last modified: Wed May 29 03:23:52 2024, max compression
+gzip compressed data, was "pybare-1.0.1.tar", last modified: Thu May 30 17:03:13 2024, max compression
```

## Comparing `pybare-1.0.0.tar` & `pybare-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 noah      (1000) users      (100)        0 2024-05-29 03:23:52.419556 pybare-1.0.0/
--rw-r--r--   0 noah      (1000) users      (100)     1053 2024-05-24 01:30:00.000000 pybare-1.0.0/LICENSE
--rw-r--r--   0 noah      (1000) users      (100)     2639 2024-05-29 03:23:52.419556 pybare-1.0.0/PKG-INFO
--rw-r--r--   0 noah      (1000) users      (100)     2145 2024-05-29 02:02:09.000000 pybare-1.0.0/README.md
-drwxr-xr-x   0 noah      (1000) users      (100)        0 2024-05-29 03:23:52.419556 pybare-1.0.0/bare/
--rw-r--r--   0 noah      (1000) users      (100)      788 2024-05-29 03:17:56.000000 pybare-1.0.0/bare/__init__.py
--rw-r--r--   0 noah      (1000) users      (100)     4674 2024-05-29 03:20:16.000000 pybare-1.0.0/bare/barearray.py
--rw-r--r--   0 noah      (1000) users      (100)     3738 2024-05-29 03:18:36.000000 pybare-1.0.0/bare/barestruct.py
--rw-r--r--   0 noah      (1000) users      (100)      671 2024-05-29 01:42:58.000000 pybare-1.0.0/bare/baretype.py
--rw-r--r--   0 noah      (1000) users      (100)     2348 2024-05-29 02:24:31.000000 pybare-1.0.0/bare/data.py
--rw-r--r--   0 noah      (1000) users      (100)     3565 2024-05-29 03:17:30.000000 pybare-1.0.0/bare/map.py
--rw-r--r--   0 noah      (1000) users      (100)     3318 2024-05-29 03:14:56.000000 pybare-1.0.0/bare/misc.py
--rw-r--r--   0 noah      (1000) users      (100)     8788 2024-05-29 03:07:19.000000 pybare-1.0.0/bare/number.py
--rw-r--r--   0 noah      (1000) users      (100)     8272 2024-05-29 03:20:18.000000 pybare-1.0.0/bare/test_encoder.py
--rw-r--r--   0 noah      (1000) users      (100)     6175 2024-05-29 03:18:02.000000 pybare-1.0.0/bare/union.py
--rw-r--r--   0 noah      (1000) users      (100)     1281 2024-05-29 03:17:44.000000 pybare-1.0.0/bare/util.py
-drwxr-xr-x   0 noah      (1000) users      (100)        0 2024-05-29 03:23:52.419556 pybare-1.0.0/pybare.egg-info/
--rw-r--r--   0 noah      (1000) users      (100)     2639 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/PKG-INFO
--rw-r--r--   0 noah      (1000) users      (100)      318 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/SOURCES.txt
--rw-r--r--   0 noah      (1000) users      (100)        1 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/dependency_links.txt
--rw-r--r--   0 noah      (1000) users      (100)        5 2024-05-29 03:23:52.000000 pybare-1.0.0/pybare.egg-info/top_level.txt
--rw-r--r--   0 noah      (1000) users      (100)       38 2024-05-29 03:23:52.419556 pybare-1.0.0/setup.cfg
--rw-r--r--   0 noah      (1000) users      (100)      742 2024-05-29 03:22:55.000000 pybare-1.0.0/setup.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-30 17:03:13.129910 pybare-1.0.1/
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1053 2024-05-22 19:27:02.000000 pybare-1.0.1/LICENSE
+-rw-r--r--   0 noah      (1000) noah      (1000)     2639 2024-05-30 17:03:13.129910 pybare-1.0.1/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2145 2024-05-30 16:48:15.000000 pybare-1.0.1/README.md
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-30 17:03:13.129910 pybare-1.0.1/bare/
+-rw-rw-r--   0 noah      (1000) noah      (1000)      766 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     4654 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/barearray.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     3739 2024-05-30 16:56:39.000000 pybare-1.0.1/bare/barestruct.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)      662 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/baretype.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2349 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/data.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     3567 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/map.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     3320 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/misc.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    10598 2024-05-30 16:58:41.000000 pybare-1.0.1/bare/number.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     8310 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/test_encoder.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6178 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/union.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1282 2024-05-30 16:48:36.000000 pybare-1.0.1/bare/util.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-05-30 17:03:13.129910 pybare-1.0.1/pybare.egg-info/
+-rw-r--r--   0 noah      (1000) noah      (1000)     2639 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)      318 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/SOURCES.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        1 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/dependency_links.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        5 2024-05-30 17:03:13.000000 pybare-1.0.1/pybare.egg-info/top_level.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       38 2024-05-30 17:03:13.129910 pybare-1.0.1/setup.cfg
+-rw-rw-r--   0 noah      (1000) noah      (1000)      743 2024-05-30 17:02:32.000000 pybare-1.0.1/setup.py
```

### Comparing `pybare-1.0.0/LICENSE` & `pybare-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybare-1.0.0/PKG-INFO` & `pybare-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybare
-Version: 1.0.0
+Version: 1.0.1
 Summary: A declarative implementation of BARE for Python
 Home-page: https://sr.ht/~chiefnoah/PyBARE/
 Author: Noah Pederson
 Author-email: noah@packetlost.dev
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybare-1.0.0/README.md` & `pybare-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pybare-1.0.0/bare/__init__.py` & `pybare-1.0.1/bare/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 pybare is a Python library for writing and reading binary data using the BARE
 serialization format.
 """
+
 from .barearray import Array, array
 from .barestruct import Field, Struct
 from .data import Data, data
 from .map import Map, map
 from .misc import Enum, Str, Void
-from .number import (F32, F64, I8, I16, I32, I64, U8, U16, U32, U64, Bool, Int,
-                     UInt)
+from .number import F32, F64, I8, I16, I32, I64, U8, U16, U32, U64, Bool, Int, UInt
 from .union import Union, UnionVariant, optional, union
 
 __all__ = [
     "F32",
     "F64",
     "I8",
     "I16",
```

### Comparing `pybare-1.0.0/bare/barearray.py` & `pybare-1.0.1/bare/barearray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import io
-from typing import (Any, BinaryIO, Generic, Iterable, List, Optional, Self,
-                    Type, TypeVar)
+from typing import Any, BinaryIO, Generic, Iterable, List, Optional, Self, Type, TypeVar
 
 from .number import UInt
 
 T = TypeVar("T")
 A = List[T]
 
 
 __all__ = ["Array", "array"]
 
+
 class ArrayMeta(type):
     def __new__(
         cls,
         name,
         bases,
         namespace,
         *,
@@ -66,14 +66,15 @@
 
         class MyArray(Array, inner=UInt, size=10):
             ...
 
     You do *not* need to specify any fields or methods on the subclass, though you may.
     The above class `MyArray` is a fixed size array of 10 `UInt` values.
     """
+
     value: list[A]
     _type: Type[T]
     _size: int | None
 
     def __init__(self, value: Iterable[A]):
         self.value = ArrayValidator(self.__class__._type)
         inner = []
```

### Comparing `pybare-1.0.0/bare/barestruct.py` & `pybare-1.0.1/bare/barestruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, BinaryIO
 
 from .util import Field
 
 
 __all__ = ["Struct"]
 
+
 class StructMeta(type):
     def __new__(cls, clsname, bases, clsdict):
         fields = {}
         has_fields = False
         for name, attr in clsdict.items():
             if isinstance(attr, Field):
                 has_fields = True
```

### Comparing `pybare-1.0.0/bare/baretype.py` & `pybare-1.0.1/bare/baretype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from abc import abstractmethod
 from io import BytesIO
-from typing import (Any, BinaryIO, ByteString, Generic, Protocol, Type,
-                    TypeVar, runtime_checkable)
+from typing import (
+    Any,
+    BinaryIO,
+    ByteString,
+    Generic,
+    Protocol,
+    Type,
+    TypeVar,
+    runtime_checkable,
+)
 
 T = TypeVar("T")
 
 
 class BAREType(Protocol, Generic[T]):
     @abstractmethod
-    def pack(self, value: T) -> ByteString:
-        ...
+    def pack(self, value: T) -> ByteString: ...
 
     @classmethod
     @abstractmethod
-    def unpack(cls, fp: BinaryIO) -> T:
-        ...
+    def unpack(cls, fp: BinaryIO) -> T: ...
 
     @classmethod
     @abstractmethod
     def validate(cls, value: T) -> bool:
         return False
 
     @classmethod
     @abstractmethod
     def __eq__(cls, other: Any) -> bool:
         return False
 
     @classmethod
     @abstractmethod
-    def __hash__(cls):
-        ...
+    def __hash__(cls): ...
```

### Comparing `pybare-1.0.0/bare/data.py` & `pybare-1.0.1/bare/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     a fixed-size data type.
 
     An example:
         class MyData(Data, size=10):
             ...
 
     """
+
     _size: Optional[int]
 
     def __init__(self, value: bytes):
         if self._size and len(value) != self._size:
             raise ValueError(
                 f"Bytes was not expected size ({self._size}). Got {len(value)}"
             )
```

### Comparing `pybare-1.0.0/bare/map.py` & `pybare-1.0.1/bare/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 K = TypeVar("K", bound=BAREType)
 V = TypeVar("V", bound=BAREType)
 D = BAREType[Mapping[K, V]]
 
 __all__ = ["Map", "map"]
 
+
 class MapMeta(type):
     _key_type: Any
     _value_type: Any
 
     def __new__(
         cls,
         name,
@@ -44,14 +45,15 @@
 
 
     `Map` implements a dict-like interface and may be used as such. Both the types of
     keys and values are validated against their BARE types `validate` class method.
 
     All keys and values are normalized to their BARE type wrappers.
     """
+
     _values: dict
 
     def __init__(self, initial_values: Mapping[K, V]):
         self._values = {}
         for key, value in initial_values.items():
             self[self._key_type(key)] = self._value_type(value)
```

### Comparing `pybare-1.0.0/bare/misc.py` & `pybare-1.0.1/bare/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import EnumType, IntEnum
 from typing import Any, BinaryIO, Self
 
 from .number import UInt
 
 __all__ = ["Enum", "Void", "Str"]
 
+
 class Enum(IntEnum, metaclass=EnumType):
     """
     A BARE enum type. It is a subclass of `IntEnum` and is used to represent
     a BARE enum type.
 
     An example:
         class MyEnum(Enum):
@@ -20,14 +21,15 @@
         print(MyEnum.A)  # prints 1
         print(MyEnum.B)  # prints 2
         print(MyEnum.C)  # prints 3
 
         print(MyEnum.A is MyEnum.B)  # prints False
         print(MyEnum.A == 1)  # prints True
     """
+
     def pack(self) -> bytes:
         return UInt(self.value).pack()
 
     @classmethod
     def unpack(cls, fp: BinaryIO) -> Self:
         x = UInt.unpack(fp).value
         return cls(x)
@@ -55,14 +57,15 @@
 class Void:
     """
     A Void type. It is similar to the `None` type, but is used to represent
     a BARE void type.
 
     If should *generally* be used directly, but is also used implicitly in `option`.
     """
+
     def pack(self) -> bytes:
         return bytes()
 
     @classmethod
     def unpack(cls, _: BinaryIO) -> Self:
         return cls()
 
@@ -86,14 +89,15 @@
     It should generally be used directly.
 
     An example:
         x = Str("Hello")
         x.pack()  # prints b'\x05Hello'
         Str.unpack(x.pack())  # => Str("Hello")
     """
+
     value: str
 
     def __init__(self, value: str):
         if not self.validate(value):
             raise TypeError(f"Str must wrap a python str. Got {type(value)}")
         self.value = value
 
@@ -124,8 +128,8 @@
             return NotImplemented
 
     def __hash__(self):
         return hash(self.__class__)
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
-        return f"{name}(\"{self.value})\""
+        return f'{name}("{self.value})"'
```

### Comparing `pybare-1.0.0/bare/test_encoder.py` & `pybare-1.0.1/bare/test_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,36 @@
 import enum
 import inspect
 import io
 import os
 
 import pytest
 
-from bare import (I32, I64, U8, Array, Data, Enum, Field, Int, Map, Str,
-                  Struct, UInt, Union, Void, array, data, map, optional,
-                  union, UnionVariant)
+from bare import (
+    I32,
+    I64,
+    U8,
+    Array,
+    Data,
+    Enum,
+    Field,
+    Int,
+    Map,
+    Str,
+    Struct,
+    UInt,
+    Union,
+    Void,
+    array,
+    data,
+    map,
+    optional,
+    union,
+    UnionVariant,
+)
 
 
 class Nested(Struct):
     s = Field(Str)
 
 
 class Example(Struct):
@@ -79,16 +98,16 @@
     map = Map(Str(), Str(), value={"test": "test"})
     assert map.value["test"] == "test"
     map2 = Map(Str, Str)
     map2.value["another"] = "test"
     assert map2.value["another"] == "test"
 
 
-class MyArray(Array, inner=Int):
-    ...
+class MyArray(Array, inner=Int): ...
+
 
 class ArrayTest(Struct):
     a = Field(MyArray)
     n = Field(array(Nested, size=1))
 
 
 def test_array_struct():
@@ -120,16 +139,15 @@
 
     ex.nested = Nested(s="test")
     assert ex.nested.s == "test"
     with pytest.raises(TypeError):
         ex.nested = "test"
 
 
-class ExampleUnion(Union, variants=(Str, Int)):
-    ...
+class ExampleUnion(Union, variants=(Str, Int)): ...
 
 
 class UnionTest(Struct):
     e = Field(ExampleUnion)
     b = Field(union(Str, Int))
     c = Field(union(OptionalStruct, ArrayTest))
 
@@ -214,16 +232,15 @@
     metadata = Field(map(Str, Data))
 
 
 class TerminatedEmployee(Void):
     pass
 
 
-class Person(Union, variants=(Customer, Employee, TerminatedEmployee)):
-    ...
+class Person(Union, variants=(Customer, Employee, TerminatedEmployee)): ...
 
 
 @pytest.mark.parametrize(
     "file", ["customer.bin", "employee.bin", "people.bin", "terminated.bin"]
 )
 def test_people(file):
     with open(os.path.join(os.path.dirname(__file__), "_examples", file), "br") as f:
@@ -305,14 +322,15 @@
     unpacked = a.unpack(buf)
     assert unpacked == a
 
 
 class B(Struct):
     c = Field(Int)
 
+
 class X(Struct):
     a = Field(Str)
     b = Field(B)
 
 
 def test_struct():
     s = X(a="a test string", b=B(c=12345))
@@ -325,14 +343,15 @@
 
 def test_map():
     expected = b"\x02\x04\x74\x65\x73\x74\x04\x74\x65\x73\x74\x07\x61\x6e\x6f\x74\x68\x65\x72\x04\x63\x61\x73\x65"
     anon_map = map(Str, Str)
     m = anon_map({"test": "test", "another": "case"})
     assert m.pack() == expected
 
+
 def test_union_variant():
     MyUnion = union(UnionVariant(Str, 2), UInt)
     x = MyUnion(Str("hello"))
     fp = io.BytesIO(x.pack())
     assert fp.getbuffer()[0] == 0x2
     y = MyUnion.unpack(fp)
     assert y.value == Str("hello")
```

### Comparing `pybare-1.0.0/bare/union.py` & `pybare-1.0.1/bare/union.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         namespace["_variants"] = variants_map
         namespace["_discriminants"] = discriminants
         return super().__new__(cls, clsname, bases, namespace)
 
 
 T = TypeVar("T")
 
+
 class UnionValidator(Generic[T]):
     def __init__(self, ty: set[type]):
         self.ty = ty
 
     def __get__(self, inst, _) -> T | Iterable[type]:
         if inst is None:
             return tuple(self.ty)
@@ -69,14 +70,15 @@
 
     The wrapped value may be access using `.value`, note that it is not unwrapped
     implicitly (you will always recieve the BARE type wrapper, ex. UInt(123)
                 as opposed to 123)
 
 
     """
+
     # TODO: type annotations based on this
     value: Any
     _variants: dict[int, type]
     _discriminants: dict[type, int]
 
     def __init__(self, value: Any, *_args, **_kwargs):
         self.value = UnionValidator(self._variants)
@@ -134,14 +136,15 @@
     Use in any place you would otherwise use a BARE type when defining variants
     of a `Union`
 
     For example:
         class MyUnion(Union, variants=(UnionVariant(Str, 3), Int)):
             ...
     """
+
     def __init__(self, variant, discriminant: int):
         self.variant = variant
         self.discriminant = discriminant
 
 
 def union_member_error(t: type, variants: Iterable[type]):
     variants = " | ".join([str(x) for x in variants])
```

### Comparing `pybare-1.0.0/bare/util.py` & `pybare-1.0.1/bare/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     It is reponsible for performing type validation on assignment of struct fields.
 
     For example:
         class MyStruct(Struct):
             a = Field(UInt)
             b = Field(Str)
     """
+
     attr: str
     name: str
     ty: Type[T]
 
     def __init__(self, ty: Type[T], attr: str | None = None):
         # ignore the typing here because these will always be set when assigned to an
         # object
```

### Comparing `pybare-1.0.0/pybare.egg-info/PKG-INFO` & `pybare-1.0.1/pybare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybare
-Version: 1.0.0
+Version: 1.0.1
 Summary: A declarative implementation of BARE for Python
 Home-page: https://sr.ht/~chiefnoah/PyBARE/
 Author: Noah Pederson
 Author-email: noah@packetlost.dev
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

