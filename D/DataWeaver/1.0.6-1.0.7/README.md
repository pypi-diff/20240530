# Comparing `tmp/dataweaver-1.0.6.tar.gz` & `tmp/dataweaver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataweaver-1.0.6.tar", last modified: Fri May 17 15:36:56 2024, max compression
+gzip compressed data, was "dataweaver-1.0.7.tar", last modified: Thu May 30 14:41:11 2024, max compression
```

## Comparing `dataweaver-1.0.6.tar` & `dataweaver-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:36:56.502581 dataweaver-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-17 15:36:52.000000 dataweaver-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24152 2024-05-17 15:36:56.502581 dataweaver-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23439 2024-05-17 15:36:52.000000 dataweaver-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-17 15:36:52.000000 dataweaver-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:36:56.502581 dataweaver-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:36:56.498582 dataweaver-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:36:56.502581 dataweaver-1.0.6/src/DataWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24152 2024-05-17 15:36:56.000000 dataweaver-1.0.6/src/DataWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-17 15:36:56.000000 dataweaver-1.0.6/src/DataWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:36:56.000000 dataweaver-1.0.6/src/DataWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 15:36:56.000000 dataweaver-1.0.6/src/DataWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 15:36:56.000000 dataweaver-1.0.6/src/DataWeaver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:36:56.502581 dataweaver-1.0.6/src/data_weaver/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-17 15:36:52.000000 dataweaver-1.0.6/src/data_weaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-17 15:36:52.000000 dataweaver-1.0.6/src/data_weaver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-17 15:36:52.000000 dataweaver-1.0.6/src/data_weaver/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-17 15:36:52.000000 dataweaver-1.0.6/src/data_weaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:41:11.841670 dataweaver-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 14:41:03.000000 dataweaver-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24155 2024-05-30 14:41:11.837669 dataweaver-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23442 2024-05-30 14:41:03.000000 dataweaver-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-30 14:41:03.000000 dataweaver-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:41:11.841670 dataweaver-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:41:11.837669 dataweaver-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:41:11.837669 dataweaver-1.0.7/src/DataWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24155 2024-05-30 14:41:11.000000 dataweaver-1.0.7/src/DataWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 14:41:11.000000 dataweaver-1.0.7/src/DataWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:41:11.000000 dataweaver-1.0.7/src/DataWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 14:41:11.000000 dataweaver-1.0.7/src/DataWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 14:41:11.000000 dataweaver-1.0.7/src/DataWeaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:41:11.837669 dataweaver-1.0.7/src/data_weaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 14:41:03.000000 dataweaver-1.0.7/src/data_weaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-30 14:41:03.000000 dataweaver-1.0.7/src/data_weaver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-30 14:41:03.000000 dataweaver-1.0.7/src/data_weaver/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-30 14:41:03.000000 dataweaver-1.0.7/src/data_weaver/utils.py
```

### Comparing `dataweaver-1.0.6/LICENSE` & `dataweaver-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.6/PKG-INFO` & `dataweaver-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.6
+Version: 1.0.7
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -318,15 +318,15 @@
 
 | Function Name | Description |
 | --- | --- |
 | `capitalize` | Converts the first character of the string to uppercase and the rest to lowercase. |
 | `lower` | Converts all characters in the string to lowercase. |
 | `upper` | Converts all characters in the string to uppercase. |
 | `title` | Converts the first character of each word to uppercase and the remaining characters of each word to lowercase. |
-| `remove_accent` | Removes accents from characters in the string. |
+| `remove_accents` | Removes accents from characters in the string. |
 | `concat(delimiter=' ')` | Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space. /!\ All elements must be strings |
 | `join(delimiter=' ')` | Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space. |
 | `prefix(string='prefix-')` | Prepends the specified string to the beginning of the target string. Default prefix is "prefix-". |
 | `suffix(string='-suffix')` | Appends the specified string to the end of the target string. Default suffix is "-suffix". |
 | `split(delimiter=' ')` | Splits the string into a list of substrings around the specified delimiter. Default is a space. |
 | `replace(old, new)` | Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new. |
 | `regex(pattern, replace)` | Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace. |
@@ -452,23 +452,23 @@
 
   ```json
   {
     "fullName": "John Doe",
   }
   ```
 
-- `remove_accent`: Removes accents from characters in the string.
+- `remove_accents`: Removes accents from characters in the string.
 
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
-      "person.name": "remove_accent",
+      "person.name": "remove_accents",
     }
   }
   ```
 
   The object below:
 
   ```json
```

### Comparing `dataweaver-1.0.6/README.md` & `dataweaver-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 
 | Function Name | Description |
 | --- | --- |
 | `capitalize` | Converts the first character of the string to uppercase and the rest to lowercase. |
 | `lower` | Converts all characters in the string to lowercase. |
 | `upper` | Converts all characters in the string to uppercase. |
 | `title` | Converts the first character of each word to uppercase and the remaining characters of each word to lowercase. |
-| `remove_accent` | Removes accents from characters in the string. |
+| `remove_accents` | Removes accents from characters in the string. |
 | `concat(delimiter=' ')` | Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space. /!\ All elements must be strings |
 | `join(delimiter=' ')` | Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space. |
 | `prefix(string='prefix-')` | Prepends the specified string to the beginning of the target string. Default prefix is "prefix-". |
 | `suffix(string='-suffix')` | Appends the specified string to the end of the target string. Default suffix is "-suffix". |
 | `split(delimiter=' ')` | Splits the string into a list of substrings around the specified delimiter. Default is a space. |
 | `replace(old, new)` | Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new. |
 | `regex(pattern, replace)` | Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace. |
@@ -437,23 +437,23 @@
 
   ```json
   {
     "fullName": "John Doe",
   }
   ```
 
-- `remove_accent`: Removes accents from characters in the string.
+- `remove_accents`: Removes accents from characters in the string.
 
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
-      "person.name": "remove_accent",
+      "person.name": "remove_accents",
     }
   }
   ```
 
   The object below:
 
   ```json
```

### Comparing `dataweaver-1.0.6/pyproject.toml` & `dataweaver-1.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DataWeaver"
-version = "1.0.6"
+version = "1.0.7"
 authors = [{name = "RICHARD Quentin", email = "richard.quentin88@gmail.com"}]
 description = "DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing."
 readme = "README.md"
 license = {text = "MIT License"}  # Update the license as appropriate
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dataweaver-1.0.6/src/DataWeaver.egg-info/PKG-INFO` & `dataweaver-1.0.7/src/DataWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.6
+Version: 1.0.7
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -318,15 +318,15 @@
 
 | Function Name | Description |
 | --- | --- |
 | `capitalize` | Converts the first character of the string to uppercase and the rest to lowercase. |
 | `lower` | Converts all characters in the string to lowercase. |
 | `upper` | Converts all characters in the string to uppercase. |
 | `title` | Converts the first character of each word to uppercase and the remaining characters of each word to lowercase. |
-| `remove_accent` | Removes accents from characters in the string. |
+| `remove_accents` | Removes accents from characters in the string. |
 | `concat(delimiter=' ')` | Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space. /!\ All elements must be strings |
 | `join(delimiter=' ')` | Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space. |
 | `prefix(string='prefix-')` | Prepends the specified string to the beginning of the target string. Default prefix is "prefix-". |
 | `suffix(string='-suffix')` | Appends the specified string to the end of the target string. Default suffix is "-suffix". |
 | `split(delimiter=' ')` | Splits the string into a list of substrings around the specified delimiter. Default is a space. |
 | `replace(old, new)` | Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new. |
 | `regex(pattern, replace)` | Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace. |
@@ -452,23 +452,23 @@
 
   ```json
   {
     "fullName": "John Doe",
   }
   ```
 
-- `remove_accent`: Removes accents from characters in the string.
+- `remove_accents`: Removes accents from characters in the string.
 
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
-      "person.name": "remove_accent",
+      "person.name": "remove_accents",
     }
   }
   ```
 
   The object below:
 
   ```json
```

### Comparing `dataweaver-1.0.6/src/data_weaver/main.py` & `dataweaver-1.0.7/src/data_weaver/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         Args:
             source_key (list): The key to retrieve the value from.
 
         Returns:
             list: The handled list.
 
         """
-        handled_list, is_default = [get_value_with_default(sub_key)[0] for sub_key in source_key], any(get_value_with_default(sub_key)[1] for sub_key in source_key)
+        handled_list, is_default = [get_value_with_default(sub_key)[0] for sub_key in source_key], all(get_value_with_default(sub_key)[1] for sub_key in source_key)
         if is_default:
             return handled_list
         return transform_value(handled_list, target_key)
 
     def handle_default(source_key):
         """
         Handles the default value for the given key.
```

### Comparing `dataweaver-1.0.6/src/data_weaver/transforms.py` & `dataweaver-1.0.7/src/data_weaver/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         return f"{val}{suffix}"
     return apply_to_value(value, suffix_val)
 
 def split(value: str, delimiter: str = ' ') -> list:
     return value.split(delimiter)
 
 def join(values: list, delimiter: str = ' ') -> str:
-    return delimiter.join(map(str, values))
+    values = [str(value) if value is not None else '' for value in values]
+    return delimiter.join(values)
 
 def lower(value: str | list | dict) -> str:
     def lower_val(val):
         return val.lower()
     return apply_to_value(value, lower_val)
 
 def title(value: str | list | dict) -> str:
```

### Comparing `dataweaver-1.0.6/src/data_weaver/utils.py` & `dataweaver-1.0.7/src/data_weaver/utils.py`

 * *Files identical despite different names*

