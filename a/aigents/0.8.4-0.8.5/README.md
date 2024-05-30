# Comparing `tmp/aigents-0.8.4.tar.gz` & `tmp/aigents-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.8.4.tar", max compression
+gzip compressed data, was "aigents-0.8.5.tar", max compression
```

## Comparing `aigents-0.8.4.tar` & `aigents-0.8.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.4/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.4/README.md
--rw-r--r--   0        0        0     1044 2024-05-24 18:11:00.987176 aigents-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.4/src/aigents/__init__.py
--rw-r--r--   0        0        0    19579 2024-05-23 17:40:43.911432 aigents-0.8.4/src/aigents/base.py
--rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.4/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.4/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2022 2024-05-23 17:40:44.175432 aigents-0.8.4/src/aigents/context/base.py
--rw-r--r--   0        0        0    13226 2024-05-23 17:40:43.911432 aigents-0.8.4/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.4/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.4/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.4/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.4/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.4/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    17636 2024-05-23 17:40:44.183432 aigents-0.8.4/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.4/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.4/src/aigents/context/utils.py
--rw-r--r--   0        0        0    33109 2024-05-24 18:10:36.447780 aigents-0.8.4/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.4/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.4/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.4/src/aigents/prompts.py
--rw-r--r--   0        0        0     2821 2024-05-23 17:39:47.123406 aigents-0.8.4/src/aigents/settings.py
--rw-r--r--   0        0        0     6813 2024-05-23 17:40:43.911432 aigents-0.8.4/src/aigents/utils.py
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.5/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.5/README.md
+-rw-r--r--   0        0        0     1044 2024-05-30 12:40:00.987564 aigents-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.5/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19579 2024-05-23 17:40:43.911432 aigents-0.8.5/src/aigents/base.py
+-rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.5/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.5/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-23 17:40:44.175432 aigents-0.8.5/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13226 2024-05-23 17:40:43.911432 aigents-0.8.5/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.5/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.5/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.5/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.5/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.5/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    17636 2024-05-23 17:40:44.183432 aigents-0.8.5/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.5/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.5/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    33109 2024-05-24 18:10:36.447780 aigents-0.8.5/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.5/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.5/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.5/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2861 2024-05-30 12:39:42.015624 aigents-0.8.5/src/aigents/settings.py
+-rw-r--r--   0        0        0     6813 2024-05-23 17:40:43.911432 aigents-0.8.5/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.5/PKG-INFO
```

### Comparing `aigents-0.8.4/LICENSE` & `aigents-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/README.md` & `aigents-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/pyproject.toml` & `aigents-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.8.4"
+version = "0.8.5"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.8.4/src/aigents/__init__.py` & `aigents-0.8.5/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/base.py` & `aigents-0.8.5/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/constants.py` & `aigents-0.8.5/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/context/base.py` & `aigents-0.8.5/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/context/core.py` & `aigents-0.8.5/src/aigents/context/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/context/nlp/base.py` & `aigents-0.8.5/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/context/nlp/processors.py` & `aigents-0.8.5/src/aigents/context/nlp/processors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/context/nlp/utils.py` & `aigents-0.8.5/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/context/utils.py` & `aigents-0.8.5/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/core.py` & `aigents-0.8.5/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/errors.py` & `aigents-0.8.5/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/prompts.py` & `aigents-0.8.5/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/src/aigents/settings.py` & `aigents-0.8.5/src/aigents/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,58 +46,57 @@
 Authors: {author}
 {DELIMITER}
 """
 
 CONFIG_LOG = {
     "version": 1,
     "formatters": {
-        "client": {"format": "%(levelname)s: %(message)s"},
-        "standard": {
+        "aigents_default": {"format": "%(levelname)s: %(message)s"},
+        "aigents_standard": {
             "format": (
                 "%(levelname)s (at %(pathname)s - %(funcName)s "
                 "in line %(lineno)d): %(message)s"
             )
         },
-        "debug": {
+        "aigents_debug": {
             "format": (
                 "%(asctime)s %(levelname)s (at %(funcName)s "
                 "in line %(lineno)d):"
                 "\n\t|──file: %(pathname)s"
                 "\n\t|──task name: %(taskName)s"
                 "\n\t└──message: %(message)s\n"
             ),
             "datefmt": "%y-%m-%d %H:%M:%S"
         }
     },
     "handlers": {
-        "client": {
+        "aigents_client": {
             "class": "logging.StreamHandler",
-            "formatter": "client",
+            "formatter": "aigents_default",
             "level": "INFO"
         },
-        "standard": {
+        "aigents_standard": {
             "class": "logging.StreamHandler",
-            "formatter": "standard",
+            "formatter": "aigents_standard",
             "level": "DEBUG"
         },
-        "debug": {
+        "aigents_debug": {
             "class": "logging.StreamHandler",
-            "formatter": "debug",
+            "formatter": "aigents_debug",
             "level": "DEBUG"
         }
     },
-    "root": {"handlers": ["standard"], "level": "DEBUG"},
     "loggers": {
-        "client": {
-            "handlers": ["client"],
+        "aigents_client": {
+            "handlers": ["aigents_client"],
             "level": "DEBUG",
             "propagate": False,
             "disable_existing_loggers": False
         },
         "aigents": {
-            "handlers": ["standard"],
+            "handlers": ["aigents_standard"],
             "level": "DEBUG",
             "propagate": False,
             "disable_existing_loggers": False
         }
     }
 }
```

### Comparing `aigents-0.8.4/src/aigents/utils.py` & `aigents-0.8.5/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.4/PKG-INFO` & `aigents-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.8.4
+Version: 0.8.5
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

