# Comparing `tmp/duckduckgo_search-6.1.2.tar.gz` & `tmp/duckduckgo_search-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-6.1.2.tar", last modified: Wed May 29 00:25:56 2024, max compression
+gzip compressed data, was "duckduckgo_search-6.1.3.tar", last modified: Thu May 30 21:06:53 2024, max compression
```

## Comparing `duckduckgo_search-6.1.2.tar` & `duckduckgo_search-6.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:25:56.605153 duckduckgo_search-6.1.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-29 00:25:56.605153 duckduckgo_search-6.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    17467 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:25:56.601153 duckduckgo_search-6.1.2/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    42430 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:25:56.605153 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-29 00:25:56.000000 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-29 00:25:56.000000 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:25:56.000000 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-29 00:25:56.000000 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 00:25:56.000000 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 00:25:56.000000 duckduckgo_search-6.1.2/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:25:56.605153 duckduckgo_search-6.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:25:56.605153 duckduckgo_search-6.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/tests/test_duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-29 00:25:45.000000 duckduckgo_search-6.1.2/tests/test_duckduckgo_search_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.578731 duckduckgo_search-6.1.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-30 21:06:53.578731 duckduckgo_search-6.1.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17467 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.574731 duckduckgo_search-6.1.3/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42430 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.574731 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:06:53.578731 duckduckgo_search-6.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.574731 duckduckgo_search-6.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/tests/test_duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/tests/test_duckduckgo_search_async.py
```

### Comparing `duckduckgo_search-6.1.2/LICENSE.md` & `duckduckgo_search-6.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/PKG-INFO` & `duckduckgo_search-6.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 6.1.2
+Version: 6.1.3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
-Requires-Dist: pyreqwest_impersonate>=0.4.6
+Requires-Dist: pyreqwest_impersonate>=0.4.7
 Requires-Dist: orjson>=3.10.3
 Provides-Extra: lxml
 Requires-Dist: lxml>=5.2.2; extra == "lxml"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.6; extra == "dev"
```

### Comparing `duckduckgo_search-6.1.2/README.md` & `duckduckgo_search-6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search/__init__.py` & `duckduckgo_search-6.1.3/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search/cli.py` & `duckduckgo_search-6.1.3/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search_async.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search/utils.py` & `duckduckgo_search-6.1.3/duckduckgo_search/utils.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-6.1.3/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 6.1.2
+Version: 6.1.3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
-Requires-Dist: pyreqwest_impersonate>=0.4.6
+Requires-Dist: pyreqwest_impersonate>=0.4.7
 Requires-Dist: orjson>=3.10.3
 Provides-Extra: lxml
 Requires-Dist: lxml>=5.2.2; extra == "lxml"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.6; extra == "dev"
```

### Comparing `duckduckgo_search-6.1.2/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-6.1.3/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/pyproject.toml` & `duckduckgo_search-6.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.7",
-    "pyreqwest_impersonate>=0.4.6",
+    "pyreqwest_impersonate>=0.4.7",
     "orjson>=3.10.3",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
```

### Comparing `duckduckgo_search-6.1.2/tests/test_cli.py` & `duckduckgo_search-6.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/tests/test_duckduckgo_search.py` & `duckduckgo_search-6.1.3/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.2/tests/test_duckduckgo_search_async.py` & `duckduckgo_search-6.1.3/tests/test_duckduckgo_search_async.py`

 * *Files identical despite different names*

