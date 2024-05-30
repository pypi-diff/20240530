# Comparing `tmp/wiederverwendbar-0.2.6.tar.gz` & `tmp/wiederverwendbar-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.2.6.tar", last modified: Wed May 29 08:20:08 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.7.tar", last modified: Wed May 29 14:43:18 2024, max compression
```

## Comparing `wiederverwendbar-0.2.6.tar` & `wiederverwendbar-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0       19 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/README.md
--rw-r--r--   0        0        0      718 2024-05-29 08:20:08.059440 wiederverwendbar-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/__init__.py
--rw-r--r--   0        0        0     1113 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/admin.py
--rw-r--r--   0        0        0     1734 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/eval_file.py
--rw-r--r--   0        0        0     3174 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/eval_value.py
--rw-r--r--   0        0        0      407 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/find_class_method.py
--rw-r--r--   0        0        0     1162 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/wait_ping.py
--rw-r--r--   0        0        0      186 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/__init__.py
--rw-r--r--   0        0        0      600 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/rich_console_handler.py
--rw-r--r--   0        0        0      624 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/stream_console_handler.py
--rw-r--r--   0        0        0     2378 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
--rw-r--r--   0        0        0     3036 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger.py
--rw-r--r--   0        0        0     5665 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_settings.py
--rw-r--r--   0        0        0     2375 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_singleton.py
--rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/__init__.py
--rw-r--r--   0        0        0     2145 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/file_config.py
--rw-r--r--   0        0        0      762 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/indexable_model.py
--rw-r--r--   0        0        0     7477 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/singleton.py
--rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0      890 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/logger.py
--rw-r--r--   0        0        0      920 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/singletons.py
--rw-r--r--   0        0        0      466 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/test.py
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/README.md
+-rw-r--r--   0        0        0      763 2024-05-29 14:43:18.042643 wiederverwendbar-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0     1113 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/functions/admin.py
+-rw-r--r--   0        0        0     1734 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/functions/eval_file.py
+-rw-r--r--   0        0        0     3174 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/functions/eval_value.py
+-rw-r--r--   0        0        0      407 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0     1162 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/functions/wait_ping.py
+-rw-r--r--   0        0        0      186 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0     2375 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/mongoengine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/mongoengine/fields/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/mongoengine/fields/ipv4_address_field.py
+-rw-r--r--   0        0        0      548 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/mongoengine/property_document.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/pydantic/__init__.py
+-rw-r--r--   0        0        0     2145 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/pydantic/file_config.py
+-rw-r--r--   0        0        0      762 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/pydantic/indexable_model.py
+-rw-r--r--   0        0        0     7453 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/tests/logger.py
+-rw-r--r--   0        0        0      920 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/tests/singletons.py
+-rw-r--r--   0        0        0      466 2024-05-29 14:42:41.646601 wiederverwendbar-0.2.7/tests/test.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.7/PKG-INFO
```

### Comparing `wiederverwendbar-0.2.6/pyproject.toml` & `wiederverwendbar-0.2.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 ]
 dependencies = [
     "pydantic>=2.7.1",
     "pydantic-settings>=2.2.1",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
-version = "0.2.6"
+version = "0.2.7"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 rich = [
     "rich>=13.7.1",
 ]
 typer = [
     "typer>=0.12.3",
 ]
 ping = [
     "pythonping>=1.1.4",
 ]
+mongoengine = [
+    "mongoengine>=0.28.2",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/functions/admin.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/functions/admin.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/functions/eval_file.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/functions/eval_file.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/functions/eval_value.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/functions/eval_value.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/functions/wait_ping.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/functions/wait_ping.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/rich_console_handler.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/rich_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/stream_console_handler.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/stream_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/logger/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_settings.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/logger/logger_settings.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_singleton.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/logger/logger_singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/file_config.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/pydantic/file_config.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/indexable_model.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/pydantic/indexable_model.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/src/wiederverwendbar/singleton.py` & `wiederverwendbar-0.2.7/src/wiederverwendbar/singleton.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,16 +175,14 @@
         Delete all singletons in map
         """
 
         # if ordered is None, delete by class attribute
         if ordered is None:
             ordered = cls.delete_ordered_on_exit
 
-        print(ordered)
-
         singleton_names = list(cls.get_all(ordered=ordered).keys())
         singleton_names.reverse()
         for name in singleton_names:
             cls.delete_by_name(name)
 
     @classmethod
     def delete_by_name(cls, name: str):
```

### Comparing `wiederverwendbar-0.2.6/tests/logger.py` & `wiederverwendbar-0.2.7/tests/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/tests/singletons.py` & `wiederverwendbar-0.2.7/tests/singletons.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.6/PKG-INFO` & `wiederverwendbar-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: wiederverwendbar
-Version: 0.2.6
+Version: 0.2.7
 Summary: A collection of scripts, classes and tools they are "wiederverwendbar".
 Author-Email: Julius Koenig <info@bastelquartier.de>
 License: GPL-3.0
 Requires-Python: >=3.12
 Requires-Dist: pydantic>=2.7.1
 Requires-Dist: pydantic-settings>=2.2.1
 Requires-Dist: rich>=13.7.1; extra == "rich"
 Requires-Dist: typer>=0.12.3; extra == "typer"
 Requires-Dist: pythonping>=1.1.4; extra == "ping"
+Requires-Dist: mongoengine>=0.28.2; extra == "mongoengine"
 Provides-Extra: rich
 Provides-Extra: typer
 Provides-Extra: ping
+Provides-Extra: mongoengine
 Description-Content-Type: text/markdown
 
 # wiederverwendbar
```

