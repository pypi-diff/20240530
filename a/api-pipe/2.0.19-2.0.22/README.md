# Comparing `tmp/api_pipe-2.0.19.tar.gz` & `tmp/api_pipe-2.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_pipe-2.0.19.tar", max compression
+gzip compressed data, was "api_pipe-2.0.22.tar", max compression
```

## Comparing `api_pipe-2.0.19.tar` & `api_pipe-2.0.22.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       11 2024-05-26 17:18:29.555149 api_pipe-2.0.19/README.md
--rw-r--r--   0        0        0      557 2024-05-26 17:15:05.000000 api_pipe-2.0.19/pyproject.toml
--rw-r--r--   0        0        0       69 2024-05-26 17:15:05.000000 api_pipe-2.0.19/src/api_pipe/__init__.py
--rw-r--r--   0        0        0     8504 2024-05-26 17:18:29.555149 api_pipe-2.0.19/src/api_pipe/api.py
--rw-r--r--   0        0        0      827 2024-05-26 17:18:29.555149 api_pipe-2.0.19/src/api_pipe/config.py
--rw-r--r--   0        0        0      555 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/directory.py
--rw-r--r--   0        0        0     1577 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/error.py
--rw-r--r--   0        0        0     1491 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/logger.py
--rw-r--r--   0        0        0     3212 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/manual_test_run.py
--rw-r--r--   0        0        0     3570 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/params.py
--rw-r--r--   0        0        0     1056 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/params_schema.py
--rw-r--r--   0        0        0        3 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/steps/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/steps/fetch.py
--rw-r--r--   0        0        0     1900 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/steps/fetch_async.py
--rw-r--r--   0        0        0     1002 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/steps/filter.py
--rw-r--r--   0        0        0      649 2024-05-26 17:18:29.556149 api_pipe-2.0.19/src/api_pipe/steps/key.py
--rw-r--r--   0        0        0     1237 2024-05-26 17:18:29.557149 api_pipe-2.0.19/src/api_pipe/steps/map.py
--rw-r--r--   0        0        0      913 2024-05-26 17:18:29.557149 api_pipe-2.0.19/src/api_pipe/steps/select.py
--rw-r--r--   0        0        0      507 2024-05-26 17:18:29.557149 api_pipe-2.0.19/src/api_pipe/steps/to_json.py
--rw-r--r--   0        0        0      738 2024-05-26 17:18:29.557149 api_pipe-2.0.19/src/api_pipe/steps/to_python.py
--rw-r--r--   0        0        0      720 2024-05-26 17:18:29.557149 api_pipe-2.0.19/src/api_pipe/url.py
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-2.0.19/PKG-INFO
+-rw-r--r--   0        0        0     7154 2024-05-30 05:04:48.511228 api_pipe-2.0.22/README.md
+-rw-r--r--   0        0        0      561 2024-05-30 05:00:25.000000 api_pipe-2.0.22/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-05-30 05:00:25.000000 api_pipe-2.0.22/src/api_pipe/__init__.py
+-rw-r--r--   0        0        0     8504 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/api.py
+-rw-r--r--   0        0        0      827 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/config.py
+-rw-r--r--   0        0        0      555 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/directory.py
+-rw-r--r--   0        0        0     1577 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/error.py
+-rw-r--r--   0        0        0     1491 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/logger.py
+-rw-r--r--   0        0        0     3212 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/manual_test_run.py
+-rw-r--r--   0        0        0     3570 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/params.py
+-rw-r--r--   0        0        0     1056 2024-05-30 05:04:42.562233 api_pipe-2.0.22/src/api_pipe/params_schema.py
+-rw-r--r--   0        0        0        3 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/fetch.py
+-rw-r--r--   0        0        0     1900 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/fetch_async.py
+-rw-r--r--   0        0        0     1002 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/filter.py
+-rw-r--r--   0        0        0      649 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/key.py
+-rw-r--r--   0        0        0     1237 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/map.py
+-rw-r--r--   0        0        0      913 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/select.py
+-rw-r--r--   0        0        0      507 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/to_json.py
+-rw-r--r--   0        0        0      738 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/steps/to_python.py
+-rw-r--r--   0        0        0      721 2024-05-30 05:04:42.563233 api_pipe-2.0.22/src/api_pipe/url.py
+-rw-r--r--   0        0        0     7591 1970-01-01 00:00:00.000000 api_pipe-2.0.22/PKG-INFO
```

### Comparing `api_pipe-2.0.19/pyproject.toml` & `api_pipe-2.0.22/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "api-pipe"
-version = "2.0.19"
+version = "2.0.22"
 description = "API Pipe"
-authors = ["Rafael Roman Otero <rromanotero@gmail.com>"]
+authors = ["Rafael Roman Otero <rromanotero@romanlabs.com>"]
 readme = "README.md"
 packages = [{include = "api_pipe", from = "src"}]
 
 [tool.poetry.scripts]
 manual-test-run = "api_pipe.manual_test_run:main"
 
 [tool.poetry.dependencies]
```

### Comparing `api_pipe-2.0.19/src/api_pipe/api.py` & `api_pipe-2.0.22/src/api_pipe/api.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/config.py` & `api_pipe-2.0.22/src/api_pipe/config.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/directory.py` & `api_pipe-2.0.22/src/api_pipe/directory.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/error.py` & `api_pipe-2.0.22/src/api_pipe/error.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/logger.py` & `api_pipe-2.0.22/src/api_pipe/logger.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/manual_test_run.py` & `api_pipe-2.0.22/src/api_pipe/manual_test_run.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/params.py` & `api_pipe-2.0.22/src/api_pipe/params.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/params_schema.py` & `api_pipe-2.0.22/src/api_pipe/params_schema.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/fetch.py` & `api_pipe-2.0.22/src/api_pipe/steps/fetch.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/fetch_async.py` & `api_pipe-2.0.22/src/api_pipe/steps/fetch_async.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/filter.py` & `api_pipe-2.0.22/src/api_pipe/steps/filter.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/key.py` & `api_pipe-2.0.22/src/api_pipe/steps/key.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/map.py` & `api_pipe-2.0.22/src/api_pipe/steps/map.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/select.py` & `api_pipe-2.0.22/src/api_pipe/steps/select.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/steps/to_python.py` & `api_pipe-2.0.22/src/api_pipe/steps/to_python.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.19/src/api_pipe/url.py` & `api_pipe-2.0.22/src/api_pipe/url.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         '''
             Init
         '''
         self.value = value
 
     def __truediv__(self, other) -> "Url":
         '''
-            Truediv
+            Truediv.
         '''
         _other = other.value if isinstance(other, Url) else other
         return Url(f"{self.value}/{_other}")
 
     def __str__(self):
         '''
             Str
```

