# Comparing `tmp/opentelemetry_instrumentation_milvus-0.21.0.tar.gz` & `tmp/opentelemetry_instrumentation_milvus-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_milvus-0.21.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_milvus-0.21.1.tar", max compression
```

## Comparing `opentelemetry_instrumentation_milvus-0.21.0.tar` & `opentelemetry_instrumentation_milvus-0.21.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      561 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_milvus-0.21.0/README.md
--rw-r--r--   0        0        0     2750 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/__init__.py
--rw-r--r--   0        0        0       42 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/config.py
--rw-r--r--   0        0        0      699 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/utils.py
--rw-r--r--   0        0        0       23 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/version.py
--rw-r--r--   0        0        0     6793 2024-05-27 16:54:22.291271 opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/wrapper.py
--rw-r--r--   0        0        0     1389 2024-05-27 16:54:47.591633 opentelemetry_instrumentation_milvus-0.21.0/pyproject.toml
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_milvus-0.21.0/PKG-INFO
+-rw-r--r--   0        0        0      561 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_milvus-0.21.1/README.md
+-rw-r--r--   0        0        0     2750 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/config.py
+-rw-r--r--   0        0        0      740 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/utils.py
+-rw-r--r--   0        0        0       23 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/version.py
+-rw-r--r--   0        0        0     6793 2024-05-30 00:59:17.942688 opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/wrapper.py
+-rw-r--r--   0        0        0     1389 2024-05-30 00:59:54.687038 opentelemetry_instrumentation_milvus-0.21.1/pyproject.toml
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_milvus-0.21.1/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_milvus-0.21.0/README.md` & `opentelemetry_instrumentation_milvus-0.21.1/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/__init__.py` & `opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/utils.py` & `opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/utils.py`

 * *Files 12% similar despite different names*

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

### Comparing `opentelemetry_instrumentation_milvus-0.21.0/opentelemetry/instrumentation/milvus/wrapper.py` & `opentelemetry_instrumentation_milvus-0.21.1/opentelemetry/instrumentation/milvus/wrapper.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.21.0/pyproject.toml` & `opentelemetry_instrumentation_milvus-0.21.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-milvus"
-version = "0.21.0"
+version = "0.21.1"
 description = "OpenTelemetry Milvus instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-milvus"
```

### Comparing `opentelemetry_instrumentation_milvus-0.21.0/PKG-INFO` & `opentelemetry_instrumentation_milvus-0.21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-milvus
-Version: 0.21.0
+Version: 0.21.1
 Summary: OpenTelemetry Milvus instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-milvus
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-milvus Version:
-0.21.0 Summary: OpenTelemetry Milvus instrumentation Home-page: https://
+0.21.1 Summary: OpenTelemetry Milvus instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-milvus License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

