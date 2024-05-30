# Comparing `tmp/guppylang-0.3.0.tar.gz` & `tmp/guppylang-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guppylang-0.3.0.tar", max compression
+gzip compressed data, was "guppylang-0.4.0.tar", max compression
```

## Comparing `guppylang-0.3.0.tar` & `guppylang-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-01-16 13:03:20.692812 guppylang-0.3.0/LICENCE
--rw-r--r--   0        0        0      240 2024-03-06 14:35:45.141750 guppylang-0.3.0/guppylang/__init__.py
--rw-r--r--   0        0        0    11717 2024-05-16 08:19:39.071491 guppylang-0.3.0/guppylang/ast_util.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.099571 guppylang-0.3.0/guppylang/cfg/__init__.py
--rw-r--r--   0        0        0     6805 2024-04-11 15:37:05.443728 guppylang-0.3.0/guppylang/cfg/analysis.py
--rw-r--r--   0        0        0     5600 2024-01-18 13:08:34.099944 guppylang-0.3.0/guppylang/cfg/bb.py
--rw-r--r--   0        0        0    20103 2024-03-19 17:26:38.075014 guppylang-0.3.0/guppylang/cfg/builder.py
--rw-r--r--   0        0        0     2034 2024-01-18 13:08:34.100296 guppylang-0.3.0/guppylang/cfg/cfg.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.100352 guppylang-0.3.0/guppylang/checker/__init__.py
--rw-r--r--   0        0        0     9267 2024-04-16 10:39:14.815309 guppylang-0.3.0/guppylang/checker/cfg_checker.py
--rw-r--r--   0        0        0     7303 2024-05-21 08:25:07.488971 guppylang-0.3.0/guppylang/checker/core.py
--rw-r--r--   0        0        0    43253 2024-05-15 11:05:11.494825 guppylang-0.3.0/guppylang/checker/expr_checker.py
--rw-r--r--   0        0        0     6515 2024-05-16 08:19:39.072106 guppylang-0.3.0/guppylang/checker/func_checker.py
--rw-r--r--   0        0        0     6466 2024-03-19 17:26:38.077637 guppylang-0.3.0/guppylang/checker/stmt_checker.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.101552 guppylang-0.3.0/guppylang/compiler/__init__.py
--rw-r--r--   0        0        0     6864 2024-05-16 08:39:58.377179 guppylang-0.3.0/guppylang/compiler/cfg_compiler.py
--rw-r--r--   0        0        0     2774 2024-05-16 08:39:58.377318 guppylang-0.3.0/guppylang/compiler/core.py
--rw-r--r--   0        0        0    16773 2024-05-22 14:23:20.915219 guppylang-0.3.0/guppylang/compiler/expr_compiler.py
--rw-r--r--   0        0        0     3433 2024-05-16 08:39:58.377812 guppylang-0.3.0/guppylang/compiler/func_compiler.py
--rw-r--r--   0        0        0     3509 2024-05-16 08:39:58.377937 guppylang-0.3.0/guppylang/compiler/stmt_compiler.py
--rw-r--r--   0        0        0     9397 2024-05-16 08:39:58.378210 guppylang-0.3.0/guppylang/decorator.py
--rw-r--r--   0        0        0        0 2024-04-16 10:39:14.818760 guppylang-0.3.0/guppylang/definition/__init__.py
--rw-r--r--   0        0        0     4063 2024-05-16 08:39:58.378467 guppylang-0.3.0/guppylang/definition/common.py
--rw-r--r--   0        0        0    10028 2024-05-16 08:39:58.378624 guppylang-0.3.0/guppylang/definition/custom.py
--rw-r--r--   0        0        0     4153 2024-05-16 08:39:58.378758 guppylang-0.3.0/guppylang/definition/declaration.py
--rw-r--r--   0        0        0     6560 2024-05-16 08:39:58.378889 guppylang-0.3.0/guppylang/definition/function.py
--rw-r--r--   0        0        0      768 2024-04-16 10:39:14.820919 guppylang-0.3.0/guppylang/definition/parameter.py
--rw-r--r--   0        0        0    10623 2024-05-16 08:19:39.074117 guppylang-0.3.0/guppylang/definition/struct.py
--rw-r--r--   0        0        0     1745 2024-05-16 08:39:58.379178 guppylang-0.3.0/guppylang/definition/ty.py
--rw-r--r--   0        0        0     2880 2024-05-16 08:39:58.379286 guppylang-0.3.0/guppylang/definition/value.py
--rw-r--r--   0        0        0     6043 2024-03-19 17:26:38.079877 guppylang-0.3.0/guppylang/error.py
--rw-r--r--   0        0        0        0 2024-01-30 13:18:23.816770 guppylang-0.3.0/guppylang/graph.hugr
--rw-r--r--   0        0        0    17256 2024-05-14 08:36:03.085334 guppylang-0.3.0/guppylang/graph.json
--rw-r--r--   0        0        0        0 2024-05-16 08:39:58.379321 guppylang-0.3.0/guppylang/hugr_builder/__init__.py
--rw-r--r--   0        0        0    30252 2024-05-16 08:39:58.379625 guppylang-0.3.0/guppylang/hugr_builder/hugr.py
--rw-r--r--   0        0        0     8223 2024-05-16 08:39:58.379735 guppylang-0.3.0/guppylang/hugr_builder/visualise.py
--rw-r--r--   0        0        0     9099 2024-05-16 08:39:58.379946 guppylang-0.3.0/guppylang/module.py
--rw-r--r--   0        0        0     4173 2024-05-15 11:05:11.496569 guppylang-0.3.0/guppylang/nodes.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.104139 guppylang-0.3.0/guppylang/prelude/__init__.py
--rw-r--r--   0        0        0    12756 2024-05-21 08:31:14.534985 guppylang-0.3.0/guppylang/prelude/_internal.py
--rw-r--r--   0        0        0    21940 2024-05-21 08:25:07.490151 guppylang-0.3.0/guppylang/prelude/builtins.py
--rw-r--r--   0        0        0     2695 2024-05-16 08:39:58.380535 guppylang-0.3.0/guppylang/prelude/quantum.py
--rw-r--r--   0        0        0        0 2024-03-04 15:19:40.627545 guppylang-0.3.0/guppylang/py.typed
--rw-r--r--   0        0        0    57008 2024-05-14 08:36:02.964537 guppylang-0.3.0/guppylang/test
--rw-r--r--   0        0        0   110258 2024-05-14 08:36:03.079698 guppylang-0.3.0/guppylang/test.svg
--rw-r--r--   0        0        0        0 2024-03-19 17:26:38.082129 guppylang-0.3.0/guppylang/tys/__init__.py
--rw-r--r--   0        0        0     2952 2024-05-16 15:53:50.323816 guppylang-0.3.0/guppylang/tys/arg.py
--rw-r--r--   0        0        0     5348 2024-05-21 08:25:07.490527 guppylang-0.3.0/guppylang/tys/builtin.py
--rw-r--r--   0        0        0     1835 2024-05-08 13:56:29.603685 guppylang-0.3.0/guppylang/tys/common.py
--rw-r--r--   0        0        0     1865 2024-05-16 10:25:22.563789 guppylang-0.3.0/guppylang/tys/const.py
--rw-r--r--   0        0        0     6818 2024-05-16 15:53:50.324510 guppylang-0.3.0/guppylang/tys/param.py
--rw-r--r--   0        0        0     5232 2024-05-16 08:19:39.075330 guppylang-0.3.0/guppylang/tys/parsing.py
--rw-r--r--   0        0        0     4489 2024-05-21 08:25:07.490807 guppylang-0.3.0/guppylang/tys/printing.py
--rw-r--r--   0        0        0     2209 2024-05-15 14:51:55.689897 guppylang-0.3.0/guppylang/tys/subst.py
--rw-r--r--   0        0        0    22318 2024-05-21 08:25:07.491323 guppylang-0.3.0/guppylang/tys/ty.py
--rw-r--r--   0        0        0     1174 2024-03-19 17:26:38.084390 guppylang-0.3.0/guppylang/tys/var.py
--rw-r--r--   0        0        0     1226 2024-05-22 14:23:20.916921 guppylang-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      646 2024-03-06 14:35:45.146062 guppylang-0.3.0/quickstart.md
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 guppylang-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 10:08:45.374321 guppylang-0.4.0/LICENCE
+-rw-r--r--   0        0        0      244 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/__init__.py
+-rw-r--r--   0        0        0    11717 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/ast_util.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/cfg/__init__.py
+-rw-r--r--   0        0        0     6805 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/cfg/analysis.py
+-rw-r--r--   0        0        0     5600 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/cfg/bb.py
+-rw-r--r--   0        0        0    20103 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/cfg/builder.py
+-rw-r--r--   0        0        0     2034 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/cfg/cfg.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/checker/__init__.py
+-rw-r--r--   0        0        0     9267 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/checker/cfg_checker.py
+-rw-r--r--   0        0        0     7303 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/checker/core.py
+-rw-r--r--   0        0        0    43253 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/checker/expr_checker.py
+-rw-r--r--   0        0        0     6513 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/checker/func_checker.py
+-rw-r--r--   0        0        0     6466 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/checker/stmt_checker.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/compiler/__init__.py
+-rw-r--r--   0        0        0     6864 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/compiler/cfg_compiler.py
+-rw-r--r--   0        0        0     2774 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/compiler/core.py
+-rw-r--r--   0        0        0    16773 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/compiler/expr_compiler.py
+-rw-r--r--   0        0        0     3433 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/compiler/func_compiler.py
+-rw-r--r--   0        0        0     3509 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/compiler/stmt_compiler.py
+-rw-r--r--   0        0        0     9397 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/decorator.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/__init__.py
+-rw-r--r--   0        0        0     4063 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/common.py
+-rw-r--r--   0        0        0    10028 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/custom.py
+-rw-r--r--   0        0        0     4153 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/declaration.py
+-rw-r--r--   0        0        0     6560 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/function.py
+-rw-r--r--   0        0        0      768 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/parameter.py
+-rw-r--r--   0        0        0    10623 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/struct.py
+-rw-r--r--   0        0        0     1745 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/ty.py
+-rw-r--r--   0        0        0     2880 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/definition/value.py
+-rw-r--r--   0        0        0     6043 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/error.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/hugr_builder/__init__.py
+-rw-r--r--   0        0        0    30252 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/hugr_builder/hugr.py
+-rw-r--r--   0        0        0     8223 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/hugr_builder/visualise.py
+-rw-r--r--   0        0        0     9099 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/module.py
+-rw-r--r--   0        0        0     4173 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/nodes.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/prelude/__init__.py
+-rw-r--r--   0        0        0    12756 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/prelude/_internal.py
+-rw-r--r--   0        0        0    22319 2024-05-30 10:08:45.378321 guppylang-0.4.0/guppylang/prelude/builtins.py
+-rw-r--r--   0        0        0     2695 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/prelude/quantum.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/py.typed
+-rw-r--r--   0        0        0        0 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/__init__.py
+-rw-r--r--   0        0        0     2952 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/arg.py
+-rw-r--r--   0        0        0     5348 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/builtin.py
+-rw-r--r--   0        0        0     1835 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/common.py
+-rw-r--r--   0        0        0     1865 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/const.py
+-rw-r--r--   0        0        0     6818 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/param.py
+-rw-r--r--   0        0        0     5232 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/parsing.py
+-rw-r--r--   0        0        0     4489 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/printing.py
+-rw-r--r--   0        0        0     2209 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/subst.py
+-rw-r--r--   0        0        0    22318 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/ty.py
+-rw-r--r--   0        0        0     1174 2024-05-30 10:08:45.382321 guppylang-0.4.0/guppylang/tys/var.py
+-rw-r--r--   0        0        0     1226 2024-05-30 10:08:45.382321 guppylang-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      646 2024-05-30 10:08:45.382321 guppylang-0.4.0/quickstart.md
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 guppylang-0.4.0/PKG-INFO
```

### Comparing `guppylang-0.3.0/LICENCE` & `guppylang-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/ast_util.py` & `guppylang-0.4.0/guppylang/ast_util.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/cfg/analysis.py` & `guppylang-0.4.0/guppylang/cfg/analysis.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/cfg/bb.py` & `guppylang-0.4.0/guppylang/cfg/bb.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/cfg/builder.py` & `guppylang-0.4.0/guppylang/cfg/builder.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/cfg/cfg.py` & `guppylang-0.4.0/guppylang/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/checker/cfg_checker.py` & `guppylang-0.4.0/guppylang/checker/cfg_checker.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/checker/core.py` & `guppylang-0.4.0/guppylang/checker/core.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/checker/expr_checker.py` & `guppylang-0.4.0/guppylang/checker/expr_checker.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/checker/func_checker.py` & `guppylang-0.4.0/guppylang/checker/func_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             raise GuppyError(
                 "Return type must be annotated. Try adding a `-> None` annotation.",
                 func_def,
             )
         raise GuppyError("Return type must be annotated", func_def)
 
     # TODO: Prepopulate mapping when using Python 3.12 style generic functions
-    param_var_mapping: dict[str, "Parameter"] = {}
+    param_var_mapping: dict[str, Parameter] = {}
     input_tys = []
     input_names = []
     for inp in func_def.args.args:
         if inp.annotation is None:
             raise GuppyError("Argument type must be annotated", inp)
         ty = type_from_ast(inp.annotation, globals, param_var_mapping)
         input_tys.append(ty)
```

### Comparing `guppylang-0.3.0/guppylang/checker/stmt_checker.py` & `guppylang-0.4.0/guppylang/checker/stmt_checker.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/compiler/cfg_compiler.py` & `guppylang-0.4.0/guppylang/compiler/cfg_compiler.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/compiler/core.py` & `guppylang-0.4.0/guppylang/compiler/core.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/compiler/expr_compiler.py` & `guppylang-0.4.0/guppylang/compiler/expr_compiler.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/compiler/func_compiler.py` & `guppylang-0.4.0/guppylang/compiler/func_compiler.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/compiler/stmt_compiler.py` & `guppylang-0.4.0/guppylang/compiler/stmt_compiler.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/decorator.py` & `guppylang-0.4.0/guppylang/decorator.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/common.py` & `guppylang-0.4.0/guppylang/definition/common.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/custom.py` & `guppylang-0.4.0/guppylang/definition/custom.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/declaration.py` & `guppylang-0.4.0/guppylang/definition/declaration.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/function.py` & `guppylang-0.4.0/guppylang/definition/function.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/parameter.py` & `guppylang-0.4.0/guppylang/definition/parameter.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/struct.py` & `guppylang-0.4.0/guppylang/definition/struct.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/ty.py` & `guppylang-0.4.0/guppylang/definition/ty.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/definition/value.py` & `guppylang-0.4.0/guppylang/definition/value.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/error.py` & `guppylang-0.4.0/guppylang/error.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/hugr_builder/hugr.py` & `guppylang-0.4.0/guppylang/hugr_builder/hugr.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/hugr_builder/visualise.py` & `guppylang-0.4.0/guppylang/hugr_builder/visualise.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/module.py` & `guppylang-0.4.0/guppylang/module.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/nodes.py` & `guppylang-0.4.0/guppylang/nodes.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/prelude/_internal.py` & `guppylang-0.4.0/guppylang/prelude/_internal.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/prelude/builtins.py` & `guppylang-0.4.0/guppylang/prelude/builtins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Guppy module for builtin types and operations."""
 
 # mypy: disable-error-code="empty-body, misc, override, valid-type, no-untyped-def"
 
+from typing import Any
+
 from hugr.serialization import tys
 
 from guppylang.decorator import guppy
 from guppylang.definition.custom import DefaultCallChecker, NoopCompiler
+from guppylang.error import GuppyError
 from guppylang.hugr_builder.hugr import DummyOp
 from guppylang.module import GuppyModule
 from guppylang.prelude._internal import (
     CallableChecker,
     CoercingChecker,
     DunderChecker,
     FailingChecker,
@@ -30,14 +33,23 @@
 
 builtins = GuppyModule("builtins", import_builtins=False)
 
 T = guppy.type_var(builtins, "T")
 L = guppy.type_var(builtins, "L", linear=True)
 
 
+def py(*_args: Any) -> Any:
+    """Function to tag compile-time evaluated Python expressions in a Guppy context.
+
+    This function throws an error when execute in a Python context. It is only intended
+    to be used inside Guppy functions.
+    """
+    raise GuppyError("`py` can only by used in a Guppy context")
+
+
 @guppy.extend_type(builtins, bool_type_def)
 class Bool:
     @guppy.hugr_op(builtins, logic_op("And", [tys.TypeArg(tys.BoundedNatArg(n=2))]))
     def __and__(self: bool, other: bool) -> bool: ...
 
     @guppy.custom(builtins, NoopCompiler())
     def __bool__(self: bool) -> bool: ...
```

### Comparing `guppylang-0.3.0/guppylang/prelude/quantum.py` & `guppylang-0.4.0/guppylang/prelude/quantum.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/arg.py` & `guppylang-0.4.0/guppylang/tys/arg.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/builtin.py` & `guppylang-0.4.0/guppylang/tys/builtin.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/common.py` & `guppylang-0.4.0/guppylang/tys/common.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/const.py` & `guppylang-0.4.0/guppylang/tys/const.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/param.py` & `guppylang-0.4.0/guppylang/tys/param.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/parsing.py` & `guppylang-0.4.0/guppylang/tys/parsing.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/printing.py` & `guppylang-0.4.0/guppylang/tys/printing.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/subst.py` & `guppylang-0.4.0/guppylang/tys/subst.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/ty.py` & `guppylang-0.4.0/guppylang/tys/ty.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/guppylang/tys/var.py` & `guppylang-0.4.0/guppylang/tys/var.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/pyproject.toml` & `guppylang-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guppylang"
-version = "0.3.0"
+version = "0.4.0"
 description = "Pythonic quantum-classical programming language"
 authors = ["Mark Koch <mark.koch@quantinuum.com>"]
 license = "Apache-2.0"
 readme = "quickstart.md"
 repository = "https://github.com/CQCL/guppy"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 hugr = "~0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 mypy = "^1.8.0"
 pre-commit = "^3.6.0"
-ruff = ">=0.4.2"
+ruff = ">=0.4.5"
 maturin = "^1.4.0"
 pytket = "*"
 
 [tool.poetry.group.validation]
 optional = true
 
 [tool.poetry.group.validation.dependencies]
```

### Comparing `guppylang-0.3.0/quickstart.md` & `guppylang-0.4.0/quickstart.md`

 * *Files identical despite different names*

### Comparing `guppylang-0.3.0/PKG-INFO` & `guppylang-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guppylang
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pythonic quantum-classical programming language
 Home-page: https://github.com/CQCL/guppy
 License: Apache-2.0
 Author: Mark Koch
 Author-email: mark.koch@quantinuum.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

