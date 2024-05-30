# Comparing `tmp/pywise-0.4.0.tar.gz` & `tmp/pywise-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywise-0.4.0.tar", max compression
+gzip compressed data, was "pywise-0.6.0.tar", max compression
```

## Comparing `pywise-0.4.0.tar` & `pywise-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     6474 2022-03-09 03:15:19.030870 pywise-0.4.0/README.md
--rw-r--r--   0        0        0        0 2020-06-25 02:05:22.660525 pywise-0.4.0/core_utils/__init__.py
--rw-r--r--   0        0        0     2415 2020-06-25 02:05:22.660525 pywise-0.4.0/core_utils/archives.py
--rw-r--r--   0        0        0     5779 2022-03-09 03:15:19.030870 pywise-0.4.0/core_utils/common.py
--rw-r--r--   0        0        0     3005 2022-03-09 03:21:11.795253 pywise-0.4.0/core_utils/schema.py
--rw-r--r--   0        0        0    22864 2022-03-09 03:21:11.795253 pywise-0.4.0/core_utils/serialization.py
--rw-r--r--   0        0        0      793 2022-03-09 03:22:11.270640 pywise-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7280 2022-03-09 03:25:50.779446 pywise-0.4.0/setup.py
--rw-r--r--   0        0        0     7120 2022-03-09 03:25:50.780070 pywise-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-05-30 06:28:10.787825 pywise-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6796 2024-05-30 06:28:10.788603 pywise-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 19:00:18.670587 pywise-0.6.0/core_utils/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-30 06:28:10.789002 pywise-0.6.0/core_utils/archives.py
+-rw-r--r--   0        0        0     6050 2024-05-30 06:28:10.789423 pywise-0.6.0/core_utils/common.py
+-rw-r--r--   0        0        0     8956 2024-05-30 06:28:10.789755 pywise-0.6.0/core_utils/env.py
+-rw-r--r--   0        0        0     2548 2024-05-30 06:28:10.789965 pywise-0.6.0/core_utils/format.py
+-rw-r--r--   0        0        0     8635 2024-05-30 06:28:10.790231 pywise-0.6.0/core_utils/loggers.py
+-rw-r--r--   0        0        0     3026 2024-05-30 06:28:10.790497 pywise-0.6.0/core_utils/schema.py
+-rw-r--r--   0        0        0    22486 2024-05-30 06:28:10.790817 pywise-0.6.0/core_utils/serialization.py
+-rw-r--r--   0        0        0     6438 2024-05-30 06:28:10.791320 pywise-0.6.0/core_utils/timer.py
+-rw-r--r--   0        0        0     5543 2024-05-30 06:28:10.791545 pywise-0.6.0/core_utils/url_bucket_kv.py
+-rw-r--r--   0        0        0     3173 2024-05-30 06:28:10.792375 pywise-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 pywise-0.6.0/PKG-INFO
```

### Comparing `pywise-0.4.0/README.md` & `pywise-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 Every command must be run within the `poetry`-managed environment.
 For instance, to open a Python shell, you would execute:
 ```
 poetry run python
 ```
 Alternatively, you may activate the environment by performing `poetry shell` and directly invoke Python programs.
 
+### Development Practices
+Install pre-commit `git` hooks using `pre-commit install`. Hooks are defined in the `.pre-commit-config.yaml` file.
+
+CI enforces linting using all pre-commit hooks.
+
+NOTE: Dependencies in hooks **MUST** be kept in-sync with the 
+      `dev-dependencies` section in `pyproject.toml` for `poetry.
+
 
 #### Testing
 To run tests, execute:
 ```
 poetry run pytest -v
 ```
 To run tests against all supported environments, use [`tox`](https://tox.readthedocs.io/en/latest/):
```

### Comparing `pywise-0.4.0/core_utils/archives.py` & `pywise-0.6.0/core_utils/archives.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import shutil
 import tarfile
 from pathlib import Path
-from typing import Optional
+from typing import Literal, Optional, Sequence
+
+__all__: Sequence[str] = (
+    "extract_archive",
+    "CompressionTypes",
+)
+
+CompressionTypes = Literal["gz", "bz2", "xz"]
 
 
 def extract_archive(
     src_archive: Path,
     dest_dir: Path,
-    compression_ext: Optional[str] = None,
+    compression_ext: Optional[CompressionTypes] = None,
     overwrite: bool = False,
 ) -> None:
     """Uncompress and extract the source tar archive as a directory as the named destination path.
 
     This function extracts the (possibly compressed) tar archive, specified by :param:`src_archive`,
     and writes its contents as a directory, specified by :param:`dest_dir`.
 
@@ -39,20 +46,25 @@
     if not src_archive.is_file():
         raise IOError(f"Source artifact file does not exist: {src_archive}")
     if not overwrite and dest_dir.exists():
         raise ValueError(f"Destination exists and overwrite is false: {dest_dir}")
 
     if compression_ext is None:
         if src_archive.name.endswith("gz"):
-            compression_ext = "gz"
+            comp_ext: Literal["gz", "bz2", "xz", "*"] = "gz"
         elif src_archive.name.endswith("bz2"):
-            compression_ext = "bz2"
+            comp_ext = "bz2"
         elif src_archive.name.endswith("xz"):
-            compression_ext = "xz"
+            comp_ext = "xz"
         else:
-            compression_ext = "*"
-    mode = f"r:{compression_ext}"
+            raise ValueError(
+                "If not supplying compression extension explicitly, the source archive filename must have a "
+                f"known compatible format file extension. Unrecognized: {src_archive}"
+            )
+    else:
+        comp_ext = compression_ext
+    mode = f"r:{comp_ext}"
 
     with tarfile.open(name=str(src_archive.absolute()), mode=mode) as archive:
         if dest_dir.exists() and overwrite:
             shutil.rmtree(dest_dir)
         archive.extractall(path=str(dest_dir.absolute()))
```

### Comparing `pywise-0.4.0/core_utils/common.py` & `pywise-0.6.0/core_utils/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 from importlib import import_module
-from typing import _GenericAlias, Any, Tuple, Optional, Type, TypeVar, get_args  # type: ignore
+from typing import (  # type: ignore
+    Any,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+    _GenericAlias,  # type: ignore
+    get_args,
+)
+
+__all__: Sequence[str] = (
+    "type_name",
+    "import_by_name",
+    "split_module_value",
+    "dynamic_load",
+    "checkable_type",
+)
 
 
 def type_name(t: type, keep_main: bool = True) -> str:
     """Complete name, module & specific type name, for the given type.
     Does not supply the module in the returned complete name for built-in types.
 
     When possible, also adds generic type arguments (w/ their at-runtime values)
@@ -27,15 +44,15 @@
             pass
         return str(t)
 
     if issubclass(type(t), _GenericAlias):
         return str(t)
 
     if isinstance(t, TypeVar):  # type: ignore
-        return str(t)
+        return str(t)  # type: ignore
 
     full_name = f"{mod}.{t.__name__}"
     try:
         # generic parameters ?
         args = tuple(map(type_name, get_args(t)))  # type: ignore
         if len(args) > 0:
             a = ", ".join(args)
@@ -70,14 +87,15 @@
     :raises ModuleNotFoundError If :param:`full_name` is not a valid complete name.
     """
     if validate:
         full_name = _strip_non_empty(full_name, "Complete path name")
 
     try:
         try:
+            # validate=False because we have already checked
             module_name, value_name = split_module_value(full_name, validate=False)
             return dynamic_load(module_name, value_name, validate=False)
         except ValueError:
             # no '.' separator
             return import_module(full_name)
     except ModuleNotFoundError as e:
         try:
@@ -105,17 +123,15 @@
     """
     if validate:
         full_name = _strip_non_empty(full_name, "Complete path name")
     m, v = full_name.rsplit(".", maxsplit=1)
     return m, v
 
 
-def dynamic_load(
-    module_name: str, value_name: Optional[str], validate: bool = True
-) -> Any:
+def dynamic_load(module_name: str, value_name: Optional[str], validate: bool = True) -> Any:
     """Dynamically load a Python module, class, function, or object from its module and specific name.
 
     Loads the module :param:`module_name`. If :param:`value_name` is not None,
     then this function also loads the :param:`value_name` defined in the loaded module.
 
     :raises ValueError If :param:`validiate`:
                        - and :param:`module_name` is empty
```

### Comparing `pywise-0.4.0/core_utils/schema.py` & `pywise-0.6.0/core_utils/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+from dataclasses import is_dataclass
 from typing import (
-    Type,
-    Iterable,
-    Union,
     Any,
+    Callable,
+    Iterable,
     Mapping,
     Sequence,
-    get_args,
-    cast,
-    Callable,
     Tuple,
+    Type,
+    Union,
+    cast,
+    get_args,
 )
-from dataclasses import is_dataclass
 
-from core_utils.common import type_name, checkable_type
+from core_utils.common import checkable_type, type_name
 from core_utils.serialization import (
-    is_typed_namedtuple,
-    _namedtuple_field_types,
     _dataclass_field_types_defaults,
+    _namedtuple_field_types,
+    is_typed_namedtuple,
 )
 
-
 __all__ = ["dict_type_representation", "Discover"]
 
 Discover = Union[Mapping[str, Union[str, Mapping[str, Any]]], Sequence[Any]]
 """Schematic representation of a :func:`serializable` datatype.
 
 A dictionary of (field name, discovery type on field) pairs or a sequence thereof.
 This recursive data type definition can't be expressed in mypy yet (0.720).
@@ -38,25 +37,26 @@
     """The dictionary JSON-like named attribute & expected type representation computed
     from the supplied NamedTuple-deriving or @dataclass decorated type.
     """
     try:
         return _dict_type(nt_or_dc_type)
     except Exception as e:
         raise TypeError(
-            f"Failed to discover field-type attributes of type: '{nt_or_dc_type}", e,
+            f"Failed to discover field-type attributes of type: '{nt_or_dc_type}",
+            e,
         )
 
 
 def _dict_type(t: type):
     if is_typed_namedtuple(t) or is_dataclass(t):
         if is_typed_namedtuple(t):
-            field_types_of: Callable[
-                [], Iterable[Tuple[str, type]]
-            ] = lambda: _namedtuple_field_types(
-                t  # type: ignore
+            field_types_of: Callable[[], Iterable[Tuple[str, type]]] = (
+                lambda: _namedtuple_field_types(
+                    t  # type: ignore
+                )
             )
         else:
 
             def field_types_of() -> Iterable[Tuple[str, type]]:
                 for a, b, _ in _dataclass_field_types_defaults(t):
                     yield a, b
```

### Comparing `pywise-0.4.0/core_utils/serialization.py` & `pywise-0.6.0/core_utils/serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import traceback
+from dataclasses import _MISSING_TYPE, Field, dataclass, is_dataclass
 from enum import Enum
 from typing import (
     Any,
+    Callable,
+    Dict,
     Iterable,
-    Type,
-    Tuple,
-    Set,
+    Iterator,
+    List,
     Mapping,
-    TypeVar,
-    Callable,
     Optional,
-    Iterator,
     Sequence,
-    get_origin,
-    get_args,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
     Union,
     cast,
-    List,
-    Dict,
+    get_args,
+    get_origin,
 )
-from dataclasses import dataclass, is_dataclass, Field, _MISSING_TYPE
 
-from core_utils.common import type_name, checkable_type, split_module_value
+from core_utils.common import checkable_type, split_module_value, type_name
 
 __all__ = [
     "serialize",
     "deserialize",
     "CustomFormat",
     "is_namedtuple",
     "is_typed_namedtuple",
@@ -105,22 +105,24 @@
         return value.name
 
     else:
         return value
 
 
 def deserialize(
-    type_value: Type, value: Any, custom: Optional[CustomFormat] = None,
+    type_value: Type,
+    value: Any,
+    custom: Optional[CustomFormat] = None,
 ) -> Any:
     """Does final conversion of the `dict`-like `value` into an instance of `type_value`.
 
     NOTE: If the input type `type_value` is a sequence, then deserialization is attempted on each
     element. If it is a `dict`, then deserialization is attempted on each key and value. If this
     specified type is a namedtuple, dataclass, or enum, then it will be appropriately handled.
-    Values without these explicit types are returned as-is.
+    EnvValues without these explicit types are returned as-is.
 
     The :param:`custom` optional mapping provides callers with the ability to handle deserialization
     of complex types that are from an external source. E.g. To deserialize `numpy` arrays, one may use:
     ```
     custom = {numpy.ndarray: lambda lst: numpy.array(lst)}
     ```
     NOTE: If :param:`custom` is present, its deserialization functions are given priority.
@@ -131,15 +133,15 @@
         return custom[type_value](value)
 
     if type_value == Any:
         return value
 
     if isinstance(type_value, TypeVar):  # type: ignore
         # is a generic type alias: cannot do much with this, so return as-is
-        return value
+        return value  # type: ignore
 
     checking_type_value: Type = checkable_type(type_value)
 
     if is_namedtuple(checking_type_value):
         return _namedtuple_from_dict(type_value, value, custom)
 
     elif is_dataclass(checking_type_value):
@@ -168,33 +170,28 @@
             #     ok_to_deserialize_into = isinstance(value, get_origin(possible_type))
             # if ok_to_deserialize_into:
             #     return deserialize(possible_type, value, custom)
             try:
                 return deserialize(possible_type, value, custom)
             except Exception:
                 continue
-        raise FieldDeserializeFail(
-            field_name="", expected_type=type_value, actual_value=value
-        )
+        raise FieldDeserializeFail(field_name="", expected_type=type_value, actual_value=value)
 
     elif issubclass(checking_type_value, Mapping):
         _args = get_args(type_value)
         k_type = cast(type, _args[0])
         v_type = cast(type, _args[1])
         return {
-            deserialize(k_type, k, custom): deserialize(v_type, v, custom)
-            for k, v in value.items()
+            deserialize(k_type, k, custom): deserialize(v_type, v, custom) for k, v in value.items()
         }
 
     elif issubclass(checking_type_value, Tuple) and checking_type_value != str:  # type: ignore
         tuple_type_args = get_args(type_value)
         converted = map(
-            lambda type_val_pair: deserialize(
-                type_val_pair[0], type_val_pair[1], custom
-            ),
+            lambda type_val_pair: deserialize(type_val_pair[0], type_val_pair[1], custom),
             zip(tuple_type_args, value),
         )
         return tuple(converted)
 
     elif issubclass(checking_type_value, Iterable) and checking_type_value != str:
         # special case: fail-fast on trying to treat a dict as list-like
         if isinstance(value, dict):
@@ -217,19 +214,15 @@
         # iff the expected type is one of JSON's value types.
         if (
             (value is None and not _is_optional(checking_type_value))
             or (any(map(lambda t: t == type_value, (int, float, str, bool))))
             and not isinstance(value, checking_type_value)
         ):
             # numeric check: some ints can be a float
-            if (
-                float == type_value
-                and isinstance(value, int)
-                and int(float(value)) == value
-            ):
+            if float == type_value and isinstance(value, int) and int(float(value)) == value:
                 value = float(value)
             # and some floats can be ints
             elif int == type_value and isinstance(value, float) and int(value) == value:
                 value = int(value)
             # but in general we just identified a value that
             # didn't deserialize to its expected type
             else:
@@ -258,17 +251,16 @@
     f = getattr(t, "_fields", None)
     if not isinstance(f, tuple):
         return False
     return all(type(n) == str for n in f)
 
 
 def is_typed_namedtuple(x: Any) -> bool:
-    """Check to see if a value is a `typing.NamedTuple` instance or `type`.
-    """
-    return is_namedtuple(x) and getattr(x, "_field_types", None) is not None
+    """Check to see if a value is a `typing.NamedTuple` instance or `type`."""
+    return is_namedtuple(x) and getattr(x, "__annotations__", None) is not None
 
 
 def _namedtuple_from_dict(
     namedtuple_type: Type[SomeNamedTuple],
     data: dict,
     custom: Optional[CustomFormat] = None,
 ) -> SomeNamedTuple:
@@ -288,15 +280,15 @@
                     custom,
                 )
             )
             return namedtuple_type._make(field_values)  # type: ignore
 
         except AttributeError as ae:  # pragma: no cover
             raise TypeError(
-                "Did you pass in a valid NamedTuple type? It needs ._field_types "
+                "Did you pass in a valid NamedTuple type? It needs .__annotations__ "
                 "to return the list of valid field names & expected types! "
                 "And ._make to accept the initialization values. Type "
                 f"'{type_name(namedtuple_type)}' does not work. ",
                 ae,
             )
     else:
         raise TypeError(
@@ -304,33 +296,33 @@
             f"collections.namedtuple not a: {type_name(namedtuple_type)}"
         )
 
 
 def _namedtuple_field_types(
     namedtuple_type: Type[SomeNamedTuple],
 ) -> Iterable[Tuple[str, Type]]:
-    """Obtain the fields & expected types of a NamedTuple-deriving type.
-    """
-    return namedtuple_type._field_types.items()  # type: ignore
+    """Obtain the fields & expected types of a NamedTuple-deriving type."""
+    return namedtuple_type.__annotations__.items()  # type: ignore
 
 
 def _namedtuple_field_defaults(
     namedtuple_type: Type[SomeNamedTuple],
 ) -> Mapping[str, Any]:
     return {
         k: serialize(v, no_none_values=False)
         for k, v in namedtuple_type._field_defaults.items()  # type: ignore
     }
 
 
 def _dataclass_from_dict(
-    dataclass_type: Type, data: dict, custom: Optional[CustomFormat],
+    dataclass_type: Type,
+    data: dict,
+    custom: Optional[CustomFormat],
 ) -> Any:
-    """Constructs an @dataclass instance using :param:`data`.
-    """
+    """Constructs an @dataclass instance using :param:`data`."""
     is_generic_dataclass = hasattr(dataclass_type, "__origin__") and is_dataclass(
         dataclass_type.__origin__
     )
     if is_dataclass(dataclass_type) or is_generic_dataclass:
         try:
             all_field_type_default: List[Tuple[str, Type, Optional[Any]]] = list(
                 _dataclass_field_types_defaults(dataclass_type)
@@ -351,31 +343,28 @@
             if maybe_default is not None:
                 field_defaults[field] = maybe_default
 
         deserialized_fields = _values_for_type(
             field_and_types, data, dataclass_type, field_defaults, custom
         )
         deserialized_fields = list(deserialized_fields)
-        field_values = dict(
-            zip(map(lambda x: x[0], field_and_types), deserialized_fields)
-        )
+        field_values = dict(zip(map(lambda x: x[0], field_and_types), deserialized_fields))
         instantiated_dataclass = dataclass_type(**field_values)
         return instantiated_dataclass
     else:
         raise TypeError(
             f"Expecting a type that is annotated with @dataclass, "
             f"not a '{type_name(dataclass_type)}'"
         )
 
 
 def _dataclass_field_types_defaults(
     dataclass_type: Type,
 ) -> Iterable[Tuple[str, Type, Optional[Any]]]:
-    """Obtain the fields & their expected types for the given @dataclass type.
-    """
+    """Obtain the fields & their expected types for the given @dataclass type."""
     if hasattr(dataclass_type, "__origin__"):
         dataclass_fields = dataclass_type.__origin__.__dataclass_fields__  # type: ignore
         generic_to_concrete = dict(_align_generic_concrete(dataclass_type))
 
         def handle_field(data_field: Field) -> Tuple[str, Type, Optional[Any]]:
             if data_field.type in generic_to_concrete:
                 typ = generic_to_concrete[data_field.type]
@@ -423,37 +412,35 @@
             generics = [TypeVar("KT"), TypeVar("VT_co")]  # type: ignore
             values = get_args(data_type_with_generics)
         else:
             # should be a dataclass
             generics = origin.__parameters__  # type: ignore
             values = get_args(data_type_with_generics)  # type: ignore
         for g, v in zip(generics, values):
-            yield g, v
+            yield g, v  # type: ignore
     except AttributeError as e:
         raise ValueError(
             f"Cannot find __origin__, __dataclass_fields__ on type '{data_type_with_generics}'",
             e,
         )
 
 
 def _fill(generic_to_concrete, generic_type):
-    """Fill-in the parameterized types in generic_type using the generic-to-concrete type mapping.
-    """
+    """Fill-in the parameterized types in generic_type using the generic-to-concrete type mapping."""
     tn = type_name(generic_type, keep_main=False)
     for g in generic_type.__parameters__:
         tn = tn.replace(
             str(type_name(g, keep_main=False)),
             str(type_name(generic_to_concrete[g], keep_main=False)),
         )
     return tn
 
 
 def _exec(origin_type, tn):
-    """Using the module where `origin_type` is defined, instantiate the class defined in the `tn` string.
-    """
+    """Using the module where `origin_type` is defined, instantiate the class defined in the `tn` string."""
     module, _ = split_module_value(type_name(origin_type, keep_main=True))
     m_bits = module.split(".")
     # fmt: off
     e_str = (
         "import typing\n"
         "from typing import *\n"
     )
@@ -504,26 +491,18 @@
             # iff the expected type is one of JSON's value types.
             if (
                 (value is None and not _is_optional(field_type))
                 or (any(map(lambda t: t == field_type, (int, float, str, bool))))
                 and not isinstance(value, field_type)
             ):
                 # numeric check: some ints can be a float
-                if (
-                    float == field_type
-                    and isinstance(value, int)
-                    and int(float(value)) == value
-                ):
+                if float == field_type and isinstance(value, int) and int(float(value)) == value:
                     value = float(value)
                 # and some floats can be ints
-                elif (
-                    int == field_type
-                    and isinstance(value, float)
-                    and int(value) == value
-                ):
+                elif int == field_type and isinstance(value, float) and int(value) == value:
                     value = int(value)
                 # but in general we just identified a value that
                 # didn't deserialize to its expected type
                 else:
                     raise FieldDeserializeFail(
                         field_name=field_name,
                         expected_type=field_type,
@@ -545,32 +524,26 @@
 
         try:
             if value is not None:
                 yield deserialize(field_type, value, custom)  # type: ignore
             else:
                 yield None
         except Exception as e:
-            print(
-                "ERROR deserializing field:'"
-                + str(field_name)
-                + "'\n"
-                + traceback.format_exc()
-            )
+            print("ERROR deserializing field:'" + str(field_name) + "'\n" + traceback.format_exc())
             if isinstance(e, (FieldDeserializeFail, MissingRequired)):
                 raise e
             else:
                 raise FieldDeserializeFail(
                     field_name=field_name, expected_type=field_type, actual_value=value
                 ) from e
 
 
 @dataclass(frozen=True)
 class MissingRequired(Exception):
-    """Exception encountered when a data dict is missing a required field.
-    """
+    """Exception encountered when a data dict is missing a required field."""
 
     field_name: str
     field_expected_type: type
     expected_containing_type: type
 
     def __str__(self) -> str:
         reason = self.__cause__
@@ -579,16 +552,15 @@
             f"Missing '{self.field_name}' (expected type of '{self.field_expected_type}') "
             f"in data dict for type '{type_name(self.expected_containing_type)}'.{extra_reason}"
         )
 
 
 @dataclass(frozen=True)
 class FieldDeserializeFail(Exception):
-    """General exception indicating that some error occurred when deserializing a specific field.
-    """
+    """General exception indicating that some error occurred when deserializing a specific field."""
 
     field_name: str
     expected_type: type
     actual_value: Any
 
     def __str__(self) -> str:
         reason = self.__cause__
@@ -602,23 +574,21 @@
             f"Instead, found value '{self.actual_value}', "
             f"which has incorrect type '{type_name(type(self.actual_value))}'."
             f"{extra_reason}"
         )
 
 
 def _is_optional(t: type) -> bool:
-    """Evaluates to true iff the input is a type that is equivalent to an `Optional`.
-    """
+    """Evaluates to true iff the input is a type that is equivalent to an `Optional`."""
     try:
         type_args = get_args(t)
         only_one_none_type = (
             len(list(filter(lambda x: x == type(None), type_args))) == 1  # type: ignore
         )
         return only_one_none_type
     except Exception:
         return False
 
 
 def _is_union(t: type) -> bool:
-    """Evaluates to true iff the input is a union (not an Optional) type.
-    """
+    """Evaluates to true iff the input is a union (not an Optional) type."""
     return get_origin(t) is Union and not _is_optional(t)
```

### Comparing `pywise-0.4.0/setup.py` & `pywise-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,205 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pywise
+Version: 0.6.0
+Summary: Robust serialization support for NamedTuple & @dataclass data types.
+Home-page: https://github.com/malcolmgreaves/pywise
+License: Apache-2.0
+Author: Malcolm Greaves
+Author-email: greaves.malcolm@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 
-packages = \
-['core_utils']
+# `pywise`
+[![PyPI version](https://badge.fury.io/py/pywise.svg)](https://badge.fury.io/py/pywise) [![CircleCI](https://circleci.com/gh/malcolmgreaves/pywise/tree/main.svg?style=svg)](https://circleci.com/gh/malcolmgreaves/pywise/tree/main) [![Coverage Status](https://coveralls.io/repos/github/malcolmgreaves/pywise/badge.svg?branch=main)](https://coveralls.io/github/malcolmgreaves/pywise?branch=main)
 
-package_data = \
-{'': ['*']}
+Contains functions that provide general utility and build upon the Python 3 standard library. It has no external dependencies.
+  - `serialization`: serialization & deserialization for `NamedTuple`-deriving & `@dataclass` decorated classes
+  - `archives`: uncompress tar archives
+  - `common`: utilities
+  - `schema`: obtain a `dict`-like structure describing the fields & types for any serialzable type (helpful to view as JSON)
 
-setup_kwargs = {
-    'name': 'pywise',
-    'version': '0.4.0',
-    'description': 'Robust serialization support for NamedTuple & @dataclass data types.',
-    'long_description': '# `pywise`\n[![PyPI version](https://badge.fury.io/py/pywise.svg)](https://badge.fury.io/py/pywise) [![CircleCI](https://circleci.com/gh/malcolmgreaves/pywise/tree/main.svg?style=svg)](https://circleci.com/gh/malcolmgreaves/pywise/tree/main) [![Coverage Status](https://coveralls.io/repos/github/malcolmgreaves/pywise/badge.svg?branch=main)](https://coveralls.io/github/malcolmgreaves/pywise?branch=main)\n\nContains functions that provide general utility and build upon the Python 3 standard library. It has no external dependencies.\n  - `serialization`: serialization & deserialization for `NamedTuple`-deriving & `@dataclass` decorated classes\n  - `archives`: uncompress tar archives\n  - `common`: utilities\n  - `schema`: obtain a `dict`-like structure describing the fields & types for any serialzable type (helpful to view as JSON)\n\nThis project\'s most notable functionality are the `serialize` and `deserialize` funtions of `core_utils.serialization`.\nTake a look at the end of this document for example use.\n\n\n\n## Development Setup\nThis project uses [`poetry`](https://python-poetry.org/) for virtualenv and dependency management. We recommend using [`brew`](https://brew.sh/) to install `poetry` system-wide.\n\nTo install the project\'s dependencies, perform:\n```\npoetry install\n```\n\nEvery command must be run within the `poetry`-managed environment.\nFor instance, to open a Python shell, you would execute:\n```\npoetry run python\n```\nAlternatively, you may activate the environment by performing `poetry shell` and directly invoke Python programs.\n\n\n#### Testing\nTo run tests, execute:\n```\npoetry run pytest -v\n```\nTo run tests against all supported environments, use [`tox`](https://tox.readthedocs.io/en/latest/):\n```\npoetry run tox -p\n```\nNOTE: To run `tox`, you must have all necessary Python interpreters available.\n      We recommend using [`pyenv`](https://github.com/pyenv/pyenv) to manage your Python versions.\n\n\n#### Dev Tools\nThis project uses `black` for code formatting, `flake8` for linting, and\n`mypy` for type checking. Use the following commands to ensure code quality:\n```\n# formats all code in-place\nblack .\n\n# typechecks\nmypy --ignore-missing-imports --follow-imports=silent --show-column-numbers --warn-unreachable .\n\n# lints code\nflake8 --max-line-length=100 --ignore=E501,W293,E303,W291,W503,E203,E731,E231,E721,E722,E741 .\n```\n\n\n## Documentation via Examples\n\n#### Nested @dataclass and NamedTuple\nLets say you have an address book that you want to write to and from JSON.\nWe\'ll define our data types for our `AddressBook`:\n\n```python\nfrom typing import Optional, Union, Sequence\nfrom dataclasses import dataclass\nfrom enum import Enum, auto\n\n@dataclass(frozen=True)\nclass Name:\n    first: str\n    last: str\n    middle: Optional[str] = None\n\nclass PhoneNumber(NamedTuple):\n    area_code: int\n    number: int\n    extension: Optional[int] = None\n\n@dataclass(frozen=True)\nclass EmailAddress:\n    name: str\n    domain: str\n\nclass ContactType(Enum):\n    personal, professional = auto(), auto()\n\nclass Emergency(NamedTuple):\n    full_name: str\n    contact: Union[PhoneNumber, EmailAddress]\n\n@dataclass(frozen=True)\nclass Entry:\n    name: Name\n    number: PhoneNumber\n    email: EmailAddress\n    contact_type: ContactType\n    emergency_contact: Emergency\n\n@dataclass(frozen=True)\nclass AddressBook:\n    entries: Sequence[Entry]\n```\n\nFor illustration, let\'s consider the following instantiated `AddressBook`:\n```python\nab = AddressBook([\n    Entry(Name(\'Malcolm\', \'Greaves\', middle=\'W\'), \n          PhoneNumber(510,3452113),\n          EmailAddress(\'malcolm\',\'world.com\'),\n          contact_type=ContactType.professional,\n          emergency_contact=Emergency("Superman", PhoneNumber(262,1249865,extension=1))\n    ),\n])\n```\n\nWe can convert our `AddressBook` data type into a JSON-formatted string using `serialize`:\n```python\nfrom core_utils.serialization import serialize\nimport json\n\ns = serialize(ab)\nj = json.dumps(s, indent=2)\nprint(j)\n```\n\nAnd we can easily convert the JSON string back into a new instanitated `AddressBook` using `deserialize`:\n```python\nfrom core_utils.serialization import deserialize\n\nd = json.loads(j)\nnew_ab = deserialize(AddressBook, d)\nprint(ab == new_ab)\n# NOTE: The @dataclass(frozen=True) is only needed to make this equality work.\n#       Any @dataclass decorated type is serializable. \n```\n\nNote that the `deserialize` function needs the type to deserialize the data into. The deserizliation\ntype-matching is _structural_: it will work so long as the data type\'s structure (of field names and\nassociated types) is compatible with the supplied data.\n\n\n#### Custom Serialization\nIn the event that one desires to use `serialize` and `deserialize` with data types from third-party libraries (e.g. `numpy` arrays) or custom-defined `class`es that are not decorated with `@dataclass` or derive from `NamedTuple`, one may supply a `CustomFormat`.\n\n`CustomFormat` is a mapping that associates precise types with custom serialization functions. When supplied to `serialize`, the values in the mapping accept an instance of the exact type and produces a serializable representation. In the `deserialize` function, they convert such a serialized representation into a bonafide instance of the type.\n\nTo illustrate their use, we\'ll deine `CustomFormat` `dict`s that allow us to serialize `numpy` multi-dimensional arrays:\n```python\nimport numpy as np\nfrom core_utils.serialization import *\n\n\ncustom_serialization: CustomFormat = {\n    np.ndarray: lambda arr: arr.tolist()\n}\n\ncustom_deserialization: CustomFormat = {\n    np.ndarray: lambda lst: np.array(lst)\n}\n```\n\nNow, we may supply `custom_{serialization,deserialization}` to our functions. We\'ll use them to perform a "round-trip" serialization of a four-dimensional array of floating point numbers to and from a JSON-formatted `str`:\n```python\nimport json\n\nv_original = np.random.random((1,2,3,4))\ns = serialize(v_original, custom=custom_serialization)\nj = json.dumps(s)\n\nd = json.loads(j)\nv_deser = deserialize(np.ndarray, d, custom=custom_deserialization)\n\nprint((v_original == v_deser).all())\n```\n\nIt\'s important to note that, when supplying a `CustomFormat` the serialization functions take priority over the default behavior (except for `Any`, as it is _always_ considered a pass-through). Moreover, types must match **exactly** to the keys in the mapping. Thus, if using a generic type, you must supply separate key-value entires for each distinct type parameterization.\n\n',
-    'author': 'Malcolm Greaves',
-    'author_email': 'greaves.malcolm@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/malcolmgreaves/pywise',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
+This project's most notable functionality are the `serialize` and `deserialize` funtions of `core_utils.serialization`.
+Take a look at the end of this document for example use.
+
+
+
+## Development Setup
+This project uses [`poetry`](https://python-poetry.org/) for virtualenv and dependency management. We recommend using [`brew`](https://brew.sh/) to install `poetry` system-wide.
+
+To install the project's dependencies, perform:
+```
+poetry install
+```
+
+Every command must be run within the `poetry`-managed environment.
+For instance, to open a Python shell, you would execute:
+```
+poetry run python
+```
+Alternatively, you may activate the environment by performing `poetry shell` and directly invoke Python programs.
+
+### Development Practices
+Install pre-commit `git` hooks using `pre-commit install`. Hooks are defined in the `.pre-commit-config.yaml` file.
+
+CI enforces linting using all pre-commit hooks.
+
+NOTE: Dependencies in hooks **MUST** be kept in-sync with the 
+      `dev-dependencies` section in `pyproject.toml` for `poetry.
+
+
+#### Testing
+To run tests, execute:
+```
+poetry run pytest -v
+```
+To run tests against all supported environments, use [`tox`](https://tox.readthedocs.io/en/latest/):
+```
+poetry run tox -p
+```
+NOTE: To run `tox`, you must have all necessary Python interpreters available.
+      We recommend using [`pyenv`](https://github.com/pyenv/pyenv) to manage your Python versions.
+
+
+#### Dev Tools
+This project uses `black` for code formatting, `flake8` for linting, and
+`mypy` for type checking. Use the following commands to ensure code quality:
+```
+# formats all code in-place
+black .
+
+# typechecks
+mypy --ignore-missing-imports --follow-imports=silent --show-column-numbers --warn-unreachable .
+
+# lints code
+flake8 --max-line-length=100 --ignore=E501,W293,E303,W291,W503,E203,E731,E231,E721,E722,E741 .
+```
+
+
+## Documentation via Examples
+
+#### Nested @dataclass and NamedTuple
+Lets say you have an address book that you want to write to and from JSON.
+We'll define our data types for our `AddressBook`:
+
+```python
+from typing import Optional, Union, Sequence
+from dataclasses import dataclass
+from enum import Enum, auto
+
+@dataclass(frozen=True)
+class Name:
+    first: str
+    last: str
+    middle: Optional[str] = None
+
+class PhoneNumber(NamedTuple):
+    area_code: int
+    number: int
+    extension: Optional[int] = None
+
+@dataclass(frozen=True)
+class EmailAddress:
+    name: str
+    domain: str
+
+class ContactType(Enum):
+    personal, professional = auto(), auto()
+
+class Emergency(NamedTuple):
+    full_name: str
+    contact: Union[PhoneNumber, EmailAddress]
+
+@dataclass(frozen=True)
+class Entry:
+    name: Name
+    number: PhoneNumber
+    email: EmailAddress
+    contact_type: ContactType
+    emergency_contact: Emergency
+
+@dataclass(frozen=True)
+class AddressBook:
+    entries: Sequence[Entry]
+```
+
+For illustration, let's consider the following instantiated `AddressBook`:
+```python
+ab = AddressBook([
+    Entry(Name('Malcolm', 'Greaves', middle='W'), 
+          PhoneNumber(510,3452113),
+          EmailAddress('malcolm','world.com'),
+          contact_type=ContactType.professional,
+          emergency_contact=Emergency("Superman", PhoneNumber(262,1249865,extension=1))
+    ),
+])
+```
+
+We can convert our `AddressBook` data type into a JSON-formatted string using `serialize`:
+```python
+from core_utils.serialization import serialize
+import json
+
+s = serialize(ab)
+j = json.dumps(s, indent=2)
+print(j)
+```
+
+And we can easily convert the JSON string back into a new instanitated `AddressBook` using `deserialize`:
+```python
+from core_utils.serialization import deserialize
+
+d = json.loads(j)
+new_ab = deserialize(AddressBook, d)
+print(ab == new_ab)
+# NOTE: The @dataclass(frozen=True) is only needed to make this equality work.
+#       Any @dataclass decorated type is serializable. 
+```
+
+Note that the `deserialize` function needs the type to deserialize the data into. The deserizliation
+type-matching is _structural_: it will work so long as the data type's structure (of field names and
+associated types) is compatible with the supplied data.
+
+
+#### Custom Serialization
+In the event that one desires to use `serialize` and `deserialize` with data types from third-party libraries (e.g. `numpy` arrays) or custom-defined `class`es that are not decorated with `@dataclass` or derive from `NamedTuple`, one may supply a `CustomFormat`.
+
+`CustomFormat` is a mapping that associates precise types with custom serialization functions. When supplied to `serialize`, the values in the mapping accept an instance of the exact type and produces a serializable representation. In the `deserialize` function, they convert such a serialized representation into a bonafide instance of the type.
+
+To illustrate their use, we'll deine `CustomFormat` `dict`s that allow us to serialize `numpy` multi-dimensional arrays:
+```python
+import numpy as np
+from core_utils.serialization import *
+
+
+custom_serialization: CustomFormat = {
+    np.ndarray: lambda arr: arr.tolist()
+}
+
+custom_deserialization: CustomFormat = {
+    np.ndarray: lambda lst: np.array(lst)
 }
+```
+
+Now, we may supply `custom_{serialization,deserialization}` to our functions. We'll use them to perform a "round-trip" serialization of a four-dimensional array of floating point numbers to and from a JSON-formatted `str`:
+```python
+import json
+
+v_original = np.random.random((1,2,3,4))
+s = serialize(v_original, custom=custom_serialization)
+j = json.dumps(s)
+
+d = json.loads(j)
+v_deser = deserialize(np.ndarray, d, custom=custom_deserialization)
+
+print((v_original == v_deser).all())
+```
+
+It's important to note that, when supplying a `CustomFormat` the serialization functions take priority over the default behavior (except for `Any`, as it is _always_ considered a pass-through). Moreover, types must match **exactly** to the keys in the mapping. Thus, if using a generic type, you must supply separate key-value entires for each distinct type parameterization.
 
 
-setup(**setup_kwargs)
```

