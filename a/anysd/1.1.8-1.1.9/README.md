# Comparing `tmp/anysd-1.1.8.tar.gz` & `tmp/anysd-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anysd-1.1.8.tar", max compression
+gzip compressed data, was "anysd-1.1.9.tar", max compression
```

## Comparing `anysd-1.1.8.tar` & `anysd-1.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2022-11-09 18:00:11.152135 anysd-1.1.8/LICENSE
--rw-r--r--   0        0        0     6633 2022-11-09 18:00:05.548135 anysd-1.1.8/README.md
--rwxr-xr-x   0        0        0       39 2024-02-17 15:43:54.994992 anysd-1.1.8/publish.sh
--rw-r--r--   0        0        0      896 2024-02-26 14:02:38.286516 anysd-1.1.8/pyproject.toml
--rw-r--r--   0        0        0       21 2024-02-12 14:55:35.051038 anysd-1.1.8/src/anysd/__init__.py
--rw-r--r--   0        0        0     1659 2024-02-21 04:27:20.389429 anysd-1.1.8/src/anysd/conf.py
--rw-r--r--   0        0        0        0 2022-11-09 18:00:11.276135 anysd-1.1.8/src/anysd/config.toml
--rw-r--r--   0        0        0    28513 2024-02-26 14:02:38.282516 anysd-1.1.8/src/anysd/main.py
--rw-r--r--   0        0        0      124 2024-02-12 15:12:47.446453 anysd-1.1.8/src/anysd/utils.py
--rw-r--r--   0        0        0     7623 1970-01-01 00:00:00.000000 anysd-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-11-09 18:00:11.152135 anysd-1.1.9/LICENSE
+-rw-r--r--   0        0        0     6633 2022-11-09 18:00:05.548135 anysd-1.1.9/README.md
+-rwxr-xr-x   0        0        0       39 2024-02-17 15:43:54.994992 anysd-1.1.9/publish.sh
+-rw-r--r--   0        0        0      896 2024-02-26 14:15:43.209046 anysd-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-02-12 14:55:35.051038 anysd-1.1.9/src/anysd/__init__.py
+-rw-r--r--   0        0        0     1659 2024-02-21 04:27:20.389429 anysd-1.1.9/src/anysd/conf.py
+-rw-r--r--   0        0        0        0 2022-11-09 18:00:11.276135 anysd-1.1.9/src/anysd/config.toml
+-rw-r--r--   0        0        0    28608 2024-02-26 14:15:07.173886 anysd-1.1.9/src/anysd/main.py
+-rw-r--r--   0        0        0      124 2024-02-12 15:12:47.446453 anysd-1.1.9/src/anysd/utils.py
+-rw-r--r--   0        0        0     7623 1970-01-01 00:00:00.000000 anysd-1.1.9/PKG-INFO
```

### Comparing `anysd-1.1.8/LICENSE` & `anysd-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anysd-1.1.8/README.md` & `anysd-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `anysd-1.1.8/pyproject.toml` & `anysd-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "anysd"
-version = "1.1.8"
+version = "1.1.9"
 description = "For building ussd applications faster, with navigation management out of the box"
 readme = "README.md"
 authors = ["Somwaki <somwaki@gmail.com>", "Steven Ondieki <ondiekisteven1@gmail.com>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `anysd-1.1.8/src/anysd/conf.py` & `anysd-1.1.9/src/anysd/conf.py`

 * *Files identical despite different names*

### Comparing `anysd-1.1.8/src/anysd/main.py` & `anysd-1.1.9/src/anysd/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,16 @@
             if self.get_step_type(current_step) == ListInput:
                 list_ref: ListInput = self.get_step_item(current_step)
                 valid_last_input = list_ref.validate(
                     key=last_input,
                     msisdn=msisdn,
                     session_id=session_id,
                     ussd_string=ussd_string,
-                    lang=lang
+                    lang=lang,
+                    last_input=last_input
                 )
 
                 # handle bs logic
                 _res = self._validate_last_input(
                     current_step, last_input, msisdn=msisdn, session_id=session_id)
 
                 if isinstance(_res, tuple) and len(_res) == 2:
@@ -227,15 +228,16 @@
                 if _field_name and _field_name.replace("_", "").isalnum() and not _field_name[0].isnumeric():
                     if self.get_step_type(current_step) == ListInput:
                         _state[_field_name] = self.get_step_item(current_step).get_item(
                             idx=last_input,
                             msisdn=msisdn,
                             session_id=session_id,
                             lang=lang,
-                            ussd_string=ussd_string
+                            ussd_string=ussd_string,
+                            last_input=last_input,
                         )
                     else:
                         _state[_field_name] = last_input
                 else:
                     logger.warning(
                         f'field_name "{_field_name}" is not valid. It should be contain letters, underscores and '
                         f'numbers, but begin with a letter or underscore')
```

### Comparing `anysd-1.1.8/PKG-INFO` & `anysd-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anysd
-Version: 1.1.8
+Version: 1.1.9
 Summary: For building ussd applications faster, with navigation management out of the box
 License: MIT
 Keywords: ussd,navigation
 Author: Somwaki
 Author-email: somwaki@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

