# Comparing `tmp/pytest-structlog-0.8.tar.gz` & `tmp/pytest_structlog-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-structlog-0.8.tar", last modified: Wed Mar 13 02:28:02 2024, max compression
+gzip compressed data, was "pytest_structlog-0.9.tar", last modified: Thu May 30 13:16:32 2024, max compression
```

## Comparing `pytest-structlog-0.8.tar` & `pytest_structlog-0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-03-13 02:28:02.148605 pytest-structlog-0.8/
--rw-r--r--   0 wim        (501) staff       (20)     1066 2021-02-10 08:04:23.000000 pytest-structlog-0.8/LICENSE
--rw-r--r--   0 wim        (501) staff       (20)       78 2024-02-04 03:52:18.000000 pytest-structlog-0.8/MANIFEST.in
--rw-r--r--   0 wim        (501) staff       (20)     4733 2024-03-13 02:28:02.148333 pytest-structlog-0.8/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)     4236 2024-02-04 03:52:18.000000 pytest-structlog-0.8/README.rst
--rw-r--r--   0 wim        (501) staff       (20)     1102 2024-02-04 05:17:45.000000 pytest-structlog-0.8/pyproject.toml
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-03-13 02:28:02.144681 pytest-structlog-0.8/pytest_structlog/
--rw-r--r--   0 wim        (501) staff       (20)     6363 2024-03-13 02:27:40.000000 pytest-structlog-0.8/pytest_structlog/__init__.py
--rw-r--r--   0 wim        (501) staff       (20)        0 2024-02-04 03:52:18.000000 pytest-structlog-0.8/pytest_structlog/py.typed
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-03-13 02:28:02.148057 pytest-structlog-0.8/pytest_structlog.egg-info/
--rw-r--r--   0 wim        (501) staff       (20)     4733 2024-03-13 02:28:02.000000 pytest-structlog-0.8/pytest_structlog.egg-info/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)      470 2024-03-13 02:28:02.000000 pytest-structlog-0.8/pytest_structlog.egg-info/SOURCES.txt
--rw-r--r--   0 wim        (501) staff       (20)        1 2024-03-13 02:28:02.000000 pytest-structlog-0.8/pytest_structlog.egg-info/dependency_links.txt
--rw-r--r--   0 wim        (501) staff       (20)       47 2024-03-13 02:28:02.000000 pytest-structlog-0.8/pytest_structlog.egg-info/entry_points.txt
--rw-r--r--   0 wim        (501) staff       (20)       25 2024-03-13 02:28:02.000000 pytest-structlog-0.8/pytest_structlog.egg-info/requires.txt
--rw-r--r--   0 wim        (501) staff       (20)       17 2024-03-13 02:28:02.000000 pytest-structlog-0.8/pytest_structlog.egg-info/top_level.txt
--rw-r--r--   0 wim        (501) staff       (20)       38 2024-03-13 02:28:02.148659 pytest-structlog-0.8/setup.cfg
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-03-13 02:28:02.147653 pytest-structlog-0.8/tests/
--rw-r--r--   0 wim        (501) staff       (20)      664 2024-02-04 05:14:00.000000 pytest-structlog-0.8/tests/test_issue14.py
--rw-r--r--   0 wim        (501) staff       (20)     1019 2024-02-04 05:12:41.000000 pytest-structlog-0.8/tests/test_issue18.py
--rw-r--r--   0 wim        (501) staff       (20)      941 2024-02-04 05:12:41.000000 pytest-structlog-0.8/tests/test_issue20.py
--rw-r--r--   0 wim        (501) staff       (20)     1147 2024-02-04 05:12:41.000000 pytest-structlog-0.8/tests/test_issue24.py
--rw-r--r--   0 wim        (501) staff       (20)     1489 2024-03-13 02:27:40.000000 pytest-structlog-0.8/tests/test_issue30.py
--rw-r--r--   0 wim        (501) staff       (20)     5129 2024-02-04 05:14:00.000000 pytest-structlog-0.8/tests/test_log.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-05-30 13:16:32.344321 pytest_structlog-0.9/
+-rw-r--r--   0 wim        (501) staff       (20)     1066 2021-02-10 08:04:23.000000 pytest_structlog-0.9/LICENSE
+-rw-r--r--   0 wim        (501) staff       (20)       78 2024-02-04 03:52:18.000000 pytest_structlog-0.9/MANIFEST.in
+-rw-r--r--   0 wim        (501) staff       (20)     4733 2024-05-30 13:16:32.343994 pytest_structlog-0.9/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)     4236 2024-02-04 03:52:18.000000 pytest_structlog-0.9/README.rst
+-rw-r--r--   0 wim        (501) staff       (20)     1102 2024-02-04 05:17:45.000000 pytest_structlog-0.9/pyproject.toml
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-05-30 13:16:32.337074 pytest_structlog-0.9/pytest_structlog/
+-rw-r--r--   0 wim        (501) staff       (20)     6707 2024-05-30 13:16:16.000000 pytest_structlog-0.9/pytest_structlog/__init__.py
+-rw-r--r--   0 wim        (501) staff       (20)        0 2024-02-04 03:52:18.000000 pytest_structlog-0.9/pytest_structlog/py.typed
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-05-30 13:16:32.343644 pytest_structlog-0.9/pytest_structlog.egg-info/
+-rw-r--r--   0 wim        (501) staff       (20)     4733 2024-05-30 13:16:32.000000 pytest_structlog-0.9/pytest_structlog.egg-info/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)      492 2024-05-30 13:16:32.000000 pytest_structlog-0.9/pytest_structlog.egg-info/SOURCES.txt
+-rw-r--r--   0 wim        (501) staff       (20)        1 2024-05-30 13:16:32.000000 pytest_structlog-0.9/pytest_structlog.egg-info/dependency_links.txt
+-rw-r--r--   0 wim        (501) staff       (20)       47 2024-05-30 13:16:32.000000 pytest_structlog-0.9/pytest_structlog.egg-info/entry_points.txt
+-rw-r--r--   0 wim        (501) staff       (20)       25 2024-05-30 13:16:32.000000 pytest_structlog-0.9/pytest_structlog.egg-info/requires.txt
+-rw-r--r--   0 wim        (501) staff       (20)       17 2024-05-30 13:16:32.000000 pytest_structlog-0.9/pytest_structlog.egg-info/top_level.txt
+-rw-r--r--   0 wim        (501) staff       (20)       38 2024-05-30 13:16:32.344373 pytest_structlog-0.9/setup.cfg
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-05-30 13:16:32.343115 pytest_structlog-0.9/tests/
+-rw-r--r--   0 wim        (501) staff       (20)      664 2024-02-04 05:14:00.000000 pytest_structlog-0.9/tests/test_issue14.py
+-rw-r--r--   0 wim        (501) staff       (20)     1019 2024-02-04 05:12:41.000000 pytest_structlog-0.9/tests/test_issue18.py
+-rw-r--r--   0 wim        (501) staff       (20)      941 2024-02-04 05:12:41.000000 pytest_structlog-0.9/tests/test_issue20.py
+-rw-r--r--   0 wim        (501) staff       (20)     1147 2024-02-04 05:12:41.000000 pytest_structlog-0.9/tests/test_issue24.py
+-rw-r--r--   0 wim        (501) staff       (20)     1489 2024-03-13 02:36:30.000000 pytest_structlog-0.9/tests/test_issue30.py
+-rw-r--r--   0 wim        (501) staff       (20)     1351 2024-05-30 13:16:16.000000 pytest_structlog-0.9/tests/test_issue32.py
+-rw-r--r--   0 wim        (501) staff       (20)     5487 2024-03-13 02:37:31.000000 pytest_structlog-0.9/tests/test_log.py
```

### Comparing `pytest-structlog-0.8/LICENSE` & `pytest_structlog-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/PKG-INFO` & `pytest_structlog-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-structlog
-Version: 0.8
+Version: 0.9
 Summary: Structured logging assertions
 Author-email: Wim Glenn <hey@wimglenn.com>
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/pytest-structlog
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytest-structlog-0.8/README.rst` & `pytest_structlog-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/pyproject.toml` & `pytest_structlog-0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/pytest_structlog/__init__.py` & `pytest_structlog-0.9/pytest_structlog/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from structlog.contextvars import clear_contextvars
 from structlog.contextvars import merge_contextvars
 from structlog.typing import EventDict
 from structlog.typing import Processor
 from structlog.typing import WrappedLogger
 
 
-__version__ = "0.8"
+__version__ = "0.9"
 
 
 class EventList(List[EventDict]):
     """A list subclass that overrides ordering operations.
     Instead of A <= B being a lexicographical comparison,
     now it means every element of A is contained within B,
     in the same order, although there may be other items
@@ -136,14 +136,20 @@
     cap = StructuredLogCapture()
     new_processors: List[Processor] = []
     for processor in original_processors:
         if isinstance(processor, structlog.stdlib.PositionalArgumentsFormatter):
             # if there was a positional argument formatter in there, keep it
             # see https://github.com/wimglenn/pytest-structlog/issues/18
             new_processors.append(processor)
+        elif processor is structlog.processors.format_exc_info:
+            # traceback render
+            # see https://github.com/wimglenn/pytest-structlog/issues/32
+            new_processors.append(processor)
+        elif processor is getattr(structlog.processors, "dict_tracebacks", object()):
+            new_processors.append(processor)
         elif processor is merge_contextvars:
             # if merging contextvars, preserve
             # see https://github.com/wimglenn/pytest-structlog/issues/20
             new_processors.append(processor)
     new_processors.append(cap.process)
     structlog.configure(processors=new_processors, cache_logger_on_first_use=False)
     cap.original_configure = cfg = structlog.configure  # type:ignore[attr-defined]
```

### Comparing `pytest-structlog-0.8/pytest_structlog.egg-info/PKG-INFO` & `pytest_structlog-0.9/pytest_structlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-structlog
-Version: 0.8
+Version: 0.9
 Summary: Structured logging assertions
 Author-email: Wim Glenn <hey@wimglenn.com>
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/pytest-structlog
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytest-structlog-0.8/tests/test_issue14.py` & `pytest_structlog-0.9/tests/test_issue14.py`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/tests/test_issue18.py` & `pytest_structlog-0.9/tests/test_issue18.py`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/tests/test_issue20.py` & `pytest_structlog-0.9/tests/test_issue20.py`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/tests/test_issue24.py` & `pytest_structlog-0.9/tests/test_issue24.py`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/tests/test_issue30.py` & `pytest_structlog-0.9/tests/test_issue30.py`

 * *Files identical despite different names*

### Comparing `pytest-structlog-0.8/tests/test_log.py` & `pytest_structlog-0.9/tests/test_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,19 @@
     log = logger.bind(k="v")
     log.debug("dbg")
     log.info("inf", kk="more context")
     log = log.unbind("k")
     log.warning("uh-oh")
 
 
+def i_warned_you_twice():
+    logger.warn("and you didn't listen")
+    logger.warning("now look what happened")
+
+
 def test_capture_creates_items(log: StructuredLogCapture):
     assert not log.events
     spline_reticulator()
     assert log.events
 
 
 def test_assert_without_context(log: StructuredLogCapture):
@@ -192,9 +197,17 @@
     expected = {"event": "dynamic-level", "level": name, "other": 42}
 
     assert log.log(level, "dynamic-level", other=42) == expected
     assert log.log(name, "dynamic-level", other=42) == expected
     assert log.log(name.upper(), "dynamic-level", other=42) == expected
 
 
-def test_event_factory__bad_level_number(log: StructuredLogCapture):
+def test_event_factory_bad_level_number(log: StructuredLogCapture):
     assert log.log(1234, "text") == {"event": "text", "level": "level 1234"}
+
+
+def test_warn_warning_alias(log: StructuredLogCapture):
+    i_warned_you_twice()
+    assert log.events == [
+        {"event": "and you didn't listen", "level": "warning"},
+        {"event": "now look what happened", "level": "warning"},
+    ]
```

