# Comparing `tmp/data-plumber-http-0.3.0.tar.gz` & `tmp/data-plumber-http-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-plumber-http-0.3.0.tar", last modified: Tue Apr 16 21:28:06 2024, max compression
+gzip compressed data, was "data-plumber-http-1.0.0.tar", last modified: Thu May 30 13:29:23 2024, max compression
```

## Comparing `data-plumber-http-0.3.0.tar` & `data-plumber-http-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.590482 data-plumber-http-0.3.0/
--rwxrwxrwx   0 root         (0) root         (0)     1080 2024-01-22 19:31:33.000000 data-plumber-http-0.3.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)    10758 2024-04-16 21:28:06.590299 data-plumber-http-0.3.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     9284 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.581728 data-plumber-http-0.3.0/data_plumber_http/
--rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-14 11:44:45.000000 data-plumber-http-0.3.0/data_plumber_http/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.584313 data-plumber-http-0.3.0/data_plumber_http/decorators/
--rwxrwxrwx   0 root         (0) root         (0)      329 2024-04-14 11:13:20.000000 data-plumber-http-0.3.0/data_plumber_http/decorators/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1503 2024-04-14 22:14:15.000000 data-plumber-http-0.3.0/data_plumber_http/decorators/flask_input.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.585690 data-plumber-http-0.3.0/data_plumber_http/keys/
--rwxrwxrwx   0 root         (0) root         (0)      163 2024-04-14 09:01:26.000000 data-plumber-http-0.3.0/data_plumber_http/keys/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       62 2024-04-14 09:02:00.000000 data-plumber-http-0.3.0/data_plumber_http/keys/all_of.py
--rwxrwxrwx   0 root         (0) root         (0)       62 2024-04-14 09:01:53.000000 data-plumber-http-0.3.0/data_plumber_http/keys/one_of.py
--rwxrwxrwx   0 root         (0) root         (0)     1881 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/keys/property.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.589732 data-plumber-http-0.3.0/data_plumber_http/types/
--rwxrwxrwx   0 root         (0) root         (0)     3983 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/types/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1318 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/data_plumber_http/types/array.py
--rwxrwxrwx   0 root         (0) root         (0)      354 2024-04-14 22:13:32.000000 data-plumber-http-0.3.0/data_plumber_http/types/boolean.py
--rwxrwxrwx   0 root         (0) root         (0)     3094 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/data_plumber_http/types/file_system_object.py
--rwxrwxrwx   0 root         (0) root         (0)     1608 2024-04-14 20:05:12.000000 data-plumber-http-0.3.0/data_plumber_http/types/float.py
--rwxrwxrwx   0 root         (0) root         (0)     1603 2024-04-14 20:04:49.000000 data-plumber-http-0.3.0/data_plumber_http/types/integer.py
--rwxrwxrwx   0 root         (0) root         (0)      383 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/types/null.py
--rwxrwxrwx   0 root         (0) root         (0)      908 2024-04-14 22:13:42.000000 data-plumber-http-0.3.0/data_plumber_http/types/number.py
--rwxrwxrwx   0 root         (0) root         (0)    13793 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/types/object.py
--rwxrwxrwx   0 root         (0) root         (0)     1500 2024-04-14 22:13:52.000000 data-plumber-http-0.3.0/data_plumber_http/types/string.py
--rwxrwxrwx   0 root         (0) root         (0)     2093 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/data_plumber_http/types/url.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.583613 data-plumber-http-0.3.0/data_plumber_http.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    10758 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      864 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       76 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-16 21:28:06.590571 data-plumber-http-0.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1924 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:29:23.609618 data-plumber-http-1.0.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1080 2024-01-22 19:31:33.000000 data-plumber-http-1.0.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       35 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)    18741 2024-05-30 13:29:23.609419 data-plumber-http-1.0.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    16179 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:29:23.598169 data-plumber-http-1.0.0/data_plumber_http/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-26 20:00:04.000000 data-plumber-http-1.0.0/data_plumber_http/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:29:23.601224 data-plumber-http-1.0.0/data_plumber_http/decorators/
+-rwxrwxrwx   0 root         (0) root         (0)      329 2024-04-14 11:13:20.000000 data-plumber-http-1.0.0/data_plumber_http/decorators/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1508 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/decorators/flask_input.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:29:23.603437 data-plumber-http-1.0.0/data_plumber_http/keys/
+-rwxrwxrwx   0 root         (0) root         (0)      999 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/keys/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5698 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/keys/all_of.py
+-rwxrwxrwx   0 root         (0) root         (0)     2365 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/keys/conditional_key.py
+-rwxrwxrwx   0 root         (0) root         (0)     6764 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/keys/one_of.py
+-rwxrwxrwx   0 root         (0) root         (0)     6978 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/keys/property.py
+-rwxrwxrwx   0 root         (0) root         (0)      694 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/output.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/py.typed
+-rwxrwxrwx   0 root         (0) root         (0)     4522 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:29:23.608768 data-plumber-http-1.0.0/data_plumber_http/types/
+-rwxrwxrwx   0 root         (0) root         (0)     2576 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      429 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/any.py
+-rwxrwxrwx   0 root         (0) root         (0)     1327 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/array.py
+-rwxrwxrwx   0 root         (0) root         (0)      356 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/boolean.py
+-rwxrwxrwx   0 root         (0) root         (0)     3555 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/file_system_object.py
+-rwxrwxrwx   0 root         (0) root         (0)     3600 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/float.py
+-rwxrwxrwx   0 root         (0) root         (0)     3599 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/integer.py
+-rwxrwxrwx   0 root         (0) root         (0)      375 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/null.py
+-rwxrwxrwx   0 root         (0) root         (0)     1695 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/number.py
+-rwxrwxrwx   0 root         (0) root         (0)    10876 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/object.py
+-rwxrwxrwx   0 root         (0) root         (0)     1550 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/string.py
+-rwxrwxrwx   0 root         (0) root         (0)     2159 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/uri.py
+-rwxrwxrwx   0 root         (0) root         (0)     2144 2024-05-30 13:23:09.000000 data-plumber-http-1.0.0/data_plumber_http/types/url.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 13:29:23.600396 data-plumber-http-1.0.0/data_plumber_http.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    18741 2024-05-30 13:29:23.000000 data-plumber-http-1.0.0/data_plumber_http.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2024-05-30 13:29:23.000000 data-plumber-http-1.0.0/data_plumber_http.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-30 13:29:23.000000 data-plumber-http-1.0.0/data_plumber_http.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       24 2024-05-30 13:29:23.000000 data-plumber-http-1.0.0/data_plumber_http.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-30 13:29:23.000000 data-plumber-http-1.0.0/data_plumber_http.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-30 13:29:23.609710 data-plumber-http-1.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1966 2024-05-30 13:29:06.000000 data-plumber-http-1.0.0/setup.py
```

### Comparing `data-plumber-http-0.3.0/LICENSE` & `data-plumber-http-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.3.0/data_plumber_http/decorators/flask_input.py` & `data-plumber-http-1.0.0/data_plumber_http/decorators/flask_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from typing import Callable
 from functools import wraps
 
 from flask import request, Response
 from data_plumber import Pipeline
 
-from data_plumber_http.types import Responses
+from data_plumber_http.settings import Responses
 
 
 def flask_args():
     return request.args
 
 
 def flask_form():
@@ -51,15 +51,15 @@
 
     def decorator(view):
         @wraps(view)
         def wrapped(*args, **kwargs):
             output = handler.run(
                 json=json()
             )
-            if output.last_status != Responses.GOOD.status:
+            if output.last_status != Responses().GOOD.status:
                 return Response(
                     response=output.last_message,
                     status=output.last_status,
                     mimetype="text/plain"
                 )
             return view(*args, **(kwargs | output.data.value))
         return wrapped
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http/types/array.py` & `data-plumber-http-1.0.0/data_plumber_http/types/array.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Optional
 
-from . import _DPType, Responses
+from . import DPType, Responses
 
 
-class Array(_DPType):
+class Array(DPType):
     """
     An `Array` corresponds to the JSON-type 'array'.
 
     Keyword arguments:
     items -- type specification for items of this `Array`
              (default `None`; accept any content)
     """
     TYPE = list
 
-    def __init__(self, items: Optional[_DPType] = None):
+    def __init__(self, items: Optional[DPType] = None):
         self._items = items
 
     def make(self, json, loc: str) -> tuple[Any, str, int]:
         if self._items is None:
             return (
                 json,
-                Responses.GOOD.msg,
-                Responses.GOOD.status
+                Responses().GOOD.msg,
+                Responses().GOOD.status
             )
         array = []
         for element in json:
             if not isinstance(element, self._items.TYPE):
                 return (
                     None,
                     f"Element in '{loc}' has bad type. Expected "
                     + f"'{self._items.__name__}' but found "
                     + f"'{type(element).__name__}'.",
-                    Responses.BAD_TYPE.status
+                    Responses().BAD_TYPE.status
                 )
             child = self._items.make(element, loc)
-            if child[2] != Responses.GOOD.status:
+            if child[2] != Responses().GOOD.status:
                 return (None, child[1], child[2])
             array.append(child[0])
         return (
             array,
-            Responses.GOOD.msg,
-            Responses.GOOD.status
+            Responses().GOOD.msg,
+            Responses().GOOD.status
         )
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http/types/file_system_object.py` & `data-plumber-http-1.0.0/data_plumber_http/types/file_system_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, Optional, Callable
+from typing import Any, Optional
 from pathlib import Path
 
-from . import _DPType, Responses
+from . import DPType, Responses
 
 
-class FileSystemObject(_DPType):
+class FileSystemObject(DPType):
     """
     A `FileSystemObject` corresponds to a `pathlib.Path` that is given
     either absolute or relative to the cwd. The output is a
     `pathlib.Path`-object.
 
     Keyword arguments:
     relative_to -- make call to `pathlib.Path.relative_to` before
@@ -56,36 +56,46 @@
         path = Path(json)
         if self._relative_to is not None:
             try:
                 path = path.relative_to(self._relative_to)
             except ValueError as exc_info:
                 return (
                     None,
-                    Responses.BAD_VALUE.msg.format(
-                        json,
-                        loc,
-                        f"path relative to '{self._relative_to}' ({exc_info})"
+                    Responses().BAD_VALUE.msg.format(
+                        origin=json,
+                        loc=loc,
+                        expected=f"path relative to '{self._relative_to}' ({exc_info})"
                     ),
-                    Responses.BAD_VALUE.status
+                    Responses().BAD_VALUE.status
                 )
         if self._cwd is not None:
             path = self._cwd / path
         for step, req in self._validation_map.items():
             if req is None:
                 continue
             if getattr(path, step)() != req:
                 if req:
+                    if path.exists():
+                        return (
+                            None,
+                            Responses().BAD_RESOURCE.msg.format(
+                                res=json, loc=loc, details=f"expected '{step}'"
+                            ),
+                            Responses().BAD_RESOURCE.status
+                        )
                     return (
                         None,
-                        Responses.RESOURCE_NOT_FOUND.msg.format(json, loc),
-                        Responses.RESOURCE_NOT_FOUND.status
+                        Responses().RESOURCE_NOT_FOUND.msg.format(
+                            res=json, loc=loc
+                        ),
+                        Responses().RESOURCE_NOT_FOUND.status
                     )
                 return (
                     None,
-                    Responses.CONFLICT.msg.format(json, loc),
-                    Responses.CONFLICT.status
+                    Responses().CONFLICT.msg.format(res=json, loc=loc),
+                    Responses().CONFLICT.status
                 )
         return (
             path,
-            Responses.GOOD.msg,
-            Responses.GOOD.status
+            Responses().GOOD.msg,
+            Responses().GOOD.status
         )
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http/types/float.py` & `data-plumber-http-1.0.0/data_plumber_http/types/url.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 from typing import Any, Optional
+from urllib.parse import urlparse
 
-from . import _DPType, Responses
+from . import DPType, Responses
 
 
-class Float(_DPType):
+class Url(DPType):
     """
-    A `Float` represents a floating point number.
+    A `Url` essentially is a `String` which has to match a url-format of
+    `<scheme>://<netloc>/<path>;<params>?<query>#<fragment>`. The output
+    is either a string or a named tuple (see `return_parsed`).
 
     Keyword arguments:
-    values -- list of values allowed in this field
-              (default `None`)
-    range_ -- tuple of lower and upper bound for values in this field
-              (default `None`)
+    schemes -- list of strings that are accepted as url-schemes
+               (default `None` (accept any))
+    require_netloc -- if `True`, only urls with non-empty netloc are
+                      accepted
+                      (default `False`)
+    return_parsed -- if `True`, returns a named tuple as generated by
+                     `urllib.parse.urlparse` instead of string
+                     (default `False`)
     """
-    TYPE = float
+    TYPE = str
 
     def __init__(
         self,
-        values: Optional[list[float]] = None,
-        range_: Optional[tuple[int | float, int | float]] = None
+        schemes: Optional[list[str]] = None,
+        require_netloc: bool = False,
+        return_parsed: bool = False
     ):
-        self._values = values
-        self._range = range_
+        self._schemes = schemes
+        self._require_netloc = require_netloc
+        self._return_parsed = return_parsed
 
     def make(self, json, loc: str) -> tuple[Any, str, int]:
-        # validate values
-        if self._values is not None \
-                and json not in self._values:
+        url = urlparse(json)
+        if self._schemes is not None and url.scheme not in self._schemes:
             return (
                 None,
-                Responses.BAD_VALUE.msg.format(
-                    json,
-                    loc,
-                    "one of " + ", ".join(f"'{v}'" for v in self._values)
+                Responses().BAD_VALUE.msg.format(
+                    origin=json,
+                    loc=loc,
+                    expected="scheme to be "
+                    + ("one of " if len(self._schemes) > 1 else "")
+                    + ", ".join(f"'{v}'" for v in self._schemes)
                 ),
-                Responses.BAD_VALUE.status
+                Responses().BAD_VALUE.status
             )
-        # validate range
-        if self._range is not None \
-                and (json < self._range[0] or json > self._range[1]):
+        if self._require_netloc and url.netloc == "":
             return (
                 None,
-                Responses.BAD_VALUE.msg.format(
-                    json,
-                    loc,
-                    f"a number in the range [{self._range[0]}, {self._range[1]}]"
+                Responses().BAD_VALUE.msg.format(
+                    origin=json,
+                    loc=loc,
+                    expected="non-empty netloc"
                 ),
-                Responses.BAD_VALUE.status
+                Responses().BAD_VALUE.status
             )
         return (
-            self.TYPE(json),
-            Responses.GOOD.msg,
-            Responses.GOOD.status
+            url if self._return_parsed else json,
+            Responses().GOOD.msg,
+            Responses().GOOD.status
         )
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http/types/object.py` & `data-plumber-http-1.0.0/data_plumber_http/types/object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,79 @@
-from typing import TypeAlias, Mapping, Optional, Any
+from typing import TypeAlias, Mapping, Optional, Callable, Any
 
 from data_plumber import Pipeline, Stage
+from data_plumber.output import StageRecord
 
-from data_plumber_http.keys import _DPKey, Property
-from . import _DPType, Responses, Output
+from data_plumber_http.output import Output
+from data_plumber_http.keys import DPKey, Property
+from . import DPType, Responses
 
 
-Properties: TypeAlias = Mapping[_DPKey, "_DPType | Properties"]
+Properties: TypeAlias = Mapping[DPKey, "DPType | Properties"]
 
 
-class Object(_DPType):
+class Object(DPType):
     """
     An `Object` corresponds to the JSON-type 'object'.
 
     Keyword arguments:
-    model -- data model for this `Object` (gets passed the entire output
-             of a validation-run as kwargs)
+    model -- data model or factory for this `Object` (gets passed the
+             entire output of a validation-run as kwargs)
              (default `None`; corresponds to dictionary)
     properties -- mapping for explicitly expected contents of this
                   `Object`
                   (default `None`)
-    additional_properties -- type for implicitly expected contents of
-                             this `Object` (mutually exclusive with
-                             `accept_only`)
-                             (default `None`)
-    accept_only -- if set, on execution a `json` is rejected with 400
-                   status if it contains a key that is not in
-                   `accept_only` (mutually exclusive with
-                   `additional_properties`)
+
+    Mutually exclusive arguments:
+    additional_properties -- either boolean or field type (`DPType`)
+                             boolean: if `True`, ignore any additional
+                             fields; if `False`, respond with
+                             `Responses().UNKNOWN_PROPERTY` for fields
+                             that are not listed in `properties`
+                             type: required type specification for
+                             implicitly expected contents of this
+                             `Object`; corresponding fields in `json`
+                             are added to the output
+                             (default `None`; treated like `True`)
+    accept_only -- if set, on execution a `json` is rejected with
+                   `Responses().UNKNOWN_PROPERTY` if it contains a key
+                   that is not in `accept_only`
                    (default `None`)
     free_form -- if `True`, accept and use any content that has not been
                  defined explicitly via `properties`
                  (default `False`)
     """
     TYPE = dict
 
     def __init__(
         self,
-        model: Optional[type] = None,
+        model: Optional[type | Callable[..., Any]] = None,
         properties: Optional[Properties] = None,
-        additional_properties: Optional[_DPType] = None,
+        additional_properties: Optional[bool | DPType] = None,
         accept_only: Optional[list[str]] = None,
         free_form: bool = False
     ) -> None:
         self._model = model or dict
-        self._properties = properties or {}
+        self.properties = properties or {}
 
-        if properties is not None \
-                and len(set(k.name for k in properties.keys())) < len(properties):
+        if properties is not None:
+            _properties: Optional[list[Property]] = list(
+                k for k in properties.keys() if isinstance(k, Property)
+            )
+        else:
+            _properties = properties
+        if _properties is not None \
+                and len(set(k.name for k in _properties)) < len(_properties):
             names = set()
             raise ValueError(
                 "Conflicting property name(s) in Object: "
                 + str(
                     [
-                        k.name for k in properties.keys()
-                        if k.name in names or names.add(k.name)
+                        k.name for k in _properties
+                        if k.name in names or names.add(k.name)  # type: ignore [func-returns-value]
                     ]
                 )
             )
 
         if additional_properties and accept_only:
             raise ValueError(
                 f"Value of 'additional_properties' ({additional_properties}) "
@@ -70,177 +85,88 @@
                 + f"conflicts with value of 'free_form' ({free_form})."
             )
         if accept_only and free_form:
             raise ValueError(
                 f"Value of 'accept_only' ({accept_only}) "
                 + f"conflicts with value of 'free_form' ({free_form})."
             )
-        self._additional_properties = additional_properties
-        self._accept_only = accept_only
         self._free_form = free_form
+        self._accept_only = accept_only
+        if isinstance(additional_properties, bool):
+            self._additional_properties = additional_properties
+            self._additional_properties_typespec = None
+            if not additional_properties:
+                self._accept_only = list(set().union(
+                    *[
+                        k.get_origins(v)
+                        for k, v in properties.items()
+                    ]
+                )) if properties is not None else []
+        else:
+            self._additional_properties = True
+            self._additional_properties_typespec = additional_properties
 
     @staticmethod
     def _reject_unknown_args(accepted, loc):
         return Stage(
             primer=lambda json, **kwargs: next(
                 (k for k in json.keys() if k not in accepted),
                 None
             ),
             status=lambda primer, **kwargs:
-                Responses.GOOD.status if not primer
-                else Responses.UNKNOWN_PROPERTY.status,
-            message=lambda primer, **kwargs:
-                Responses.GOOD.msg if not primer
-                else Responses.UNKNOWN_PROPERTY.msg.format(
-                    primer,
-                    loc,
-                    ", ".join(map(lambda x: f"'{x}'", accepted))
-                )
-        )
-
-    @staticmethod
-    def _arg_exists_hard(k, loc):
-        return Stage(
-            primer=lambda json, **kwargs: k.origin in json,
-            status=lambda primer, **kwargs:
-                Responses.GOOD.status if primer
-                else Responses.MISSING_REQUIRED.status,
-            message=lambda primer, **kwargs:
-                Responses.GOOD.msg if primer
-                else Responses.MISSING_REQUIRED.msg.format(
-                    loc,
-                    k.origin
-                )
-        )
-
-    @staticmethod
-    def _arg_exists_soft(k):
-        return Stage(
-            primer=lambda json, **kwargs: k.origin in json,
-            status=lambda primer, **kwargs:
-                Responses.GOOD.status if primer
-                else Responses.MISSING_OPTIONAL.status,
+                Responses().GOOD.status if not primer
+                else Responses().UNKNOWN_PROPERTY.status,
             message=lambda primer, **kwargs:
-                "" if primer else Responses.MISSING_OPTIONAL.msg
-        )
-
-    @staticmethod
-    def _arg_has_type(k, v, loc):
-        return Stage(
-            requires={k.name: Responses.GOOD.status},
-            primer=lambda json, **kwargs: isinstance(json[k.origin], v.TYPE),
-            status=lambda primer, **kwargs:
-                Responses.GOOD.status if primer else Responses.BAD_TYPE.status,
-            message=lambda primer, json, **kwargs:
-                Responses.GOOD.msg if primer
-                else Responses.BAD_TYPE.msg.format(
-                    k.origin,
-                    loc,
-                    v.__name__,
-                    type(json[k.origin]).__name__
+                Responses().GOOD.msg if not primer
+                else Responses().UNKNOWN_PROPERTY.msg.format(
+                    origin=primer,
+                    loc=loc,
+                    accepted="accepted: " + ", ".join(map(lambda x: f"'{x}'", accepted))
+                        if len(accepted) > 0 else "none accepted"
                 )
         )
 
     @staticmethod
-    def _make_instance(k, v, loc):
-        return Stage(
-            requires={k.name: Responses.GOOD.status},
-            primer=lambda json, **kwargs:
-                v.make(json[k.origin], loc),
-            export=lambda primer, **kwargs:
-                {f"EXPORT_{k.name}": primer[0]}
-                if primer[2] == Responses.GOOD.status
-                else {},
-            status=lambda primer, **kwargs: primer[2],
-            message=lambda primer, **kwargs: primer[1]
-        )
-
-    @staticmethod
-    def _set_default(k):
-        if k.default is not None:
-            # default is set
-            return Stage(
-                requires={k.name: Responses.MISSING_OPTIONAL.status},
-                primer=k.default
-                    if callable(k.default)
-                    else lambda **kwargs: k.default,
-                export=lambda primer, **kwargs:
-                    {f"EXPORT_{k.name}": primer},
-                status=lambda **kwargs: Responses.GOOD.status,
-                message=lambda **kwargs: Responses.GOOD.msg
-            )
-        # default to None or omit completely
-        return Stage(
-            requires={k.name: Responses.MISSING_OPTIONAL.status},
-            export=lambda primer, **kwargs:
-                {f"EXPORT_{k.name}": None}
-                if k.fill_with_none
-                else {},
-            status=lambda **kwargs: Responses.GOOD.status,
-            message=lambda **kwargs: Responses.GOOD.msg
-        )
-
-    @staticmethod
-    def _output(k):
-        return Stage(
-            primer=lambda **kwargs:
-                f"EXPORT_{k.name}" in kwargs,
-            action=lambda out, primer, **kwargs:
-                [
-                    out.update({"kwargs": {}})
-                    if "kwargs" not in out
-                    else None,
-                    out.kwargs.update(
-                        {k.name: kwargs.get(f"EXPORT_{k.name}")}
-                        if primer
-                        else {}
-                    )
-                ],
-            status=lambda **kwargs: Responses.GOOD.status,
-            message=lambda **kwargs: Responses.GOOD.msg
-        )
-
-    @staticmethod
     def _process_additional_properties(keys, dptype, loc):
         """
         Defines a `Stage` in which an `Object`-based `Pipeline` is built
         and executed. The `Object` contains `Properties` which appear in
         the `json` but not as `Property` in the original `Object`. This
         way, the given fields in the `json` can be validated regarding
         their type.
 
         Keyword arguments:
         keys -- list of field names defined in the original `Object`
-        dptype -- `_DPType` of the additional properties
+        dptype -- `DPType` of the additional properties
         loc -- position in original `json`
         """
         return Stage(
             primer=lambda json, **kwargs: Object(
                     properties={
                         Property(k): dptype for k in additional
                     }
                 ).assemble(loc).run(json=json)
                 if len(
                     additional := [k for k in json.keys() if k not in keys]
                 ) > 0
                 else None,  # return None if Object is empty > simply return with
-                            # Responses.GOOD
+                            # Responses().GOOD
             action=lambda out, primer, **kwargs:
                 [
                     out.update({"kwargs": {}})
                     if "kwargs" not in out
                     else None,
                     out.kwargs.update(primer.data.get("kwargs", {}))
                 ]
-                if primer and primer.last_status == Responses.GOOD.status
+                if primer and primer.last_status == Responses().GOOD.status
                 else None,
             status=lambda primer, **kwargs:
-                primer.last_status if primer else Responses.GOOD.status,
+                primer.last_status if primer else Responses().GOOD.status,
             message=lambda primer, **kwargs:
-                primer.last_message if primer else Responses.GOOD.msg,
+                primer.last_message if primer else Responses().GOOD.msg,
         )
 
     @staticmethod
     def _process_free_form(keys):
         """
         Defines a `Stage` that collects the json-content that is not
         defined as `Properties` in the original `Object` and adds those
@@ -255,116 +181,98 @@
             action=lambda out, primer, **kwargs:
                 [
                     out.update({"kwargs": {}})
                     if "kwargs" not in out
                     else None,
                     out.kwargs.update(primer)
                 ],
-            status=lambda **kwargs: Responses.GOOD.status,
-            message=lambda **kwargs: Responses.GOOD.msg,
+            status=lambda **kwargs: Responses().GOOD.status,
+            message=lambda **kwargs: Responses().GOOD.msg,
         )
 
     def make(self, json, loc: str) -> tuple[Any, str, int]:
         """
         Validate and instantiate type based on `json`.
 
         Returns with a tuple of
         * object if valid or None,
         * problem description if invalid,
-        * status code (`Responses.GOOD` if valid)
+        * status code (`Responses().GOOD` if valid)
 
         Keyword arguments:
         json -- data to generate object from
         loc -- current location in validation process for generating
                informative messages
         """
         output = self.assemble(loc).run(json=json)
         return (
             (
                 output.data.value
-                if output.last_status == Responses.GOOD.status
+                if output.last_status == Responses().GOOD.status
                 else None
             ),
-            output.last_message or Responses.GOOD.msg,
-            output.last_status or Responses.GOOD.status
+            output.last_message or Responses().GOOD.msg,
+            output.last_status or Responses().GOOD.status
         )
 
     def assemble(self, _loc: Optional[str] = None) -> Pipeline:
         """
         Returns `Pipeline` that processes a `json`-input.
         """
         def finalizer(data, records, **kwargs):
-            if records[-1].status == Responses.GOOD.status:
-                data.value = self._model(**data.kwargs)
+            try:
+                if records[-1].status == Responses().GOOD.status:
+                    data.value = self._model(**data.kwargs)
+            except IndexError:  # empty Object
+                records.append(StageRecord(
+                    0, "finalizer", Responses().GOOD.msg, Responses().GOOD.status
+                ))
+                data.value = self._model()
         p = Pipeline(
             exit_on_status=lambda status: status >= 400,
             initialize_output=Output,
             finalize_output=finalizer
         )
         __loc = _loc or "."
         if self._accept_only is not None:
             p.append(
                 __loc,
                 **{__loc: self._reject_unknown_args(self._accept_only, __loc)}
             )
-        elif self._additional_properties is not None:
+        if self._additional_properties_typespec is not None:
             # additional properties
             p.append(
                 f"{__loc}[additionalProperties]",
                 **{
                     f"{__loc}[additionalProperties]":
                         self._process_additional_properties(
-                            [k.origin for k in self._properties.keys()],
-                            self._additional_properties,
+                            list(set().union(
+                                *[
+                                    k.get_origins(v)
+                                    for k, v in self.properties.items()
+                                ]
+                            )),
+                            self._additional_properties_typespec,
                             _loc
                         )
                 }
             )
-        elif self._free_form:
+        if self._free_form:
             # free-form
             p.append(
                 f"{__loc}[freeForm]",
                 **{
                     f"{__loc}[freeForm]":
                         self._process_free_form(
-                            [k.origin for k in self._properties.keys()]
+                            list(set().union(
+                                *[
+                                    k.get_origins(v)
+                                    for k, v in self.properties.items()
+                                ]
+                            ))
                         )
                 }
             )
-        for k, v in self._properties.items():
-            # k.name: validate existence
-            if k.required and k.default is None:
-                p.append(
-                    k.name,
-                    **{k.name: self._arg_exists_hard(k, __loc)}
-                )
-            else:
-                p.append(k.name, **{k.name: self._arg_exists_soft(k)})
-            # {k.name}[type]: validate type
-            p.append(
-                f"{k.name}[type]",
-                **{f"{k.name}[type]": self._arg_has_type(k, v, __loc)}
-            )
-            # {k.name}[dptype]: validate, make, and export instance as
-            #                   f"EXPORT_{k.name}" (if valid)
-            p.append(
-                f"{k.name}[dptype]",
-                **{f"{k.name}[dptype]": self._make_instance(
-                    k, v, (_loc or "") + "." + k.origin
-                )}
-            )
-            if k.validation_only:
-                continue
-            # {k.name}[default]: apply default if required (or set None
-            #   if property has fill_with_none set) and export as
-            #   f"EXPORT_{k.name}"
-            p.append(
-                f"{k.name}[default]",
-                **{f"{k.name}[default]": self._set_default(k)}
-            )
-            # {k.name}[output]: output to data
-            p.append(
-                f"{k.name}[output]",
-                **{f"{k.name}[output]": self._output(k)}
-            )
+        for k, v in self.properties.items():
+            p.append(k.assemble(v, _loc))
 
         return p
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http/types/string.py` & `data-plumber-http-1.0.0/data_plumber_http/types/string.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional
 import re
 
-from . import _DPType, Responses
+from . import DPType, Responses
 
 
-class String(_DPType):
+class String(DPType):
     """
     A `String` corresponds to the JSON-type 'string'.
 
     Keyword arguments:
     pattern -- regex-pattern that the value of this field has to match
                (default `None`)
     enum -- list of allowed values for this field
@@ -26,29 +26,29 @@
 
     def make(self, json, loc: str) -> tuple[Any, str, int]:
         # validate pattern
         if self._pattern is not None \
                 and not re.fullmatch(self._pattern, json):
             return (
                 None,
-                Responses.BAD_VALUE.msg.format(
-                    json, loc, f"pattern '{self._pattern}'"
+                Responses().BAD_VALUE.msg.format(
+                    origin=json, loc=loc, expected=f"pattern '{self._pattern}'"
                 ),
-                Responses.BAD_VALUE.status
+                Responses().BAD_VALUE.status
             )
         # validate enum
         if self._enum is not None \
                 and json not in self._enum:
             return (
                 None,
-                Responses.BAD_VALUE.msg.format(
-                    json,
-                    loc,
-                    "one of " + ", ".join(f"'{v}'" for v in self._enum)
+                Responses().BAD_VALUE.msg.format(
+                    origin=json,
+                    loc=loc,
+                    expected="one of " + ", ".join(f"'{v}'" for v in self._enum)
                 ),
-                Responses.BAD_VALUE.status
+                Responses().BAD_VALUE.status
             )
         return (
             self.TYPE(json),
-            Responses.GOOD.msg,
-            Responses.GOOD.status
+            Responses().GOOD.msg,
+            Responses().GOOD.status
         )
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http/types/url.py` & `data-plumber-http-1.0.0/data_plumber_http/types/uri.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from typing import Any, Optional
 from urllib.parse import urlparse
 
-from . import _DPType, Responses
+from . import DPType, Responses
 
 
-class Url(_DPType):
+class Uri(DPType):
     """
-    A `Url` essentially is a `String` which has to match a url-format of
-    `<scheme>://<netloc>/<path>;<params>?<query>#<fragment>`. The output
+    A `Uri` essentially is a `String` which has to match a uri-format of
+    `<scheme>://<authority>/<path>?<query>#<fragment>`. The output
     is either a string or a named tuple (see `return_parsed`).
 
     Keyword arguments:
-    schemes -- list of string that are accepted as url-schemes
+    schemes -- list of strings that are accepted as uri-schemes
                (default `None` (accept any))
-    require_netloc -- if `True`, only urls with non-empty netloc are
-                      accepted
+    require_authority -- if `True`, only uris with non-empty authority
+                      are accepted
                       (default `False`)
     return_parsed -- if `True`, returns a named tuple as generated by
                      `urllib.parse.urlparse` instead of string
                      (default `False`)
     """
     TYPE = str
 
     def __init__(
         self,
         schemes: Optional[list[str]] = None,
-        require_netloc: bool = False,
+        require_authority: bool = False,
         return_parsed: bool = False
     ):
         self._schemes = schemes
-        self._require_netloc = require_netloc
+        self._require_authority = require_authority
         self._return_parsed = return_parsed
 
     def make(self, json, loc: str) -> tuple[Any, str, int]:
-        url = urlparse(json)
-        if self._schemes is not None and url.scheme not in self._schemes:
+        uri = urlparse(json)
+        if self._schemes is not None and uri.scheme not in self._schemes:
             return (
                 None,
-                Responses.BAD_VALUE.msg.format(
-                    json,
-                    loc,
-                    "scheme to be "
+                Responses().BAD_VALUE.msg.format(
+                    origin=json,
+                    loc=loc,
+                    expected="scheme to be "
                     + ("one of " if len(self._schemes) > 1 else "")
                     + ", ".join(f"'{v}'" for v in self._schemes)
                 ),
-                Responses.BAD_VALUE.status
+                Responses().BAD_VALUE.status
             )
-        if self._require_netloc and url.netloc == "":
+        if self._require_authority and uri.netloc == "":
             return (
                 None,
-                Responses.BAD_VALUE.msg.format(
-                    json,
-                    loc,
-                    "non-empty netloc"
+                Responses().BAD_VALUE.msg.format(
+                    origin=json,
+                    loc=loc,
+                    expected="non-empty authority"
                 ),
-                Responses.BAD_VALUE.status
+                Responses().BAD_VALUE.status
             )
         return (
-            url if self._return_parsed else json,
-            Responses.GOOD.msg,
-            Responses.GOOD.status
+            uri if self._return_parsed else json,
+            Responses().GOOD.msg,
+            Responses().GOOD.status
         )
```

### Comparing `data-plumber-http-0.3.0/data_plumber_http.egg-info/SOURCES.txt` & `data-plumber-http-1.0.0/data_plumber_http.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 data_plumber_http/__init__.py
+data_plumber_http/output.py
+data_plumber_http/py.typed
+data_plumber_http/settings.py
 data_plumber_http.egg-info/PKG-INFO
 data_plumber_http.egg-info/SOURCES.txt
 data_plumber_http.egg-info/dependency_links.txt
 data_plumber_http.egg-info/requires.txt
 data_plumber_http.egg-info/top_level.txt
 data_plumber_http/decorators/__init__.py
 data_plumber_http/decorators/flask_input.py
 data_plumber_http/keys/__init__.py
 data_plumber_http/keys/all_of.py
+data_plumber_http/keys/conditional_key.py
 data_plumber_http/keys/one_of.py
 data_plumber_http/keys/property.py
 data_plumber_http/types/__init__.py
+data_plumber_http/types/any.py
 data_plumber_http/types/array.py
 data_plumber_http/types/boolean.py
 data_plumber_http/types/file_system_object.py
 data_plumber_http/types/float.py
 data_plumber_http/types/integer.py
 data_plumber_http/types/null.py
 data_plumber_http/types/number.py
 data_plumber_http/types/object.py
 data_plumber_http/types/string.py
+data_plumber_http/types/uri.py
 data_plumber_http/types/url.py
```

### Comparing `data-plumber-http-0.3.0/setup.py` & `data-plumber-http-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,38 +18,41 @@
 requirements = \
     (Path(__file__).parent / "requirements.txt") \
         .read_text(encoding="utf8") \
         .strip() \
         .split("\n")
 
 setup(
-    version="0.3.0",
+    version="1.0.0",
     name="data-plumber-http",
     description="http extension for the data-plumber python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Steffen Richters-Finger",
     author_email="srichters@uni-muenster.de",
     license="MIT",
     license_files=("LICENSE",),
     url="https://pypi.org/project/data-plumber-http/",
     project_urls={
         "Source": "https://github.com/RichtersFinger/data-plumber-http"
     },
     python_requires=">=3.10",
     install_requires=requirements,
-    extras_require={
-        "tests": ["pytest>=7.4,<8", "pytest-cov>=4.1,<5", "flask>=3"],
-    },
     packages=[
         "data_plumber_http",
         "data_plumber_http.types",
         "data_plumber_http.keys",
         "data_plumber_http.decorators",
     ],
+    package_data={
+        "data_plumber_http": [
+            "data_plumber_http/py.typed",
+        ],
+    },
+    include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```

