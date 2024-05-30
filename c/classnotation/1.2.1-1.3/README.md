# Comparing `tmp/classnotation-1.2.1.tar.gz` & `tmp/classnotation-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classnotation-1.2.1.tar", last modified: Mon May 20 04:11:43 2024, max compression
+gzip compressed data, was "classnotation-1.3.tar", last modified: Thu May 30 16:34:31 2024, max compression
```

## Comparing `classnotation-1.2.1.tar` & `classnotation-1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:11:43.928415 classnotation-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      283 2024-05-20 04:11:43.928415 classnotation-1.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:11:43.928415 classnotation-1.2.1/classnotation/
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-02 14:45:56.000000 classnotation-1.2.1/classnotation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8517 2024-05-02 14:45:56.000000 classnotation-1.2.1/classnotation/dumper.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-04-15 05:55:22.000000 classnotation-1.2.1/classnotation/json_types.py
--rw-rw-rw-   0 root         (0) root         (0)    13159 2024-05-20 04:11:20.000000 classnotation-1.2.1/classnotation/loader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:11:37.000000 classnotation-1.2.1/classnotation/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:11:43.928415 classnotation-1.2.1/classnotation.egg-info/
--rw-r--r--   0 root         (0) root         (0)      139 2024-05-20 04:11:43.000000 classnotation-1.2.1/classnotation.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-20 04:11:20.000000 classnotation-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 04:11:43.928415 classnotation-1.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:34:31.245644 classnotation-1.3/
+-rw-r--r--   0 root         (0) root         (0)      281 2024-05-30 16:34:31.245644 classnotation-1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:34:31.245644 classnotation-1.3/classnotation/
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-30 16:34:24.000000 classnotation-1.3/classnotation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8517 2024-05-30 16:34:24.000000 classnotation-1.3/classnotation/dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-05-30 16:34:24.000000 classnotation-1.3/classnotation/json_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    14206 2024-05-30 16:34:24.000000 classnotation-1.3/classnotation/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 16:34:24.000000 classnotation-1.3/classnotation/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-05-30 16:34:24.000000 classnotation-1.3/classnotation/typecheck_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:34:31.245644 classnotation-1.3/classnotation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-30 16:34:31.000000 classnotation-1.3/classnotation.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-30 16:24:34.000000 classnotation-1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 16:34:31.245644 classnotation-1.3/setup.cfg
```

### Comparing `classnotation-1.2.1/classnotation/dumper.py` & `classnotation-1.3/classnotation/dumper.py`

 * *Files identical despite different names*

### Comparing `classnotation-1.2.1/classnotation/loader.py` & `classnotation-1.3/classnotation/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Dict, Any, Type, TypeVar, List, get_origin, get_args, Union, Optional, Literal, Tuple
+from typing import Any, Type, TypeVar, List, get_origin, get_args, Union, Optional, Literal, Tuple, ForwardRef
 from dataclasses import fields, is_dataclass
 import logging
 import enum
 import importlib
 import json
-from .json_types import JSONData, JSONObject
+from .json_types import JSONObject
+from .typecheck_error import TypeCheckError
+
 
 T = TypeVar('T')
 
 
 class DataclassLoader:
     allow_whole_float_as_int: bool
     strict: bool
@@ -57,168 +59,180 @@
         self,
         data_class: Type[T],
         data: JSONObject,
         _stack: Tuple[str, ...],
 
     ) -> T:
         if not is_dataclass(data_class):
-            raise TypeError("Expected a dataclass type as `data_class`")
+            raise TypeCheckError("Expected a dataclass type as `data_class`", _stack)
 
-        field_type_lookup = {field.name: resolve_field_type(field.type, data_class) for field in fields(data_class)}
+        field_type_lookup = {field.name: field.type for field in fields(data_class)}
         field_renaming = {field.metadata["json"]: field.name for field in fields(data_class) if "json" in field.metadata}
         validated_data = {}
 
         for json_key, value in data.items():
 
             if not isinstance(json_key, str):
-                raise TypeError("Expected only string keys when loading dict into dataclass but found `{}` of type {} at {}".format(json_key, type(json_key), ".".join(_stack)))
+                raise TypeCheckError(
+                    "Expected only string keys when loading dict into dataclass but found `{}` of type {}".format(json_key, type(json_key)),
+                    _stack,
+                )
 
             field_name = json_key
             if json_key in field_renaming:
                 field_name = field_renaming[json_key]
 
             if field_name in field_type_lookup:
                 field_type = field_type_lookup[field_name]
 
-                validated_data[field_name] = self.validate_field(value, field_type, _stack=(*_stack, json_key))
+                validated_data[field_name] = self.validate_field(value, field_type, data_class,_stack=(*_stack, json_key))
 
             else:
-                error_message = "Warning: Field '{json_key}' found in json at {stack} but it not present in the dataclass {dataclass}.".format(
-                    json_key=json_key,
-                    stack=".".join(_stack),
-                    dataclass=data_class,
-                )
+
                 if not self.strict:
+                    error_message = "Warning: Field '{json_key}' found in json at {stack} but it not present in the dataclass {dataclass}.".format(
+                        json_key=json_key,
+                        stack=".".join(_stack),
+                        dataclass=data_class,
+                    )
                     logging.warning(error_message)
                 else:
-                    raise TypeError(error_message)
+                    raise TypeCheckError(
+                        "Warning: Field '{json_key}' found but it not present in the dataclass {dataclass}.".format(
+                            json_key=json_key,
+                            dataclass=data_class,
+                        ),
+                        _stack,
+                    )
 
         try:
             return data_class(**validated_data)
-        except TypeError as e:
+        except TypeCheckError as e:
             print("Error found at", ".".join(_stack)) # TODO: this should be incorporated into the message somehow
             raise e
 
     ################################################################################
     #
     ################################################################################
     def validate_field(
         self,
         value: Any,
         field_type: Type[T],
+        parent_object: Any,
         _stack: Tuple[str, ...],
     ) -> T:
+        field_type = resolve_field_type(field_type, parent_object)
         field_origin = get_origin(field_type)
 
         # List[]
         if field_origin == list:
             if isinstance(value, list):
                 retval = [
                     self.validate_field(
-                        element,
-                        get_args(field_type)[0],
+                        value=element,
+                        field_type=get_args(field_type)[0],
+                        parent_object=parent_object,
                         _stack=(*_stack, "[{}]".format(i))
                     ) for i, element in enumerate(value)
                 ]
                 return retval
 
         # Dict[]
         elif field_origin == dict:
             if isinstance(value, dict):
                 retval = {
-                    self.validate_field(k, get_args(field_type)[0], _stack=(*_stack, str(k))):
-                    self.validate_field(v, get_args(field_type)[1], _stack=(*_stack, "[{}]".format(k.__repr__())))
+                    self.validate_field(value=k, field_type=get_args(field_type)[0], parent_object=parent_object,_stack=(*_stack, str(k))):
+                    self.validate_field(value=v, field_type=get_args(field_type)[1], parent_object=parent_object,_stack=(*_stack, "[{}]".format(k.__repr__())))
                     for k, v in value.items()
                 }
                 return retval
 
         # Set[]
         elif field_origin == set:
             if isinstance(value, list) or isinstance(value, set) or isinstance(value, tuple):
                 retval = set([
-                    self.validate_field(element, get_args(field_type)[0], _stack=(*_stack, "[{}]".format(i)))
+                    self.validate_field(value=element, field_type=get_args(field_type)[0], parent_object=parent_object,_stack=(*_stack, "[{}]".format(i)))
                     for i, element in enumerate(value)
                 ])
                 return retval
 
         # Tuple[]
         elif (get_origin(field_type) == tuple):
             if isinstance(value, list) or isinstance(value, tuple):
 
                 args = get_args(field_type)
                 # Variable Length Tuples
                 if len(args) == 2 and args[1] == Ellipsis:
                     retval = tuple(
-                        self.validate_field(element, get_args(field_type)[0], _stack=(*_stack, "[{}]".format(i)))
+                        self.validate_field(value=element, field_type=get_args(field_type)[0], parent_object=parent_object,_stack=(*_stack, "[{}]".format(i)))
                         for i, element in enumerate(value)
                     )
                     return retval
 
                 # Fixed Length Tuples
                 else:
                     if len(args) != len(value):
-                        raise TypeError("Different Number of elements found for tuple then expected found {} ({}), expected {}".format(len(value), value, len(args)))
+                        raise TypeCheckError(
+                            "Different Number of elements found for tuple then expected found {} ({}), expected {}".format(len(value), value, len(args)),
+                            _stack,
+                        )
 
                     retval = tuple(
-                        self.validate_field(value[i], args[i], _stack=(*_stack, "[{}]".format(i)))
+                        self.validate_field(value=value[i], field_type=args[i], parent_object=parent_object,_stack=(*_stack, "[{}]".format(i)))
                         for i in range(len(value))
                     )
                     return retval
 
         # Union[] and Optional[]
         elif field_origin == Union:
-            all_errors: List[TypeError] = []
+            all_errors: List[TypeCheckError] = []
             for arg in get_args(field_type):
                 try:
-                    return self.validate_field(value, arg, _stack=_stack)
-                except TypeError as e:
+                    return self.validate_field(value=value, field_type=arg, parent_object=parent_object,_stack=_stack)
+                except TypeCheckError as e:
                     all_errors.append(e)
 
             if len(all_errors) > 0:
                 # Build an error message that contains the errors from parsing each of the possible types in the union
                 combined_message: List[str] = ["Expected one of union type `{}` at `{}`".format(field_type, ".".join(_stack))]
                 for i, error in enumerate(all_errors):
                     prefix: str = "  {}: ".format(i)
-                    for line in error.args[0].split("\n"):
+                    for line in error.__str__().split("\n"):
                         combined_message.append(prefix + line)
                         prefix = " " * len(prefix)
 
-                raise TypeError("\n".join(combined_message))
+                raise TypeCheckError("\n".join(combined_message), _stack)
 
         # Literal[]
         elif field_origin == Literal:
             arg_value = get_args(field_type)[0]
             if type(value) is str and type(arg_value) is bytes:
                 value = value.encode("utf-8")
 
             if value != arg_value:
-                raise TypeError("Expected a literal '{}' but got '{}".format(get_args(field_type)[0], value))
+                raise TypeCheckError("Expected a literal '{}' but got '{}'".format(get_args(field_type)[0], value), _stack)
             return value
 
         elif field_origin is None:
-            # Special case of None Type
-            if field_type is None and value is None:
-                return value
-
             # Special case to call out that bool is historically an instance of int
             # and we want to be sure a bool is not trying to be assigned to an int.
             # TODO: we might want to make a custom isinstance function instead.
-            elif type(value) is bool and field_type in (int, float):
+            if type(value) is bool and field_type in (int, float):
                 pass
 
             # General case of scalar types
-            elif isinstance(value, field_type):
+            elif isinstance(value, field_type): #TODO, This can bug sometimes if field_type is not a "type" for any reason. We should sanitize it at the very least to produce a useful error
                 return value
 
             # Enums
             elif issubclass(field_type, enum.Enum):
                 for element in field_type:
                     if element.value == value:
                         return field_type(value)
-                raise TypeError("Invalid Enum value for {}: {}".format(field_type, value))
+                raise TypeCheckError("Invalid Enum value for {}: {}".format(field_type, value), _stack)
 
             # Sub Dataclass
             elif isinstance(value, dict) and is_dataclass(field_type):
                 retval = self._load_data(field_type, value, _stack=_stack)
                 return retval
 
             # Special handling for floats as integers (as JSON numbers are parsed as floats)
@@ -230,34 +244,38 @@
                 return float(value)
 
             # Special handling for strings as bytes
             elif field_type is bytes and isinstance(value, str):
                 return value.encode("utf-8")
 
             # If we get here, nothing above parsed properly
-            raise TypeError("Unhandled scalar type `{found_type}` at `{stack}`. Expected `{target_type}`.".format(
-                found_type=type(value),
-                stack=".".join(_stack),
-                target_type=field_type)
+            raise TypeCheckError(
+                "Unhandled scalar type `{found_type}`. Expected `{target_type}`.".format(
+                    found_type=type(value),
+                    target_type=field_type
+                ),
+                _stack,
             )
 
         else:
-            raise TypeError(
+            raise TypeCheckError(
                 "Error: Field '{data_key} in dataclass has an unexpected origin type of {data_origin}. This might be a bug in dataclass loader, please report it.".format(
                     data_key=".".join(_stack),
-                    data_origin=field_origin
-                )
+                    data_origin=field_origin,
+                ),
+                _stack,
             )
 
-        raise TypeError(
+        raise TypeCheckError(
             "Error: Field '{data_key}' is {data_type} but dataclass expected {dataclass_type}".format(
                 data_key=".".join(_stack),
                 data_type=type(value),
                 dataclass_type=field_type,
-            )
+            ),
+            _stack,
         )
 
 
 ################################################################################
 # resolve_field_type
 #
 # This function takes a type annotation and resolves it into an actual type if
@@ -265,40 +283,39 @@
 # expecting a real type value and not a string representation of the type. One
 # function is the commonly used `isinstance()`.
 ################################################################################
 def resolve_field_type(
     field_type: Any,
     defined_in_object: Optional[Any] = None
 ) -> Type:
+    if isinstance(field_type, ForwardRef):
+        field_type = field_type.__forward_arg__
+
     # Handle stringy types
     if isinstance(field_type, str):
         if defined_in_object is None:
             raise TypeError("Stringy Type found but no object path can be used to decode the type")
 
         module_name = defined_in_object.__module__
         module = importlib.import_module(module_name)
 
         # Iterate through the full type grabbing the next subtype in the list
         found_type: Any = module
         for element in field_type.split("."):
             found_type = getattr(found_type, element)
 
-        # Sanity Check
-        if not isinstance(found_type, type):
-            raise TypeError("Cannot find the specified type {}".format(field_type))
-
-        return found_type
+        return resolve_field_type(found_type, defined_in_object)
 
     # Handle most types
     elif isinstance(field_type, type):
         return field_type
 
     # Special case for the "None" type
     elif field_type is None:
-        return field_type
+        return type(None)
 
     # Handle typing generic types, for example List[int]
     elif get_origin(field_type) is not None:
         return field_type
 
     else:
         raise TypeError("Invalid type found on field {} (of type {})".format(field_type, type(field_type)))
```

