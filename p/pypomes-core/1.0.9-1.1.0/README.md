# Comparing `tmp/pypomes_core-1.0.9.tar.gz` & `tmp/pypomes_core-1.1.0.tar.gz`

## Comparing `pypomes_core-1.0.9.tar` & `pypomes_core-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24938 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/PKG-INFO
```

### Comparing `pypomes_core-1.0.9/src/pypomes_core/.ruff.toml` & `pypomes_core-1.1.0/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/__init__.py` & `pypomes_core-1.1.0/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/email_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/env_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/file_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/json_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/list_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/str_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.1.0/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/validation_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,54 +9,43 @@
 VALIDATION_MSG_PREFIX: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_PREFIX", APP_PREFIX)
 
 
 def validate_value(attr: str,
                    val: str | int | float,
                    min_val: int = None,
                    max_val: int = None,
-                   default: bool | list[Any] = None) -> str:
+                   values: list[Any] = None,
+                   mandatory: bool = False) -> str:
     """
     Validate *val* according to value, range, or membership in values list, as specified.
 
     :param attr: the name of the attribute
     :param val: the value to be validated
     :param min_val: if val is a string, specifies its minimum length; otherwise, specifies its minimum value
     :param max_val: if val is a string, specifies its maximum length; otherwise, specifies its maximum value
-    :param default: if boolean, requires val to be specified; if list, requires val to be in it
+    :param values: if provided, requires 'val' to be in it
+    :param mandatory:  requires 'val' to be specified;
     :return: None if val passes validation, or the corresponding error message otherwise
     """
     # initialize the return variable
     result: str | None = None
 
-    # 'val' can be None, and None can be in 'default'
-    if isinstance(default, list):
-        if val not in default:
-            if not val:
-                # 112: Required attribute
-                result = validate_format_error(112, f"@{attr}")
-            else:
-                length: int = len(default)
-                if length == 1:
-                    # 125: Invalid value {}: must be {}
-                    result = validate_format_error(125, val, default[0], f"@{attr}")
-                else:
-                    # is 'None' or '' the last element in list ?
-                    if default[-1] in ("", None):
-                        # yes, omit it from the message
-                        length -= 1
-                    # again, is 'None' or '' the last element in list ?
-                    if default[-1] in ("", None):
-                        # yes, omit it from the message
-                        length -= 1
-                    # 126: Invalid value {}: must be one of {}
-                    result = validate_format_error(126, val, default[:length], f"@{attr}")
-    elif not val:
-        if isinstance(default, bool) and default:
+    if val is None or val == "":
+        if isinstance(mandatory, bool) and mandatory:
             # 112: Required attribute
             result = validate_format_error(112, f"@{attr}")
+    elif isinstance(values, list):
+        if val not in values:
+            length: int = len(values)
+            if length == 1:
+                # 125: Invalid value {}: must be {}
+                result = validate_format_error(125, val, values[0], f"@{attr}")
+            else:
+                # 126: Invalid value {}: must be one of {}
+                result = validate_format_error(126, val, values[:length], f"@{attr}")
     elif isinstance(val, str):
         length: int = len(val)
         if min_val is not None and max_val == min_val and length != min_val:
             # 124: Invalid value {}: length must be {}
             result = validate_format_error(124, val, min_val, f"@{attr}")
         elif max_val is not None and max_val < length:
             # 123: Invalid value {}: length longer than {}
@@ -84,317 +73,340 @@
                   attr: str,
                   default: bool = None,
                   mandatory: bool = False,
                   logger: Logger = None) -> bool:
     """
     Validate the boolean value associated with *attr* in *scheme*.
 
-    If provided, this value must be a *bool*, or the string *t*, *true*, *f*, or *false*.
+    If provided, this value must be on of:
+        - a *bool*
+        - the string *1*, *t*, or *true*
+        - the string *0*, *f*, or *false*
+        - the integer *1* or *0*
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the name of the attribute whose value is being validated
-    :param default: default value, if not found
-    :param mandatory: specifies whether the value must be provided
+    :param default: default value, overiding 'mandatory'
+    :param mandatory: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
+    # initialize the return variable
+    result: bool | None = None
+
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
-    result = scheme.get(suffix)
+    value = scheme.get(suffix)
 
     # validate it
-    if result is None or result == "":
+    if value is None or value == "":
         if default is not None:
-            result = default
+            value = default
         elif mandatory:
             # 112: Required attribute
             stat = validate_format_error(112, f"@{attr}")
-    elif isinstance(result, str):
-        if result.lower() in ["t", "true"]:
-            result = True
-        elif result.lower() in ["f", "false"]:
-            result = False
-    elif not isinstance(result, bool):
+    elif isinstance(value, str):
+        if value.lower() in ["1", "t", "true"]:
+            value = True
+        elif value.lower() in ["0", "f", "false"]:
+            value = False
+        else:
+            # 128: Invalid value {}: must be type {}
+            stat = validate_format_error(128, value, "bool", f"@{attr}")
+    # bool is subtype of int
+    elif isinstance(value, int) and not isinstance(value, bool):
+        if value == 1:
+            value = True
+        elif value == 0:
+            value = False
+        else:
+            # 128: Invalid value {}: must be type {}
+            stat = validate_format_error(128, value, "bool", f"@{attr}")
+    elif not isinstance(value, bool):
         # 128: Invalid value {}: must be type {}
-        stat = validate_format_error(128, result, "bool", f"@{attr}")
+        stat = validate_format_error(128, value, "bool", f"@{attr}")
 
     if stat:
         __validate_log(errors, stat, logger)
+    else:
+        result = value
 
     return result
 
 
 def validate_int(errors: list[str] | None,
                  scheme: dict,
                  attr: str,
                  min_val: int = None,
                  max_val: int = None,
-                 default: bool | int | list[int] = None,
+                 default: int | list[int] = None,
+                 mandatory: bool = False,
                  logger: Logger = None) -> int:
     """
     Validate the *int* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *int*, or a valid string representation of a *int*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param min_val: the minimum value accepted
     :param max_val:  the maximum value accepted
-    :param default: if int, specifies the default value;
-                    if bool, requires the value to be specified;
-                    if list, requires the value to be in it
+    :param default: if 'int', specifies the default value, overriding the other constraints
+                    if 'list', requires the value, if provided, to be in it
+    :param mandatory: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
+    # initialize the return variable
+    result: int | None = None
+
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
-    result: int | None = scheme.get(suffix)
-
-    # handle the empty string
-    if result == "":
-        result = None
+    value: int = scheme.get(suffix)
 
     # validate it
-    if isinstance(result, str) and result.isnumeric():
-        result = int(result)
-    # bool is subtype of int
-    elif result is not None and \
-            (isinstance(result, bool) or not isinstance(result, int)):
+    if value is None and isinstance(default, int):
+        value = default
+    # 'bool' is subtype of 'int'
+    elif value is not None and \
+         (isinstance(value, bool) or not isinstance(value, int)):
         # 128: Invalid value {}: must be type {}
-        stat = validate_format_error(128, result, "int", f"@{attr}")
-    elif isinstance(default, int) and not isinstance(default, bool):
-        if result is None:
-            result = default
-        else:
-            stat = validate_value(attr, result, min_val, max_val)
+        stat = validate_format_error(128, value, "int", f"@{attr}")
     else:
-        stat = validate_value(attr, result, min_val, max_val, default)
-
-    if not stat:
-        stat = validate_value(attr, result, min_val, max_val, default)
+        if isinstance(value, str) and value.isnumeric():
+            value = int(value)
+        values = default if isinstance(default, list) else None
+        stat = validate_value(attr, value, min_val, max_val, values, mandatory)
 
     if stat:
         __validate_log(errors, stat, logger)
+    else:
+        result = value
 
     return result
 
 
 def validate_float(errors: list[str] | None,
                    scheme: dict,
                    attr: str,
                    min_val: float = None,
                    max_val: float = None,
-                   default: bool | int | float | list[float | int] = None,
+                   mandatory: bool = False,
+                   default: int | float | list[float | int] = None,
                    logger: Logger = None) -> float:
     """
     Validate the *float* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *float*, or a valid string representation of a *float*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param min_val: the minimum value accepted
     :param max_val:  the maximum value accepted
-    :param default: if float, specifies the default value;
-                    if bool, requires the value to be specified;
-                    if list, requires the value to be in it
+    :param default: if 'float' or 'int', specifies the default value, overriding the other constraints
+                    if 'list', requires the value, if provided, to be in it
+    :param mandatory: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
+    # initialize the return variable
+    result: float | None = None
+
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
-    result: float | None = scheme.get(suffix)
-
-    # handle the empty string
-    if result == "":
-        result = None
+    value: float = scheme.get(suffix)
 
     # validate it
-    if isinstance(result, str) and result.replace(".", "", 1).isnumeric():
-        result = float(result)
-    elif result is not None and not isinstance(result, int) and not isinstance(result, float):
+    if value is None and isinstance(default, int | float):
+        value = float(default)
+    elif isinstance(value, bool) or \
+         value is not None and not isinstance(value, int | float):
         # 128: Invalid value {}: must be type {}
-        stat = validate_format_error(128, result, "float", f"@{attr}")
+        stat = validate_format_error(128, value, "float", f"@{attr}")
     else:
-        # bool é subtipo de int
-        if isinstance(result, int) and not isinstance(result, bool):
-            result = float(result)
-        if isinstance(default, float):
-            if result is None:
-                result = default
-            else:
-                stat = validate_value(attr, result, min_val, max_val)
-        else:
-            stat = validate_value(attr, result, min_val, max_val, default)
-
-    if not stat:
-        stat = validate_value(attr, result, min_val, max_val, default)
+        if (isinstance(value, int) and not isinstance(value, bool)) or \
+           (isinstance(value, str) and value.replace(".", "", 1).isnumeric()):
+            value = float(value)
+        values = default if isinstance(default, list) else None
+        stat = validate_value(attr, value, min_val, max_val, values, mandatory)
 
     if stat:
         __validate_log(errors, stat, logger)
+    else:
+        result = value
 
     return result
 
 
 def validate_str(errors: list[str] | None,
                  scheme: dict,
                  attr: str,
                  min_length: int = None,
                  max_length: int = None,
-                 default: bool | str | list[str] = None,
+                 default: str | list[str] = None,
+                 mandatory: bool = False,
                  logger: Logger = None) -> str:
     """
     Validate the *str* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *str*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param min_length: the minimum length accepted
     :param max_length:  the maximum length accepted
-    :param default: if str, specifies the default value;
-                    if bool, requires the value to be specified;
-                    if list, requires the value to be in it
+    :param default: if 'str', specifies the default value, overrinding the other constraints
+                    if 'list', requires the value, if provided, to be in it
+    :param mandatory: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
+    # initialize the return variable
+    result: str | None = None
+
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
-    # obtain and validate the value
-    result: str | None = scheme.get(suffix)
-    if result and not isinstance(result, str):
+    # obtain the value
+    value: str | None = scheme.get(suffix)
+
+    # validate it
+    if value is None and isinstance(default, str):
+        value = default
+    elif value is not None and not isinstance(value, str):
         # 128: Invalid value {}: must be type {}
-        stat = validate_format_error(128, result, "str", f"@{attr}")
-    elif isinstance(default, str):
-        if result is None:
-            result = default
-        else:
-            stat = validate_value(attr, result, min_length, max_length)
+        stat = validate_format_error(128, value, "str", f"@{attr}")
     else:
-        stat = validate_value(attr, result, min_length, max_length, default)
+        values = default if isinstance(default, list) else None
+        stat = validate_value(attr, value, min_length, max_length, values, mandatory)
 
     if stat:
-        result = None
         __validate_log(errors, stat, logger)
+    else:
+        result = value
 
     return result
 
 
 def validate_date(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
                   day_first: bool = False,
-                  default: bool | date = None,
+                  default: date = None,
+                  mandatory: bool = False,
                   logger: Logger = None) -> date:
     """
     Validate the *date* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *date*, or a valid string representation of a *date*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param day_first: indicates that the day precedes the month in the string representing the date
-    :param default: if date, specifies the default value;
-                    if bool, requires the value to be specified
+    :param default: optional default value, overrides 'mandatory'
+    :param mandatory: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # import needed module
     from .datetime_pomes import date_parse
 
     # initialize the return variable
     result: date | None = None
 
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
-    # obtain and validate the value
-    date_str: str = scheme.get(suffix)
-    if date_str:
-        result = date_parse(date_str, dayfirst=day_first)
+    # obtain the value
+    value: str = scheme.get(suffix)
+
+    # validate it
+    if value:
+        result = date_parse(value, dayfirst=day_first)
         if not result:
             # 121: Invalid value {}
-            stat = validate_format_error(121, date_str, f"@{attr}")
+            stat = validate_format_error(121, value, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL).date():
             # 129: Invalid value {}: date is later than the current date
-            stat = validate_format_error(129, date_str, f"@{attr}")
-    elif isinstance(default, bool) and default:
-        # 112: Required attribute
-        stat = validate_format_error(112, f"@{attr}")
+            stat = validate_format_error(129, value, f"@{attr}")
     elif isinstance(default, date):
         result = default
+    elif isinstance(mandatory, bool) and mandatory:
+        # 112: Required attribute
+        stat = validate_format_error(112, f"@{attr}")
 
     if stat:
+        result = None
         __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_datetime(errors: list[str] | None,
                       scheme: dict,
                       attr: str,
                       day_first: bool = True,
-                      default: bool | datetime = None,
+                      default: datetime = None,
+                      mandatory: bool = False,
                       logger: Logger = None) -> datetime:
     """
     Validate the *datetime* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *date*, or a valid string representation of a *date*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param day_first: indicates that the day precedes the month in the string representing the date
-    :param default: if datetime, specifies the default value;
-                    if bool, requires the value to be specified
+    :param default: optional default value, overrides 'mandatory'
+    :param mandatory: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # import needed module
     from .datetime_pomes import datetime_parse
 
     # initialize the return variable
     result: datetime | None = None
 
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
-    date_str: str = scheme[suffix]
-    if date_str:
-        result = datetime_parse(date_str, dayfirst=day_first)
+    value: str = scheme[suffix]
+    if value:
+        result = datetime_parse(value, dayfirst=day_first)
         if not result:
             # 121: Invalid value {}
-            stat = validate_format_error(121, date_str, f"@{attr}")
+            stat = validate_format_error(121, value, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL):
             # 129: Invalid value {}: date is later than the current date
-            stat = validate_format_error(129, date_str, f"@{attr}")
-    elif isinstance(default, bool) and default:
+            stat = validate_format_error(129, value, f"@{attr}")
+    elif isinstance(default, datetime):
+        result = default
+    elif isinstance(mandatory, bool) and mandatory:
         # 112: Required attribute
         stat = validate_format_error(112, f"@{attr}")
-    elif isinstance(default, datetime):
-            result = default
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypomes_core-1.0.9/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.1.0/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/LICENSE` & `pypomes_core-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.9/pyproject.toml` & `pypomes_core-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.9/PKG-INFO` & `pypomes_core-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.9
+Version: 1.1.0
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

