# Comparing `tmp/opentelemetry_instrumentation_ollama-0.21.0.tar.gz` & `tmp/opentelemetry_instrumentation_ollama-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_ollama-0.21.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_ollama-0.21.1.tar", max compression
```

## Comparing `opentelemetry_instrumentation_ollama-0.21.0.tar` & `opentelemetry_instrumentation_ollama-0.21.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1146 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_ollama-0.21.0/README.md
--rw-r--r--   0        0        0     9986 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_ollama-0.21.0/opentelemetry/instrumentation/ollama/__init__.py
--rw-r--r--   0        0        0       42 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_ollama-0.21.0/opentelemetry/instrumentation/ollama/config.py
--rw-r--r--   0        0        0      699 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_ollama-0.21.0/opentelemetry/instrumentation/ollama/utils.py
--rw-r--r--   0        0        0       23 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_ollama-0.21.0/opentelemetry/instrumentation/ollama/version.py
--rw-r--r--   0        0        0     1399 2024-05-27 16:54:48.871652 opentelemetry_instrumentation_ollama-0.21.0/pyproject.toml
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_ollama-0.21.0/PKG-INFO
+-rw-r--r--   0        0        0     1146 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_ollama-0.21.1/README.md
+-rw-r--r--   0        0        0     9986 2024-05-30 00:59:17.946688 opentelemetry_instrumentation_ollama-0.21.1/opentelemetry/instrumentation/ollama/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-30 00:59:17.946688 opentelemetry_instrumentation_ollama-0.21.1/opentelemetry/instrumentation/ollama/config.py
+-rw-r--r--   0        0        0      740 2024-05-30 00:59:17.946688 opentelemetry_instrumentation_ollama-0.21.1/opentelemetry/instrumentation/ollama/utils.py
+-rw-r--r--   0        0        0       23 2024-05-30 00:59:17.946688 opentelemetry_instrumentation_ollama-0.21.1/opentelemetry/instrumentation/ollama/version.py
+-rw-r--r--   0        0        0     1399 2024-05-30 00:59:55.947050 opentelemetry_instrumentation_ollama-0.21.1/pyproject.toml
+-rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_ollama-0.21.1/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_ollama-0.21.0/README.md` & `opentelemetry_instrumentation_ollama-0.21.1/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_ollama-0.21.0/opentelemetry/instrumentation/ollama/__init__.py` & `opentelemetry_instrumentation_ollama-0.21.1/opentelemetry/instrumentation/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_ollama-0.21.0/opentelemetry/instrumentation/ollama/utils.py` & `opentelemetry_instrumentation_ollama-0.21.1/opentelemetry/instrumentation/ollama/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,12 +12,14 @@
     # Obtain a logger specific to the function's module
     logger = logging.getLogger(func.__module__)
 
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
-            logger.warning("Failed to execute %s, error: %s", func.__name__, str(e))
+            logger.debug(
+                "OpenLLMetry failed to trace in %s, error: %s", func.__name__, str(e)
+            )
             if Config.exception_logger:
                 Config.exception_logger(e)
 
     return wrapper
```

### Comparing `opentelemetry_instrumentation_ollama-0.21.0/pyproject.toml` & `opentelemetry_instrumentation_ollama-0.21.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-ollama"
-version = "0.21.0"
+version = "0.21.1"
 description = "OpenTelemetry Ollama instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-ollama"
 license = "Apache-2.0"
```

### Comparing `opentelemetry_instrumentation_ollama-0.21.0/PKG-INFO` & `opentelemetry_instrumentation_ollama-0.21.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-ollama
-Version: 0.21.0
+Version: 0.21.1
 Summary: OpenTelemetry Ollama instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-ollama
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-ollama Version:
-0.21.0 Summary: OpenTelemetry Ollama instrumentation Home-page: https://
+0.21.1 Summary: OpenTelemetry Ollama instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-ollama License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

