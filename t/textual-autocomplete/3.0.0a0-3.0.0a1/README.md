# Comparing `tmp/textual_autocomplete-3.0.0a0.tar.gz` & `tmp/textual_autocomplete-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_autocomplete-3.0.0a0.tar", max compression
+gzip compressed data, was "textual_autocomplete-3.0.0a1.tar", max compression
```

## Comparing `textual_autocomplete-3.0.0a0.tar` & `textual_autocomplete-3.0.0a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-05-11 10:33:52.764840 textual_autocomplete-3.0.0a0/LICENSE
--rw-r--r--   0        0        0     5108 2024-05-11 10:33:52.766486 textual_autocomplete-3.0.0a0/README.md
--rw-r--r--   0        0        0      689 2024-05-30 19:19:42.586863 textual_autocomplete-3.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      296 2024-05-29 12:50:02.250077 textual_autocomplete-3.0.0a0/textual_autocomplete/__init__.py
--rw-r--r--   0        0        0    18968 2024-05-29 23:18:44.386489 textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete.py
--rw-r--r--   0        0        0    15880 2024-05-30 19:19:06.338711 textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete2.py
--rw-r--r--   0        0        0        0 2022-11-23 09:28:07.225383 textual_autocomplete-3.0.0a0/textual_autocomplete/py.typed
--rw-r--r--   0        0        0     5750 1970-01-01 00:00:00.000000 textual_autocomplete-3.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 10:33:52.764840 textual_autocomplete-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0     5108 2024-05-11 10:33:52.766486 textual_autocomplete-3.0.0a1/README.md
+-rw-r--r--   0        0        0      689 2024-05-30 19:34:36.033430 textual_autocomplete-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      296 2024-05-29 12:50:02.250077 textual_autocomplete-3.0.0a1/textual_autocomplete/__init__.py
+-rw-r--r--   0        0        0    18968 2024-05-29 23:18:44.386489 textual_autocomplete-3.0.0a1/textual_autocomplete/_autocomplete.py
+-rw-r--r--   0        0        0    15882 2024-05-30 19:34:23.564028 textual_autocomplete-3.0.0a1/textual_autocomplete/_autocomplete2.py
+-rw-r--r--   0        0        0        0 2022-11-23 09:28:07.225383 textual_autocomplete-3.0.0a1/textual_autocomplete/py.typed
+-rw-r--r--   0        0        0     5750 1970-01-01 00:00:00.000000 textual_autocomplete-3.0.0a1/PKG-INFO
```

### Comparing `textual_autocomplete-3.0.0a0/LICENSE` & `textual_autocomplete-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_autocomplete-3.0.0a0/README.md` & `textual_autocomplete-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `textual_autocomplete-3.0.0a0/pyproject.toml` & `textual_autocomplete-3.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-autocomplete"
-version = "3.0.0a0"
+version = "3.0.0a1"
 description = "Easily add autocomplete dropdowns to your Textual apps."
 authors = ["Darren Burns <darrenb900@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "textual_autocomplete" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete.py` & `textual_autocomplete-3.0.0a1/textual_autocomplete/_autocomplete.py`

 * *Files identical despite different names*

### Comparing `textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete2.py` & `textual_autocomplete-3.0.0a1/textual_autocomplete/_autocomplete2.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
         for item in items:
             text = item.main
             if value.lower() in text.plain.lower():
                 matches.append(
                     DropdownItem(
                         left_meta=item.left_meta,
                         main=item.main,
-                        popup=item.popup,
+                        # popup=item.popup,
                         search_string=search_string,
                         highlight_ranges=item.highlight_ranges,
                         highlight_style=highlight_style
                         if item.highlight_style is None
                         else item.highlight_style,
                     )
                 )
```

### Comparing `textual_autocomplete-3.0.0a0/PKG-INFO` & `textual_autocomplete-3.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-autocomplete
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Easily add autocomplete dropdowns to your Textual apps.
 Author: Darren Burns
 Author-email: darrenb900@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

