# Comparing `tmp/hogql_parser-1.0.7.tar.gz` & `tmp/hogql_parser-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hogql_parser-1.0.7.tar", last modified: Fri Apr  5 10:50:56 2024, max compression
+gzip compressed data, was "hogql_parser-1.0.8.tar", last modified: Tue May 21 08:18:28 2024, max compression
```

## Comparing `hogql_parser-1.0.7.tar` & `hogql_parser-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    73182 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLLexer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   319116 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLParser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLParserBaseVisitor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLParserVisitor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/error.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/hogql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    80472 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/string.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:18:28.649929 hogql_parser-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    73182 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/HogQLLexer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   319116 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/HogQLParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/HogQLParserBaseVisitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/HogQLParserVisitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-21 08:18:28.649929 hogql_parser-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/error.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:18:28.649929 hogql_parser-1.0.8/hogql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-21 08:18:28.000000 hogql_parser-1.0.8/hogql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 08:18:28.000000 hogql_parser-1.0.8/hogql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:18:28.000000 hogql_parser-1.0.8/hogql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 08:18:28.000000 hogql_parser-1.0.8/hogql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    80432 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:18:28.649929 hogql_parser-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-21 08:18:24.000000 hogql_parser-1.0.8/string.cpp
```

### Comparing `hogql_parser-1.0.7/HogQLLexer.cpp` & `hogql_parser-1.0.8/HogQLLexer.cpp`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.7/HogQLParser.cpp` & `hogql_parser-1.0.8/HogQLParser.cpp`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.7/PKG-INFO` & `hogql_parser-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hogql_parser
-Version: 1.0.7
+Version: 1.0.8
 Summary: HogQL parser for internal PostHog use
 Home-page: https://github.com/PostHog/posthog/tree/master/hogql_parser
 Author: PostHog Inc.
 Author-email: hey@posthog.com
 Maintainer: PostHog Inc.
 Maintainer-email: hey@posthog.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hogql_parser-1.0.7/error.cpp` & `hogql_parser-1.0.8/error.cpp`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.7/hogql_parser.egg-info/PKG-INFO` & `hogql_parser-1.0.8/hogql_parser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hogql-parser
-Version: 1.0.7
+Version: 1.0.8
 Summary: HogQL parser for internal PostHog use
 Home-page: https://github.com/PostHog/posthog/tree/master/hogql_parser
 Author: PostHog Inc.
 Author-email: hey@posthog.com
 Maintainer: PostHog Inc.
 Maintainer-email: hey@posthog.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hogql_parser-1.0.7/parser.cpp` & `hogql_parser-1.0.8/parser.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -853,30 +853,27 @@
     }
     return boost::algorithm::join(tokens, " ");
   }
 
   VISIT_UNSUPPORTED(JoinOpCross)
 
   VISIT(JoinConstraintClause) {
-    if (ctx->USING()) {
-      throw NotImplementedError("Unsupported: JOIN ... USING");
-    }
     PyObject* column_expr_list = visitAsPyObject(ctx->columnExprList());
     Py_ssize_t column_expr_list_size = PyList_Size(column_expr_list);
     if (column_expr_list_size == -1) {
       Py_DECREF(column_expr_list);
       throw PyInternalError();
     }
     if (column_expr_list_size > 1) {
       Py_DECREF(column_expr_list);
       throw NotImplementedError("Unsupported: JOIN ... ON with multiple expressions");
     }
     PyObject* expr = Py_NewRef(PyList_GET_ITEM(column_expr_list, 0));
     Py_DECREF(column_expr_list);
-    RETURN_NEW_AST_NODE("JoinConstraint", "{s:N}", "expr", expr);
+    RETURN_NEW_AST_NODE("JoinConstraint", "{s:N,s:s}", "expr", expr, "constraint_type", ctx->USING() ? "USING" : "ON");
   }
 
   VISIT(SampleClause) {
     PyObject* sample_ratio_expr = visitAsPyObject(ctx->ratioExpr(0));
     PyObject* offset_ratio_expr;
     try {
       offset_ratio_expr = visitAsPyObjectOrNone(ctx->ratioExpr(1));
```

### Comparing `hogql_parser-1.0.7/pyproject.toml` & `hogql_parser-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.7/setup.py` & `hogql_parser-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     library_dirs=[f"{homebrew_location}/lib/"] if is_macos else ["/usr/lib/", "/usr/lib64/"],
     libraries=["antlr4-runtime"],
     extra_compile_args=["-std=c++20"],
 )
 
 setup(
     name="hogql_parser",
-    version="1.0.7",
+    version="1.0.8",
     url="https://github.com/PostHog/posthog/tree/master/hogql_parser",
     author="PostHog Inc.",
     author_email="hey@posthog.com",
     maintainer="PostHog Inc.",
     maintainer_email="hey@posthog.com",
     description="HogQL parser for internal PostHog use",
     long_description=open("README.md").read(),
```

### Comparing `hogql_parser-1.0.7/string.cpp` & `hogql_parser-1.0.8/string.cpp`

 * *Files identical despite different names*

