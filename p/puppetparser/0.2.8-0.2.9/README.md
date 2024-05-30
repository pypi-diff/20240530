# Comparing `tmp/puppetparser-0.2.8.tar.gz` & `tmp/puppetparser-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puppetparser-0.2.8.tar", max compression
+gzip compressed data, was "puppetparser-0.2.9.tar", max compression
```

## Comparing `puppetparser-0.2.8.tar` & `puppetparser-0.2.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.8/LICENSE
--rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.8/README.md
--rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.8/puppetparser/.gitignore
--rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.8/puppetparser/__init__.py
--rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.8/puppetparser/__main__.py
--rw-r--r--   0        0        0    12018 2024-05-17 17:03:35.701533 puppetparser-0.2.8/puppetparser/model.py
--rw-r--r--   0        0        0    65624 2024-05-17 17:10:00.096096 puppetparser-0.2.8/puppetparser/parser.py
--rw-r--r--   0        0        0     1001 2024-05-17 10:50:47.862136 puppetparser-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.9/LICENSE
+-rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.9/README.md
+-rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.9/puppetparser/.gitignore
+-rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.9/puppetparser/__init__.py
+-rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.9/puppetparser/__main__.py
+-rw-r--r--   0        0        0    12015 2024-05-17 17:38:27.492561 puppetparser-0.2.9/puppetparser/model.py
+-rw-r--r--   0        0        0    66199 2024-05-30 15:03:10.604698 puppetparser-0.2.9/puppetparser/parser.py
+-rw-r--r--   0        0        0     1001 2024-05-30 15:04:42.683452 puppetparser-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.9/PKG-INFO
```

### Comparing `puppetparser-0.2.8/LICENSE` & `puppetparser-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.8/README.md` & `puppetparser-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.8/puppetparser/model.py` & `puppetparser-0.2.9/puppetparser/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         return self.value == __o.value
 
     def __hash__(self) -> int:
         if self.value is None:
             return 0
 
         return self.value.__hash__()  # type: ignore
-    
+
+
 class Id(Value[str]):
     def __init__(
         self, line: int, col: int, end_line: int, end_col: int, value: str
     ) -> None:
         super().__init__(line, col, end_line, end_col, value)
```

### Comparing `puppetparser-0.2.8/puppetparser/parser.py` & `puppetparser-0.2.9/puppetparser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,26 +680,33 @@
                 find_column(script, p.lexpos(1)),
                 p.lineno(2),
                 find_column(script, p.lexpos(2)),
             )
 
     def p_virtual_resource(p: YaccProduction):
         r"resource : AT ID LBRACKET resource_list RBRACKET"
+        id = Id(
+            p.lineno(2),
+            find_column(script, p.lexpos(2)),
+            p.lineno(2),
+            find_column(script, p.lexpos(2)) + len(p[2]),
+            "@" + p[2],
+        )
         if len(p[4]) == 1:
             p[0] = Resource(
                 p.lineno(2),
                 find_column(script, p.lexpos(2)),
                 p.lineno(5),
                 find_column(script, p.lexpos(5)) + 1,
-                "@" + p[2],
+                id,
                 p[4][0][0],
                 p[4][0][1],
             )
         else:
-            resources = map(lambda r: Resource(r[2], r[3], r[4], r[5], "@" + p[2], r[0], r[1]), p[4])  # type: ignore
+            resources = map(lambda r: Resource(r[2], r[3], r[4], r[5], id, r[0], r[1]), p[4])  # type: ignore
             default = None
             for r in resources:
                 if isinstance(r.title, Value) and r.title.value == "default":
                     default = r
                     break
             resources = list(
                 filter(
@@ -715,26 +722,34 @@
                 find_column(script, p.lexpos(5)) + 1,
                 default,
                 resources,
             )
 
     def p_exported_resource(p: YaccProduction):
         r"resource : AT AT ID LBRACKET resource_list RBRACKET"
+        id = Id(
+            p.lineno(3),
+            find_column(script, p.lexpos(3)),
+            p.lineno(3),
+            find_column(script, p.lexpos(3)) + len(p[3]),
+            "@@" + p[3],
+        )
+
         if len(p[4]) == 1:
             p[0] = Resource(
                 p.lineno(3),
                 find_column(script, p.lexpos(3)),
                 p.lineno(6),
                 find_column(script, p.lexpos(6)) + 1,
-                "@@" + p[3],
+                id,
                 p[5][0][0],
                 p[5][0][1],
             )
         else:
-            resources = map(lambda r: Resource(r[2], r[3], r[4], r[5], "@@" + p[3], r[0], r[1]), p[5])  # type: ignore
+            resources = map(lambda r: Resource(r[2], r[3], r[4], r[5], id, r[0], r[1]), p[5])  # type: ignore
             default = None
             for r in resources:
                 if isinstance(r.title, Value) and r.title.value == "default":
                     default = r
                     break
             resources = list(
                 filter(
@@ -788,20 +803,27 @@
             p[1],
             None,
             p[3],
         )
 
     def p_resource_default(p: YaccProduction):
         r"resource : ID_TYPE LBRACKET attributes RBRACKET"
+        id = Id(
+            p.lineno(1),
+            find_column(script, p.lexpos(1)),
+            p.lineno(1),
+            find_column(script, p.lexpos(1)) + len(p[1]),
+            p[1],
+        )
         p[0] = Resource(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(4),
             find_column(script, p.lexpos(4)) + 1,
-            p[1],
+            id,
             None,
             p[3],
         )
 
     def p_resource_declaration(p: YaccProduction):
         r"resource : DEFINE ID LPAREN parameters RPAREN LBRACKET block RBRACKET"
         p[0] = ResourceDeclaration(
@@ -828,26 +850,26 @@
 
     def p_resource_collector(p: YaccProduction):
         r"resource_collector : ID_TYPE LANGLEBRACKET rc_expression RANGLEBRACKET"
         p[0] = ResourceCollector(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(4),
-            find_column(script, p.lexpos(4)) + 1,
+            find_column(script, p.lexpos(4)) + 2,
             p[1],
             p[3],
         )
 
     def p_resource_collector_empty(p: YaccProduction):
         r"resource_collector : ID_TYPE LANGLEBRACKET RANGLEBRACKET"
         p[0] = ResourceCollector(
             p.lineno(1),
             find_column(script, p.lexpos(1)),
             p.lineno(3),
-            find_column(script, p.lexpos(3)) + 1,
+            find_column(script, p.lexpos(3)) + 2,
             p[1],
             None,
         )
 
     def p_resource_collector_expression_equal(p: YaccProduction):
         r"rc_expression : rc_expression CMP_EQUAL rc_expression"
         p[0] = Operation(
```

### Comparing `puppetparser-0.2.8/pyproject.toml` & `puppetparser-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "puppetparser"
-version = "0.2.8"
+version = "0.2.9"
 description = "A parser from Puppet to an object model"
 authors = ["Nuno Saavedra <nuno.saavedra@tecnico.ulisboa.pt>"]
 license = "GPL-3.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `puppetparser-0.2.8/PKG-INFO` & `puppetparser-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puppetparser
-Version: 0.2.8
+Version: 0.2.9
 Summary: A parser from Puppet to an object model
 License: GPL-3.0
 Keywords: puppet,parser,object model
 Author: Nuno Saavedra
 Author-email: nuno.saavedra@tecnico.ulisboa.pt
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

