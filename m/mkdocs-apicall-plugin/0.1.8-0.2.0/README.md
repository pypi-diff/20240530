# Comparing `tmp/mkdocs_apicall_plugin-0.1.8.tar.gz` & `tmp/mkdocs_apicall_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_apicall_plugin-0.1.8.tar", max compression
+gzip compressed data, was "mkdocs_apicall_plugin-0.2.0.tar", max compression
```

## Comparing `mkdocs_apicall_plugin-0.1.8.tar` & `mkdocs_apicall_plugin-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-08-01 08:46:40.346405 mkdocs_apicall_plugin-0.1.8/LICENSE
--rw-r--r--   0        0        0     5919 2023-08-01 08:46:40.346405 mkdocs_apicall_plugin-0.1.8/README.md
--rw-r--r--   0        0        0       22 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/__init__.py
--rw-r--r--   0        0        0     2801 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/abstract.py
--rw-r--r--   0        0        0     1078 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/curl.py
--rw-r--r--   0        0        0     1119 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/javascript.py
--rw-r--r--   0        0        0     5625 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/main.py
--rw-r--r--   0        0        0      795 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/python.py
--rw-r--r--   0        0        0      713 2023-08-01 08:46:40.350405 mkdocs_apicall_plugin-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6844 1970-01-01 00:00:00.000000 mkdocs_apicall_plugin-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 07:18:00.031096 mkdocs_apicall_plugin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5935 2024-05-30 07:18:00.031096 mkdocs_apicall_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/__init__.py
+-rw-r--r--   0        0        0     2801 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/abstract.py
+-rw-r--r--   0        0        0     1078 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/curl.py
+-rw-r--r--   0        0        0     1119 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/javascript.py
+-rw-r--r--   0        0        0     5625 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/main.py
+-rw-r--r--   0        0        0      795 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/python.py
+-rw-r--r--   0        0        0      720 2024-05-30 07:18:00.035096 mkdocs_apicall_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6830 1970-01-01 00:00:00.000000 mkdocs_apicall_plugin-0.2.0/PKG-INFO
```

### Comparing `mkdocs_apicall_plugin-0.1.8/LICENSE` & `mkdocs_apicall_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.8/README.md` & `mkdocs_apicall_plugin-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -144,10 +144,13 @@
 | `_url`             | `str`                 | API endpoint to reach                                                                 |
 | `_headers`         | `Dict[str, Any]`      | HTTP headers                                                                          |
 | `_body`            | `str`                 | Raw body as string (as it is written in the API call within the markdown source file) |
 | `_max_line_length` | `int`                 | Maximum line length desired                                                           |
 | `_print_icon`      | `bool`                | Whether the icon will be printed (normally it does have impact on your dev)           |
 | `_language_config` | `dict`                | Language specific configuration                                                       |
 
-:warning: You are responsible of the possible default values of the`_language_config` attribute.
+> [!WARNING]  
+> You are responsible of the possible default values of the`_language_config` attribute.
+
+> [!WARNING]  
+> You are encouraged to render code differently according to the value of `_max_line_length`. One may imagine at least an *inline* and a *multiline* rendering.
 
-:warning: You are encouraged to render code differently according to the value of `_max_line_length`. One may imagine at least an *inline* and a *multiline* rendering.
```

### Comparing `mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/abstract.py` & `mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/curl.py` & `mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/curl.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/javascript.py` & `mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/javascript.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/main.py` & `mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/main.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.8/mkdocs_apicall_plugin/python.py` & `mkdocs_apicall_plugin-0.2.0/mkdocs_apicall_plugin/python.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.8/pyproject.toml` & `mkdocs_apicall_plugin-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "mkdocs-apicall-plugin"
-version = "0.1.8"
+version = "0.2.0"
 description = "Auto-generate code samples to make API calls"
 authors = ["Alban Siffer <alban@situation.sh>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/asiffer/mkdocs-apicall-plugin"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.1.4"
-black = "^23.1.0"
-Pygments = "^2.14.0"
+mkdocs = ">=1.4.2"
+mkdocs-material = ">=9.1.4"
+black = ">=23.1.0"
+Pygments = ">=2.14.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
-coverage = "^7.2.2"
-mkdocs-markdownextradata-plugin = "^0.2.5"
+pytest = ">=7.2.2"
+coverage = ">=7.2.2"
+mkdocs-markdownextradata-plugin = ">=0.2.5"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 apicall = 'mkdocs_apicall_plugin.main:APICallPlugin'
```

### Comparing `mkdocs_apicall_plugin-0.1.8/PKG-INFO` & `mkdocs_apicall_plugin-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mkdocs-apicall-plugin
-Version: 0.1.8
+Version: 0.2.0
 Summary: Auto-generate code samples to make API calls
 Home-page: https://github.com/asiffer/mkdocs-apicall-plugin
 License: Apache-2.0
 Author: Alban Siffer
 Author-email: alban@situation.sh
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pygments (>=2.14.0,<3.0.0)
-Requires-Dist: black (>=23.1.0,<24.0.0)
-Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.1.4,<10.0.0)
+Requires-Dist: Pygments (>=2.14.0)
+Requires-Dist: black (>=23.1.0)
+Requires-Dist: mkdocs (>=1.4.2)
+Requires-Dist: mkdocs-material (>=9.1.4)
 Project-URL: Repository, https://github.com/asiffer/mkdocs-apicall-plugin
 Description-Content-Type: text/markdown
 
 # mkdocs-apicall-plugin
 
 [![Build](https://github.com/asiffer/mkdocs-apicall-plugin/actions/workflows/build.yaml/badge.svg)](https://github.com/asiffer/mkdocs-apicall-plugin/actions/workflows/build.yaml)
 [![Publish](https://github.com/asiffer/mkdocs-apicall-plugin/actions/workflows/publish.yaml/badge.svg)](https://github.com/asiffer/mkdocs-apicall-plugin/actions/workflows/publish.yaml)
@@ -167,10 +167,14 @@
 | `_url`             | `str`                 | API endpoint to reach                                                                 |
 | `_headers`         | `Dict[str, Any]`      | HTTP headers                                                                          |
 | `_body`            | `str`                 | Raw body as string (as it is written in the API call within the markdown source file) |
 | `_max_line_length` | `int`                 | Maximum line length desired                                                           |
 | `_print_icon`      | `bool`                | Whether the icon will be printed (normally it does have impact on your dev)           |
 | `_language_config` | `dict`                | Language specific configuration                                                       |
 
-:warning: You are responsible of the possible default values of the`_language_config` attribute.
+> [!WARNING]  
+> You are responsible of the possible default values of the`_language_config` attribute.
+
+> [!WARNING]  
+> You are encouraged to render code differently according to the value of `_max_line_length`. One may imagine at least an *inline* and a *multiline* rendering.
+
 
-:warning: You are encouraged to render code differently according to the value of `_max_line_length`. One may imagine at least an *inline* and a *multiline* rendering.
```

