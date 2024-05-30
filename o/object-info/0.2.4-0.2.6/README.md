# Comparing `tmp/object_info-0.2.4.tar.gz` & `tmp/object_info-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object_info-0.2.4.tar", last modified: Fri May  3 12:14:50 2024, max compression
+gzip compressed data, was "object_info-0.2.6.tar", last modified: Thu May 30 13:18:29 2024, max compression
```

## Comparing `object_info-0.2.4.tar` & `object_info-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 12:14:50.608662 object_info-0.2.4/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 object_info-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    13531 2024-05-03 12:14:50.608409 object_info-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    12576 2024-05-03 12:10:10.000000 object_info-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 12:14:50.599773 object_info-0.2.4/object_info/
--rw-rw-rw-   0        0        0       21 2023-11-27 14:37:20.000000 object_info-0.2.4/object_info/__init__.py
--rw-rw-rw-   0        0        0    17571 2024-05-03 12:08:45.000000 object_info-0.2.4/object_info/main.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:14:50.606792 object_info-0.2.4/object_info.egg-info/
--rw-rw-rw-   0        0        0    13531 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 12:14:50.610176 object_info-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 object_info-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:18:29.127586 object_info-0.2.6/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 object_info-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0    13531 2024-05-30 13:18:29.127586 object_info-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12576 2024-05-30 13:17:43.000000 object_info-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 13:18:29.121356 object_info-0.2.6/object_info/
+-rw-rw-rw-   0        0        0      775 2024-05-30 10:58:52.000000 object_info-0.2.6/object_info/__init__.py
+-rw-rw-rw-   0        0        0    14756 2024-05-30 13:17:39.000000 object_info-0.2.6/object_info/object_info.py
+-rw-rw-rw-   0        0        0     3859 2024-05-30 13:17:39.000000 object_info-0.2.6/object_info/type_checker.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:18:29.126915 object_info-0.2.6/object_info.egg-info/
+-rw-rw-rw-   0        0        0    13531 2024-05-30 13:18:29.000000 object_info-0.2.6/object_info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-30 13:18:29.000000 object_info-0.2.6/object_info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:18:29.000000 object_info-0.2.6/object_info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 13:18:29.000000 object_info-0.2.6/object_info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:18:29.128630 object_info-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 object_info-0.2.6/setup.py
```

### Comparing `object_info-0.2.4/LICENSE` & `object_info-0.2.6/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 Copyright (c) 2023 Andrei Starichenko
 
+IMPORTANT: SEE ADDITIONAL DEPENDANT LICENSES FROM LIST OF USED PROJECTS FROM REQUIREMENTS.TXT!
+
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
 the following conditions:
```

### Comparing `object_info-0.2.4/PKG-INFO` & `object_info-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object_info
-Version: 0.2.4
+Version: 0.2.6
 Summary: print info about object (attributes+properties+methods results)
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/object_info
 Keywords: object info,object attributes,object properties,object methods,print attributes,print properties,print methods
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# object_info (v0.2.4)
+# object_info (v0.2.6)
 
 ## DESCRIPTION_SHORT
 print info about object (attributes+properties+methods results)
 
 ## DESCRIPTION_LONG
 Designed to print info about object (properties+methods results)
```

### Comparing `object_info-0.2.4/README.md` & `object_info-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# object_info (v0.2.4)
+# object_info (v0.2.6)
 
 ## DESCRIPTION_SHORT
 print info about object (attributes+properties+methods results)
 
 ## DESCRIPTION_LONG
 Designed to print info about object (properties+methods results)
```

### Comparing `object_info-0.2.4/object_info/main.py` & `object_info-0.2.6/object_info/object_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,17 @@
 from typing import *
 import re
 # from enum import Enum
 from dataclasses import dataclass, astuple, asdict, field
 
-
-# =====================================================================================================================
-pass
+from .type_checker import *
 
 
 # =====================================================================================================================
-class TypeChecker:
-    TYPES_ELEMENTARY_SINGLE: tuple = (
-        type(None), bool,
-        str, bytes,
-        int, float,
-    )
-    TYPES_ELEMENTARY_COLLECTION: tuple = (
-        tuple, list,
-        set, dict,
-    )
-    TYPES_ELEMENTARY: tuple = (*TYPES_ELEMENTARY_SINGLE, *TYPES_ELEMENTARY_COLLECTION,)
-
-    @staticmethod
-    def check__name_is_build_in(name: str) -> bool:
-        return name.startswith("__") and name.endswith("__")
-
-    @staticmethod
-    def check__iterable(
-            # self,
-            source: Any,
-            dict_as_iterable: bool = True,
-            str_and_bytes_as_iterable: bool = True,
-    ) -> bool:
-        """checks if SOURCE is iterable.
-
-        :param source: SOURCE data
-        :param dict_as_iterable: if you dont want to use dict in your selecting,
-            becouse maybe you need flatten all elements in list/set/tuple into one sequence
-            and dict (as extended list) will be irrelevant!
-        :param str_and_bytes_as_iterable: usually in data processing you need to work with str-type elements as OneSolid element
-            but not iterating through chars!
-        """
-        if isinstance(source, dict):
-            return dict_as_iterable
-        elif isinstance(source, (str, bytes)):
-            return str_and_bytes_as_iterable
-        elif isinstance(source, (tuple, list, set,)):  # need to get it explicitly!!!
-            return True
-        elif hasattr(source, '__iter__') or hasattr(source, '__getitem__'):
-            return True
-
-        # FINAL ---------------------
-        return False
-
-    @staticmethod
-    def check__iterable_but_not_str(source):
-        """checks if SOURCE is iterable, but not exactly str!!!"""
-        return TypeChecker.check__iterable(source, str_and_bytes_as_iterable=False)
-
-    @staticmethod
-    def check__elementary(source) -> bool:
-        return isinstance(source, TypeChecker.TYPES_ELEMENTARY)
-
-    @staticmethod
-    def check__elementary_single(source) -> bool:
-        return isinstance(source, TypeChecker.TYPES_ELEMENTARY_SINGLE)
-
-    @staticmethod
-    def check__elementary_collection(source) -> bool:
-        return isinstance(source, TypeChecker.TYPES_ELEMENTARY_COLLECTION)
-
-    @staticmethod
-    def check__elementary_collection_not_dict(source) -> bool:
-        return isinstance(source, TypeChecker.TYPES_ELEMENTARY_COLLECTION) and not isinstance(source, dict)
-
-    @staticmethod
-    def check__Exception(source) -> bool:
-        return isinstance(source, Exception)
-
-    @staticmethod
-    def check__Object(source) -> bool:
-        return not TypeChecker.check__elementary(source) and not TypeChecker.check__Exception(source)
+pass
 
 
 # =====================================================================================================================
 def _value_search_by_list(source=None, search_list=[]):
     match_item = None
 
     for search_item in search_list:
@@ -275,15 +202,15 @@
                 attr_is_method = True
                 try:
                     value = value()
                 except Exception as exx:
                     self.ITEM.METHODS__EXX.update({name: exx})
                     continue
 
-            # print(f"{name=}/{attr_obj=}/type={type(attr_obj)}/elementary={isinstance(attr_obj, TYPES_ELEMENTARY)}")
+            # print(f"{name=}/{attr_obj=}/type={type(attr_obj)}/elementary={isinstance(attr_obj, TYPES__ELEMENTARY)}")
 
             # PLACE VALUE ---------------------------------------------------------------------
             if TypeChecker.check__elementary_single(value):
                 if attr_is_method:
                     self.ITEM.METHODS__ELEMENTARY_SINGLE.update({name: value})
                 else:
                     self.ITEM.PROPERTIES__ELEMENTARY_SINGLE.update({name: value})
@@ -331,28 +258,28 @@
 
         _block_intend = "\t" * intend
 
         # -------------------------------
         block_value = f"{value}"
         if isinstance(value, ItemInternal):
             block_type = f"{value.KEY}:{value.VALUE}"
-        elif TypeChecker.check__Exception(value):
+        elif TypeChecker.check__exception(value):
             block_value = f"{value!r}"
 
         # -------------------------------
         result = f"{block_name:20}\t{block_type:12}:{_block_intend}{block_value}"
 
         if self.MAX_LINE_LEN and len(result) > self.MAX_LINE_LEN:
             result = result[:self.MAX_LINE_LEN - 3*2] + "..."
 
         # --------------------------------------------------------------------------------------
         print(result)
 
         # -------------------------------
-        if name and TypeChecker.check__Object(value):
+        if name and TypeChecker.check__instance(value):
             # additional print for object
             self._print_line__name_type_value(name=None, type_replace="__repr()", value=f"{value!r}")
 
         return result
 
     # =================================================================================================================
     def _print_block__head(self) -> None:
@@ -382,16 +309,16 @@
         self._print_line__name_type_value(name=name, value=value)
         if len(str(value)) <= self.MAX_LINE_LEN:
             return
 
         # SINGLE/EXX/OBJECTS ---------------------------------------------------------------------
         if any([
             TypeChecker.check__elementary_single(value),
-            TypeChecker.check__Exception(value),
-            TypeChecker.check__Object(value),
+            TypeChecker.check__exception(value),
+            TypeChecker.check__instance(value),
         ]):
             pass
 
         # COLLECTION -----------------------------------------------------------------------------
         if TypeChecker.check__elementary_collection(value):
             # start some pretty style -------------------------------------
             if not isinstance(value, dict):
```

### Comparing `object_info-0.2.4/object_info.egg-info/PKG-INFO` & `object_info-0.2.6/object_info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object_info
-Version: 0.2.4
+Version: 0.2.6
 Summary: print info about object (attributes+properties+methods results)
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/object_info
 Keywords: object info,object attributes,object properties,object methods,print attributes,print properties,print methods
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# object_info (v0.2.4)
+# object_info (v0.2.6)
 
 ## DESCRIPTION_SHORT
 print info about object (attributes+properties+methods results)
 
 ## DESCRIPTION_LONG
 Designed to print info about object (properties+methods results)
```

### Comparing `object_info-0.2.4/setup.py` & `object_info-0.2.6/setup.py`

 * *Files identical despite different names*

