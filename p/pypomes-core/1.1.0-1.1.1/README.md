# Comparing `tmp/pypomes_core-1.1.0.tar.gz` & `tmp/pypomes_core-1.1.1.tar.gz`

## Comparing `pypomes_core-1.1.0.tar` & `pypomes_core-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24938 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.1/PKG-INFO
```

### Comparing `pypomes_core-1.1.0/src/pypomes_core/.ruff.toml` & `pypomes_core-1.1.1/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/__init__.py` & `pypomes_core-1.1.1/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/email_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/env_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/file_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/json_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/list_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/str_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.1.1/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/validation_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 
 
 def validate_value(attr: str,
                    val: str | int | float,
                    min_val: int = None,
                    max_val: int = None,
                    values: list[Any] = None,
-                   mandatory: bool = False) -> str:
+                   required: bool = False) -> str:
     """
     Validate *val* according to value, range, or membership in values list, as specified.
 
     :param attr: the name of the attribute
     :param val: the value to be validated
     :param min_val: if val is a string, specifies its minimum length; otherwise, specifies its minimum value
     :param max_val: if val is a string, specifies its maximum length; otherwise, specifies its maximum value
     :param values: if provided, requires 'val' to be in it
-    :param mandatory:  requires 'val' to be specified;
+    :param required:  requires 'val' to be specified;
     :return: None if val passes validation, or the corresponding error message otherwise
     """
     # initialize the return variable
     result: str | None = None
 
     if val is None or val == "":
-        if isinstance(mandatory, bool) and mandatory:
+        if isinstance(required, bool) and required:
             # 112: Required attribute
             result = validate_format_error(112, f"@{attr}")
     elif isinstance(values, list):
         if val not in values:
             length: int = len(values)
             if length == 1:
                 # 125: Invalid value {}: must be {}
@@ -68,30 +68,30 @@
     return result
 
 
 def validate_bool(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
                   default: bool = None,
-                  mandatory: bool = False,
+                  required: bool = False,
                   logger: Logger = None) -> bool:
     """
     Validate the boolean value associated with *attr* in *scheme*.
 
     If provided, this value must be on of:
         - a *bool*
         - the string *1*, *t*, or *true*
         - the string *0*, *f*, or *false*
         - the integer *1* or *0*
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the name of the attribute whose value is being validated
-    :param default: default value, overiding 'mandatory'
-    :param mandatory: specifies whether a value must be provided
+    :param default: default value, overiding 'required'
+    :param required: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # initialize the return variable
     result: bool | None = None
 
     stat: str | None = None
@@ -101,15 +101,15 @@
     # retrieve the value
     value = scheme.get(suffix)
 
     # validate it
     if value is None or value == "":
         if default is not None:
             value = default
-        elif mandatory:
+        elif required:
             # 112: Required attribute
             stat = validate_format_error(112, f"@{attr}")
     elif isinstance(value, str):
         if value.lower() in ["1", "t", "true"]:
             value = True
         elif value.lower() in ["0", "f", "false"]:
             value = False
@@ -139,29 +139,29 @@
 
 def validate_int(errors: list[str] | None,
                  scheme: dict,
                  attr: str,
                  min_val: int = None,
                  max_val: int = None,
                  default: int | list[int] = None,
-                 mandatory: bool = False,
+                 required: bool = False,
                  logger: Logger = None) -> int:
     """
     Validate the *int* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *int*, or a valid string representation of a *int*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param min_val: the minimum value accepted
     :param max_val:  the maximum value accepted
     :param default: if 'int', specifies the default value, overriding the other constraints
                     if 'list', requires the value, if provided, to be in it
-    :param mandatory: specifies whether a value must be provided
+    :param required: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # initialize the return variable
     result: int | None = None
 
     stat: str | None = None
@@ -179,45 +179,45 @@
          (isinstance(value, bool) or not isinstance(value, int)):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, value, "int", f"@{attr}")
     else:
         if isinstance(value, str) and value.isnumeric():
             value = int(value)
         values = default if isinstance(default, list) else None
-        stat = validate_value(attr, value, min_val, max_val, values, mandatory)
+        stat = validate_value(attr, value, min_val, max_val, values, required)
 
     if stat:
         __validate_log(errors, stat, logger)
     else:
         result = value
 
     return result
 
 
 def validate_float(errors: list[str] | None,
                    scheme: dict,
                    attr: str,
                    min_val: float = None,
                    max_val: float = None,
-                   mandatory: bool = False,
+                   required: bool = False,
                    default: int | float | list[float | int] = None,
                    logger: Logger = None) -> float:
     """
     Validate the *float* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *float*, or a valid string representation of a *float*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param min_val: the minimum value accepted
     :param max_val:  the maximum value accepted
     :param default: if 'float' or 'int', specifies the default value, overriding the other constraints
                     if 'list', requires the value, if provided, to be in it
-    :param mandatory: specifies whether a value must be provided
+    :param required: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # initialize the return variable
     result: float | None = None
 
     stat: str | None = None
@@ -235,15 +235,15 @@
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, value, "float", f"@{attr}")
     else:
         if (isinstance(value, int) and not isinstance(value, bool)) or \
            (isinstance(value, str) and value.replace(".", "", 1).isnumeric()):
             value = float(value)
         values = default if isinstance(default, list) else None
-        stat = validate_value(attr, value, min_val, max_val, values, mandatory)
+        stat = validate_value(attr, value, min_val, max_val, values, required)
 
     if stat:
         __validate_log(errors, stat, logger)
     else:
         result = value
 
     return result
@@ -251,29 +251,29 @@
 
 def validate_str(errors: list[str] | None,
                  scheme: dict,
                  attr: str,
                  min_length: int = None,
                  max_length: int = None,
                  default: str | list[str] = None,
-                 mandatory: bool = False,
+                 required: bool = False,
                  logger: Logger = None) -> str:
     """
     Validate the *str* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *str*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param min_length: the minimum length accepted
     :param max_length:  the maximum length accepted
     :param default: if 'str', specifies the default value, overrinding the other constraints
                     if 'list', requires the value, if provided, to be in it
-    :param mandatory: specifies whether a value must be provided
+    :param required: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # initialize the return variable
     result: str | None = None
 
     stat: str | None = None
@@ -287,42 +287,42 @@
     if value is None and isinstance(default, str):
         value = default
     elif value is not None and not isinstance(value, str):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, value, "str", f"@{attr}")
     else:
         values = default if isinstance(default, list) else None
-        stat = validate_value(attr, value, min_length, max_length, values, mandatory)
+        stat = validate_value(attr, value, min_length, max_length, values, required)
 
     if stat:
         __validate_log(errors, stat, logger)
     else:
         result = value
 
     return result
 
 
 def validate_date(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
                   day_first: bool = False,
                   default: date = None,
-                  mandatory: bool = False,
+                  required: bool = False,
                   logger: Logger = None) -> date:
     """
     Validate the *date* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *date*, or a valid string representation of a *date*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param day_first: indicates that the day precedes the month in the string representing the date
-    :param default: optional default value, overrides 'mandatory'
-    :param mandatory: specifies whether a value must be provided
+    :param default: optional default value, overrides 'required'
+    :param required: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # import needed module
     from .datetime_pomes import date_parse
 
     # initialize the return variable
@@ -342,15 +342,15 @@
             # 121: Invalid value {}
             stat = validate_format_error(121, value, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL).date():
             # 129: Invalid value {}: date is later than the current date
             stat = validate_format_error(129, value, f"@{attr}")
     elif isinstance(default, date):
         result = default
-    elif isinstance(mandatory, bool) and mandatory:
+    elif isinstance(required, bool) and required:
         # 112: Required attribute
         stat = validate_format_error(112, f"@{attr}")
 
     if stat:
         result = None
         __validate_log(errors, stat, logger)
 
@@ -358,27 +358,27 @@
 
 
 def validate_datetime(errors: list[str] | None,
                       scheme: dict,
                       attr: str,
                       day_first: bool = True,
                       default: datetime = None,
-                      mandatory: bool = False,
+                      required: bool = False,
                       logger: Logger = None) -> datetime:
     """
     Validate the *datetime* value associated with *attr* in *scheme*.
 
     If provided, this value must be a *date*, or a valid string representation of a *date*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the value to be validated
     :param attr: the attribute associated with the value to be validated
     :param day_first: indicates that the day precedes the month in the string representing the date
-    :param default: optional default value, overrides 'mandatory'
-    :param mandatory: specifies whether a value must be provided
+    :param default: optional default value, overrides 'required'
+    :param required: specifies whether a value must be provided
     :param logger: optional logger
     :return: the validated value, or None if validation failed
     """
     # import needed module
     from .datetime_pomes import datetime_parse
 
     # initialize the return variable
@@ -396,42 +396,42 @@
             # 121: Invalid value {}
             stat = validate_format_error(121, value, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL):
             # 129: Invalid value {}: date is later than the current date
             stat = validate_format_error(129, value, f"@{attr}")
     elif isinstance(default, datetime):
         result = default
-    elif isinstance(mandatory, bool) and mandatory:
+    elif isinstance(required, bool) and required:
         # 112: Required attribute
         stat = validate_format_error(112, f"@{attr}")
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_ints(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
                   min_val: int = None,
                   max_val: int = None,
-                  mandatory: bool = False,
+                  required: bool = False,
                   logger: Logger = None) -> list[int]:
     """
     Validate the list of *int* values associated with *attr* in *scheme*.
 
     If provided, this list must contain *ints*, or valid string representations of *ints*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the list of values to be validated
     :param attr: the attribute associated with the list of values to be validated
     :param min_val: the minimum value accepted
     :param max_val:  the maximum value accepted
-    :param mandatory: whether the list of values must be provided
+    :param required: whether the list of values must be provided
     :param logger: optional logger
     :return: the list of validated values, or None if validation failed
     """
     # initialize the return variable
     result: list[Any] | None = None
 
     stat: str | None = None
@@ -445,49 +445,49 @@
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, int):
                         stat = validate_value(f"@{attr}[{inx+1}]", value, min_val, max_val)
                     else:
                         # 128: Invalid value {}: must be type {}
                         stat = validate_format_error(128, value, "int", f"@{attr}[{inx+1}]")
-            elif mandatory:
+            elif required:
                 # 112: Required attribute
                 stat = validate_format_error(112, f"@{attr}")
         else:
             # 128: Invalid value {}: must be type {}
             stat = validate_format_error(128, result, "list", f"@{attr}")
     except (KeyError, TypeError):
-        if mandatory:
+        if required:
             # 112: Required attribute
             stat = validate_format_error(112, f"@{attr}")
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_strs(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
                   min_length: int,
                   max_length: int,
-                  mandatory: bool = False,
+                  required: bool = False,
                   logger: Logger = None) -> list[str]:
     """
     Validate the list of *str* values associated with *attr* in *scheme*.
 
     If provided, this list must contain *strs*.
 
     :param errors: incidental error messages
     :param scheme: dictionary containing the list of values to be validated
     :param attr: the attribute associated with the list of values to be validated
     :param min_length: the minimum length accepted
     :param max_length:  the maximum length accepted
-    :param mandatory: whether the list of values must be provided
+    :param required: whether the list of values must be provided
     :param logger: optional logger
     :return: the list of validated values, or None if validation failed
     """
     # initialize the return variable
     result: list[Any] | None = None
 
     stat: str | None = None
@@ -501,22 +501,22 @@
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, str):
                         stat = validate_value(f"@{attr}[{inx+1}]", value, min_length, max_length)
                     else:
                         # 128: Invalid value {}: must be type {}
                         stat = validate_format_error(128, value, "str", f"@{attr}[{inx+1}]")
-            elif mandatory:
+            elif required:
                 # 112: Required attribute
                 stat = validate_format_error(112, f"@{attr}")
         else:
             # 128: Invalid value {}: must be type {}
             stat = validate_format_error(128, result, "list", f"@{attr}")
     except (KeyError, TypeError):
-        if mandatory:
+        if required:
             # 112: Required attribute
             stat = validate_format_error(112, f"@{attr}")
 
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
```

### Comparing `pypomes_core-1.1.0/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.1.1/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/LICENSE` & `pypomes_core-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.0/pyproject.toml` & `pypomes_core-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.1.0/PKG-INFO` & `pypomes_core-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.1.0
+Version: 1.1.1
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

