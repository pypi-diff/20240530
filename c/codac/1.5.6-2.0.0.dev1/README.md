# Comparing `tmp/codac-1.5.6-cp39-cp39-win_amd64.whl.zip` & `tmp/codac-2.0.0.dev1-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,13 @@
-Zip file size: 2056143 bytes, number of entries: 24
--rw-rw-rw-  2.0 fat     1395 b- defN 24-Apr-11 12:15 codac/__init__.py
--rw-rw-rw-  2.0 fat   343552 b- defN 24-Apr-11 12:19 codac/codac2.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  3726336 b- defN 24-Apr-11 12:19 codac/core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   890368 b- defN 24-Apr-11 12:19 codac/unsupported.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-11 12:15 codac/version.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 12:15 codac/tests/__init__.py
--rw-rw-rw-  2.0 fat     1302 b- defN 24-Apr-11 12:15 codac/tests/test_actions.py
--rw-rw-rw-  2.0 fat    31638 b- defN 24-Apr-11 12:15 codac/tests/test_arithmetic.py
--rw-rw-rw-  2.0 fat    16259 b- defN 24-Apr-11 12:15 codac/tests/test_cn.py
--rw-rw-rw-  2.0 fat     3773 b- defN 24-Apr-11 12:15 codac/tests/test_ctc_constell.py
--rw-rw-rw-  2.0 fat     1362 b- defN 24-Apr-11 12:15 codac/tests/test_ctcbox.py
--rw-rw-rw-  2.0 fat     1620 b- defN 24-Apr-11 12:15 codac/tests/test_ctccartprod.py
--rw-rw-rw-  2.0 fat     2023 b- defN 24-Apr-11 12:15 codac/tests/test_ctcdelay.py
--rw-rw-rw-  2.0 fat    45322 b- defN 24-Apr-11 12:15 codac/tests/test_ctceval.py
--rw-rw-rw-  2.0 fat      939 b- defN 24-Apr-11 12:15 codac/tests/test_ctcstatic.py
--rw-rw-rw-  2.0 fat    13567 b- defN 24-Apr-11 12:15 codac/tests/test_definition.py
--rw-rw-rw-  2.0 fat     1156 b- defN 24-Apr-11 12:15 codac/tests/test_function.py
--rw-rw-rw-  2.0 fat     4061 b- defN 24-Apr-11 12:15 codac/tests/test_multi_arithmetic.py
--rw-rw-rw-  2.0 fat     1524 b- defN 24-Apr-11 12:15 codac/tests/test_numpy.py
--rw-rw-rw-  2.0 fat     2057 b- defN 24-Apr-11 12:15 codac/tests/test_sepbox.py
--rw-rw-rw-  2.0 fat      630 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1982 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/RECORD
-24 files, 5090983 bytes uncompressed, 2052959 bytes compressed:  59.7%
+Zip file size: 643074 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     1465 b- defN 24-May-30 11:56 codac/__init__.py
+-rw-rw-rw-  2.0 fat  1366528 b- defN 24-May-30 11:58 codac/core.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    95232 b- defN 24-May-30 11:58 codac/graphics.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    95744 b- defN 24-May-30 11:57 codac/unsupported.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 24-May-30 11:56 codac/version.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-30 11:56 codac/tests/__init__.py
+-rw-rw-rw-  2.0 fat      248 b- defN 24-May-30 11:56 codac/tests/codac2_tests.py
+-rw-rw-rw-  2.0 fat      652 b- defN 24-May-30 11:58 codac-2.0.0.dev1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-30 11:58 codac-2.0.0.dev1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-30 11:58 codac-2.0.0.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      890 b- defN 24-May-30 11:58 codac-2.0.0.dev1.dist-info/RECORD
+11 files, 1560876 bytes uncompressed, 641568 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,73 +1,34 @@
 Filename: codac/__init__.py
 Comment: 
 
-Filename: codac/codac2.cp39-win_amd64.pyd
+Filename: codac/core.cp310-win_amd64.pyd
 Comment: 
 
-Filename: codac/core.cp39-win_amd64.pyd
+Filename: codac/graphics.cp310-win_amd64.pyd
 Comment: 
 
-Filename: codac/unsupported.cp39-win_amd64.pyd
+Filename: codac/unsupported.cp310-win_amd64.pyd
 Comment: 
 
 Filename: codac/version.py
 Comment: 
 
 Filename: codac/tests/__init__.py
 Comment: 
 
-Filename: codac/tests/test_actions.py
+Filename: codac/tests/codac2_tests.py
 Comment: 
 
-Filename: codac/tests/test_arithmetic.py
+Filename: codac-2.0.0.dev1.dist-info/METADATA
 Comment: 
 
-Filename: codac/tests/test_cn.py
+Filename: codac-2.0.0.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: codac/tests/test_ctc_constell.py
+Filename: codac-2.0.0.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: codac/tests/test_ctcbox.py
-Comment: 
-
-Filename: codac/tests/test_ctccartprod.py
-Comment: 
-
-Filename: codac/tests/test_ctcdelay.py
-Comment: 
-
-Filename: codac/tests/test_ctceval.py
-Comment: 
-
-Filename: codac/tests/test_ctcstatic.py
-Comment: 
-
-Filename: codac/tests/test_definition.py
-Comment: 
-
-Filename: codac/tests/test_function.py
-Comment: 
-
-Filename: codac/tests/test_multi_arithmetic.py
-Comment: 
-
-Filename: codac/tests/test_numpy.py
-Comment: 
-
-Filename: codac/tests/test_sepbox.py
-Comment: 
-
-Filename: codac-1.5.6.dist-info/METADATA
-Comment: 
-
-Filename: codac-1.5.6.dist-info/WHEEL
-Comment: 
-
-Filename: codac-1.5.6.dist-info/top_level.txt
-Comment: 
-
-Filename: codac-1.5.6.dist-info/RECORD
+Filename: codac-2.0.0.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## codac/__init__.py

```diff
@@ -1,39 +1,47 @@
-# Verifying that the former module pyibex 
-# has not been loaded, which could cause conflicts
-import sys
-if 'pyibex' in sys.modules:
-  print('\nWarning: pyIbex has been merged into Codac, please do not use it anymore.')
-  print('Conflicts may occur between the two libraries.\n')
-
 from codac.core import *
 from .version import __version__
 
+class AnalyticFunction:
 
-# Predefined contractor objects
-
-class ctc:
-
-  delay = CtcDelay()
-  deriv = CtcDeriv()
-  eval = CtcEval()
-  dist = CtcDist()
-  polar = CtcPolar()
-
-
-# Deprecated functions from the former pyIbex library:
-
-def pySIVIA(X0, ops, epsilon, figure_name='', draw_boxes=True, save_result=True, color_maybe='', color_out='', color_in=''):
-  print('\nWarning: pySIVIA(..) is deprecated and has been replaced by SIVIA(..).')
-  print('More information can be found with help(SIVIA).\n')
-  print('Example of use:\n')
-  print('  SIVIA(x0, sep, 0.05, regular_paving=False, display_result=True, fig_name="SIVIA", return_result=True, color_map={SetValue.IN:"k[r]", SetValue.OUT:"k[b]", SetValue.UNKNOWN:"k[y]"})\n')
-
-  cmap = {}
-  if color_in:
-    cmap[SetValue.IN] = color_in
-  if color_out:
-    cmap[SetValue.OUT] = color_out
-  if color_maybe:
-    cmap[SetValue.UNKNOWN] = color_maybe
-
-  return SIVIA(X0, ops, epsilon, regular_paving=False, display_result=draw_boxes, fig_name=figure_name, return_result=save_result, color_map=cmap)
+  def __init__(self, args, e):
+    if isinstance(e, (ScalarVar,ScalarExpr)):
+      self.f = AnalyticFunction_Scalar(args,e)
+    elif isinstance(e, (VectorVar,VectorExpr)):
+      self.f = AnalyticFunction_Vector(args,e)
+    else:
+      raise ValueError("Can only build functions from scalar or vector expressions")
+
+  def input_size(self):
+    return self.f.input_size()
+
+  def eval(self,*args):
+    return self.f.eval(*args)
+
+  def __call__(self,*args):
+    lst=[]
+    for arg in args:
+      if isinstance(arg, (ScalarVar,ScalarExpr,Interval)):
+        lst.append(ScalarExpr(arg).raw_copy())
+      elif isinstance(arg, (VectorVar,VectorExpr,IntervalVector)):
+        lst.append(VectorExpr(arg).raw_copy())
+      else:
+        raise ValueError("Invalid input argument: ", arg)
+    return self.f(lst)
+
+  def __repr__(self):
+    return str(self.f)
+
+class CtcInverse(CtcIntervalVector):
+
+  def __init__(self, f, y):
+    CtcIntervalVector.__init__(self, f.input_size())
+    if isinstance(f.f, AnalyticFunction_Scalar):
+      self.c = CtcInverse_Interval(f.f,Interval(y))
+    elif isinstance(f.f, AnalyticFunction_Vector):
+      self.c = CtcInverse_IntervalVector(f.f,IntervalVector(y))
+    else:
+      raise ValueError("Can only build CtcInverse from scalar or vector functions")
+
+  def contract(self,x):
+    self.c.contract(x)
+    return x
```

## codac/version.py

```diff
@@ -1 +1 @@
-__version__="1.5.6"
+__version__="2.0.0"
```

