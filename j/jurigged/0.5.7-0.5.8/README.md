# Comparing `tmp/jurigged-0.5.7.tar.gz` & `tmp/jurigged-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jurigged-0.5.7.tar", max compression
+gzip compressed data, was "jurigged-0.5.8.tar", max compression
```

## Comparing `jurigged-0.5.7.tar` & `jurigged-0.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1061 2021-01-28 15:43:23.746829 jurigged-0.5.7/LICENSE
--rw-r--r--   0        0        0    12727 2022-05-17 03:33:13.315280 jurigged-0.5.7/README.md
--rw-r--r--   0        0        0      287 2022-05-24 17:12:26.728730 jurigged-0.5.7/jurigged/__init__.py
--rw-r--r--   0        0        0       60 2021-07-15 15:34:09.159592 jurigged-0.5.7/jurigged/__main__.py
--rw-r--r--   0        0        0    33354 2023-11-29 14:37:09.225082 jurigged-0.5.7/jurigged/codetools.py
--rw-r--r--   0        0        0     9917 2023-11-21 01:44:23.287372 jurigged-0.5.7/jurigged/live.py
--rw-r--r--   0        0        0     1456 2021-11-11 01:54:03.509009 jurigged-0.5.7/jurigged/loop/__init__.py
--rw-r--r--   0        0        0     4238 2021-11-11 01:54:03.509101 jurigged-0.5.7/jurigged/loop/basic.py
--rw-r--r--   0        0        0     5702 2023-01-20 02:20:31.677363 jurigged-0.5.7/jurigged/loop/develoop.py
--rw-r--r--   0        0        0    15569 2023-01-31 01:59:13.460305 jurigged-0.5.7/jurigged/loop/richloop.py
--rw-r--r--   0        0        0     2214 2021-03-24 06:08:48.424179 jurigged-0.5.7/jurigged/parse.py
--rw-r--r--   0        0        0     4034 2021-05-27 00:26:39.965265 jurigged-0.5.7/jurigged/recode.py
--rw-r--r--   0        0        0     7149 2023-11-29 14:35:44.886839 jurigged-0.5.7/jurigged/register.py
--rw-r--r--   0        0        0     2984 2022-04-27 21:09:17.534241 jurigged-0.5.7/jurigged/rescript.py
--rw-r--r--   0        0        0    10533 2022-04-27 21:02:17.184975 jurigged-0.5.7/jurigged/runpy.py
--rw-r--r--   0        0        0     1278 2021-11-04 19:33:02.441801 jurigged-0.5.7/jurigged/utils.py
--rw-r--r--   0        0        0       18 2023-11-29 14:57:46.679391 jurigged-0.5.7/jurigged/version.py
--rw-r--r--   0        0        0     1310 2023-11-29 14:57:46.658631 jurigged-0.5.7/pyproject.toml
--rw-r--r--   0        0        0    13717 1970-01-01 00:00:00.000000 jurigged-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2021-01-28 15:43:23.746829 jurigged-0.5.8/LICENSE
+-rw-r--r--   0        0        0    12727 2022-05-17 03:33:13.315280 jurigged-0.5.8/README.md
+-rw-r--r--   0        0        0      287 2024-04-13 23:52:23.560668 jurigged-0.5.8/jurigged/__init__.py
+-rw-r--r--   0        0        0       60 2021-07-15 15:34:09.159592 jurigged-0.5.8/jurigged/__main__.py
+-rw-r--r--   0        0        0    34573 2024-05-30 00:30:20.679538 jurigged-0.5.8/jurigged/codetools.py
+-rw-r--r--   0        0        0    10108 2024-05-30 01:05:16.475828 jurigged-0.5.8/jurigged/live.py
+-rw-r--r--   0        0        0     1456 2021-11-11 01:54:03.509009 jurigged-0.5.8/jurigged/loop/__init__.py
+-rw-r--r--   0        0        0     4238 2021-11-11 01:54:03.509101 jurigged-0.5.8/jurigged/loop/basic.py
+-rw-r--r--   0        0        0     5702 2023-01-20 02:20:31.677363 jurigged-0.5.8/jurigged/loop/develoop.py
+-rw-r--r--   0        0        0    15569 2023-01-31 01:59:13.460305 jurigged-0.5.8/jurigged/loop/richloop.py
+-rw-r--r--   0        0        0     2214 2024-04-13 23:52:23.560948 jurigged-0.5.8/jurigged/parse.py
+-rw-r--r--   0        0        0     4034 2021-05-27 00:26:39.965265 jurigged-0.5.8/jurigged/recode.py
+-rw-r--r--   0        0        0     7149 2023-11-29 14:35:44.886839 jurigged-0.5.8/jurigged/register.py
+-rw-r--r--   0        0        0     2984 2022-04-27 21:09:17.534241 jurigged-0.5.8/jurigged/rescript.py
+-rw-r--r--   0        0        0    10533 2022-04-27 21:02:17.184975 jurigged-0.5.8/jurigged/runpy.py
+-rw-r--r--   0        0        0     1453 2024-05-30 01:08:04.801129 jurigged-0.5.8/jurigged/utils.py
+-rw-r--r--   0        0        0       18 2024-05-30 01:20:14.259546 jurigged-0.5.8/jurigged/version.py
+-rw-r--r--   0        0        0     1313 2024-05-30 01:20:14.233026 jurigged-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0    13717 1970-01-01 00:00:00.000000 jurigged-0.5.8/PKG-INFO
```

### Comparing `jurigged-0.5.7/LICENSE` & `jurigged-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/README.md` & `jurigged-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/codetools.py` & `jurigged-0.5.8/jurigged/codetools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,40 @@
+import __future__
+
 import ast
 import re
+import sys
 from abc import abstractmethod
-from ast import _splitlines_no_ff as splitlines
+from ast import _splitlines_no_ff as _splitlines
 from collections import Counter
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from contextvars import ContextVar
 from dataclasses import dataclass, field, replace as dc_replace
 from types import CodeType, ModuleType
 from typing import List, Optional, Union
 
 from codefind import ConformException, code_registry as codereg, conform
 from ovld import ovld
 
 from .parse import Variables, variables
 from .utils import EventSource, shift_lineno
 
 current_info = ContextVar("current_info", default=None)
+_future_feature_names = set(__future__.all_feature_names)
+
+
+if sys.version_info < (3, 12):  # pragma: no cover
+    splitlines = _splitlines
+else:  # pragma: no cover
+
+    def splitlines(s):
+        lines = _splitlines(s)
+        if len(lines) > 0 and lines[-1] == "":
+            return lines[:-1]
+        return lines
 
 
 sep_at_start = re.compile(r"^ *[\n;]")
 sep_at_end = re.compile(r"[\n;] *$")
 
 
 class StaleException(Exception):
@@ -39,14 +54,37 @@
     def __setitem__(self, item, value):
         return setattr(self.cls, item, value)
 
     def get(self, item, dflt):
         return getattr(self.cls, item, dflt)
 
 
+def _get_future_compiler_flags(glb) -> int:
+    """use future feature names to get any that are set in the global namespace
+
+    `|` these together to get the flags for the compile function
+
+    see the source code for the `__future__` module for more info
+    """
+    flags = 0
+    for key in glb.keys() & _future_feature_names:
+        with suppress(Exception):
+            flags |= glb[key].compiler_flag
+    return flags
+
+
+def _compile_with_flags(node, mode, filename, glb, flags=0):
+    """compile the node with the future flags from the global namespace
+
+    for now that means respect `from __future__ import annotations` if it exists
+    """
+    flags |= _get_future_compiler_flags(glb)
+    return compile(node, mode=mode, filename=filename, flags=flags)
+
+
 @dataclass
 class Info:
     filename: str
     module_name: str
     source: str
     lines: list
     varinfo: Variables = None
@@ -236,15 +274,17 @@
     ##############
     # Evaluation #
     ##############
 
     def evaluate(self, glb, lcl):
         if self.node is not None:
             node = ast.Module(body=[self.node], type_ignores=[])
-            code = compile(node, mode="exec", filename=self.filename)
+            code = _compile_with_flags(
+                node, mode="exec", filename=self.filename, glb=glb
+            )
             code = code.replace(co_name="<adjust>")
             exec(code, glb, lcl)
             codereg.assimilate(
                 code.replace(co_name=""), path=self.codepath(skip=1)
             )
 
     #############
@@ -781,15 +821,17 @@
                 ),
                 new_node,
             )
             ast.fix_missing_locations(wrap)
             node = ast.Module(body=[wrap], type_ignores=[])
         else:
             node = ast.Module(body=[new_node], type_ignores=[])
-        code = compile(node, mode="exec", filename=ext.filename)
+        code = _compile_with_flags(
+            node, mode="exec", filename=ext.filename, glb=glb
+        )
         code = code.replace(co_name="<adjust>")
         exec(code, glb, lcl)
         if closure:
             creator = lcl["##create_closure"]
             # It does not matter what arguments we provide here, because we will move the
             # function's __code__ elsewhere, so it will use a different closure
             new_obj = creator(*names)
```

### Comparing `jurigged-0.5.7/jurigged/live.py` & `jurigged-0.5.8/jurigged/live.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ovld import ovld
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 from watchdog.observers.polling import PollingObserverVFS
 
 from . import codetools, runpy
 from .register import registry
-from .utils import EventSource, glob_filter
+from .utils import EventSource, glob_filter, or_filter
 from .version import version
 
 log = logging.getLogger(__name__)
 T = blessed.Terminal()
 DEFAULT_DEBOUNCE = 0.05
 
 
@@ -150,25 +150,38 @@
     def schedule(self, observer):
         # Watch the directory, because when watching a file, the watcher stops when
         # it is deleted and will not pick back up if the file is recreated. This happens
         # when some editors save.
         observer.schedule(self, os.path.dirname(self.filename))
 
 
+@ovld
+def to_filter(pattern: str):
+    return glob_filter(pattern)
+
+
+@ovld
+def to_filter(patterns: list):
+    return or_filter([to_filter(p) for p in patterns])
+
+
+@ovld
+def to_filter(obj: object):
+    return obj
+
+
 def watch(
     pattern="./*.py",
     logger=default_logger,
     registry=registry,
     autostart=True,
     debounce=DEFAULT_DEBOUNCE,
     poll=False,
 ):
-    registry.auto_register(
-        filter=glob_filter(pattern) if isinstance(pattern, str) else pattern
-    )
+    registry.auto_register(filter=to_filter(pattern))
     registry.set_logger(logger)
     watcher = Watcher(
         registry,
         debounce=debounce,
         poll=poll,
     )
     if autostart:
@@ -246,14 +259,15 @@
         action="store_true",
         help="Run an interactive session after the program ends",
     )
     parser.add_argument(
         "--watch",
         "-w",
         metavar="PATH",
+        action="append",
         help="Wildcard path/directory for which files to watch",
     )
     parser.add_argument(
         "--debounce",
         "-d",
         type=float,
         help="Interval to wait for to refresh a modified file, in seconds",
@@ -303,15 +317,15 @@
         help="Print version",
     )
     parser.add_argument(
         "rest", metavar="...", nargs=argparse.REMAINDER, help="Script arguments"
     )
     opts = parser.parse_args()
 
-    pattern = glob_filter(opts.watch or ".")
+    pattern = to_filter(opts.watch or ".")
     watch_args = {
         "pattern": pattern,
         "logger": default_logger if opts.verbose else conservative_logger,
         "debounce": opts.debounce or DEFAULT_DEBOUNCE,
         "poll": opts.poll,
     }
```

### Comparing `jurigged-0.5.7/jurigged/loop/__init__.py` & `jurigged-0.5.8/jurigged/loop/__init__.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/loop/basic.py` & `jurigged-0.5.8/jurigged/loop/basic.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/loop/develoop.py` & `jurigged-0.5.8/jurigged/loop/develoop.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/loop/richloop.py` & `jurigged-0.5.8/jurigged/loop/richloop.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/parse.py` & `jurigged-0.5.8/jurigged/parse.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/recode.py` & `jurigged-0.5.8/jurigged/recode.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/register.py` & `jurigged-0.5.8/jurigged/register.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/rescript.py` & `jurigged-0.5.8/jurigged/rescript.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/runpy.py` & `jurigged-0.5.8/jurigged/runpy.py`

 * *Files identical despite different names*

### Comparing `jurigged-0.5.7/jurigged/utils.py` & `jurigged-0.5.8/jurigged/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,24 @@
 
     def matcher(filename):
         return fnmatch.fnmatch(filename, pattern)
 
     return matcher
 
 
+def or_filter(filters):
+    if len(filters) == 1:
+        return filters[0]
+
+    def matcher(filename):
+        return any(f(filename) for f in filters)
+
+    return matcher
+
+
 def shift_lineno(co, delta):
     if isinstance(co, types.CodeType):
         return co.replace(
             co_firstlineno=co.co_firstlineno + delta,
             co_consts=tuple(shift_lineno(ct, delta) for ct in co.co_consts),
         )
     else:
```

### Comparing `jurigged-0.5.7/PKG-INFO` & `jurigged-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurigged
-Version: 0.5.7
+Version: 0.5.8
 Summary: Live update of Python functions
 Home-page: https://github.com/breuleux/jurigged
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

