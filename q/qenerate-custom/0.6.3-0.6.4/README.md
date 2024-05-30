# Comparing `tmp/qenerate_custom-0.6.3.tar.gz` & `tmp/qenerate_custom-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qenerate_custom-0.6.3.tar", max compression
+gzip compressed data, was "qenerate_custom-0.6.4.tar", max compression
```

## Comparing `qenerate_custom-0.6.3.tar` & `qenerate_custom-0.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11350 2024-01-28 03:42:33.193282 qenerate_custom-0.6.3/LICENSE
--rw-r--r--   0        0        0     6551 2024-02-19 04:06:37.654447 qenerate_custom-0.6.3/README.md
--rw-r--r--   0        0        0     1544 2024-02-19 04:20:10.257096 qenerate_custom-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/__init__.py
--rw-r--r--   0        0        0     1528 2024-02-19 04:11:27.322090 qenerate_custom-0.6.3/qenerate/cli.py
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/__init__.py
--rw-r--r--   0        0        0     3797 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/code_command.py
--rw-r--r--   0        0        0     2105 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/feature_flag_parser.py
--rw-r--r--   0        0        0      440 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/introspection_command.py
--rw-r--r--   0        0        0      856 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/plugin.py
--rw-r--r--   0        0        0     5302 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/preprocessor.py
--rw-r--r--   0        0        0     1652 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/core/unwrapper.py
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/__init__.py
--rw-r--r--   0        0        0     2123 2024-01-28 04:03:16.335007 qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/mapper.py
--rw-r--r--   0        0        0    18954 2024-01-28 09:04:19.756624 qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/plugin.py
--rw-r--r--   0        0        0     7188 2024-01-28 09:04:19.752624 qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/typed_ast.py
--rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 qenerate_custom-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11350 2024-01-28 03:42:33.193282 qenerate_custom-0.6.4/LICENSE
+-rw-r--r--   0        0        0     6551 2024-02-19 04:06:37.654447 qenerate_custom-0.6.4/README.md
+-rw-r--r--   0        0        0     1544 2024-05-30 01:42:14.782705 qenerate_custom-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/__init__.py
+-rw-r--r--   0        0        0     1528 2024-02-19 04:11:27.322090 qenerate_custom-0.6.4/qenerate/cli.py
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/__init__.py
+-rw-r--r--   0        0        0     3797 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/code_command.py
+-rw-r--r--   0        0        0     2105 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/feature_flag_parser.py
+-rw-r--r--   0        0        0      440 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/introspection_command.py
+-rw-r--r--   0        0        0      856 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/plugin.py
+-rw-r--r--   0        0        0     5302 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/preprocessor.py
+-rw-r--r--   0        0        0     1652 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/unwrapper.py
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0     2123 2024-01-28 04:03:16.335007 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/mapper.py
+-rw-r--r--   0        0        0    18838 2024-05-30 01:38:06.562076 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/plugin.py
+-rw-r--r--   0        0        0     7188 2024-01-28 09:04:19.752624 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/typed_ast.py
+-rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 qenerate_custom-0.6.4/PKG-INFO
```

### Comparing `qenerate_custom-0.6.3/LICENSE` & `qenerate_custom-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/README.md` & `qenerate_custom-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/pyproject.toml` & `qenerate_custom-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qenerate-custom"
-version = "0.6.3"
+version = "0.6.4"
 description = "Code Generator for GraphQL Query and Fragment Data Classes"
 authors = ["Red Hat - Service Delivery - AppSRE <sd-app-sre@redhat.com>"]
 maintainers = ["Red Hat - Service Delivery - AppSRE <sd-app-sre@redhat.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/app-sre/qenerate"
 repository = "https://github.com/app-sre/qenerate"
 documentation = "https://github.com/app-sre/qenerate"
```

### Comparing `qenerate_custom-0.6.3/qenerate/cli.py` & `qenerate_custom-0.6.4/qenerate/cli.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/core/code_command.py` & `qenerate_custom-0.6.4/qenerate/core/code_command.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/core/feature_flag_parser.py` & `qenerate_custom-0.6.4/qenerate/core/feature_flag_parser.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/core/plugin.py` & `qenerate_custom-0.6.4/qenerate/core/plugin.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/core/preprocessor.py` & `qenerate_custom-0.6.4/qenerate/core/preprocessor.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/core/unwrapper.py` & `qenerate_custom-0.6.4/qenerate/core/unwrapper.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/mapper.py` & `qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/mapper.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/plugin.py` & `qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,15 @@
     f"{INDENT}Json,\n"
     ")"
 )
 
 CONF = (
     f"class {BASE_CLASS_NAME}(BaseModel):\n"
     f"{INDENT}class Config:\n"
-    # https://pydantic-docs.helpmanual.io/usage/model_config/#smart-union
     # https://stackoverflow.com/a/69705356/4478420
-    f"{INDENT}{INDENT}smart_union=True\n"
     f"{INDENT}{INDENT}extra=Extra.forbid"
 )
 
 
 def query_convenience_function(cls: str) -> str:
     return f"""
 def query(query_func: Callable, **kwargs: Any) -> {cls}:
```

### Comparing `qenerate_custom-0.6.3/qenerate/plugins/pydantic_v1/typed_ast.py` & `qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/typed_ast.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.3/PKG-INFO` & `qenerate_custom-0.6.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qenerate-custom
-Version: 0.6.3
+Version: 0.6.4
 Summary: Code Generator for GraphQL Query and Fragment Data Classes
 Home-page: https://github.com/app-sre/qenerate
 License: Apache-2.0
 Author: Red Hat - Service Delivery - AppSRE
 Author-email: sd-app-sre@redhat.com
 Maintainer: Red Hat - Service Delivery - AppSRE
 Maintainer-email: sd-app-sre@redhat.com
```

