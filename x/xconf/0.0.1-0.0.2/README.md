# Comparing `tmp/xconf-0.0.1.tar.gz` & `tmp/xconf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xconf-0.0.1.tar", last modified: Sun Jan 30 05:45:43 2022, max compression
+gzip compressed data, was "xconf-0.0.2.tar", last modified: Thu May 30 00:37:36 2024, max compression
```

## Comparing `xconf-0.0.1.tar` & `xconf-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2022-01-30 05:45:43.001355 xconf-0.0.1/
--rw-r--r--   0 josephlong   (501) staff       (20)     1149 2021-11-17 22:12:28.000000 xconf-0.0.1/LICENSE
--rw-r--r--   0 josephlong   (501) staff       (20)     2875 2022-01-30 05:45:43.001220 xconf-0.0.1/PKG-INFO
--rw-r--r--   0 josephlong   (501) staff       (20)     2573 2021-11-17 22:12:28.000000 xconf-0.0.1/README.md
--rw-r--r--   0 josephlong   (501) staff       (20)       38 2022-01-30 05:45:43.001411 xconf-0.0.1/setup.cfg
--rw-r--r--   0 josephlong   (501) staff       (20)      431 2022-01-30 05:45:26.000000 xconf-0.0.1/setup.py
-drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2022-01-30 05:45:42.998422 xconf-0.0.1/xconf/
--rw-r--r--   0 josephlong   (501) staff       (20)    12844 2021-12-18 21:40:09.000000 xconf-0.0.1/xconf/__init__.py
-drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2022-01-30 05:45:42.998876 xconf-0.0.1/xconf/vendor/
--rw-r--r--   0 josephlong   (501) staff       (20)        0 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/__init__.py
-drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2022-01-30 05:45:43.000128 xconf-0.0.1/xconf/vendor/dacite/
--rw-r--r--   0 josephlong   (501) staff       (20)       81 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/__init__.py
--rw-r--r--   0 josephlong   (501) staff       (20)      415 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/config.py
--rw-r--r--   0 josephlong   (501) staff       (20)     5501 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/core.py
--rw-r--r--   0 josephlong   (501) staff       (20)       52 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/data.py
--rw-r--r--   0 josephlong   (501) staff       (20)     1040 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/dataclasses.py
--rw-r--r--   0 josephlong   (501) staff       (20)     2587 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/exceptions.py
--rw-r--r--   0 josephlong   (501) staff       (20)     5875 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/dacite/types.py
--rw-r--r--   0 josephlong   (501) staff       (20)    57970 2021-11-17 22:12:28.000000 xconf-0.0.1/xconf/vendor/py310_dataclasses.py
-drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2022-01-30 05:45:43.000859 xconf-0.0.1/xconf.egg-info/
--rw-r--r--   0 josephlong   (501) staff       (20)     2875 2022-01-30 05:45:42.000000 xconf-0.0.1/xconf.egg-info/PKG-INFO
--rw-r--r--   0 josephlong   (501) staff       (20)      776 2022-01-30 05:45:42.000000 xconf-0.0.1/xconf.egg-info/SOURCES.txt
--rw-r--r--   0 josephlong   (501) staff       (20)        1 2022-01-30 05:45:42.000000 xconf-0.0.1/xconf.egg-info/dependency_links.txt
--rw-r--r--   0 josephlong   (501) staff       (20)       13 2022-01-30 05:45:42.000000 xconf-0.0.1/xconf.egg-info/requires.txt
--rw-r--r--   0 josephlong   (501) staff       (20)        6 2022-01-30 05:45:42.000000 xconf-0.0.1/xconf.egg-info/top_level.txt
+drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2024-05-30 00:37:36.218639 xconf-0.0.2/
+-rw-r--r--   0 josephlong   (501) staff       (20)     1149 2021-11-17 22:12:28.000000 xconf-0.0.2/LICENSE
+-rw-r--r--   0 josephlong   (501) staff       (20)     3462 2024-05-30 00:37:36.218369 xconf-0.0.2/PKG-INFO
+-rw-r--r--   0 josephlong   (501) staff       (20)     2894 2024-05-30 00:11:34.000000 xconf-0.0.2/README.md
+-rw-r--r--   0 josephlong   (501) staff       (20)       38 2024-05-30 00:37:36.218715 xconf-0.0.2/setup.cfg
+-rw-r--r--   0 josephlong   (501) staff       (20)      657 2024-05-30 00:35:30.000000 xconf-0.0.2/setup.py
+drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2024-05-30 00:37:36.203711 xconf-0.0.2/xconf/
+-rw-r--r--   0 josephlong   (501) staff       (20)    15453 2024-05-30 00:11:40.000000 xconf-0.0.2/xconf/__init__.py
+drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2024-05-30 00:37:36.204790 xconf-0.0.2/xconf/contrib/
+-rw-r--r--   0 josephlong   (501) staff       (20)    11744 2024-05-29 22:22:36.000000 xconf-0.0.2/xconf/contrib/__init__.py
+-rw-r--r--   0 josephlong   (501) staff       (20)     1613 2022-12-05 02:48:48.000000 xconf-0.0.2/xconf/fs.py
+drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2024-05-30 00:37:36.205322 xconf-0.0.2/xconf/vendor/
+-rw-r--r--   0 josephlong   (501) staff       (20)        0 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/__init__.py
+drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2024-05-30 00:37:36.217456 xconf-0.0.2/xconf/vendor/dacite/
+-rw-r--r--   0 josephlong   (501) staff       (20)       81 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/__init__.py
+-rw-r--r--   0 josephlong   (501) staff       (20)      415 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/config.py
+-rw-r--r--   0 josephlong   (501) staff       (20)     5501 2022-08-03 03:36:22.000000 xconf-0.0.2/xconf/vendor/dacite/core.py
+-rw-r--r--   0 josephlong   (501) staff       (20)       52 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/data.py
+-rw-r--r--   0 josephlong   (501) staff       (20)     1040 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/dataclasses.py
+-rw-r--r--   0 josephlong   (501) staff       (20)     2587 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/exceptions.py
+-rw-r--r--   0 josephlong   (501) staff       (20)        0 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/py.typed
+-rw-r--r--   0 josephlong   (501) staff       (20)     5875 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/dacite/types.py
+-rw-r--r--   0 josephlong   (501) staff       (20)    57970 2021-11-17 22:12:28.000000 xconf-0.0.2/xconf/vendor/py310_dataclasses.py
+drwxr-xr-x   0 josephlong   (501) staff       (20)        0 2024-05-30 00:37:36.217720 xconf-0.0.2/xconf.egg-info/
+-rw-r--r--   0 josephlong   (501) staff       (20)     3462 2024-05-30 00:37:36.000000 xconf-0.0.2/xconf.egg-info/PKG-INFO
+-rw-r--r--   0 josephlong   (501) staff       (20)      843 2024-05-30 00:37:36.000000 xconf-0.0.2/xconf.egg-info/SOURCES.txt
+-rw-r--r--   0 josephlong   (501) staff       (20)        1 2024-05-30 00:37:36.000000 xconf-0.0.2/xconf.egg-info/dependency_links.txt
+-rw-r--r--   0 josephlong   (501) staff       (20)       74 2024-05-30 00:37:36.000000 xconf-0.0.2/xconf.egg-info/requires.txt
+-rw-r--r--   0 josephlong   (501) staff       (20)        6 2024-05-30 00:37:36.000000 xconf-0.0.2/xconf.egg-info/top_level.txt
```

### Comparing `xconf-0.0.1/LICENSE` & `xconf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xconf-0.0.1/PKG-INFO` & `xconf-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,100 @@
 Metadata-Version: 2.1
 Name: xconf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Turns TOML files and command-line arguments into dataclasses for config
-Home-page: UNKNOWN
 Author: Joseph D. Long
 Author-email: jdl@zesty.space
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: toml>=0.10.2
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Provides-Extra: contrib
+Requires-Dist: fsspec; extra == "contrib"
+Requires-Dist: ray; extra == "contrib"
+Provides-Extra: all
+Requires-Dist: ray; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: fsspec; extra == "all"
 
 # `xconf` - Dataclasses and TOML for command configuration
 
 ## Demo
 
-An example of how to use `xconf.Command`, `xconf.field`, and `xconf.config` is in `demo.py`. Run it to see its configuration keys.
+An example of how to use `xconf.Command`, `xconf.field`, and `xconf.config` is in `xconf_demo.py`. Run it to see its configuration keys.
 
 ```
-$ python demo.py demo_command -h
+$ python xconf_demo.py demo_command -h
 demo_command: Demo command
-usage: demo.py demo_command [-c CONFIG_FILE] [-h] [-v] [--dump-config] [vars ...]
+usage: xconf_demo.py demo_command [-c CONFIG_FILE] [-h] [-v] [--dump-config] [vars ...]
 
 positional arguments:
   vars                  Config variables set with 'key.key.key=value' notation
 
 optional arguments:
   -c CONFIG_FILE, --config-file CONFIG_FILE
-                        Path to config file (default: demo_command.conf.toml)
+                        Path to config file (default: demo_command.conf)
   -h, --help            Print usage information
   -v, --verbose         Enable debug logging
   --dump-config         Dump final configuration state as TOML and exit
+
 configuration keys:
   collections
       dict[str, ExtendedThingie]
   collections.<str>.name
       str
+     <ExtendedThingie>
   collections.<str>.extended
       bool
+     <ExtendedThingie>
   either_one
       [int, str]
   should_bar
       bool
      (default: False)
   should_foo
       bool
     Whether demo should foo
   number_list
       list[int]
     List of favorite numbers
+  float_list
+      list[float]
+    List of favorite floating-point numbers
+  str_list
+      list[str]
+    List of favorite strings
   sequence
       list[ExtendedThingie]
+     (default: [])
+  sequence[#].name
+      str
+     <ExtendedThingie>
+  sequence[#].extended
+      bool
+     <ExtendedThingie>
 ```
 
 ### Default config file
 
-The command name, `demo_command`, is generated from the class name and used to find a default configuration file (`demo_command.conf.toml`) in the current directory.
+The command name, `demo_command`, is generated from the class name and used to find a default configuration file (`demo_command.conf`) in the current directory.
 
 ### Providing arguments at the command line
 
 Any configuration key from the help output can be supplied on the command line in a `dotted.name=value` format.
 
 For lists of primitive types (`str`, `int`, `float`), you can just use commas to separate the values on the right hand side of the `=`. Example: `number_list=1,2,3`.
 
 To override a single entry in a list, use `some_name[#]` or `dotted[#].name=value` where `#` is an integer index will work. Example: `number_list[0]=99`
 
 String values are bare (i.e. no quotation marks around `value`). Boolean values are case-insensitive `true`, `t`, or 1 for True, `false`, `f`, or 0 for False.
 
 ### Structuring the command
 
-See `demo.py` for an example. Note that commands must subclass `xconf.Command` *and* apply the `@xconf.config` decorator. Options are defined by a hierarchy of dataclasses. (For uninteresting reasons, they aren't *strictly speaking* `import dataclass` dataclasses.)
+See `xconf_demo.py` for an example. Note that commands must subclass `xconf.Command` *and* apply the `@xconf.config` decorator. Options are defined by a hierarchy of dataclasses. (For uninteresting reasons, they aren't *strictly speaking* `import dataclass` dataclasses.)
 
 ## License
 
-All code outside `xconf/vendor/` is provided under the terms of the [MIT License](./LICENSE), except for `demo.py` and `demo_command.conf.toml`, which are released into the public domain for you to build off of.
+All code outside `xconf/vendor/` is provided under the terms of the [MIT License](./LICENSE), except for `xconf_demo.py` and `demo_command.conf`, which are released into the public domain for you to build off of.
 
 Note that code under `xconf/vendor/` is used under the terms of the licenses listed there.
-
-
```

### Comparing `xconf-0.0.1/README.md` & `xconf-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,81 @@
 # `xconf` - Dataclasses and TOML for command configuration
 
 ## Demo
 
-An example of how to use `xconf.Command`, `xconf.field`, and `xconf.config` is in `demo.py`. Run it to see its configuration keys.
+An example of how to use `xconf.Command`, `xconf.field`, and `xconf.config` is in `xconf_demo.py`. Run it to see its configuration keys.
 
 ```
-$ python demo.py demo_command -h
+$ python xconf_demo.py demo_command -h
 demo_command: Demo command
-usage: demo.py demo_command [-c CONFIG_FILE] [-h] [-v] [--dump-config] [vars ...]
+usage: xconf_demo.py demo_command [-c CONFIG_FILE] [-h] [-v] [--dump-config] [vars ...]
 
 positional arguments:
   vars                  Config variables set with 'key.key.key=value' notation
 
 optional arguments:
   -c CONFIG_FILE, --config-file CONFIG_FILE
-                        Path to config file (default: demo_command.conf.toml)
+                        Path to config file (default: demo_command.conf)
   -h, --help            Print usage information
   -v, --verbose         Enable debug logging
   --dump-config         Dump final configuration state as TOML and exit
+
 configuration keys:
   collections
       dict[str, ExtendedThingie]
   collections.<str>.name
       str
+     <ExtendedThingie>
   collections.<str>.extended
       bool
+     <ExtendedThingie>
   either_one
       [int, str]
   should_bar
       bool
      (default: False)
   should_foo
       bool
     Whether demo should foo
   number_list
       list[int]
     List of favorite numbers
+  float_list
+      list[float]
+    List of favorite floating-point numbers
+  str_list
+      list[str]
+    List of favorite strings
   sequence
       list[ExtendedThingie]
+     (default: [])
+  sequence[#].name
+      str
+     <ExtendedThingie>
+  sequence[#].extended
+      bool
+     <ExtendedThingie>
 ```
 
 ### Default config file
 
-The command name, `demo_command`, is generated from the class name and used to find a default configuration file (`demo_command.conf.toml`) in the current directory.
+The command name, `demo_command`, is generated from the class name and used to find a default configuration file (`demo_command.conf`) in the current directory.
 
 ### Providing arguments at the command line
 
 Any configuration key from the help output can be supplied on the command line in a `dotted.name=value` format.
 
 For lists of primitive types (`str`, `int`, `float`), you can just use commas to separate the values on the right hand side of the `=`. Example: `number_list=1,2,3`.
 
 To override a single entry in a list, use `some_name[#]` or `dotted[#].name=value` where `#` is an integer index will work. Example: `number_list[0]=99`
 
 String values are bare (i.e. no quotation marks around `value`). Boolean values are case-insensitive `true`, `t`, or 1 for True, `false`, `f`, or 0 for False.
 
 ### Structuring the command
 
-See `demo.py` for an example. Note that commands must subclass `xconf.Command` *and* apply the `@xconf.config` decorator. Options are defined by a hierarchy of dataclasses. (For uninteresting reasons, they aren't *strictly speaking* `import dataclass` dataclasses.)
+See `xconf_demo.py` for an example. Note that commands must subclass `xconf.Command` *and* apply the `@xconf.config` decorator. Options are defined by a hierarchy of dataclasses. (For uninteresting reasons, they aren't *strictly speaking* `import dataclass` dataclasses.)
 
 ## License
 
-All code outside `xconf/vendor/` is provided under the terms of the [MIT License](./LICENSE), except for `demo.py` and `demo_command.conf.toml`, which are released into the public domain for you to build off of.
+All code outside `xconf/vendor/` is provided under the terms of the [MIT License](./LICENSE), except for `xconf_demo.py` and `demo_command.conf`, which are released into the public domain for you to build off of.
 
 Note that code under `xconf/vendor/` is used under the terms of the licenses listed there.
```

### Comparing `xconf-0.0.1/xconf/__init__.py` & `xconf-0.0.2/xconf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,79 @@
 """Minimal configuration system to populate dataclasses with a
 mix of config files in TOML and command-line arguments"""
 import textwrap
+import pathlib
 import argparse
 import re
 import sys
 import toml
 import logging
 from enum import Enum
 from functools import partial
 import typing
 from toml import encoder
-from .vendor.py310_dataclasses import dataclass, is_dataclass, asdict
+from .vendor.py310_dataclasses import dataclass
 from .vendor import dacite
 from .vendor.dacite import UnexpectedDataError, MissingValueError
 from .vendor import py310_dataclasses as dataclasses
 from collections import defaultdict
 
+__all__ = (
+    'field',
+    'config',
+    'config_to_dict',
+    'dict_to_toml',
+    'config_to_toml',
+    'ConfigMismatch',
+    'Command',
+)
+
 log = logging.getLogger(__name__)
 
 config = partial(dataclass, kw_only=True)
 
 def convert_bool(x):
     if x in (True, False):
         return x
     if x.lower() in ('true', 't', '1'):
         return True
     elif x.lower() in ('false', 'f', '0'):
         return False
     else:
-        raise ValueError(f"Cannot convert {x} to boolean")
+        raise ValueError(f"Cannot convert {repr(x)} to boolean")
 
 
 def convert_list(x, convert_type=lambda x: x):
-    if ',' in x:
-        return [convert_type(y.strip()) for y in x.split(',')]
-    elif isinstance(x, str):
-        return [convert_type(x.strip())]
+    if isinstance(x, str):
+        # handle escaped commas by temporarily replacing with an escaped value
+        x = x.replace(r'\,', '\u0001')
+        out = []
+        for y in x.split(','):
+            val = y.replace('\u0001', ',')
+            try:
+                val = convert_type(val)
+                out.append(val)
+            except ValueError:
+                raise ValueError(f"Could not apply type conversion to {repr(val)} from list {repr(x)}")
     else:
-        return x
+        # type conversion was already handled and x is a list at this point
+        assert isinstance(x, list)
+        out = x
+    return out
 
 TYPE_HOOKS = {
     bool: convert_bool,
     int: int,
     float: float,
     list[str]: partial(convert_list, convert_type=str),
-    # list[int]: partial(convert_list, convert_type=int),
-    # list[float]: partial(convert_list, convert_type=float),
+    list[int]: partial(convert_list, convert_type=int),
+    list[float]: partial(convert_list, convert_type=float),
 }
 from_dict = partial(dacite.from_dict, config=dacite.Config(strict=True, type_hooks=TYPE_HOOKS, cast=[Enum]))
+from_dict.__doc__ = dacite.from_dict.__doc__
 
 
 class TomlEnumEncoder(encoder.TomlEncoder):
     """Encode to TOML, replacing values that are Enum subclasses with their value attribute"""
 
     def dump_value(self, v):
         if isinstance(v, Enum):
@@ -76,18 +98,14 @@
         for key, value in self.items():
             if isinstance(value, self.__class__):
                 out[key] = value.to_plain_dict()
             else:
                 out[key] = value
         return out
 
-def fail(message):
-    log.error(message)
-    sys.exit(1)
-
 def field(*args, **kwargs):
     metadata = None
     if 'help' in kwargs:
         metadata = {'help': kwargs.pop('help')}
     return dataclasses.field(*args, metadata=metadata, **kwargs)
 
 def type_name_or_choices(the_type):
@@ -109,26 +127,31 @@
             name = ''
         else:
             name = type_name_or_choices(field_type)
         members = ', '.join([type_name_or_choices(x) for x in field_type.__args__])
         return f'{name}[{members}]'
     return type_name_or_choices(field_type)
 
+fields = dataclasses.fields
+
 def list_fields(cls, prefix='', help_suffix=''):
     for fld in dataclasses.fields(cls):
         for result in list_one_dataclass_field(fld, prefix, help_suffix):
             yield result
 
 def list_one_dataclass_field(fld : dataclasses.Field, prefix, help_suffix):
     name = fld.name
     field_help = fld.metadata.get('help', '')
     fld_type = fld.type
     default = fld.default
     if not isinstance(fld.default_factory, dataclasses._MISSING_TYPE):
-        default = fld.default_factory()
+        try:
+            default = fld.default_factory()
+        except TypeError:
+            raise TypeError(f"Could not instantiate field {fld} from default factory")
     for result in list_one_field(name, fld_type, field_help, prefix, help_suffix, default=default):
         yield result
 
 def list_one_field(name, fld_type, field_help, prefix, help_suffix, default=dataclasses._MISSING_TYPE):
     if not isinstance(default, dataclasses._MISSING_TYPE):
         if isinstance(default, Enum):
             default_value = repr(default.value)
@@ -136,130 +159,124 @@
             default_value = repr(default)
         field_help += f' (default: {default_value})'
     field_help += help_suffix
     field_type_str = format_field_type(fld_type)
     prefixed_name = prefix + name
     yield prefixed_name, f'{field_type_str}', field_help
 
-    if dacite.types.is_union(fld_type): # and not dacite.types.is_optional(fld.type):
-        members = dacite.types.extract_generic(fld_type)
+    if dacite.types.is_union(fld_type) or dacite.types.is_generic_collection(fld_type):
+        if dacite.types.is_union(fld_type):
+            members = dacite.types.extract_generic(fld_type)
+        else:
+            members = [fld_type]
         for mtype in members:
             if dataclasses.is_dataclass(mtype):
                 for k, v, h in list_fields(mtype, prefix=f'{prefix}{name}.', help_suffix=help_suffix+f' <{mtype.__name__}>'):
                     yield k, v, h
             elif dacite.types.is_generic_collection(mtype):
-                collection_entry_type, = dacite.types.extract_generic(mtype)
-                for k, v, h in list_fields(collection_entry_type, prefix=f'{prefix}{name}[#].', help_suffix=help_suffix+f' <{format_field_type(collection_entry_type)}>'):
-                    yield k, v, h
+                orig_type = dacite.types.extract_origin_collection(mtype)
+                res = dacite.types.extract_generic(mtype)
+                if orig_type is dict: # mapping
+                    collection_key_type, collection_value_type = res
+                    if dataclasses.is_dataclass(collection_value_type):
+                        for k, v, h in list_fields(collection_value_type, prefix=f'{prefix}{name}.<{collection_key_type.__name__}>.', help_suffix=help_suffix+f' <{format_field_type(collection_value_type)}>'):
+                            yield k, v, h
+                    else:
+                        pass # output above with primitive types
+                elif orig_type is list:
+                    collection_entry_type, = res
+                    if dataclasses.is_dataclass(collection_entry_type):
+                        for k, v, h in list_fields(collection_entry_type, prefix=f'{prefix}{name}[#].', help_suffix=help_suffix+f' <{format_field_type(collection_entry_type)}>'):
+                            yield k, v, h
+                    else:
+                        pass # output above with primitive types
+                else:
+                    pass # unhandled parameterized generic collection (tuples? sets?)
             else:
                 # no need for additional docs for primitive types
                 continue
-    elif dacite.types.is_generic_collection(fld_type):
-        if dacite.types.extract_origin_collection(fld_type) is list:
-            # already output above for collection
-            pass
-        else:
-            # dict types
-            key_type, val_type = dacite.types.extract_generic(fld_type)
-            if dataclasses.is_dataclass(val_type):
-                # value is a dataclass, recurse into its fields
-                for k, v, h in list_fields(val_type, prefix=f'{prefix}{name}.<{key_type.__name__}>.'):
-                    yield k, v, h
-            else:
-                if dacite.types.is_union(val_type):
-                    members = dacite.types.extract_generic(val_type)
-                    if any(dataclasses.is_dataclass(m) for m in members):
-                        for mtype in members:
-                            if dataclasses.is_dataclass(val_type):
-                                for k, v, h in list_fields(val_type, prefix=f'{prefix}{name}.<{key_type.__name__}>.', help_suffix=help_suffix+f' <{format_field_type(mtype)}>'):
-                                    yield k, v, h
-                            else:
-                                yield f"{prefixed_name}.<{format_field_type(key_type)}>", format_field_type(mtype), field_help
-                    else:
-                        yield f"{prefixed_name}.<{format_field_type(key_type)}>", format_field_type(val_type), field_help
-                elif dacite.types.is_generic_collection(val_type):
-                    # TODO: when the value itself is generic, recurse into it
-                    pass
     else:
         if dataclasses.is_dataclass(fld_type):
             for k, v, h in list_fields(fld_type, prefix=f'{prefix}{name}.'):
                 yield k, v, h
 
+def add_subparser_arguments(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.add_argument(
+        "-c", "--config-file",
+        action="append",
+        default=[],
+        help=f"Path to config file, repeat to merge multiple, last one wins for repeated top-level keys",
+    )
+    parser.add_argument("-h", "--help", action='store_true', help="Print usage information")
+    parser.add_argument("-v", "--verbose", action='store_true', help="Enable debug logging")
+    parser.add_argument("--dump-config", action='store_true', help="Dump final configuration state as TOML and exit")
+    parser.add_argument("vars", nargs='*', help="Config variables set with 'key.key.key=value' notation")
+    return parser
 
 class Dispatcher:
     def __init__(self, commands):
         self.commands = commands
 
     def configure_logging(self, level):
         logging.basicConfig(level=level)
 
     def main(self):
         parser = argparse.ArgumentParser(add_help=False)
         parser.set_defaults(command_cls=None)
         subps = parser.add_subparsers(title="subcommands", description="valid subcommands")
         names_to_subparsers = {}
         for command_cls in self.commands:
-            if command_cls.name is None or command_cls.name in names_to_subparsers:
+            if command_cls.get_name() is None or command_cls.get_name() in names_to_subparsers:
                 raise Exception(f"Invalid command name for {command_cls}")
-            subp = subps.add_parser(command_cls.name, add_help=False)
-            names_to_subparsers[command_cls.name] = subp
+            subp = subps.add_parser(command_cls.get_name(), add_help=False)
+            names_to_subparsers[command_cls.get_name()] = subp
             subp.set_defaults(command_cls=command_cls)
-            default_config_file = command_cls.default_config_name
-            subp.add_argument(
-                "-c", "--config-file",
-                action="append",
-                default=[],
-                help=f"Path to config file, repeat to merge multiple (default: {default_config_file})",
-            )
-            subp.add_argument("-h", "--help", action='store_true', help="Print usage information")
-            subp.add_argument("-v", "--verbose", action='store_true', help="Enable debug logging")
-            subp.add_argument("--dump-config", action='store_true', help="Dump final configuration state as TOML and exit")
-            subp.add_argument("vars", nargs='*', help="Config variables set with 'key.key.key=value' notation")
+            add_subparser_arguments(subp)
 
         args = parser.parse_args()
         if args.command_cls is None:
             parser.print_help()
             sys.exit(1)
         if args.help:
-            print_help(args.command_cls, names_to_subparsers[args.command_cls.name])
+            print_help(args.command_cls, names_to_subparsers[args.command_cls.get_name()])
             sys.exit(0)
         self.configure_logging('DEBUG' if args.verbose else 'INFO')
         command = args.command_cls.from_args(args)
         if args.dump_config:
-            print(toml.dumps(command.config_to_dict(), encoder=TomlEnumEncoder()))
+            print(config_to_toml(command))
             sys.exit(0)
         return command.main()
 
 def print_help(cls, parser):
-    print(f"{cls.name}: {cls.__doc__}")
+    print(f"{sys.argv[0]}:")
     parser.print_help()
-    print("configuration keys:")
+    print("\nconfiguration keys:")
     fields = list_fields(cls)
     for field_key, field_type, help_text in fields:
         print(f'  {field_key}')
         print(f'      {field_type}')
         if help_text:
             wrapped = textwrap.fill(
                 help_text,
                 initial_indent='    ',
                 subsequent_indent='    '
             )
             print(wrapped)
 
-def _get_config_data(default_config_name, config_file_paths, cli_args):
+def _get_config_data(default_config_path, config_file_paths, cli_args):
+    raw_config = {}
     if len(config_file_paths):
-        raw_config = {}
         for config_file_path in config_file_paths:
             loaded_config = load_config(config_file_path)
             raw_config.update(loaded_config)
-    else:
+    elif default_config_path is not None:
         try:
-            raw_config = load_config(default_config_name)
+            raw_config = load_config(default_config_path)
         except FileNotFoundError:
-            raw_config = {}
+            pass
 
     for non_flag_arg in cli_args:
         lhs, rhs = non_flag_arg.split('=', 1)  # something.foo.bar=value
         key = lhs.split('.') # [something, foo, bar]
         base = raw_config
         for idx, subkey in enumerate(key):
             if idx == len(key) - 1:
@@ -293,35 +310,103 @@
             else:
                 base = base[subkey]
 
 
     log.debug(f'Config attributes provided: {raw_config}')
     return raw_config
 
+def config_to_dict(inst):
+    return dataclasses.asdict(inst)
+
+def dict_to_toml(config_dict):
+    return toml.dumps(config_dict, encoder=TomlEnumEncoder())
+
+def config_to_toml(inst):
+    config_dict = config_to_dict(inst)
+    return dict_to_toml(config_dict)
+
+class ConfigMismatch(Exception):
+    def __init__(self, original_exception: Exception, raw_config: dict):
+        self.original_exception = original_exception
+        self.raw_config = raw_config
+
 @dataclass
 class Command:
     @classmethod
-    @property
-    def name(cls):
+    def get_name(cls):
         name = re.sub(r'(?<!^)(?=[A-Z])', '_', cls.__name__).lower()
         return name
+
+    @classmethod
+    def get_default_config_prefix(cls) -> pathlib.Path:
+        return pathlib.Path('./')
+
     @classmethod
-    @property
-    def default_config_name(cls):
-        return f"{cls.name}.conf.toml"
+    def get_default_config_path(cls) -> pathlib.Path:
+        return cls.get_default_config_prefix() / (cls.get_name() + ".conf")
 
     def config_to_dict(self):
         return dataclasses.asdict(self)
 
     @classmethod
-    def from_args(cls, parsed_args):
-        raw_config = _get_config_data(cls.default_config_name, parsed_args.config_file, parsed_args.vars)
+    def from_config(
+        cls,
+        config_path_or_paths: typing.Union[str,list[str]]=None,
+        config_dict: dict= None,
+        settings_strs: list[str]=None,
+    ):
+        '''Initialize a class instance using config files from disk or a dictionary
+        of options
+
+        Parameters
+        ----------
+        config_path :
+        '''
+
+        config_paths = []
+        if isinstance(config_path_or_paths, str):
+            config_paths.append(config_path_or_paths)
+        elif isinstance(config_path_or_paths, list):
+            config_paths.extend(config_path_or_paths)
+        if settings_strs is None:
+            settings_strs = []
+        raw_config = _get_config_data(cls.get_default_config_path(), config_paths, settings_strs)
+        if config_dict is not None:
+            for key, value in config_dict.items():
+                if key in raw_config:
+                    old_val = raw_config[key]
+                    log.info(f"Using provided value {value} for {key} which was set to {old_val} in the loaded config files")
+            raw_config.update(config_dict)
         try:
-            return from_dict(cls, raw_config)
+            instance = from_dict(cls, raw_config)
         except (UnexpectedDataError, MissingValueError) as e:
-            log.error(f"Applying configuration failed with: {e}")
+            raise ConfigMismatch(e, raw_config)
+        return instance
+
+    @classmethod
+    def run(cls):
+        parser = argparse.ArgumentParser(add_help=False)
+        add_subparser_arguments(parser)
+        args = parser.parse_args()
+        if args.help:
+            print_help(cls, parser)
+            sys.exit(0)
+        logging.basicConfig(level='WARN')
+        logging.getLogger('__main__').setLevel('DEBUG' if args.verbose else 'INFO')
+        command = cls.from_args(args)
+        if args.dump_config:
+            print(config_to_toml(command))
+            sys.exit(0)
+        command.main()
+
+    @classmethod
+    def from_args(cls, parsed_args):
+        try:
+            return cls.from_config(config_path_or_paths=parsed_args.config_file, settings_strs=parsed_args.vars)
+        except ConfigMismatch as e:
+            log.error(f"Applying configuration failed with: {e.original_exception}")
             from pprint import pformat
-            log.error(f"File and arguments provided this configuration:\n\n{pformat(raw_config)}\n")
+            log.error(f"File and arguments provided this configuration:\n\n{pformat(e.raw_config)}\n")
             sys.exit(1)
 
     def main(self):
         raise NotImplementedError("Subclasses must implement main()")
```

### Comparing `xconf-0.0.1/xconf/vendor/dacite/core.py` & `xconf-0.0.2/xconf/vendor/dacite/core.py`

 * *Files identical despite different names*

### Comparing `xconf-0.0.1/xconf/vendor/dacite/dataclasses.py` & `xconf-0.0.2/xconf/vendor/dacite/dataclasses.py`

 * *Files identical despite different names*

### Comparing `xconf-0.0.1/xconf/vendor/dacite/exceptions.py` & `xconf-0.0.2/xconf/vendor/dacite/exceptions.py`

 * *Files identical despite different names*

### Comparing `xconf-0.0.1/xconf/vendor/dacite/types.py` & `xconf-0.0.2/xconf/vendor/dacite/types.py`

 * *Files identical despite different names*

### Comparing `xconf-0.0.1/xconf/vendor/py310_dataclasses.py` & `xconf-0.0.2/xconf/vendor/py310_dataclasses.py`

 * *Files identical despite different names*

### Comparing `xconf-0.0.1/xconf.egg-info/PKG-INFO` & `xconf-0.0.2/xconf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,100 @@
 Metadata-Version: 2.1
 Name: xconf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Turns TOML files and command-line arguments into dataclasses for config
-Home-page: UNKNOWN
 Author: Joseph D. Long
 Author-email: jdl@zesty.space
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: toml>=0.10.2
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Provides-Extra: contrib
+Requires-Dist: fsspec; extra == "contrib"
+Requires-Dist: ray; extra == "contrib"
+Provides-Extra: all
+Requires-Dist: ray; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: fsspec; extra == "all"
 
 # `xconf` - Dataclasses and TOML for command configuration
 
 ## Demo
 
-An example of how to use `xconf.Command`, `xconf.field`, and `xconf.config` is in `demo.py`. Run it to see its configuration keys.
+An example of how to use `xconf.Command`, `xconf.field`, and `xconf.config` is in `xconf_demo.py`. Run it to see its configuration keys.
 
 ```
-$ python demo.py demo_command -h
+$ python xconf_demo.py demo_command -h
 demo_command: Demo command
-usage: demo.py demo_command [-c CONFIG_FILE] [-h] [-v] [--dump-config] [vars ...]
+usage: xconf_demo.py demo_command [-c CONFIG_FILE] [-h] [-v] [--dump-config] [vars ...]
 
 positional arguments:
   vars                  Config variables set with 'key.key.key=value' notation
 
 optional arguments:
   -c CONFIG_FILE, --config-file CONFIG_FILE
-                        Path to config file (default: demo_command.conf.toml)
+                        Path to config file (default: demo_command.conf)
   -h, --help            Print usage information
   -v, --verbose         Enable debug logging
   --dump-config         Dump final configuration state as TOML and exit
+
 configuration keys:
   collections
       dict[str, ExtendedThingie]
   collections.<str>.name
       str
+     <ExtendedThingie>
   collections.<str>.extended
       bool
+     <ExtendedThingie>
   either_one
       [int, str]
   should_bar
       bool
      (default: False)
   should_foo
       bool
     Whether demo should foo
   number_list
       list[int]
     List of favorite numbers
+  float_list
+      list[float]
+    List of favorite floating-point numbers
+  str_list
+      list[str]
+    List of favorite strings
   sequence
       list[ExtendedThingie]
+     (default: [])
+  sequence[#].name
+      str
+     <ExtendedThingie>
+  sequence[#].extended
+      bool
+     <ExtendedThingie>
 ```
 
 ### Default config file
 
-The command name, `demo_command`, is generated from the class name and used to find a default configuration file (`demo_command.conf.toml`) in the current directory.
+The command name, `demo_command`, is generated from the class name and used to find a default configuration file (`demo_command.conf`) in the current directory.
 
 ### Providing arguments at the command line
 
 Any configuration key from the help output can be supplied on the command line in a `dotted.name=value` format.
 
 For lists of primitive types (`str`, `int`, `float`), you can just use commas to separate the values on the right hand side of the `=`. Example: `number_list=1,2,3`.
 
 To override a single entry in a list, use `some_name[#]` or `dotted[#].name=value` where `#` is an integer index will work. Example: `number_list[0]=99`
 
 String values are bare (i.e. no quotation marks around `value`). Boolean values are case-insensitive `true`, `t`, or 1 for True, `false`, `f`, or 0 for False.
 
 ### Structuring the command
 
-See `demo.py` for an example. Note that commands must subclass `xconf.Command` *and* apply the `@xconf.config` decorator. Options are defined by a hierarchy of dataclasses. (For uninteresting reasons, they aren't *strictly speaking* `import dataclass` dataclasses.)
+See `xconf_demo.py` for an example. Note that commands must subclass `xconf.Command` *and* apply the `@xconf.config` decorator. Options are defined by a hierarchy of dataclasses. (For uninteresting reasons, they aren't *strictly speaking* `import dataclass` dataclasses.)
 
 ## License
 
-All code outside `xconf/vendor/` is provided under the terms of the [MIT License](./LICENSE), except for `demo.py` and `demo_command.conf.toml`, which are released into the public domain for you to build off of.
+All code outside `xconf/vendor/` is provided under the terms of the [MIT License](./LICENSE), except for `xconf_demo.py` and `demo_command.conf`, which are released into the public domain for you to build off of.
 
 Note that code under `xconf/vendor/` is used under the terms of the licenses listed there.
-
-
```

### Comparing `xconf-0.0.1/xconf.egg-info/SOURCES.txt` & `xconf-0.0.2/xconf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 ./xconf/vendor/dacite/config.py
 ./xconf/vendor/dacite/core.py
 ./xconf/vendor/dacite/data.py
 ./xconf/vendor/dacite/dataclasses.py
 ./xconf/vendor/dacite/exceptions.py
 ./xconf/vendor/dacite/types.py
 xconf/__init__.py
+xconf/fs.py
 xconf.egg-info/PKG-INFO
 xconf.egg-info/SOURCES.txt
 xconf.egg-info/dependency_links.txt
 xconf.egg-info/requires.txt
 xconf.egg-info/top_level.txt
+xconf/contrib/__init__.py
 xconf/vendor/__init__.py
 xconf/vendor/py310_dataclasses.py
 xconf/vendor/dacite/__init__.py
 xconf/vendor/dacite/config.py
 xconf/vendor/dacite/core.py
 xconf/vendor/dacite/data.py
 xconf/vendor/dacite/dataclasses.py
 xconf/vendor/dacite/exceptions.py
+xconf/vendor/dacite/py.typed
 xconf/vendor/dacite/types.py
```

