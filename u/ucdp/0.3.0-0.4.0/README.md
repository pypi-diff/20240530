# Comparing `tmp/ucdp-0.3.0.tar.gz` & `tmp/ucdp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdp-0.3.0.tar", last modified: Mon May 20 21:52:05 2024, max compression
+gzip compressed data, was "ucdp-0.4.0.tar", last modified: Thu May 30 04:52:20 2024, max compression
```

## Comparing `ucdp-0.3.0.tar` & `ucdp-0.4.0.tar`

### file list

```diff
@@ -1,99 +1,145 @@
--rw-r--r--   0        0        0     1067 2024-05-20 21:51:52.867201 ucdp-0.3.0/LICENSE
--rw-r--r--   0        0        0      939 2024-05-20 21:51:52.867201 ucdp-0.3.0/README.md
--rw-r--r--   0        0        0     2635 2024-05-20 21:52:05.087167 ucdp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7153 2024-05-20 21:51:52.867201 ucdp-0.3.0/src/ucdp/__init__.py
--rw-r--r--   0        0        0     2977 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/_modbuilder.py
--rw-r--r--   0        0        0    12421 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/assigns.py
--rw-r--r--   0        0        0     2002 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/baseclassinfo.py
--rw-r--r--   0        0        0      360 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/buildproduct.py
--rw-r--r--   0        0        0     7337 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/cli.py
--rw-r--r--   0        0        0     6692 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/config.py
--rw-r--r--   0        0        0     3870 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/const.py
--rw-r--r--   0        0        0     1446 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/consts.py
--rw-r--r--   0        0        0     2942 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/dict.py
--rw-r--r--   0        0        0     3740 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/doc.py
--rw-r--r--   0        0        0     2531 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/docutil.py
--rw-r--r--   0        0        0     1144 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/regf.py
--rw-r--r--   0        0        0     1443 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/filelist/filelist_lib/filelist.py
--rw-r--r--   0        0        0       67 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/filelist/filelist_lib/mod.f
--rw-r--r--   0        0        0     1943 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/param/param_lib/param.py
--rw-r--r--   0        0        0     1810 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/fileliststandard.py
--rw-r--r--   0        0        0     1140 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/bus.py
--rw-r--r--   0        0        0     1565 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/clk_gate.py
--rw-r--r--   0        0        0     3405 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf.py
--rw-r--r--   0        0        0     1388 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf_tb.py
--rw-r--r--   0        0        0     1129 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/__init__.py
--rw-r--r--   0        0        0     2762 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/uart.py
--rw-r--r--   0        0        0     1587 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/exceptions.py
--rw-r--r--   0        0        0    20667 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/expr.py
--rw-r--r--   0        0        0    13228 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/exprparser.py
--rw-r--r--   0        0        0     8039 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/exprresolver.py
--rw-r--r--   0        0        0     4842 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/filelistparser.py
--rw-r--r--   0        0        0     3008 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/fileset.py
--rw-r--r--   0        0        0     1878 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/flipflop.py
--rw-r--r--   0        0        0     5047 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/generate.py
--rw-r--r--   0        0        0     1932 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/humannum.py
--rw-r--r--   0        0        0    12474 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/ident.py
--rw-r--r--   0        0        0     4036 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/iterutil.py
--rw-r--r--   0        0        0     3303 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/loader.py
--rw-r--r--   0        0        0     1179 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/logging.py
--rw-r--r--   0        0        0     2380 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/mod.py
--rw-r--r--   0        0        0    32835 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modbase.py
--rw-r--r--   0        0        0     2232 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modbasetop.py
--rw-r--r--   0        0        0     4113 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modconfigurable.py
--rw-r--r--   0        0        0     2928 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modcore.py
--rw-r--r--   0        0        0    10363 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modfilelist.py
--rw-r--r--   0        0        0    12681 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/moditer.py
--rw-r--r--   0        0        0     3521 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modref.py
--rw-r--r--   0        0        0     5938 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modtailored.py
--rw-r--r--   0        0        0     6332 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modtb.py
--rw-r--r--   0        0        0     3541 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modtopref.py
--rw-r--r--   0        0        0     1776 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modutil.py
--rw-r--r--   0        0        0     4072 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/mux.py
--rw-r--r--   0        0        0     6793 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/namespace.py
--rw-r--r--   0        0        0     6226 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/nameutil.py
--rw-r--r--   0        0        0      551 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/note.py
--rw-r--r--   0        0        0     4743 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/object.py
--rw-r--r--   0        0        0     5440 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/orientation.py
--rw-r--r--   0        0        0     4517 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/param.py
--rw-r--r--   0        0        0     3898 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/pathutil.py
--rw-r--r--   0        0        0     5735 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/routepath.py
--rw-r--r--   0        0        0     7224 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/signal.py
--rw-r--r--   0        0        0     8282 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/slices.py
--rw-r--r--   0        0        0       33 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/templates/main.mako
--rw-r--r--   0        0        0     1258 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/test.py
--rw-r--r--   0        0        0     3443 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/top.py
--rw-r--r--   0        0        0     3644 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typearray.py
--rw-r--r--   0        0        0     5078 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typebase.py
--rw-r--r--   0        0        0     5457 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typeclkrst.py
--rw-r--r--   0        0        0     7908 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typedescriptivestruct.py
--rw-r--r--   0        0        0    20080 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typeenum.py
--rw-r--r--   0        0        0    22840 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typescalar.py
--rw-r--r--   0        0        0     2043 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typestring.py
--rw-r--r--   0        0        0    11994 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typestruct.py
--rw-r--r--   0        0        0     1570 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/util.py
--rw-r--r--   0        0        0       13 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      936 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0    16882 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_assigns.py
--rw-r--r--   0        0        0     2892 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_baseclassinfo.py
--rw-r--r--   0        0        0     1611 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_buildproduct.py
--rw-r--r--   0        0        0     1914 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_config.py
--rw-r--r--   0        0        0     3962 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_examples.py
--rw-r--r--   0        0        0     3086 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_exprparser.py
--rw-r--r--   0        0        0     1856 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_exprresolver.py
--rw-r--r--   0        0        0     2022 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_fileset.py
--rw-r--r--   0        0        0     2077 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_flipflop.py
--rw-r--r--   0        0        0     4756 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_light_object.py
--rw-r--r--   0        0        0     6445 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_loader.py
--rw-r--r--   0        0        0     2947 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_modfilelist.py
--rw-r--r--   0        0        0     1587 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_mux.py
--rw-r--r--   0        0        0    13658 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_namespace.py
--rw-r--r--   0        0        0     4665 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_object.py
--rw-r--r--   0        0        0     8485 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_pathutil.py
--rw-r--r--   0        0        0     3362 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_routepath.py
--rw-r--r--   0        0        0     3489 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_typeenum.py
--rw-r--r--   0        0        0     5436 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_typescalar.py
--rw-r--r--   0        0        0     4047 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_typestruct.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 ucdp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-30 04:52:07.925562 ucdp-0.4.0/LICENSE
+-rw-r--r--   0        0        0      939 2024-05-30 04:52:07.925562 ucdp-0.4.0/README.md
+-rw-r--r--   0        0        0     2686 2024-05-30 04:52:20.985516 ucdp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7514 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/__init__.py
+-rw-r--r--   0        0        0     1748 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/_castingnamespace.py
+-rw-r--r--   0        0        0     2977 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/_modbuilder.py
+-rw-r--r--   0        0        0     3404 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/_sliceassign.py
+-rw-r--r--   0        0        0    17136 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/assigns.py
+-rw-r--r--   0        0        0     2002 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/baseclassinfo.py
+-rw-r--r--   0        0        0      360 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/buildproduct.py
+-rw-r--r--   0        0        0     1210 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/casting.py
+-rw-r--r--   0        0        0     7548 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/cli.py
+-rw-r--r--   0        0        0     6746 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/config.py
+-rw-r--r--   0        0        0     3870 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/const.py
+-rw-r--r--   0        0        0     1574 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/consts.py
+-rw-r--r--   0        0        0     2942 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/dict.py
+-rw-r--r--   0        0        0     3740 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/doc.py
+-rw-r--r--   0        0        0     2531 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/docutil.py
+-rw-r--r--   0        0        0     2905 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/drivers.py
+-rw-r--r--   0        0        0     1144 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/bad/glbl_bad_lib/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/bad/glbl_bad_lib/regf.py
+-rw-r--r--   0        0        0     1474 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/filelist/filelist_lib/filelist.py
+-rw-r--r--   0        0        0       67 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/filelist/filelist_lib/mod.f
+-rw-r--r--   0        0        0     1943 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/param/param_lib/param.py
+-rw-r--r--   0        0        0     1812 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/fileliststandard.py
+-rw-r--r--   0        0        0     1140 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/bus.py
+-rw-r--r--   0        0        0     1565 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/clk_gate.py
+-rw-r--r--   0        0        0     3405 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/regf.py
+-rw-r--r--   0        0        0     1388 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/regf_tb.py
+-rw-r--r--   0        0        0     1129 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/uart_lib/__init__.py
+-rw-r--r--   0        0        0     2762 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/examples/simple/uart_lib/uart.py
+-rw-r--r--   0        0        0     1509 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/exceptions.py
+-rw-r--r--   0        0        0    21287 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/expr.py
+-rw-r--r--   0        0        0    13305 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/exprparser.py
+-rw-r--r--   0        0        0    10599 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/exprresolver.py
+-rw-r--r--   0        0        0     4842 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/filelistparser.py
+-rw-r--r--   0        0        0     3008 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/fileset.py
+-rw-r--r--   0        0        0     1878 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/flipflop.py
+-rw-r--r--   0        0        0     5414 2024-05-30 04:52:07.929562 ucdp-0.4.0/src/ucdp/generate.py
+-rw-r--r--   0        0        0     1929 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/humannum.py
+-rw-r--r--   0        0        0    12796 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/ident.py
+-rw-r--r--   0        0        0     4036 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/iterutil.py
+-rw-r--r--   0        0        0     3303 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/loader.py
+-rw-r--r--   0        0        0     1179 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/logging.py
+-rw-r--r--   0        0        0     2383 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/mod.py
+-rw-r--r--   0        0        0    32707 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modbase.py
+-rw-r--r--   0        0        0     2180 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modbasetop.py
+-rw-r--r--   0        0        0     3546 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modconfigurable.py
+-rw-r--r--   0        0        0     2812 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modcore.py
+-rw-r--r--   0        0        0    10363 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modfilelist.py
+-rw-r--r--   0        0        0    12700 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/moditer.py
+-rw-r--r--   0        0        0     3674 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modref.py
+-rw-r--r--   0        0        0     5880 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modtailored.py
+-rw-r--r--   0        0        0     6910 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modtb.py
+-rw-r--r--   0        0        0     3667 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modtopref.py
+-rw-r--r--   0        0        0     2254 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/modutil.py
+-rw-r--r--   0        0        0     4110 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/mux.py
+-rw-r--r--   0        0        0     6990 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/namespace.py
+-rw-r--r--   0        0        0     6130 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/nameutil.py
+-rw-r--r--   0        0        0      549 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/note.py
+-rw-r--r--   0        0        0     4763 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/object.py
+-rw-r--r--   0        0        0     5598 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/orientation.py
+-rw-r--r--   0        0        0     4826 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/param.py
+-rw-r--r--   0        0        0     3898 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/pathutil.py
+-rw-r--r--   0        0        0     5735 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/routepath.py
+-rw-r--r--   0        0        0     7380 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/signal.py
+-rw-r--r--   0        0        0    10442 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/slices.py
+-rw-r--r--   0        0        0       33 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/templates/main.mako
+-rw-r--r--   0        0        0     1258 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/test.py
+-rw-r--r--   0        0        0     3691 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/top.py
+-rw-r--r--   0        0        0     3654 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typearray.py
+-rw-r--r--   0        0        0     4936 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typebase.py
+-rw-r--r--   0        0        0     7693 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typebaseenum.py
+-rw-r--r--   0        0        0     5457 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typeclkrst.py
+-rw-r--r--   0        0        0     7910 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typedescriptivestruct.py
+-rw-r--r--   0        0        0    14363 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typeenum.py
+-rw-r--r--   0        0        0     1247 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typehelper.py
+-rw-r--r--   0        0        0    23898 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typescalar.py
+-rw-r--r--   0        0        0     2207 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typestring.py
+-rw-r--r--   0        0        0    12013 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/typestruct.py
+-rw-r--r--   0        0        0     1570 2024-05-30 04:52:07.933562 ucdp-0.4.0/src/ucdp/util.py
+-rw-r--r--   0        0        0       13 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1126 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      451 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_assign/assigns.txt
+-rw-r--r--   0        0        0       36 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_assign_cast/assigns.txt
+-rw-r--r--   0        0        0        0 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_assign_empty/assigns.txt
+-rw-r--r--   0        0        0     2290 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_assign_empty_inst/assigns.txt
+-rw-r--r--   0        0        0      380 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_assign_slice/assigns.txt
+-rw-r--r--   0        0        0      380 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_assign_slice_inst/assigns.txt
+-rw-r--r--   0        0        0      122 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_concat/assigns.txt
+-rw-r--r--   0        0        0      205 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_const/assigns.txt
+-rw-r--r--   0        0        0      935 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_direction_error/assigns.txt
+-rw-r--r--   0        0        0      843 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_drivers/assign0.txt
+-rw-r--r--   0        0        0      391 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_drivers/assign1.txt
+-rw-r--r--   0        0        0      945 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_inst_direction_error/assigns.txt
+-rw-r--r--   0        0        0        9 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_lock/assigns.txt
+-rw-r--r--   0        0        0      461 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_reassign/assigns.txt
+-rw-r--r--   0        0        0      823 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_top_in/assigns.txt
+-rw-r--r--   0        0        0      803 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_top_inst_in/assigns.txt
+-rw-r--r--   0        0        0      116 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_top_inst_in_const/assigns.txt
+-rw-r--r--   0        0        0      150 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_top_inst_in_note/assigns.txt
+-rw-r--r--   0        0        0      803 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_top_inst_out/assigns.txt
+-rw-r--r--   0        0        0      823 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_assigns/test_top_out/assigns.txt
+-rw-r--r--   0        0        0       89 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_cli/test_gen/cleangen.txt
+-rw-r--r--   0        0        0       95 2024-05-30 04:52:07.933562 ucdp-0.4.0/tests/refdata/tests.test_cli/test_gen/gen.txt
+-rw-r--r--   0        0        0     2248 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_expr/test_const_const/result.txt
+-rw-r--r--   0        0        0     2248 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_expr/test_const_int/result.txt
+-rw-r--r--   0        0        0     1942 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_expr/test_int_const/result.txt
+-rw-r--r--   0        0        0        0 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_flipflops/test_flipflop/stderr.txt
+-rw-r--r--   0        0        0      160 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_flipflops/test_flipflop/stdout.txt
+-rw-r--r--   0        0        0        0 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_muxes/test_mux/stderr.txt
+-rw-r--r--   0        0        0      388 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/refdata/tests.test_muxes/test_mux/stdout.txt
+-rw-r--r--   0        0        0    12892 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_assigns.py
+-rw-r--r--   0        0        0     2892 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_baseclassinfo.py
+-rw-r--r--   0        0        0     1611 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_buildproduct.py
+-rw-r--r--   0        0        0     8939 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_cast.py
+-rw-r--r--   0        0        0     4271 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1914 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_config.py
+-rw-r--r--   0        0        0     3962 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_examples.py
+-rw-r--r--   0        0        0     5192 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_expr.py
+-rw-r--r--   0        0        0     8206 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_exprparser.py
+-rw-r--r--   0        0        0     8291 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_exprresolver.py
+-rw-r--r--   0        0        0     2019 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_fileset.py
+-rw-r--r--   0        0        0     2077 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_flipflop.py
+-rw-r--r--   0        0        0     2644 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_flipflops.py
+-rw-r--r--   0        0        0     1764 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_ident.py
+-rw-r--r--   0        0        0     5365 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_light_object.py
+-rw-r--r--   0        0        0     7854 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_loader.py
+-rw-r--r--   0        0        0     2501 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_modconfigurable.py
+-rw-r--r--   0        0        0     2988 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_modfilelist.py
+-rw-r--r--   0        0        0    11327 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_mods.py
+-rw-r--r--   0        0        0     2052 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_modtailored.py
+-rw-r--r--   0        0        0     4708 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_modtb.py
+-rw-r--r--   0        0        0     3483 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_muxes.py
+-rw-r--r--   0        0        0    14689 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_namespace.py
+-rw-r--r--   0        0        0     4665 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_object.py
+-rw-r--r--   0        0        0     1867 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_orientation.py
+-rw-r--r--   0        0        0     8485 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_pathutil.py
+-rw-r--r--   0        0        0     3920 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_routepath.py
+-rw-r--r--   0        0        0     3644 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_slices.py
+-rw-r--r--   0        0        0     3489 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_typeenum.py
+-rw-r--r--   0        0        0     5805 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_typescalar.py
+-rw-r--r--   0        0        0     4493 2024-05-30 04:52:07.937562 ucdp-0.4.0/tests/test_typestruct.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 ucdp-0.4.0/PKG-INFO
```

### Comparing `ucdp-0.3.0/LICENSE` & `ucdp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/README.md` & `ucdp-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/pyproject.toml` & `ucdp-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ucdp"
-version = "0.3.0"
+version = "0.4.0"
 description = "Unified Chip Design Platform"
 readme = "README.md"
 authors = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
@@ -44,14 +44,15 @@
 ]
 test = [
     "contextlib-chdir>=1.0.2",
     "coveralls>=3.3.1",
     "hypothesis>=6.100.1",
     "pytest-cov>=5.0.0",
     "tabulate>=0.9.0",
+    "test2ref>=0.4.2",
 ]
 checktypes = [
     "mypy>=1.9.0",
 ]
 doc = [
     "mkdocs-include-markdown-plugin>=6.0.5",
     "mkdocs-literate-nav>=0.6.1",
@@ -133,14 +134,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
     "return NotImplemented",
     "raise NotImplementedError()",
     "pragma: no cover",
     "assert False",
+    "raise AssertionError",
 ]
 
 [tool.mypy]
 disable_error_code = "misc"
 ignore_missing_imports = true
 plugins = "pydantic.mypy"
 overrides = [
```

### Comparing `ucdp-0.3.0/src/ucdp/__init__.py` & `ucdp-0.4.0/src/ucdp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,45 +22,48 @@
 # SOFTWARE.
 #
 
 """Unified Chip Design Platform."""
 
 from pydantic import ValidationError
 
-from .assigns import Assign, Assigns, Drivers
+from .assigns import Assign, Assigns
 from .baseclassinfo import BaseClassInfo, get_baseclassinfos
 from .buildproduct import ABuildProduct
+from .casting import Casting
 from .config import AConfig, AUniqueConfig, AVersionConfig, BaseConfig
 from .const import Const
 from .consts import AUTO, PAT_IDENTIFIER
 from .dict import Dict
 from .doc import Doc
 from .docutil import doc_from_type
-from .exceptions import BuildError, DirectionError, DuplicateError, LockError
+from .drivers import Drivers, Source, Target
+from .exceptions import BuildError, DirectionError, DuplicateError, InvalidExpr, LockError, MultipleDriverError
 from .expr import (
     BoolOp,
     ConcatExpr,
     ConstExpr,
     Expr,
     Log2Expr,
     MaximumExpr,
     MinimumExpr,
     Op,
     RangeExpr,
     SliceOp,
     SOp,
+    TernaryExpr,
 )
-from .exprparser import ExprParser, const
+from .exprparser import ExprParser, cast_booltype, const
 from .exprresolver import ExprResolver
 from .filelistparser import FileListParser
 from .fileset import FileSet, LibPath
 from .flipflop import FlipFlop
 from .generate import generate
 from .humannum import Bin, Bytes, Hex
-from .ident import Ident, IdentFilter, Idents, IdentStop, get_ident
+from .ident import Ident, IdentFilter, Idents, IdentStop, get_expridents, get_ident
 from .iterutil import Names, namefilter, split
 from .loader import load
 from .mod import AMod
 from .modbase import BaseMod
 from .modbasetop import BaseTopMod
 from .modconfigurable import AConfigurableMod
 from .modcore import ACoreMod
@@ -99,17 +102,18 @@
 from .pathutil import improved_glob, improved_resolve, startswith_envvar, use_envvars
 from .routepath import Routeable, Routeables, RoutePath, parse_routepath, parse_routepaths
 from .signal import BaseSignal, Port, Signal
 from .slices import DOWN, UP, Slice, SliceDirection
 from .test import Test
 from .typearray import ArrayType
 from .typebase import ACompositeType, AScalarType, AVecType, BaseScalarType, BaseType
+from .typebaseenum import BaseEnumType, EnumItem, EnumItemFilter
 from .typeclkrst import ClkRstAnType, ClkType, DiffClkRstAnType, DiffClkType, RstAnType, RstAType, RstType
 from .typedescriptivestruct import DescriptiveStructType
-from .typeenum import AEnumType, AGlobalEnumType, BaseEnumType, BusyType, DisType, DynamicEnumType, EnaType, EnumItem
+from .typeenum import AEnumType, AGlobalEnumType, BusyType, DisType, DynamicEnumType, EnaType
 from .typescalar import BitType, BoolType, IntegerType, RailType, SintType, UintType
 from .typestring import StringType
 from .typestruct import (
     AGlobalStructType,
     AStructType,
     BaseStructType,
     DynamicStructType,
@@ -119,21 +123,17 @@
     fwdfilter,
 )
 from .util import extend_sys_path
 
 __all__ = [
     "ABuildProduct",
     "ACompositeType",
-    "parse_routepath",
-    "parse_routepaths",
-    "Routeable",
-    "Routeables",
-    "RoutePath",
     "AConfig",
     "AConfigurableMod",
+    "ACoreMod",
     "AEnumType",
     "AGenericTbMod",
     "AGlobalEnumType",
     "AGlobalStructType",
     "AMod",
     "AOrientation",
     "ArrayType",
@@ -162,21 +162,22 @@
     "BoolType",
     "BuildError",
     "BusyType",
     "BWD",
     "bwdfilter",
     "BWDM",
     "Bytes",
+    "cast_booltype",
+    "Casting",
     "ClkRstAnType",
     "ClkType",
     "ConcatExpr",
     "const",
     "Const",
     "ConstExpr",
-    "ACoreMod",
     "DescriptiveStructType",
     "Dict",
     "didyoumean",
     "DiffClkRstAnType",
     "DiffClkType",
     "Direction",
     "DirectionError",
@@ -187,27 +188,29 @@
     "Drivers",
     "DriversDuplicateError",
     "DuplicateError",
     "DynamicEnumType",
     "DynamicStructType",
     "EnaType",
     "EnumItem",
+    "EnumItemFilter",
     "Expr",
     "ExprParser",
     "ExprResolver",
     "extend_sys_path",
     "Field",
     "FileListParser",
     "FileSet",
     "FlipFlop",
     "FWD",
     "fwdfilter",
     "FWDM",
     "generate",
     "get_baseclassinfos",
+    "get_expridents",
     "get_ident",
     "get_modbaseinfos",
     "get_repr",
     "get_snakecasename",
     "Hex",
     "Ident",
     "IdentFilter",
@@ -215,14 +218,15 @@
     "IdentStop",
     "improved_glob",
     "improved_resolve",
     "IN",
     "INM",
     "INOUT",
     "IntegerType",
+    "InvalidExpr",
     "is_tb_from_modname",
     "iter_modfilelists",
     "join_names",
     "LibPath",
     "Light",
     "LightObject",
     "load",
@@ -231,56 +235,65 @@
     "MaximumExpr",
     "MinimumExpr",
     "ModFileList",
     "ModFileLists",
     "ModPostIter",
     "ModPreIter",
     "ModRef",
+    "MultipleDriverError",
     "Mux",
     "NamedLightObject",
     "NamedObject",
     "namefilter",
     "Names",
     "Namespace",
     "Note",
     "Object",
     "Op",
     "OPEN",
     "Orientation",
     "OUT",
     "OUTM",
     "Param",
+    "parse_routepath",
+    "parse_routepaths",
     "parse",
     "PAT_IDENTIFIER",
     "Paths",
     "Placeholder",
     "Port",
     "PrivateField",
     "RailType",
     "RangeExpr",
     "resolve_modfilelist",
+    "Routeable",
+    "Routeables",
+    "RoutePath",
     "RstAnType",
     "RstAType",
     "RstType",
     "search_modfilelists",
     "Signal",
     "SintType",
     "Slice",
     "SliceDirection",
     "SliceOp",
     "SOp",
+    "Source",
     "split_prefix",
     "split_suffix",
     "split",
     "startswith_envvar",
     "str2identifier",
     "StringType",
     "StructFilter",
     "StructItem",
+    "Target",
     "ternary",
+    "TernaryExpr",
     "Test",
     "TODO",
     "ToPaths",
     "TopModRef",
     "UintType",
     "uniquemods",
     "UP",
```

### Comparing `ucdp-0.3.0/src/ucdp/_modbuilder.py` & `ucdp-0.4.0/src/ucdp/_modbuilder.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/assigns.py` & `ucdp-0.4.0/tests/test_assigns.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,349 +17,397 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
+"""Test Assigns."""
 
+import re
+from pathlib import Path
 
-"""
-Assignment Handling.
+import ucdp as u
+from pytest import fixture, raises
+from test2ref import assert_refdata
 
-The class [Assigns][ucdp.assigns.Assigns] manages sets of signal assignments.
-Either statically in modules but also within flip-flop and multiplexer definitions.
 
-??? Example "Basic Examples"
-    All of the following is happening within any hardware module, flip-flop or multiplexer,
-    but can also be used within own code.
-
-        >>> import ucdp as u
-        >>> signals = u.Idents([
-        ...     u.Port(u.ClkRstAnType(), "main_i"),
-        ...     u.Port(u.UintType(8), "vec_a_i"),
-        ...     u.Port(u.UintType(8), "vec_a_o"),
-        ...     u.Port(u.UintType(14), "vec_b_i"),
-        ...     u.Port(u.UintType(14), "vec_b_o"),
-        ...     u.Port(u.UintType(14), "vec_c_o"),
-        ...     u.Signal(u.ClkRstAnType(), "main_s"),
-        ...     u.Signal(u.UintType(8), "vec_a_s"),
-        ...     u.Signal(u.UintType(4), "vec_b_s"),
-        ...     u.Signal(u.UintType(4), "vec_c_s"),
-        ... ])
-        >>> assigns = u.Assigns(targets=signals, sources=signals)
-        >>> assigns.set_default(signals['vec_a_o'], signals['vec_a_i'])
-        >>> assigns.set_default(signals['vec_b_o'], signals['vec_b_i'])
-        >>> assigns.set(signals['vec_a_o'], signals['vec_a_s'])
-        >>> for assign in assigns:
-        ...     str(assign)
-        'vec_a_o  <----  vec_a_s'
-        'vec_b_o  <----  vec_b_i'
-
-??? failure "Multiple Assignments"
-    Multiple assignments are forbidden:
-
-        >>> assigns.set(signals['vec_a_o'], signals['vec_a_s'])
-        Traceback (most recent call last):
-        ...
-        ValueError: 'vec_a_o' already assigned to 'vec_a_s'
-
-??? Example "Default Examples"
-    Defaults are managed separately:
-
-        >>> for assign in assigns.defaults():
-        ...     str(assign)
-        'vec_a_o  <----  vec_a_i'
-        'vec_b_o  <----  vec_b_i'
-
-??? Example "Mapping"
-    With `all=True` the all target signals are mapped:
-
-        >>> assigns = u.Assigns(targets=signals, sources=signals, all=True, sub=True)
-        >>> assigns.set_default(signals['vec_a_i'], signals['vec_a_i'])
-        >>> assigns.set_default(signals['vec_b_i'], signals['vec_b_i'])
-        >>> assigns.set(signals['vec_a_i'], signals['vec_a_s'])
-        >>> for assign in assigns:
-        ...     str(assign)
-        'main_i  ---->  None'
-        'main_clk_i  ---->  None'
-        'main_rst_an_i  ---->  None'
-        'vec_a_i  ---->  vec_a_s'
-        'vec_a_o  <----  None'
-        'vec_b_i  ---->  vec_b_i'
-        'vec_b_o  <----  None'
-        'vec_c_o  <----  None'
-        'main_s  ---->  None'
-        'main_clk_s  ---->  None'
-        'main_rst_an_s  ---->  None'
-        'vec_a_s  ---->  None'
-        'vec_b_s  ---->  None'
-        'vec_c_s  ---->  None'
-
-"""
-
-from collections.abc import Iterable, Iterator
-from typing import Any
-
-from .exceptions import LockError
-from .expr import Expr
-from .ident import Ident, Idents
-from .note import Note
-from .object import Field, Object, PrivateField, model_validator
-from .orientation import BWD, FWD, IN, INOUT, OUT, Direction
-from .signal import BaseSignal, Port
-from .typebase import BaseScalarType
-
-_DIRECTION_MAP = {
-    IN: "---->",
-    OUT: "<----",
-    INOUT: "<--->",
-    None: None,
-}
-
-
-AssignSource = Expr | Note
-""" AssignSource."""
-
-# TODO: signal assignment
-
-
-class Drivers(Object):
-    """
-    Drivers.
-
-    This container tracks multiple drivers as every added signal is only allowed to be driven once.
-
-    Attributes:
-        drivers: Dictionary with drivers.
-    """
-
-    drivers: dict[str, AssignSource] = Field(default_factory=dict)
-
-    def __setitem__(self, name, item):
-        drivers = self.drivers
-        # if name in drivers:
-        #     raise ValueError(f"'{item}' already driven by '{drivers[name]}'")
-        drivers[name] = item
-
-    def __iter__(self) -> Iterator[tuple[str, AssignSource]]:  # type: ignore[override]
-        yield from self.drivers.items()
-
-
-# class Assign(LightObject):
-class Assign(Object):
-    """
-    A Single Assignment of `expr` to `target`.
-
-    Attributes:
-        target: Assigned identifier.
-        source: Assigned expression.
-    """
-
-    target: BaseSignal
-    source: AssignSource | None = None
-
-    @property
-    def name(self) -> str | None:
-        """Name."""
-        return self.target.name
-
-    @property
-    def type_(self):
-        """Type."""
-        return self.target.type_
-
-    @property
-    def doc(self):
-        """Doc."""
-        return self.target.doc
-
-    @property
-    def direction(self) -> Direction:
-        """Direction."""
-        return Direction.cast(self.target.direction)  # type: ignore[return-value]
-
-    @property
-    def ifdef(self) -> str | None:
-        """IFDEF."""
-        return self.target.ifdef
-
-    def __str__(self):
-        return f"{self.target}  {_DIRECTION_MAP[self.direction]}  {self.source}"
-
-
-_TargetAssigns = dict[str, AssignSource | None]
-
-
-class Assigns(Object):
-    """
-    Assignments.
-
-    An instance of [Assigns][ucdp.assigns.Assigns] manages a set of signal assignments.
-
-    Attributes:
-        targets: Identifiers allowed to be assigned.
-        source: Identifiers allowed to be used in assignment. `targets` by default.
-        drivers: Driver tracking, to avoid multiple drivers. To be shared between multiple assignments,
-                        where only one driver is allowed.
-        all: All Instances Assignment Mode.
-        sub: Sublevel Instance Assignment Mode.
-
-    """
-
-    targets: Idents
-    sources: Idents
-    drivers: Drivers | None = None
-    all: bool = False
-    sub: bool = False
-    _defaults: _TargetAssigns = PrivateField(default_factory=dict)
-    _assigns: _TargetAssigns = PrivateField(default_factory=dict)
-    __is_locked: bool = PrivateField(default=False)
-
-    @property
-    def is_locked(self) -> bool:
-        """Locked."""
-        return self.__is_locked
-
-    def lock(self) -> None:
-        """Lock."""
-        assert not self.__is_locked, f"{self} is already locked"
-        self.__is_locked = True
-
-    @model_validator(mode="before")
-    @classmethod
-    def __pre_init(cls, data: Any) -> Any:
-        if isinstance(data, dict):
-            data["sources"] = data.get("sources") or data.get("targets")
-        return data
-
-    def set_default(self, target: BaseSignal, source: AssignSource, cast: bool = False, overwrite: bool = False):
-        """Set Default of `target` to `source`.
-
-        Params:
-            target: Target.
-            source: Source.
-            cast: cast to target.
-            overwrite: overwrite target.
-        """
-        if self.__is_locked:
-            raise LockError(f"Cannot set default {source} to {target}")
-        assert not cast, "TODO"
-        self._check(target, source)
-        self._set(self._defaults, target, source, overwrite)
-
-    def set(self, target: BaseSignal, source: AssignSource, cast: bool = False, overwrite: bool = False):
-        """Set Assignment of `target` to `source`.
-
-        Params:
-            target: Target.
-            source: Source.
-            cast: cast to target.
-            overwrite: overwrite target.
-        """
-        if self.__is_locked:
-            raise LockError(f"Cannot set {source} to {target}")
-        assert not cast, "TODO"
-        self._check(target, source)
-        self._set(self._assigns, target, source, overwrite, drivers=self.drivers)
-
-    def get(self, target: BaseSignal) -> AssignSource | None:
-        """Get Assignment of `target`."""
-        return self._assigns.get(target.name, None)
-
-    def _check(self, target: BaseSignal, source: AssignSource):
-        if isinstance(source, Note):
-            return
-
-        # Normalize Directions
-        # IN/FWD: driver
-        # OUT/BWD: sink
-        orient = BWD if self.sub else FWD
-        sub = "sub-level " if self.sub else ""
-        targetdir = isinstance(target, Port) and (target.direction * orient)
-
-        # do not check INOUT
-        if not targetdir or not targetdir.mode:
-            return
-
-        # # Check Expression Source Direction
-        # for sourceident in get_expridents(source):
-        #     sourcedir = sourceident.direction
-        #     if sourcedir is None:
-        #         sourcedir = IN
-        #     if targetdir == sourcedir:
-        #         raise DirectionError(f"Cannot connect {sub}{target.direction} '{target}' and {sourcedir} '{source}'")
-
-        # Check Types
-        connectable = target.type_.is_connectable(source.type_)
-        if not connectable:
-            msg = f"Cannot assign '{source}' of {source.type_} to {sub}'{target}' of {target.type_}"
-            raise TypeError(msg)
-
-    def _set(
-        self,
-        assigns: _TargetAssigns,
-        target: BaseSignal,
-        source: AssignSource,
-        overwrite: bool,
-        drivers: Drivers | None = None,
-    ):
-        type_ = target.type_
-        is_target_scalar = isinstance(type_, BaseScalarType)
-        is_source_note = isinstance(source, Note)
-        targetdrvdir = IN if self.sub else OUT
-
-        # Expressions are only allowed on BaseScalarType
-        if not is_target_scalar and not (isinstance(source, Ident) | is_source_note):
-            raise ValueError(f"Cannot assign expression {source} to {target}")
-
-        subtargets: Iterable[BaseSignal]
-        subsources: Iterable[AssignSource]
-
-        if is_source_note:
-            # Note Assignments
-            subtargets = tuple(target.iter())
-            subsources = (source,) * len(subtargets)
-        elif isinstance(source, Ident):
-            # Identifier assignment
-            subtargets = target.iter()
-            subsources = source.iter()
-        else:
-            assert is_target_scalar
-            # Expression Assignment
-            subtargets = (target,)
-            subsources = (source,)
-
-        for subtarget, subsource in zip(subtargets, subsources, strict=True):
-            if not overwrite and subtarget.name in assigns:
-                raise ValueError(f"'{subtarget}' already assigned to '{assigns[subtarget.name]}'")
-            if drivers is not None and not is_source_note:
-                if subtarget.direction == targetdrvdir:
-                    drivers[subtarget.name] = subsource
-            assigns[subtarget.name] = subsource
-
-    def __iter__(self):
-        return self.iter()
-
-    def iter(self, filter_=None) -> Iterator[Assign]:
-        """Iterate over assignments."""
-        defaults = self._defaults
-        assigns = self._assigns
-        for target in self.targets.iter():
-            if filter_ and not filter_(target):
-                continue
-            expr = self._get(assigns, target, default=defaults.get(target.name, None))  # type: ignore[arg-type]
-            if expr is not None or self.all:
-                yield Assign(target=target, source=expr)
-
-    def defaults(self) -> Iterator[Assign]:
-        """Iterate Over Defaults."""
-        defaults = self._defaults
-        assigns = self._assigns
-        for target in self.targets.iter():
-            default = self._get(defaults, target)  # type: ignore[arg-type]
-            if self.all or default is not None or bool(assigns.get(target.name, None)):
-                yield Assign(target=target, source=default)
-
-    @staticmethod
-    def _get(assigns: _TargetAssigns, target: BaseSignal, default: AssignSource | None = None) -> AssignSource | None:
-        return assigns.get(target.name, default)
+class ModeType(u.AEnumType):
+    """Mode."""
+
+    keytype: u.UintType = u.UintType(2)
+
+    def _build(self):
+        self._add(0, "add")
+        self._add(1, "sub")
+        self._add(2, "max")
+
+
+class StructType(u.AStructType):
+    """My."""
+
+    comment: str = "Mode"
+
+    def _build(self):
+        self._add("mode", ModeType())
+        self._add("send", u.ArrayType(u.UintType(8), 3))
+        self._add("return", u.UintType(4), u.BWD)
+
+
+class MyType(u.AStructType):
+    """A Complex Type."""
+
+    def _build(self):
+        self._add("my0", StructType())
+        self._add("my1", StructType(), u.BWD)
+        self._add("uint", u.UintType(3))
+
+
+@fixture
+def top() -> u.Idents:
+    """Top-Identifier."""
+    return u.Idents(
+        [
+            u.Port(MyType(), "port_i"),
+            u.Port(MyType(), "port_o"),
+            u.Port(MyType(), "other_i"),
+            u.Port(MyType(), "other_o"),
+            u.Port(StructType(), "struct_i"),
+            u.Port(StructType(), "struct_o"),
+            u.Signal(StructType(), "struct_s"),
+            u.Signal(MyType(), "sig_s"),
+            u.Port(u.UintType(8), "data_i"),
+            u.Port(u.UintType(8), "data_o"),
+            u.Signal(u.UintType(8), "data0_s"),
+            u.Signal(u.UintType(8), "data1_s"),
+        ]
+    )
+
+
+@fixture
+def sub() -> u.Idents:
+    """Sub-Identifier."""
+    return u.Idents(
+        [
+            u.Port(MyType(), "sub_i"),
+            u.Port(MyType(), "sub_o"),
+            u.Port(u.UintType(8), "data_i"),
+            u.Port(u.UintType(8), "data_o"),
+        ]
+    )
+
+
+def _dump_assigns(assigns: u.Assigns, path: Path, name: str = "assigns", full: bool = False):
+    filepath = path / f"{name}.txt"
+    with filepath.open("w") as file:
+        if not full:
+            file.write("SET-ONLY\n")
+        for assign in assigns:
+            if full or assign.source is not None:
+                file.write(f"ASSIGN: {assign}\n")
+        if assigns.drivers:
+            for name, value in assigns.drivers:
+                file.write(f"DRIVER: {name}: {value}\n")
+
+
+def test_basic(top):
+    """Assign Basics."""
+    doc = u.Doc(title="title", descr="descr", comment="comment")
+    target = u.Port(u.UintType(8), "a_i", doc=doc, ifdef="IFDEF")
+    source = u.Signal(u.UintType(8), "b_s")
+    assign = u.Assign(target=target, source=source)
+
+    assert assign.name == "a_i"
+    assert assign.type_ == u.UintType(8)
+    assert assign.doc is doc
+    assert assign.direction == u.IN
+    assert assign.ifdef == "IFDEF"
+
+
+def test_assign_empty(top, tmp_path):
+    """Empty Assigns."""
+    assigns = u.Assigns(targets=top, sources=top)
+    _dump_assigns(assigns, tmp_path, full=True)
+    assert_refdata(test_assign_empty, tmp_path)
+
+
+def test_assign_empty_inst(top, tmp_path):
+    """Empty Assigns for inst."""
+    assigns = u.Assigns(targets=top, sources=top, inst=True)
+    _dump_assigns(assigns, tmp_path, full=True)
+    assert_refdata(test_assign_empty_inst, tmp_path)
+
+
+def test_reassign(top, tmp_path):
+    """Assigns."""
+    assigns = u.Assigns(targets=top, sources=top)
+    assigns.set(top["port_o"], top["other_i"])
+
+    msg = "'port_o' already assigned to 'other_i'"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(top["port_o"], top["port_i"])
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_reassign, tmp_path)
+
+
+def test_direction_error(top, tmp_path):
+    """Assigns."""
+    assigns = u.Assigns(targets=top, sources=top)
+
+    msg = "Cannot drive 'other_i' by 'port_i'"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(top["other_i"], top["port_i"])
+
+    assigns.set(top["other_o"], top["port_o"])
+    assigns.set(top["port_i"], top["port_o"])
+    assigns.set(top["data0_s"], top["data1_s"])
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_direction_error, tmp_path)
+
+
+def test_inst_direction_error(top, tmp_path):
+    """Assigns."""
+    assigns = u.Assigns(targets=top, inst=True)
+
+    msg = "Cannot drive 'other_o' by 'port_i'"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(top["other_o"], top["port_i"])
+
+    assigns.set(top["other_o"], top["port_o"])
+    assigns.set(top["other_i"], top["port_o"])
+    assigns.set(top["data0_s"], top["data1_s"])
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_inst_direction_error, tmp_path)
+
+
+def test_drivers(top, tmp_path):
+    """Multiple Drivers."""
+    drivers = u.Drivers()
+    assigns0 = u.Assigns(targets=top, sources=top, drivers=drivers)
+    assigns0.set(top["port_o"], top["other_i"])
+    assigns1 = u.Assigns(targets=top, sources=top, drivers=drivers)
+
+    msg = "'other_i' already driven by 'other_i'"
+    with raises(u.MultipleDriverError, match=re.escape(msg)):
+        assigns1.set(top["port_o"], top["other_i"])
+
+    _dump_assigns(assigns0, tmp_path, name="assign0")
+    _dump_assigns(assigns1, tmp_path, name="assign1")
+    assert_refdata(test_drivers, tmp_path)
+
+
+def test_lock(top, tmp_path):
+    """Lock."""
+    assigns = u.Assigns(targets=top, sources=top)
+    assert assigns.is_locked is False
+
+    assigns.lock()
+
+    assert assigns.is_locked is True
+
+    msg = "Cannot set 'other_i' to 'port_o'"
+    with raises(u.LockError, match=re.escape(msg)):
+        assigns.set(top["port_o"], top["other_i"])
+
+    msg = "Cannot set default 'other_i' to 'port_o'"
+    with raises(u.LockError, match=re.escape(msg)):
+        assigns.set_default(top["port_o"], top["other_i"])
+
+    msg = "Assigns are already locked. Cannot lock again."
+    with raises(u.LockError, match=re.escape(msg)):
+        assigns.lock()
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_lock, tmp_path)
+
+
+def test_assign(top, tmp_path):
+    """Test Assigns."""
+    assigns = u.Assigns(targets=top)
+
+    # valid assignment
+    assigns.set(top["port_o"], top["port_i"])
+
+    # re-assignement
+    msg = "'port_o' already assigned to 'port_i'"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(top["port_o"], top["other_i"])
+
+    # assign
+    msg = "Cannot assign 'data_o' of type UintType(8) to 'port_i' of type MyType()."
+    with raises(TypeError, match=re.escape(msg)):
+        assigns.set(top["port_i"], top["data_o"])
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_assign, tmp_path)
+
+
+def test_concat(tmp_path):
+    """Test Concatenation."""
+    a_i = u.Port(u.UintType(4), "a_i")
+    b_i = u.Port(u.UintType(4), "b_i")
+    c_o = u.Port(u.UintType(8), "c_o")
+    idents = u.Idents([a_i, b_i, c_o])
+    assigns = u.Assigns(targets=idents)
+
+    assigns.set(c_o, u.ConcatExpr((a_i, b_i)))
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_concat, tmp_path)
+
+
+def test_const(top, tmp_path):
+    """Type Error."""
+    assigns = u.Assigns(targets=top)
+    constscal = u.Const(u.UintType(8), "scal")
+    myconst = u.Const(MyType(), "const_c")
+
+    msg = "Target const_c is not a Signal, Port or Slice of them"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(myconst, top["port_i"])
+
+    assigns.set(top["data_o"], constscal)
+
+    msg = "Target const_my0_return_c is not a Signal or Port"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(top["port_o"], myconst)
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_const, tmp_path)
+
+
+def test_assign_slice(tmp_path):
+    """Test Assign slice."""
+    a_i = u.Port(u.UintType(4), "a_i")
+    b_i = u.Port(u.UintType(4), "b_i")
+    c_i = u.Port(u.UintType(4), "c_i")
+    c_o = u.Port(u.UintType(10, default=0x1A1), "c_o")
+    idents = u.Idents([a_i, b_i, c_o])
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=idents, drivers=drivers)
+
+    assigns.set(c_o[3:1], a_i[2:0])
+    assigns.set(c_o[6:5], b_i[2:1])
+
+    msg = "Slice 6:5 is already taken by SliceOp(Port(UintType(4), 'b_i', direction=IN), Slice('2:1'))"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(c_o[6:5], c_i[2:1])
+
+    msg = "Cannot slice bit(s) 11 from UintType(10, default=417)"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(c_o[11], b_i[3])
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_assign_slice, tmp_path)
+
+
+def test_assign_slice_inst(tmp_path):
+    """Test Assign slice."""
+    a_i = u.Port(u.UintType(4), "a_i")
+    b_i = u.Port(u.UintType(4), "b_i")
+    c_i = u.Port(u.UintType(4), "c_i")
+    c_o = u.Port(u.UintType(10, default=0x1A1), "c_o")
+    idents = u.Idents([a_i, b_i, c_i, c_o])
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=idents, drivers=drivers, inst=True)
+
+    assigns.set(c_o[3:1], a_i[2:0])
+    assigns.set(c_o[6:5], b_i[2:1])
+
+    msg = "Slice 6:5 is already taken by SliceOp(Port(UintType(4), 'b_i', direction=IN), Slice('2:1'))"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(c_o[6:5], c_i[2:1])
+
+    msg = "Cannot slice bit(s) 11 from UintType(10, default=417)"
+    with raises(ValueError, match=re.escape(msg)):
+        assigns.set(c_o[11], b_i[3])
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_assign_slice_inst, tmp_path)
+
+
+def test_top_in(top, tmp_path):
+    """Top - Input."""
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=top, drivers=drivers)
+    assigns.set(top["port_i"], top["port_o"])
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_top_in, tmp_path)
+
+
+def test_top_out(top, tmp_path):
+    """Top - Output."""
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=top, drivers=drivers)
+    assigns.set(top["port_o"], top["port_i"])
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_top_out, tmp_path)
+
+
+def test_top_inst_in(top, sub, tmp_path):
+    """Top with Sub - Input."""
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=sub, sources=top, inst=True, drivers=drivers)
+    assigns.set(sub["sub_i"], top["port_i"])
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_top_inst_in, tmp_path)
+
+
+def test_top_inst_out(top, sub, tmp_path):
+    """Top with Sub - Output."""
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=sub, sources=top, inst=True, drivers=drivers)
+    assigns.set(sub["sub_o"], top["port_o"])
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_top_inst_out, tmp_path)
+
+
+def test_top_inst_in_note(top, sub, tmp_path):
+    """Top with Sub - Input."""
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=sub, sources=top, inst=True, drivers=drivers)
+    assigns.set(sub["sub_my1_i"], u.TODO)
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_top_inst_in_note, tmp_path)
+
+
+def test_top_inst_in_const(top, sub, tmp_path):
+    """Top with Sub - Input."""
+    drivers = u.Drivers()
+    assigns = u.Assigns(targets=sub, sources=top, inst=True, drivers=drivers)
+    assigns.set(sub["data_i"], u.const("8h2"))
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_top_inst_in_const, tmp_path)
+
+
+def test_assign_cast(tmp_path):
+    """Test Casting."""
+
+    class MyEnumType(u.AEnumType):
+        keytype: u.UintType = u.UintType(4)
+
+        def _build(self):
+            self._add(u.AUTO, "a")
+            self._add(u.AUTO, "b")
+            self._add(u.AUTO, "c")
+
+    targets = u.Idents(
+        [
+            u.Port(u.UintType(4), "data_i"),
+            u.Port(MyEnumType(), "a_o"),
+            u.Port(MyEnumType(), "b_o"),
+            u.Port(MyEnumType(), "c_o"),
+        ]
+    )
+    assigns = u.Assigns(targets=targets)
+
+    msg = "MyEnumType(). Try to cast."
+    with raises(TypeError, match=re.escape(msg)):
+        assigns.set(targets["a_o"], targets["data_i"])
+
+    assigns.set(targets["b_o"], targets["data_i"], cast=None)
+
+    _dump_assigns(assigns, tmp_path)
+    assert_refdata(test_assign_cast, tmp_path)
```

### Comparing `ucdp-0.3.0/src/ucdp/baseclassinfo.py` & `ucdp-0.4.0/src/ucdp/baseclassinfo.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/cli.py` & `ucdp-0.4.0/src/ucdp/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 arg_filelist = click.argument("filelist", envvar="UCDP_FILELIST")
 opt_target = click.option("--target", "-t", help="Filter File List for Target", envvar="UCDP_TARGET")
 opt_show_diff = click.option(
     "--show-diff", "-s", default=False, is_flag=True, help="Show What Changed", envvar="UCDP_SHOW_DIFF"
 )
 opt_maxlevel = click.option("--maxlevel", "-L", type=int, help="Limit to maximum number of hierarchy levels.")
 opt_dry_run = click.option("--dry-run", default=False, is_flag=True, help="Do nothing.")
+opt_maxworkers = click.option("--maxworkers", "-J", type=int, help="Maximum Number of Processes.")
 
 
 def _load_top(ctx, top, paths) -> Top:
     with ctx.console.status(f"Loading {top!r}"):
         return load(top, paths=paths)
 
 
@@ -132,20 +133,21 @@
 """
 )
 @arg_top
 @opt_path
 @arg_filelist
 @opt_target
 @opt_show_diff
+@opt_maxworkers
 @pass_ctx
-def gen(ctx, top, path, filelist, target=None, show_diff=False):
+def gen(ctx, top, path, filelist, target=None, show_diff=False, maxworkers=None):
     """Generate."""
     top = _load_top(ctx, top, path)
     makolator = get_makolator(show_diff=show_diff)
-    generate(top.mod, filelist, target=target, makolator=makolator)
+    generate(top.mod, filelist, target=target, makolator=makolator, maxworkers=maxworkers)
 
 
 @ucdp.command(
     help=f"""
 Load Data Model and REMOVE Generated Files.
 
 TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
@@ -155,20 +157,21 @@
 )
 @arg_top
 @opt_path
 @arg_filelist
 @opt_target
 @opt_show_diff
 @opt_dry_run
+@opt_maxworkers
 @pass_ctx
-def cleangen(ctx, top, path, filelist, target=None, show_diff=False, dry_run=False):
+def cleangen(ctx, top, path, filelist, target=None, show_diff=False, maxworkers=None, dry_run=False):
     """Clean Generated Files."""
     top = _load_top(ctx, top, path)
     makolator = get_makolator(show_diff=show_diff)
-    clean(top.mod, filelist, target=target, makolator=makolator, dry_run=dry_run)
+    clean(top.mod, filelist, target=target, makolator=makolator, maxworkers=maxworkers, dry_run=dry_run)
 
 
 @ucdp.command(
     help=f"""
 Load Data Model and Generate File List.
 
 TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
```

### Comparing `ucdp-0.3.0/src/ucdp/config.py` & `ucdp-0.4.0/src/ucdp/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # SOFTWARE.
 #
 """Configuration."""
 
 import datetime
 import hashlib
 
-from .consts import PAT_IDENTIFIER
+from .consts import PAT_OPT_IDENTIFIER
 from .object import Field, LightObject
 
 
 class AConfig(LightObject):
     """
     Configuration Container.
 
@@ -107,20 +107,20 @@
             >>> variant2.feature
             True
 
     ???+ bug "Todo"
         * fix name type
     """
 
-    name: str = Field(pattern=PAT_IDENTIFIER)
+    name: str = Field(pattern=PAT_OPT_IDENTIFIER, default="")
 
     _posargs: tuple[str, ...] = ("name",)
 
-    def __init__(self, name, **kwargs):
-        super().__init__(name=name, **kwargs)
+    def __init__(self, name: str = "", **kwargs):
+        super().__init__(name=name, **kwargs)  # type: ignore[call-arg]
 
 
 class AUniqueConfig(LightObject):
     """
     A Unique Configuration.
 
     The configuration name is automatically derived from the attribute values.
@@ -161,15 +161,15 @@
     @property
     def name(self) -> str:
         """Assembled name from configuration values."""
         return hashlib.sha256(str(self.model_dump()).encode("utf-8")).hexdigest()[:16]
 
 
 BaseConfig = AConfig | AUniqueConfig
-""" BaseConfig """
+"""BaseConfig"""
 
 
 class AVersionConfig(AConfig):
     """
     Version Configuration Container.
 
     Attributes:
```

### Comparing `ucdp-0.3.0/src/ucdp/const.py` & `ucdp-0.4.0/src/ucdp/const.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/consts.py` & `ucdp-0.4.0/src/ucdp/examples/simple/uart_lib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,27 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-
-"""Constants."""
-
-import re
-from typing import Literal
-
-AUTO: str = "auto"
-""" AUTO. """
-
-PAT_IDENTIFIER: str = r"^[a-zA-Z]([a-zA-Z_0-9]*[a-zA-Z0-9])?$"
-""" PAT_IDENTIFIER. """
-
-RE_IDENTIFIER = re.compile(PAT_IDENTIFIER)
-""" PAT_IDENTIFIER. """
-
-UPWARDS: str = ".."
-""" UPWARDS. """
-
-Gen = Literal["no", "inplace", "full"]
-""" Gen. """
+"""UART Example."""
```

### Comparing `ucdp-0.3.0/src/ucdp/dict.py` & `ucdp-0.4.0/src/ucdp/dict.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/doc.py` & `ucdp-0.4.0/src/ucdp/doc.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/docutil.py` & `ucdp-0.4.0/src/ucdp/docutil.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/__init__.py` & `ucdp-0.4.0/src/ucdp/examples/bad/glbl_bad_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/regf.py` & `ucdp-0.4.0/src/ucdp/examples/bad/glbl_bad_lib/regf.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/filelist/filelist_lib/filelist.py` & `ucdp-0.4.0/src/ucdp/examples/filelist/filelist_lib/filelist.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,12 +31,13 @@
 class FilelistMod(u.AMod):
     """Module With Filelist."""
 
     filelists: ClassVar[u.ModFileLists] = (
         u.ModFileList(
             name="hdl",
             filepaths=("-f mod.f",),
+            inc_dirs=("inc",),
         ),
     )
 
     def _build(self) -> None:
         pass
```

### Comparing `ucdp-0.3.0/src/ucdp/examples/param/param_lib/param.py` & `ucdp-0.4.0/src/ucdp/examples/param/param_lib/param.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/fileliststandard.py` & `ucdp-0.4.0/src/ucdp/examples/simple/fileliststandard.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """HDL File Lists."""
 
     name: str = "hdl"
     filepaths: u.ToPaths = (
         # Path is relative to Module Python File
         # Environment variables are supported too
         # Wildcards are supported. Also in combination with environment variables!
-        "../src/{mod.libname}/{mod.topmodname}/{view}/{mod.modname}.sv",
+        "$PRJROOT/{mod.libname}/{mod.topmodname}/{view}/{mod.modname}.sv",
     )
 
     template_filepaths: u.ToPaths = ("main.mako",)
 
     @staticmethod
     def get_mod_placeholder(mod) -> u.Placeholder:
         """Get Module Placeholder."""
```

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/__init__.py` & `ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/bus.py` & `ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/bus.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/clk_gate.py` & `ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/clk_gate.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf.py` & `ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/regf.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf_tb.py` & `ucdp-0.4.0/src/ucdp/examples/simple/glbl_lib/regf_tb.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/__init__.py` & `ucdp-0.4.0/src/ucdp/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""UART Example."""
+
+"""
+Logging.
+"""
+
+import logging
+
+LOGGER = logging.getLogger("ucdp")
```

### Comparing `ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/uart.py` & `ucdp-0.4.0/src/ucdp/examples/simple/uart_lib/uart.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/exceptions.py` & `ucdp-0.4.0/src/ucdp/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,18 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """Exceptions."""
 
-from typing import Any
-
 
 class LockError(ValueError):
     """Lock."""
 
-    def __init__(self, inst: Any):
-        msg = f"{inst!r} is already locked for modification."
-        super().__init__(msg)
-
 
 class DuplicateError(ValueError):
     """Duplicate Error."""
 
 
 class InvalidExpr(TypeError):
     """Invalid Expression."""
@@ -45,7 +39,11 @@
 
 class DirectionError(ValueError):
     """Signal Direction Error."""
 
 
 class BuildError(RuntimeError):
     """Cannot Build Module."""
+
+
+class MultipleDriverError(ValueError):
+    """Multiple Driver Error."""
```

### Comparing `ucdp-0.3.0/src/ucdp/expr.py` & `ucdp-0.4.0/src/ucdp/expr.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 import re
 from collections.abc import Callable, Iterator
 
 from icdutil.num import calc_signed_width, calc_unsigned_width, unsigned_to_signed
 from pydantic import ValidationError
 
 from .exceptions import InvalidExpr
-from .object import Field, LightObject, model_validator
+from .object import Field, Light, Object, model_validator
 from .slices import Slice
 from .typebase import BaseScalarType, BaseType
-from .typescalar import BitType, IntegerType, SintType, UintType
+from .typehelper import BaseScalarTypes
+from .typescalar import BitType, BoolType, IntegerType, SintType, UintType
 
 _RE_CONST = re.compile(
     r"(?P<sign>[-+])?"
     r"(((?P<width>\d+)'?(?P<is_signed>s)?(?P<bnum>(b[01]+)|(o[0-7]+)|(d[0-9]+)|(h[0-9a-fA-F]+))))|(?P<num>[+-]?\d+)\b"
 )
 _NUM_BASEMAP = {
     "b": 2,
@@ -65,17 +66,22 @@
     "**": operator.pow,
     "<<": operator.lshift,
     ">>": operator.rshift,
     "|": operator.or_,
     "&": operator.and_,
     "^": operator.xor,
 }
+_SOPERMAP = {
+    "abs(": operator.abs,
+    "~": operator.inv,
+    "-": operator.neg,
+}
 
 
-class Expr(LightObject):
+class Expr(Object):
     """Base Class for all Expressions.
 
     Attributes:
         type_: Type.
     """
 
     type_: BaseType = Field(repr=False)
@@ -224,14 +230,18 @@
         if isinstance(other, int):
             other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
         return Op(other, "//", self)
 
     def __rmod__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
+        if not isinstance(other, Expr):
+            return NotImplemented
         return Op(other, "%", self)
 
     def __rpow__(self, other) -> "Op":
         if isinstance(other, int):
             other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
@@ -269,31 +279,31 @@
         if isinstance(other, int):
             other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
         return Op(other, "^", self)
 
     def __abs__(self) -> "SOp":
-        return SOp(oper=operator.abs, sign="abs(", one=self, postsign=")")
+        return SOp(sign="abs(", one=self)
 
     def __invert__(self) -> "SOp":
-        return SOp(oper=operator.inv, sign="~", one=self)
+        return SOp(sign="~", one=self)
 
     def __neg__(self) -> "SOp":
-        return SOp(oper=operator.neg, sign="-", one=self)
+        return SOp(sign="-", one=self)
 
     def __getitem__(self, slice_):
         if isinstance(slice_, Expr):
             slice_ = Slice(left=slice_, right=slice_)
         else:
             slice_ = Slice.cast(slice_)
         return SliceOp(one=self, slice_=slice_)
 
 
-class Op(Expr):
+class Op(Expr, Light):
     """Dual Operator Expression.
 
     Args:
         left: left argument.
         sign: sign.
         right: right argument.
 
@@ -308,21 +318,26 @@
     left: Expr
     oper: Callable = Field(repr=False)
     sign: str
     right: Expr
 
     _posargs: tuple[str, ...] = ("left", "sign", "right")
 
-    def __init__(self, left: Expr, sign: str, right: Expr):
+    def __init__(self, left: Expr, sign: str, right: Expr, type_: BaseType | None = None):
         oper = _OPERMAP[sign]
-        super().__init__(left=left, oper=oper, sign=sign, right=right, type_=left.type_)  # type: ignore[call-arg]
+        if type_ is None:
+            type_ = left.type_
+        super().__init__(left=left, oper=oper, sign=sign, right=right, type_=type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return int(self.oper(int(self.left), int(self.right)))
 
+    def __bool__(self):
+        return bool(self.oper(int(self.left), int(self.right)))
+
 
 class BoolOp(Op):
     """Boolean Dual Operator Expression.
 
     Args:
         left: left argument.
         sign: sign.
@@ -332,19 +347,19 @@
         oper: Operator.
         type_: Type.
 
     ???+ bug "Todo"
         * fix inherited_members / Attributes Types
     """
 
-    def __bool__(self):
-        return bool(self.oper(int(self.left), int(self.right)))
+    def __init__(self, left: Expr, sign: str, right: Expr):
+        super().__init__(left=left, sign=sign, right=right, type_=BoolType())  # type: ignore[call-arg]
 
 
-class SOp(Expr):
+class SOp(Expr, Light):
     """Single Operator Expression.
 
     Args:
         sign: sign.
         one: Expression.
 
     Attributes:
@@ -353,29 +368,31 @@
         type_: Type.
 
     ???+ bug "Todo"
         * fix inherited_members / Attributes Types
 
     """
 
-    oper: Callable
+    oper: Callable = Field(repr=False)
     sign: str
     one: Expr
     postsign: str = ""
 
-    _posargs: tuple[str, ...] = ("sign", "oper", "one")
+    _posargs: tuple[str, ...] = ("sign", "one")
 
-    def __init__(self, oper: Callable, sign: str, one: Expr, postsign: str = ""):
+    def __init__(self, sign: str, one: Expr):
+        oper = _SOPERMAP[sign]
+        postsign = ")" if "(" in sign else ""
         super().__init__(oper=oper, sign=sign, one=one, postsign=postsign, type_=one.type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return self.oper(int(self.one))
 
 
-class SliceOp(Expr):
+class SliceOp(Expr, Light):
     """Slice Expression.
 
     Args:
         one: Expression.
         slice_: Slice
 
     Attributes:
@@ -393,15 +410,15 @@
     def __init__(self, one: Expr, slice_: Slice):
         super().__init__(one=one, slice_=slice_, type_=one.type_[slice_])  # type: ignore[call-arg]
 
     def __int__(self):
         return int(self.one.type_[self.slice_].default)
 
 
-class ConstExpr(Expr):
+class ConstExpr(Expr, Light):
     """
     Constant.
 
     Args:
         type_: Type.
 
     ??? Example "ConstExpr Examples"
@@ -424,18 +441,20 @@
     def __init__(self, type_: BaseType):
         super().__init__(type_=type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return int(self.type_.default)
 
     def __getitem__(self, slice_):
+        if isinstance(slice_, Expr):
+            slice_ = Slice(left=slice_, right=slice_)
         return ConstExpr(self.type_[slice_])
 
 
-class ConcatExpr(Expr):
+class ConcatExpr(Expr, Light):
     """
     Concatenation.
 
     Args:
         items: Expressions.
 
     Attributes:
@@ -453,47 +472,44 @@
             ...     u.ConstExpr(u.UintType(7, default=1)),
             ...     u.ConstExpr(u.UintType(16, default=3)),
             ... ))
             >>> expr
             ConcatExpr((ConstExpr(UintType(5, default=5)), ... ConstExpr(UintType(16, default=3))))
             >>> int(expr)
             12325
-            >>> expr.type_
-            UintType(28, default=12325)
     """
 
     items: tuple[Expr, ...]
 
     _posargs: tuple[str, ...] = ("items",)
 
     def __init__(self, items: tuple[Expr, ...]):
+        for item in items:
+            if not isinstance(item.type_, BaseScalarType):
+                raise ValueError(f"Item {item} type is {item.type_}, but must be a Scalar Type")
+
         pairs = tuple(ConcatExpr.__iter_values(items))
         default = sum(value << shift for value, shift in pairs)
         width = pairs[-1][1] if pairs else 1
         type_ = UintType(width, default=default)
         super().__init__(items=items, type_=type_)  # type: ignore[call-arg]
 
     def __int__(self):
-        return sum(value << shift for value, shift in self.__iter_values(self.items))
+        return sum(int(value << shift) for value, shift in self.__iter_values(self.items))
 
     @staticmethod
     def __iter_values(items: tuple[Expr, ...]) -> Iterator[tuple[int, int]]:
         shift = 0
         for item in items:
-            if isinstance(item, int):
-                yield item, shift
-                shift += 32
-            else:
-                # TODO: fix type issue
-                yield int(item), shift  # type: ignore[call-overload]
-                shift += item.type_.width  # type: ignore[attr-defined]
+            yield item, shift
+            shift += item.type_.width  # type: ignore[attr-defined]
         yield 0, shift
 
 
-class TernaryExpr(Expr):
+class TernaryExpr(Expr, Light):
     """
     TernaryExpr Expression.
 
     Args:
         cond: BoolOp
         one: Expression
         other: Expression
@@ -513,15 +529,15 @@
             TernaryExpr(BoolOp(Signal(UintType(2), 'if_s'), ... Signal(UintType(16, default=20), 'other_s'))
             >>> int(expr)
             20
             >>> expr.type_
             UintType(16, default=10)
     """
 
-    type_: BaseScalarType = Field(repr=False)
+    type_: BaseScalarTypes = Field(repr=False)
     cond: BoolOp
     one: Expr
     other: Expr
 
     _posargs: tuple[str, ...] = ("cond", "one", "other")
 
     def __init__(self, cond: BoolOp, one: Expr, other: Expr):
@@ -529,15 +545,15 @@
 
     def __int__(self):
         if bool(self.cond):
             return int(self.one)
         return int(self.other)
 
 
-class Log2Expr(Expr):
+class Log2Expr(Expr, Light):
     """
     Ceiling Logarithm to base of 2.
 
     Args:
         expr: Expression
 
     Attributes:
@@ -552,27 +568,27 @@
             Log2Expr(ConstExpr(UintType(5, default=5)))
             >>> int(expr)
             2
             >>> expr.type_
             UintType(5, default=5)
     """
 
-    type_: BaseScalarType = Field(repr=False)
+    type_: BaseScalarTypes = Field(repr=False)
     expr: Expr
 
     _posargs: tuple[str, ...] = ("expr",)
 
     def __init__(self, expr: Expr):
         super().__init__(expr=expr, type_=expr.type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return int(math.log(int(self.expr), 2))
 
 
-class MinimumExpr(Expr):
+class MinimumExpr(Expr, Light):
     """
     Smallest Value.
 
     Args:
         items: Items
 
     Attributes:
@@ -591,27 +607,27 @@
             MinimumExpr((ConstExpr(UintType(5, default=5)), ... ConstExpr(UintType(16, default=3))))
             >>> int(expr)
             1
             >>> expr.type_
             UintType(5, default=5)
     """
 
-    type_: BaseScalarType = Field(repr=False)
+    type_: BaseScalarTypes = Field(repr=False)
     items: tuple[Expr, ...]
 
     _posargs: tuple[str, ...] = ("items",)
 
     def __init__(self, items: tuple[Expr, ...]):
         super().__init__(items=items, type_=items[0].type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return min(int(item) for item in self.items)
 
 
-class MaximumExpr(Expr):
+class MaximumExpr(Expr, Light):
     """
     Largest Value.
 
     Args:
         items: Items
 
     Attributes:
@@ -630,27 +646,27 @@
             MaximumExpr((ConstExpr(UintType(5, default=5)), ... ConstExpr(UintType(16, default=3))))
             >>> int(expr)
             5
             >>> expr.type_
             UintType(5, default=5)
     """
 
-    type_: BaseScalarType = Field(repr=False)
+    type_: BaseScalarTypes = Field(repr=False)
     items: tuple[Expr, ...]
 
     _posargs: tuple[str, ...] = ("items",)
 
     def __init__(self, items: tuple[Expr, ...]):
         super().__init__(items=items, type_=items[0].type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return max(int(item) for item in self.items)
 
 
-class RangeExpr(Expr):
+class RangeExpr(Expr, Light):
     """
     Value Range.
 
     Attributes:
         type_: Type.
         range_: Range.
```

### Comparing `ucdp-0.3.0/src/ucdp/exprparser.py` & `ucdp-0.4.0/src/ucdp/exprparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 """
 Expression Parser.
 """
 
 from functools import cached_property
 from typing import Any
 
+from ._castingnamespace import CastingNamespace
 from .consts import RE_IDENTIFIER
 from .exceptions import InvalidExpr
 from .expr import (
     BoolOp,
     ConcatExpr,
     ConstExpr,
     Expr,
@@ -43,58 +44,46 @@
     SOp,
     TernaryExpr,
     _parse_const,
 )
 from .namespace import Namespace
 from .note import Note
 from .object import Object, computed_field
-from .typebase import BaseType
-from .typeenum import BaseEnumType
-from .typescalar import BitType, BoolType, UintType
+from .typebase import BaseScalarType, BaseType
+from .typescalar import BoolType
 
 Parseable = Expr | str | int | BaseType | list | tuple
 Constable = int | str | ConstExpr
 Concatable = list | tuple | ConcatExpr
 
 
 class _Globals(dict):
-    def __init__(self, globals: dict, namespace: Namespace | None, strict: bool, context: str | None):
+    def __init__(self, globals: dict, namespace: Namespace | CastingNamespace | None, context: str | None):
         super().__init__(globals)
         self.namespace = namespace
-        self.strict = strict
         self.context = context
 
     def __missing__(self, key):
         if self.namespace:
-            if self.strict:
-                try:
-                    return self.namespace.get_dym(key)
-                except ValueError as err:
-                    raise NameError(f"{self.context}: {err}") from None
             try:
-                return self.namespace[key]
-            except ValueError:
-                pass
-        if self.strict:
-            raise KeyError(key)
-        return key
+                return self.namespace.get_dym(key)
+            except ValueError as err:
+                raise NameError(f"{self.context}: {err}") from None
+        return NameError(key)
 
 
 class ExprParser(Object):
     """
     ExprParser.
 
     Attributes:
         namespace (Namespace): Symbol namespace
-        strict: Do not ignore missing symbols.
-
     """
 
-    namespace: Namespace | None = None
-    strict: bool = True
+    namespace: Namespace | CastingNamespace | None = None
     context: str | None = None
 
     @computed_field
     @cached_property
     def _globals(self) -> _Globals:
         globals_ = {
             # Expressions
@@ -112,15 +101,30 @@
             "const": self.const,
             "concat": self.concat,
             "ternary": self.ternary,
             "log2": self.log2,
             "minimum": self.minimum,
             "maximum": self.maximum,
         }
-        return _Globals(globals=globals_, namespace=self.namespace, strict=self.strict, context=self.context)
+        return _Globals(globals=globals_, namespace=self.namespace, context=self.context)
+
+    def __call__(self, expr: Parseable, only=None, types=None) -> Expr:
+        """
+        Parse Expression.
+
+        This is an alias to `parse`.
+
+        Args:
+            expr: Expression
+
+        Keyword Args:
+            only: Limit expression to these final element type.
+            types: Limit expression type to to these types.
+        """
+        return self.parse(expr, only=only, types=types)
 
     def parse_note(self, expr: Parseable | Note, only=None, types=None) -> Expr | Note:
         """
         Parse Expression or Note.
 
         Args:
             expr: Expression
@@ -225,15 +229,15 @@
             if isinstance(expr, str) and RE_IDENTIFIER.match(expr):
                 try:
                     return self.namespace[expr]
                 except ValueError:
                     pass
         try:
             globals: dict[str, Any] = self._globals  # type: ignore[assignment]
-            return eval(expr, globals)  #  # noqa: S307
+            return eval(expr, globals)  # noqa: S307
         except TypeError:
             raise InvalidExpr(expr) from None
         except SyntaxError as exc:
             raise InvalidExpr(f"{expr!r}: {exc!s}") from None
 
     def const(self, value: Constable) -> ConstExpr:
         """
@@ -246,15 +250,15 @@
                 >>> p = u.ExprParser()
                 >>> p.const('10')
                 ConstExpr(IntegerType(default=10))
                 >>> p.const(10)
                 ConstExpr(IntegerType(default=10))
                 >>> p.const("10'd20")
                 ConstExpr(UintType(10, default=20))
-                >>> p.const(ConstExpr(UintType(10, default=20)))
+                >>> p.const(u.ConstExpr(u.UintType(10, default=20)))
                 ConstExpr(UintType(10, default=20))
                 >>> p.const("4'h4")
                 ConstExpr(UintType(4, default=4))
                 >>> p.const("4'sh4")
                 ConstExpr(SintType(4, default=4))
                 >>> p.const("4'shC")
                 ConstExpr(SintType(4, default=-4))
@@ -286,15 +290,15 @@
         """
         TernaryExpr Statement.
 
         ??? Example "Ternary Parser Example"
             Basics:
 
                 >>> import ucdp as u
-                >>> cond = u.Signal(u.UintType(2), 'if_s') == u.ConstExpr(UintType(2, default=1))
+                >>> cond = u.Signal(u.UintType(2), 'if_s') == u.ConstExpr(u.UintType(2, default=1))
                 >>> one = u.Signal(u.UintType(16, default=10), 'one_s')
                 >>> other = u.Signal(u.UintType(16, default=20), 'other_s')
                 >>> p = u.ExprParser()
                 >>> expr = p.ternary(cond, one, other)
                 >>> expr
                 TernaryExpr(BoolOp(Signal(UintType(2), 'if_s'), '==', ..., Signal(UintType(16, default=20), 'other_s'))
                 >>> int(expr)
@@ -368,14 +372,14 @@
 
 
 def cast_booltype(expr):
     """Cast to Boolean."""
     type_ = expr.type_
     if isinstance(type_, BoolType):
         return expr
-    if isinstance(type_, (BitType, UintType, BaseEnumType)) and int(type_.width) == 1:
-        return expr == ConstExpr(BitType(default=1))
-    raise ValueError("{expr} does not result in bool")
+    if isinstance(type_, BaseScalarType) and int(type_.width) == 1:
+        return expr == 1
+    raise ValueError(f"{expr} does not result in bool")
 
 
 _PARSER = ExprParser()
 const = _PARSER.const
```

### Comparing `ucdp-0.3.0/src/ucdp/exprresolver.py` & `ucdp-0.4.0/src/ucdp/exprresolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,32 +21,36 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
 Expression Resolver.
 """
 
+from typing import Any, ClassVar
+
 from .expr import (
     BoolOp,
     ConcatExpr,
     ConstExpr,
     Expr,
     Log2Expr,
     MaximumExpr,
     MinimumExpr,
     Op,
     RangeExpr,
     SliceOp,
     SOp,
     TernaryExpr,
 )
-from .ident import Ident
+from .ident import Ident, Idents
 from .namespace import Namespace
+from .note import Note
 from .object import Object
 from .slices import Slice
+from .typearray import ArrayType
 from .typebase import BaseScalarType, BaseType
 from .typeenum import BaseEnumType
 from .typescalar import BitType, BoolType, IntegerType, RailType, SintType, UintType
 from .typestring import StringType
 
 
 class ExprResolver(Object):
@@ -64,106 +68,144 @@
             >>> parser = u.ExprParser(namespace=idents)
             >>> expr = parser.parse('uint_s') * parser.const(2)
             >>> expr
             Op(Signal(UintType(16), 'uint_s'), '*', ConstExpr(IntegerType(default=2)))
 
             >>> resolver = u.ExprResolver(namespace=idents)
             >>> resolver.resolve(expr)
+            'uint_s * 2'
+            >>> resolver.resolve(expr, brackets=True)
             '(uint_s * 2)'
     """
 
     namespace: Namespace | None = None
+    remap: Idents | None = None
+
+    _opremap: ClassVar[dict[str, str]] = {}
+    _BRACKETTYPES: tuple[Any, ...] = (Op, BoolOp, SOp, TernaryExpr)
 
-    def resolve(self, expr: Expr) -> str:
-        """Resolve.
+    def __call__(self, expr: Expr, brackets: bool = False) -> str:
+        """
+        Resolve.
 
         Args:
             expr: Expression
+            brackets: Use brackets if necessary for topmost expr.
+        """
+        return self._resolve(expr, brackets=brackets)
+
+    def resolve(self, expr: Expr | Note, brackets: bool = False) -> str:
+        """
+        Resolve.
 
+        Args:
+            expr: Expression
+            brackets: Use brackets if necessary for topmost expr.
         """
-        return self._resolve(expr)
+        return self._resolve(expr, brackets=brackets)
 
-    def _resolve(self, expr: Expr) -> str:  # noqa: C901, PLR0911, PLR0912
+    def _resolve(self, expr: Expr | Note, brackets: bool = False) -> str:  # noqa: C901, PLR0912
         if isinstance(expr, Ident):
-            return self._resolve_ident(expr)
-        if isinstance(expr, Op):
-            return self._resolve_op(expr)
-        if isinstance(expr, BoolOp):
-            return self._resolve_boolop(expr)
-        if isinstance(expr, SOp):
-            return self._resolve_sop(expr)
-        if isinstance(expr, SliceOp):
-            return self._resolve_sliceop(expr)
-        if isinstance(expr, SOp):
-            return self._resolve_sop(expr)
-        if isinstance(expr, ConstExpr):
-            return self._resolve_constexpr(expr)
-        if isinstance(expr, ConcatExpr):
-            return self._resolve_concatexpr(expr)
-        if isinstance(expr, TernaryExpr):
-            return self._resolve_ternaryexpr(expr)
-        if isinstance(expr, Log2Expr):
-            return self._resolve_log2expr(expr)
-        if isinstance(expr, MinimumExpr):
-            return self._resolve_minimumexpr(expr)
-        if isinstance(expr, MaximumExpr):
-            return self._resolve_maximumexpr(expr)
-        if isinstance(expr, RangeExpr):
-            return self._resolve_rangeexpr(expr)
-        raise ValueError(expr)
+            resolved = self._resolve_ident(expr)
+        elif isinstance(expr, BoolOp):
+            resolved = self._resolve_boolop(expr)
+        elif isinstance(expr, SOp):
+            resolved = self._resolve_sop(expr)
+        elif isinstance(expr, Op):
+            resolved = self._resolve_op(expr)
+        elif isinstance(expr, SliceOp):
+            resolved = self._resolve_sliceop(expr)
+        elif isinstance(expr, ConstExpr):
+            resolved = self._resolve_constexpr(expr)
+        elif isinstance(expr, ConcatExpr):
+            resolved = self._resolve_concatexpr(expr)
+        elif isinstance(expr, TernaryExpr):
+            resolved = self._resolve_ternaryexpr(expr)
+        elif isinstance(expr, Log2Expr):
+            resolved = self._resolve_log2expr(expr)
+        elif isinstance(expr, MinimumExpr):
+            resolved = self._resolve_minimumexpr(expr)
+        elif isinstance(expr, MaximumExpr):
+            resolved = self._resolve_maximumexpr(expr)
+        elif isinstance(expr, RangeExpr):
+            resolved = self._resolve_rangeexpr(expr)
+        elif isinstance(expr, Note):
+            resolved = self._get_note(expr)
+        else:
+            raise ValueError(f"{expr!r} is not a valid expression.")
+        if brackets and isinstance(expr, self._BRACKETTYPES):
+            resolved = f"({resolved})"
+        return resolved
 
     def _resolve_ident(self, ident: Ident) -> str:
-        # Check if in namespace?
+        # Remapping of identifier, i.e. on instance port list
+        if self.remap is not None:
+            if ident.name in self.remap.keys():
+                ref = self.remap[ident.name]
+                if ref.value is not None and ref.value != ref:
+                    # resolve remappend identifier value
+                    return self.resolve(ref.value)
+                # just use default value
+                return self._resolve_value(ident.type_)
+
+        # Namespace checking
+        if self.namespace is not None:
+            # check if identifier exists in namespace.
+            if ident.name not in self.namespace.keys():
+                raise ValueError(f"{ident!r} not known within current namespace.")
+
         return ident.name
 
     def _resolve_op(self, op: Op) -> str:
-        left = self._resolve(op.left)
-        right = self._resolve(op.right)
-        sign = op.sign
-        if sign == "//":
-            sign = "/"
-        return f"({left} {sign} {right})"
+        left = self._resolve(op.left, brackets=True)
+        right = self._resolve(op.right, brackets=True)
+        sign = self._opremap.get(op.sign, op.sign)
+        return f"{left} {sign} {right}"
 
     def _resolve_boolop(self, op: BoolOp) -> str:
-        left = self._resolve(op.left)
-        right = self._resolve(op.right)
-        return f"({left} {op.sign} {right})"
+        left = self._resolve(op.left, brackets=True)
+        right = self._resolve(op.right, brackets=True)
+        return f"{left} {op.sign} {right}"
 
     def _resolve_sop(self, op: SOp) -> str:
         one = self._resolve(op.one)
-        return f"{op.sign}{one}"
+        return f"{op.sign}{one}{op.postsign}"
 
     def _resolve_sliceop(self, op: SliceOp) -> str:
         one = self._resolve(op.one)
         return f"{one}{self._resolve_slice(op.slice_)}"
 
+    def resolve_slice(self, slice_: Slice) -> str:
+        """Resolve Slice."""
+        return self._resolve_slice(slice_)
+
     def _resolve_slice(self, slice_: Slice) -> str:
         left = slice_.left
         right = slice_.right
         if left == right:
             if isinstance(left, int):
                 return f"[{left}]"
             return f"[{self.resolve(left)}]"
 
         if not isinstance(left, int):
             left = self.resolve(left)
         if not isinstance(right, int):
             right = self.resolve(right)
         if isinstance(left, int) and isinstance(right, int) and right == 0:
-            return f"[{left+1}-1:0]"
+            return f"[{left}:0]"
         return f"[{left}:{right}]"
 
     def _resolve_concatexpr(self, expr: ConcatExpr) -> str:
         items = ", ".join(self._resolve(item) for item in expr.items)
         return f"{{{items}}}"
 
     def _resolve_ternaryexpr(self, expr: TernaryExpr) -> str:
-        cond = self._resolve(expr.cond)
-        one = self._resolve(expr.one)
-        other = self._resolve(expr.other)
+        cond = self._resolve(expr.cond, brackets=True)
+        one = self._resolve(expr.one, brackets=True)
+        other = self._resolve(expr.other, brackets=True)
         return f"{cond} ? {one} : {other}"
 
     def _resolve_log2expr(self, expr: Log2Expr) -> str:
         raise NotImplementedError
 
     def _resolve_minimumexpr(self, expr: MinimumExpr) -> str:
         raise NotImplementedError
@@ -176,22 +218,32 @@
 
     def _resolve_constexpr(self, expr: ConstExpr) -> str:
         try:
             return self._resolve_value(expr.type_)
         except ValueError as exc:
             raise ValueError(f"{expr} {exc}") from None
 
+    def resolve_value(self, type_: BaseType, value=None) -> str:
+        """Resolve Value."""
+        return self._resolve_value(type_, value=value)
+
     def _resolve_value(self, type_: BaseType, value=None) -> str:  # noqa: C901, PLR0911, PLR0912
-        if not isinstance(type_, BaseScalarType):
-            raise ValueError("")
+        if isinstance(type_, ArrayType):
+            # TODO: value
+            itemvalue = self._resolve_value(type_.itemtype)
+            return self._get_array_value(itemvalue, type_.slice_)
 
-        # ensure value
+        if not isinstance(type_, (BaseScalarType, StringType)):
+            raise ValueError(f"Cannot resolve type {type_}")
         if value is None:
             value = type_.default
 
+        if isinstance(type_, StringType):
+            return self._get_string_value(value)
+
         # None
         if value is None:
             return ""
 
         # Expr
         if isinstance(value, Expr):
             return self.resolve(value)
@@ -202,52 +254,60 @@
         if isinstance(type_, BitType):
             return self._get_bit_value(int(value))
 
         if isinstance(type_, UintType):
             width = int(type_.width)
             if width < 1:
                 raise ValueError(f"Invalid width {width}")
-            return self._get_uint_value(value, width)
+            return self._get_uint_value(value, type_.width)
 
         if isinstance(type_, SintType):
             width = int(type_.width)
             if width < 1:
                 raise ValueError(f"Invalid width {width}")
-            return self._get_sint_value(value, width)
+            return self._get_sint_value(value, type_.width)
 
         if isinstance(type_, IntegerType):
             return self._get_integer_value(value)
 
         if isinstance(type_, RailType):
-            return self._get_rail_value(int(value))
+            return self._get_rail_value(value)
 
         if isinstance(type_, BoolType):
             return self._get_bool_value(value)
 
-        if isinstance(type_, StringType):
-            return self._get_string_value(value)
-
-        raise ValueError(type_)
+        raise AssertionError
 
     @staticmethod
     def _get_rail_value(value: int) -> str:
         return str(value)
 
     @staticmethod
     def _get_bit_value(value: int) -> str:
         return str(value)
 
     @staticmethod
-    def _get_uint_value(value: int, width: int) -> str:
+    def _get_uint_value(value: int, width: int | Expr) -> str:
         return str(value)
 
     @staticmethod
-    def _get_sint_value(value: int, width: int) -> str:
+    def _get_sint_value(value: int, width: int | Expr) -> str:
         return str(value)
 
     @staticmethod
     def _get_integer_value(value: int) -> str:
         return str(value)
 
     @staticmethod
     def _get_bool_value(value: bool) -> str:
         return str(value)
+
+    @staticmethod
+    def _get_string_value(value: int) -> str:
+        return repr(value)
+
+    @staticmethod
+    def _get_note(note: Note) -> str:
+        return repr(note.note)
+
+    def _get_array_value(self, itemvalue: str, slice_: Slice) -> str:
+        raise NotImplementedError
```

### Comparing `ucdp-0.3.0/src/ucdp/filelistparser.py` & `ucdp-0.4.0/src/ucdp/filelistparser.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/fileset.py` & `ucdp-0.4.0/src/ucdp/fileset.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/flipflop.py` & `ucdp-0.4.0/src/ucdp/flipflop.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/generate.py` & `ucdp-0.4.0/src/ucdp/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,39 +49,41 @@
 def generate(
     topmod: BaseMod,
     name: str,
     target: str | None = None,
     filelistparser: FileListParser | None = None,
     makolator: Makolator | None = None,
     maxlevel: int | None = None,
+    maxworkers: int | None = None,
 ):
     """
     Generate for Top-Module.
 
     Args:
         topmod: Top Module
         name: Filelist Name
 
     Keyword Args:
         target: Target Filter
         filelistparser: Specific File List Parser
         makolator: Specific Makolator
         maxlevel: Stop Generation on given hierarchy level.
+        maxworkers: Maximal Parallelism.
     """
     makolator = makolator or get_makolator()
     LOGGER.debug("%s", makolator.config)
     modfilelists = iter_modfilelists(
         topmod,
         name,
         target=target,
         filelistparser=filelistparser,
         replace_envvars=True,
         maxlevel=maxlevel,
     )
-    with ThreadPoolExecutor() as executor:
+    with ThreadPoolExecutor(max_workers=maxworkers) as executor:
         jobs = []
         for mod, modfilelist in modfilelists:
             if modfilelist.gen == "no":
                 continue
             filepaths: tuple[Path, ...] = modfilelist.filepaths or ()  # type: ignore[assignment]
             template_filepaths: tuple[Path, ...] = modfilelist.template_filepaths or ()  # type: ignore[assignment]
             context = {"mod": mod}
@@ -105,42 +107,48 @@
 def clean(
     topmod: BaseMod,
     name: str,
     target: str | None = None,
     filelistparser: FileListParser | None = None,
     makolator: Makolator | None = None,
     maxlevel: int | None = None,
+    maxworkers: int | None = None,
     dry_run: bool = False,
 ):
     """
     Remove Generated Files for Top-Module.
 
     Args:
         topmod: Top Module
         name: Filelist Name
 
     Keyword Args:
         target: Target Filter
         filelistparser: Specific File List Parser
         makolator: Specific Makolator
         maxlevel: Stop Generation on given hierarchy level.
+        maxworkers: Maximal Parallelism.
         dry_run: Do nothing.
     """
     makolator = makolator or get_makolator()
     LOGGER.debug("%s", makolator.config)
     modfilelists = iter_modfilelists(
         topmod,
         name,
         target=target,
         filelistparser=filelistparser,
         replace_envvars=True,
         maxlevel=maxlevel,
     )
-    for _, modfilelist in modfilelists:
-        filepaths: tuple[Path, ...] = modfilelist.filepaths or ()  # type: ignore[assignment]
-        if modfilelist.gen == "gen":
-            for filepath in filepaths:
-                print("Removing '{filepath!s}'")
-                if not dry_run:
-                    filepath.unlink(missing_ok=True)
+    with ThreadPoolExecutor(max_workers=maxworkers) as executor:
+        jobs = []
+        for _, modfilelist in modfilelists:
+            filepaths: tuple[Path, ...] = modfilelist.filepaths or ()  # type: ignore[assignment]
+            if modfilelist.gen == "full":
+                for filepath in filepaths:
+                    print(f"Removing '{filepath!s}'")
+                    if not dry_run:
+                        jobs.append(executor.submit(filepath.unlink, missing_ok=True))
+        for job in jobs:
+            job.result()
     if dry_run:
         print("DRY RUN. Nothing done.")
```

### Comparing `ucdp-0.3.0/src/ucdp/humannum.py` & `ucdp-0.4.0/src/ucdp/humannum.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 
 Hex = Annotated[
     humannum.Hex,
     BeforeValidator(lambda x: humannum.hex_(x)),
     PlainSerializer(lambda x: str(x), return_type=str),
     WithJsonSchema({"type": "string"}, mode="serialization"),
 ]
-"""Hex. """
+"""Hex."""
 
 Bytes = Annotated[
     humannum.Bytes,
     BeforeValidator(lambda x: humannum.bytes_(x)),
     PlainSerializer(lambda x: str(x), return_type=str),
     WithJsonSchema({"type": "string"}, mode="serialization"),
 ]
-"""Bytes. """
+"""Bytes."""
 
 Bin = Annotated[
     humannum.Bin,
     BeforeValidator(lambda x: humannum.bin_(x)),
     PlainSerializer(lambda x: str(x), return_type=str),
     WithJsonSchema({"type": "string"}, mode="serialization"),
 ]
-"""Bin. """
+"""Bin."""
```

### Comparing `ucdp-0.3.0/src/ucdp/ident.py` & `ucdp-0.4.0/src/ucdp/ident.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,27 +100,28 @@
 
 """
 
 from collections import deque
 from collections.abc import Callable, Iterable, Iterator
 from typing import Any
 
+from .casting import Casting
 from .consts import PAT_IDENTIFIER
 from .doc import Doc
 from .expr import ConcatExpr, ConstExpr, Expr, Log2Expr, MaximumExpr, MinimumExpr, Op, SliceOp, SOp, TernaryExpr
 from .namespace import Namespace
 from .nameutil import join_names, split_suffix
-from .object import Field, NamedObject
+from .object import Field, Light, NamedObject
 from .orientation import AOrientation
 from .typearray import ArrayType
 from .typebase import BaseType
 from .typestruct import BaseStructType
 
 
-class Ident(Expr, NamedObject):
+class Ident(Expr, NamedObject, Light):
     """Identifier.
 
     Args:
         type_: Type.
         name: Name.
 
     Attributes:
@@ -179,34 +180,38 @@
     def __iter__(self):
         return _iters([self])
 
     def iter(self, filter_=None, stop=None, value=None) -> Iterator:
         """Iterate over Hierarchy."""
         return _iters([self], filter_=filter_, stop=stop, value=value)
 
+    def cast(self, other: "Ident") -> Casting:
+        """Cast self=cast(other)."""
+        return None
+
 
 #     def iterhier(self, filter_=None, stop=None, maxlevel=None, value=None) -> Iterator:
-#         """Iterate over Hierarchy."""
+#        """Iterate over Hierarchy."""
 #         hier: List[Ident] = []
 #         for ident in self.iter(stop=stop, maxlevel=maxlevel, value=value):
 #             hier = hier[: ident.level] + [ident]
 #             if not filter_ or filter_(ident):
 #                 yield tuple(hier)
 
 #     def get(self, name, value=None):
-#         """
+#        """
 #         Get Member of Hierarchy.
 
 #         Args:
 #             name: Name
 
 #         Keyword Args:
 #             value: value
 #             dym (bool): Enriched `ValueError` exception.
-#         """
+#        """
 #         if name.startswith("_"):
 #             name = f"{self.basename}{name}"
 #         return get_ident([self], name, value=value, dym=True)
 
 IdentFilter = Callable[[Ident], bool]
 IdentStop = Callable[[Ident], bool]
 
@@ -220,20 +225,20 @@
 
     def iter(self, filter_: IdentFilter | None = None, stop: IdentStop | None = None) -> Iterator[Ident]:
         """Iterate over all Identifier."""
         for ident in self.values():
             yield from ident.iter(filter_=filter_, stop=stop)
 
     # def iterhier(self, filter_=None, stop=None, maxlevel=None) -> Iterator:
-    #     """Iterate over all Identifier and return hierarchy."""
+    #    """Iterate over all Identifier and return hierarchy."""
     #     for ident in self.values():
     #         yield from ident.iterhier(filter_=filter_, stop=stop, maxlevel=maxlevel)
 
     # def findfirst(self, filter_=None, stop=None, maxlevel=None) -> "Ident" | None:
-    #     """Iterate Over Identifier And Find First Match."""
+    #    """Iterate Over Identifier And Find First Match."""
     #     for ident in self.iter(filter_=filter_, stop=stop, maxlevel=maxlevel):
     #         return ident
     #     return None
 
     def __getitem__(self, name):
         return get_ident(self, name)
 
@@ -243,30 +248,34 @@
         elif isinstance(item, str):
             name = item
         else:
             return False
         return _get_ident(self.values(), name) is not None
 
 
-def _iters(idents: Iterable[Ident], filter_=None, stop=None, value=None) -> Iterator[Ident]:  # noqa: C901
+def _iters(idents: Iterable[Ident], filter_=None, stop=None, value=None) -> Iterator[Ident]:  # noqa: C901,PLR0912
     # highly optimized!
 
     for rootident in idents:
         stack = deque([rootident])
         while True:
             try:
                 ident = stack.pop()
             except IndexError:
                 break
 
             if stop and stop(ident):
                 break
 
             type_ = ident.type_
-            # assert value is None, "TODO"
+            if value is not None:
+                if isinstance(type_, BaseStructType):
+                    raise ValueError(f"Cannot apply value {value} for {type_}")
+                type_ = type_.new(default=value)
+                ident = ident.new(type_=type_)
 
             if not filter_ or filter_(ident):
                 yield ident
             if isinstance(type_, BaseStructType):
                 for structitem in reversed(type_.values()):
                     direction = ident.direction and ident.direction * structitem.orientation
                     suffix = (direction and direction.suffix) or ident.suffix
@@ -305,26 +314,24 @@
     #         names = [ident.name for ident in _iters(idents)]
     #         nametree = align(_get_identtree(idents), rtrim=True)
     #         msg += f" Known are\n{nametree}\n\n{msg}\n"
     #         msg += didyoumean(name, names, multiline=True)
     raise ValueError(msg)
 
 
-# def get_subname(parent: Ident, ident: Ident):
-#     """Get name relative to parent."""
-#     if parent is ident:
-#         return ident.suffix
-#     parentbasename = parent.basename
-#     name = ident.name
-#     assert name.startswith(parentbasename)
-#     return name[len(parentbasename) + 1 :]
+def get_subname(parent: Ident, ident: Ident):
+    """Get name relative to parent."""
+    if parent is ident:
+        return ident.suffix
+    parentbasename = parent.basename
+    return ident.name.removeprefix(parentbasename)[1:]
 
 
 # def get_subnames(idents):
-#     """Return names of hierarchical idents."""
+#    """Return names of hierarchical idents."""
 #     names = []
 #     prefix = ""
 #     for ident in idents:
 #         basename = ident.basename
 #         names.append(basename.removeprefix(prefix))
 #         prefix = f"{basename}_"
 #     return names
@@ -368,9 +375,9 @@
             heap.append(item.other)
         elif isinstance(item, Log2Expr):
             heap.append(item.expr)
         elif isinstance(item, Ident):
             if item.name not in idents:
                 idents[item.name] = item
         else:
-            raise TypeError(f"Unknown expr {item}")
+            raise TypeError(f"Unknown expr {item}")  # pragma: no cover
     return tuple(idents.values())
```

### Comparing `ucdp-0.3.0/src/ucdp/iterutil.py` & `ucdp-0.4.0/src/ucdp/iterutil.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/loader.py` & `ucdp-0.4.0/src/ucdp/loader.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/logging.py` & `ucdp-0.4.0/src/ucdp/typehelper.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
-Logging.
+Type Helper.
 """
 
-import logging
+from .typebase import AScalarType
+from .typeenum import BaseEnumType
 
-LOGGER = logging.getLogger("ucdp")
+BaseScalarTypes = AScalarType | BaseEnumType
```

### Comparing `ucdp-0.3.0/src/ucdp/mod.py` & `ucdp-0.4.0/src/ucdp/mod.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 # SOFTWARE.
 #
 
 """
 Hardware Module.
 """
 
-from caseconverter import snakecase
-
 from .modbasetop import BaseTopMod
+from .modutil import get_modname, get_topmodname
 
 
 class AMod(BaseTopMod):
     """
     A Normal Module With Parameters And A Fixed Number Of Ports (maybe `ifdef` encapsulated).
 
     See [BaseMod][ucdp.modbase.BaseMod] for arguments, attributes and details.
@@ -57,13 +56,13 @@
     Warning:
         There is no other build method on purpose!
     """
 
     @property
     def modname(self) -> str:
         """Module Name."""
-        return snakecase(self.__class__.__name__.removesuffix("Mod"))
+        return get_modname(self.__class__)
 
     @property
     def topmodname(self) -> str:
         """Top Module Name."""
-        return self.modname
+        return get_topmodname(self.__class__)
```

### Comparing `ucdp-0.3.0/src/ucdp/modbase.py` & `ucdp-0.4.0/src/ucdp/modbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,17 @@
 """
 
 from abc import abstractmethod
 from functools import cached_property
 from typing import Any, ClassVar, Optional, Union, no_type_check
 
 from caseconverter import snakecase
+from uniquer import uniquetuple
 
-from .assigns import Assigns, AssignSource, Drivers, Note
+from .assigns import Assigns, Drivers, Note, Source
 from .baseclassinfo import get_baseclassinfos
 from .const import Const
 from .consts import UPWARDS
 from .doc import Doc
 from .docutil import doc_from_type
 from .exceptions import LockError
 from .expr import BoolOp, Expr
@@ -53,15 +54,14 @@
 from .nameutil import join_names, split_prefix
 from .object import Field, NamedObject, Object, PrivateField, computed_field
 from .orientation import FWD, IN, Direction, Orientation
 from .param import Param
 from .routepath import Routeables, RoutePath, parse_routepaths
 from .signal import BaseSignal, Port, Signal
 from .typebase import BaseType
-from .typeclkrst import ClkType, RstAnType
 from .typedescriptivestruct import DescriptiveStructType
 from .typestruct import StructItem
 
 
 class BaseMod(NamedObject):
     """
     Hardware Module.
@@ -107,17 +107,15 @@
     __flipflops: dict[int, FlipFlop] = PrivateField(default_factory=dict)
     __muxes: Namespace = PrivateField(default_factory=Namespace)
     __parents = PrivateField(default_factory=list)
 
     def __init__(self, parent: Optional["BaseMod"] = None, name: str | None = None, **kwargs):
         cls = self.__class__
         if not cls.__name__.endswith("Mod"):
-            raise ValueError(f"Name of {cls} MUST end with 'Mod'")
-        if cls.__name__ == "BaseMod":
-            raise ValueError("BaseMod is forbidden to be used directly")
+            raise NameError(f"Name of {cls} MUST end with 'Mod'")
         if not name:
             if parent:
                 raise ValueError("'name' is required for sub modules.")
             name = snakecase(cls.__name__.removesuffix("Mod"))
         super().__init__(parent=parent, name=name, **kwargs)  # type: ignore[call-arg]
 
     @property
@@ -149,34 +147,48 @@
     def qualname(self) -> str:
         """Qualified Name (Library Name + Module Name)."""
         return f"{self.libname}.{self.modname}"
 
     @cached_property
     def basequalnames(self) -> tuple[str, ...]:
         """Qualified Name (Library Name + Module Name) of Base Modules."""
-        return tuple(f"{baseclassinfo.libname}.{baseclassinfo.modname}" for baseclassinfo in get_modbaseinfos(self))
+        return uniquetuple(f"{bci.libname}.{bci.modname}" for bci in get_modbaseinfos(self))
 
     @classmethod
     def get_modref(cls) -> ModRef:
         """Python Class Reference."""
         bci = next(get_baseclassinfos(cls))
         return ModRef(
             libname=bci.libname,
             modname=bci.modname,
             modclsname=bci.clsname,
         )
 
+    @classmethod
+    def get_basemodrefs(cls) -> tuple[ModRef, ...]:
+        """Python Class Reference."""
+        return tuple(
+            ModRef(
+                libname=bci.libname,
+                modname=bci.modname,
+                modclsname=bci.clsname,
+            )
+            for bci in get_modbaseinfos(cls)
+        )
+
     @property
     def hiername(self) -> str:
         """Hierarchical Name."""
-        has_hiername = self.has_hiername
-        basename = split_prefix(self.name)[1] if has_hiername else ""
-        if basename and self.parent:
-            return join_names(self.parent.hiername, basename)
-        return basename
+        mod: "BaseMod" | None = self
+        names: list[str] = []
+        while mod is not None:
+            if mod.has_hiername:
+                names.insert(0, split_prefix(mod.name)[1])
+            mod = mod.parent
+        return join_names(*names)
 
     @property
     @abstractmethod
     def is_tb(self) -> bool:
         """Determine if module belongs to Testbench or Design."""
 
     @property
@@ -262,15 +274,15 @@
             assert name is None
         else:
             type_: BaseType = arg
             doc = doc_from_type(type_, title=title, descr=descr, comment=comment)
             value = self.paramdict.pop(name, None)
             param = Param(type_=type_, name=name, doc=doc, ifdef=ifdef, value=value)
         if self.__is_locked:
-            raise LockError(f"{self}: Cannot add param {name!r}. Module built was already completed and is froozen.")
+            raise LockError(f"{self}: Cannot add parameter {name!r}.")
         self.namespace.add(param, exist_ok=exist_ok)
         self.params.add(param, exist_ok=exist_ok)
         return param
 
     def add_const(
         self,
         arg: BaseType | Const,
@@ -299,15 +311,15 @@
             const: Const = arg
             assert name is None
         else:
             type_: BaseType = arg
             doc = doc_from_type(type_, title=title, descr=descr, comment=comment)
             const = Const(type_=type_, name=name, doc=doc, ifdef=ifdef)
         if self.__is_locked:
-            raise LockError(f"{self}: Cannot add const {name!r}. Module built was already completed and is froozen.")
+            raise LockError(f"{self}: Cannot add constant {name!r}.")
         self.namespace.add(const, exist_ok=exist_ok)
         return const
 
     def add_type_consts(self, type_, exist_ok=False, only=None, name=None, item_suffix="e"):
         """
         Add description of `type_` as local parameters.
 
@@ -359,15 +371,15 @@
             route: Routes (iterable or string separated by ';')
         """
         doc = doc_from_type(type_, title, descr, comment)
         if direction is None:
             direction = Direction.from_name(name) or IN
         port = Port(type_, name, direction=direction, doc=doc, ifdef=ifdef)
         if self.__is_locked:
-            raise LockError(f"{self}: Cannot add port {name!r}. Module built was already completed and is froozen.")
+            raise LockError(f"{self}: Cannot add port {name!r}.")
         self.namespace[name] = port
         self.portssignals[name] = port
         self.ports[name] = port
         for routepath in parse_routepaths(route):
             self._router.add(RoutePath(expr=port), routepath)
         return port
 
@@ -396,15 +408,15 @@
             comment: Source Code Comment. Default is 'title'
             ifdef: IFDEF mapping
             route: Routes (iterable or string separated by ';')
         """
         doc = doc_from_type(type_, title, descr, comment)
         signal = Signal(type_, name, direction=direction, doc=doc, ifdef=ifdef)
         if self.__is_locked:
-            raise LockError(f"{self}: Cannot add port {name!r}. Module built was already completed and is froozen.")
+            raise LockError(f"{self}: Cannot add signal {name!r}.")
         self.namespace[name] = signal
         self.portssignals[name] = signal
         for routepath in parse_routepaths(route):
             self._router.add(RoutePath(expr=signal), routepath)
         return signal
 
     def add_port_or_signal(
@@ -473,59 +485,64 @@
     ):
         """
         Assign `target` to `source`.
 
         The assignment is done **without** routing.
 
         Args:
-            target (Expr): Target to be driven. Must be known within this module.
-            source (Expr): Source driving target. Must be known within this module.
+            target: Target to be driven. Must be known within this module.
+            source: Source driving target. Must be known within this module.
 
         Keyword Args:
             cast (bool): Cast. `False` by default.
             overwrite (bool): Overwrite existing assignment.
             filter_ (str, Callable): Target names or function to filter target identifiers.
         """
         if self.__is_locked:
-            raise LockError(
-                f"{self}: Cannot add assign '{source}' to '{target}'. "
-                "Module built was already completed and is froozen."
-            )
+            raise LockError(f"{self}: Cannot add assign '{source}' to '{target}'.")
         parser = self.parser
         assigntarget: BaseSignal = parser.parse(target, only=BaseSignal)  # type: ignore[assignment]
-        assignsource: AssignSource = parser.parse_note(source, only=AssignSource)  # type: ignore[assignment]
+        assignsource: Source = parser.parse_note(source, only=Source)  # type: ignore[assignment]
         self.assigns.set(assigntarget, assignsource, cast=cast, overwrite=overwrite)
 
     def add_inst(self, inst: "BaseMod") -> None:
         """
         Add Submodule `inst`.
 
         Args:
             inst: Instance.
         """
+        if self.__is_locked:
+            raise LockError(f"{self}: Cannot add instance '{inst}'.")
         inst.set_parent(self)
         self.insts.add(inst)  # type: ignore[arg-type]
-        assigns = Assigns(targets=inst.ports, sources=self.namespace, drivers=self.drivers, all=True, sub=True)
-        parser = ExprParser(namespace=inst.ports, strict=False, context=str(inst))
+        assigns = Assigns(targets=inst.ports, sources=self.namespace, drivers=Drivers(), inst=True)
+        parser = ExprParser(namespace=inst.ports, context=str(inst))
         self.__instcons[inst.name] = assigns, parser
 
     def get_inst(self, inst_or_name: Union["BaseMod", str]) -> "BaseMod":
         """
         Get Module Instance.
         """
         if not isinstance(inst_or_name, str):
-            return self.insts[inst_or_name.name]
+            try:
+                return self.insts[inst_or_name.name]
+            except KeyError:
+                raise ValueError(f"{inst_or_name} is not a sub-module of {self}") from None
         inst = self
         for part in inst_or_name.split("/"):
             if part == UPWARDS:
                 if inst.parent is None:
                     raise ValueError(f"{self}: {inst} has no parent.")
                 inst = inst.parent
             else:
-                inst = inst.insts[part]
+                try:
+                    inst = inst.insts.get_dym(part)  # type: ignore[assignment]
+                except ValueError as exc:
+                    raise ValueError(f"{self} has no sub-module {exc}") from None
         return inst
 
     def set_instcon(
         self,
         inst: Union["BaseMod", str],
         port: Parseable,
         expr: Parseable,
@@ -543,35 +560,26 @@
             expr: Expression. Must be known within this module.
 
         Keyword Args:
             cast: Cast. `False` by default.
             overwrite: Overwrite existing assignment.
         """
         if self.__is_locked:
-            raise LockError(
-                f"{self}: Cannot add {inst} instance connections of {port} to {expr}. "
-                "Module built was already completed and is froozen."
-            )
-        mod: "BaseMod" = self._resolve_inst(inst)
+            raise LockError(f"{self}: Cannot connect '{port}' of'{inst}' to '{expr}'.")
+        mod: "BaseMod" = self.get_inst(inst)
         assigns, parser = self.__instcons[mod.name]
         assigntarget: BaseSignal = parser.parse(port, only=BaseSignal)  # type: ignore[assignment]
-        assignsource: AssignSource = self.parser.parse_note(expr, only=AssignSource)  # type: ignore[assignment]
+        assignsource: Source = self.parser.parse_note(expr, only=Source)  # type: ignore[assignment]
         assigns.set(assigntarget, assignsource, cast=cast, overwrite=overwrite)
 
     def get_instcons(self, inst: Union["BaseMod", str]) -> Assigns:
         """Retrieve All Instance Connections Of `inst`."""
-        mod: "BaseMod" = self._resolve_inst(inst)
+        mod: "BaseMod" = self.get_inst(inst)
         return self.__instcons[mod.name][0]
 
-    def _resolve_inst(self, inst: Union["BaseMod", str]) -> "BaseMod":
-        if isinstance(inst, str):
-            return self.insts[inst]
-        # Ensure that instance is known
-        return self.insts[inst.name]
-
     def add_flipflop(
         self,
         type_: BaseType,
         name: str,
         clk: Parseable,
         rst_an: Parseable,
         nxt: Parseable | None = None,
@@ -592,20 +600,20 @@
             nxt: Next Value. Basename of `name` with _nxt_s by default.
             rst: Synchronous Reset.
             ena: Enable Condition.
             route: Routing of flip-flop output.
         """
         parser = self.parser
         if self.__is_locked:
-            raise LockError(f"{self}: Cannot add flipflop {name!r}. Module built was already completed and is froozen.")
+            raise LockError(f"{self}: Cannot add flipflop {name!r}.")
         out = self.add_signal(type_, name)
         # clk
-        clk_sig: BaseSignal = parser.parse(clk, types=ClkType, only=BaseSignal)  # type: ignore[assignment]
+        clk_sig: BaseSignal = parser.parse(clk, only=BaseSignal)  # type: ignore[assignment]
         # rst_an
-        rst_an_sig: BaseSignal = parser.parse(rst_an, types=RstAnType, only=BaseSignal)  # type: ignore[assignment]
+        rst_an_sig: BaseSignal = parser.parse(rst_an, only=BaseSignal)  # type: ignore[assignment]
         # nxt
         if nxt is None:
             nxt = self.add_signal(type_, f"{out.basename}_nxt_s")
         else:
             nxt = parser.parse(nxt)
             # TODO: check connectable of nxt and out?
         # rst
@@ -668,21 +676,21 @@
             title (str): Full Spoken Name.
             descr (str): Documentation Description.
             comment (str): Source Code Comment.
 
         See :any:`Mux.set()` how to fill the multiplexer and the example above.
         """
         if self.__is_locked:
-            raise LockError(f"{self}: Cannot add mux {name!r}. Module built was already completed and is froozen.")
+            raise LockError(f"{self}: Cannot add mux {name!r}.")
         doc = Doc(title=title, descr=descr, comment=comment)
         self.__muxes[name] = mux = Mux(
             name=name,
             targets=self.portssignals,
             namespace=self.namespace,
-            drivers=self.drivers,
+            # drivers=self.drivers,
             parser=self.parser,
             doc=doc,
         )
         return mux
 
     @property
     def muxes(self) -> tuple[Mux, ...]:
@@ -690,16 +698,16 @@
         Iterate over all Multiplexer.
         """
         return tuple(self.__muxes.values())
 
     def get_mux(self, mux: Mux | str) -> Mux:
         """Get Multiplexer."""
         if not isinstance(mux, str):
-            return self.__muxes[mux.name]
-        return self.__muxes[mux]
+            return self.__muxes.get_dym(mux.name)  # type: ignore[return-value]
+        return self.__muxes.get_dym(mux)  # type: ignore[return-value]
 
     @property
     def is_locked(self) -> bool:
         """
         Return If Module Is Already Completed And Locked For Modification.
 
         Locking is done by the build process **automatically** and **MUST NOT** be done earlier or later.
@@ -711,15 +719,15 @@
         """
         Lock.
 
         Locking is done via this method by the build process **automatically** and **MUST NOT** be done earlier or
         later. Use a different module type or enumeration or struct type, if you have issues with locking.
         """
         if self.__is_locked:
-            raise LockError(f"{self} already locked. Cannot lock again.")
+            raise LockError(f"{self} is already locked. Cannot lock again.")
         for _, obj in self:
             if isinstance(obj, Namespace):
                 obj.lock()
         self.__is_locked = True
 
     def con(self, port: Routeables, source: Routeables):
         """Connect `port` to `dest`."""
```

### Comparing `ucdp-0.3.0/src/ucdp/modbasetop.py` & `ucdp-0.4.0/src/ucdp/modbasetop.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,22 +23,20 @@
 #
 
 """
 Base Top Module.
 """
 
 from abc import abstractmethod
-from inspect import getfile
-from pathlib import Path
 from typing import Any, ClassVar
 
 from ._modbuilder import build
 from .modbase import BaseMod
 from .modfilelist import ModFileLists
-from .modutil import is_tb_from_modname
+from .modutil import get_libname, is_tb_from_modname
 from .object import PrivateField
 
 
 class BaseTopMod(BaseMod):
     """Base Class For All Top Modules."""
 
     filelists: ClassVar[ModFileLists] = ()
@@ -60,13 +58,13 @@
 
         self._build()
         build(self)
 
     @property
     def libname(self) -> str:
         """Library Name."""
-        return Path(getfile(self.__class__)).parts[-2]
+        return get_libname(self.__class__)
 
     @property
     def is_tb(self) -> bool:
         """Determine if module belongs to Testbench or Design."""
         return is_tb_from_modname(self.modname)
```

### Comparing `ucdp-0.3.0/src/ucdp/modconfigurable.py` & `ucdp-0.4.0/src/ucdp/modconfigurable.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,17 @@
 # SOFTWARE.
 #
 
 """
 Configurable Module.
 """
 
-from typing import ClassVar
-
-from caseconverter import snakecase
-
 from .config import BaseConfig
-from .modbase import BaseMod
 from .modbasetop import BaseTopMod
+from .modutil import get_topmodname
 from .nameutil import join_names
 
 
 class AConfigurableMod(BaseTopMod):
     """
     A Module Which Is Assembled According To A Receipe ([AConfig][ucdp.config.AConfig]).
 
@@ -52,28 +48,27 @@
 
     .. attention:: It is forbidden to implement `add` methods or any other *tailored* functionality.
                    Use a tailored module instead!
 
     Configurable modules are located next to the python file and use the configuration name in the module name.
 
     Attributes:
-        default_config: Direction.
         config:
 
     ??? Example "AConfigurableMod Example"
             Basics:
 
             >>> import ucdp as u
             >>> class MyConfig(u.AConfig):
             ...
             ...     feature: bool = False
 
             >>> class ProcMod(u.AConfigurableMod):
             ...
-            ...     default_config = MyConfig('default')
+            ...     config: MyConfig = MyConfig('default')
             ...
             ...     def _build(self) -> None:
             ...         if self.config.feature:
             ...             self.add_port(u.UintType(8), "feature_i")
             ...             self.add_port(u.UintType(8), "feature_o")
             ...         else:
             ...             self.add_port(u.UintType(8), "default_o")
@@ -87,29 +82,18 @@
             >>> my = ProcMod(config=MyConfig('other', feature=True))
             >>> my.modname
             'proc_other'
             >>> my.ports
             Idents([Port(UintType(8), 'feature_i', direction=IN), Port(UintType(8), 'feature_o', direction=OUT)])
     """
 
-    default_config: ClassVar[BaseConfig | None] = None
     config: BaseConfig
 
-    def __init__(
-        self, parent: BaseMod | None = None, name: str | None = None, config: BaseConfig | None = None, **kwargs
-    ):
-        if config is None:
-            config = self.__class__.default_config
-        super().__init__(parent=parent, name=name, config=config, **kwargs)  # type: ignore[call-arg]
-
     @property
     def modname(self) -> str:
         """Module Name."""
-        modname = self.basename
-        if self.config:
-            return join_names(modname, self.config.name)
-        return modname
+        return join_names(self.basename, self.config.name)
 
     @property
     def topmodname(self) -> str:
         """Top Module Name."""
-        return snakecase(self.__class__.__name__.removesuffix("Mod"))
+        return get_topmodname(self.__class__)
```

### Comparing `ucdp-0.3.0/src/ucdp/modcore.py` & `ucdp-0.4.0/src/ucdp/modcore.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 Core Module.
 """
 
 from typing import ClassVar
 
 from .modbase import BaseMod
 from .modfilelist import ModFileLists
-from .modutil import is_tb_from_modname
 from .nameutil import join_names
 from .object import model_validator
 
 
 class ACoreMod(BaseMod):
     """
     Intermediate Module Hierarchy.
@@ -74,15 +73,13 @@
     def topmodname(self) -> str:
         """Top Module Name."""
         return self.parent.topmodname
 
     @property
     def is_tb(self) -> bool:
         """Determine if module belongs to Testbench or Design."""
-        if self.parent:
-            return self.parent.is_tb
-        return is_tb_from_modname(self.modname)
+        return self.parent.is_tb
 
     @model_validator(mode="after")
     def __post_init(self) -> "ACoreMod":
         self.parent.add_inst(self)
         return self
```

### Comparing `ucdp-0.3.0/src/ucdp/modfilelist.py` & `ucdp-0.4.0/src/ucdp/modfilelist.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/moditer.py` & `ucdp-0.4.0/src/ucdp/moditer.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return iter_
 
     @staticmethod
     @abstractmethod
     def _iter(
         mods: Iterable[BaseMod], filter_: FilterFunc, stop: StopFunc, stop_insts: StopFunc, maxlevel: MaxLevel
     ) -> Iterator[BaseMod]:
-        pass
+        pass  # pragma: no cover
 
 
 class ModPreIter(BaseModIter):
     """
 
     Iterate over module hierarchy starting at `mod`, using the pre-order strategy.
 
@@ -275,15 +275,15 @@
         base: namepats must match against module `basequalnames` instead of `qual_name`.
     """
     mods = get_mods(topmod, namepats, unique=True, base=base)
     if len(mods) == 1:
         return mods[0]
     listed_mods = mods or ModPostIter(topmod, unique=True)
     if base:
-        names = sorted(uniquer.unique(chain.from_iterable(mod.basequalnames) for mod in listed_mods))
+        names = sorted(uniquer.unique(chain.from_iterable(mod.basequalnames for mod in listed_mods)))
     else:
         names = sorted(uniquer.unique(mod.qualname for mod in listed_mods))
     if mods:
         lines = (f"Found multiple hardware modules for {namepats!r}:", *names)
     else:
         lines = (f"{namepats!r} not found. Known are:", *names)
     raise ValueError("\n  ".join(lines))
@@ -307,15 +307,15 @@
     """
     if namepats:
         patfilter = namefilter(namepats)
 
         if base:
 
             def filter_(mod):
-                qualnames = uniquer.unique(*mod.basequalnames)
+                qualnames = uniquer.unique(mod.basequalnames)
                 return any(patfilter(qualname) for qualname in qualnames)
         else:
 
             def filter_(mod):
                 return patfilter(mod.qualname)
 
         return tuple(ModPostIter(topmod, filter_=filter_, unique=unique))
```

### Comparing `ucdp-0.3.0/src/ucdp/modref.py` & `ucdp-0.4.0/src/ucdp/modref.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,16 @@
             Module from a package and explicit class:
 
             >>> spec = ModRef.cast('glbl_lib.clk_gate.ClkGateMod')
             >>> spec
             ModRef('glbl_lib', 'clk_gate', modclsname='ClkGateMod')
             >>> str(spec)
             'glbl_lib.clk_gate.ClkGateMod'
+            >>> ModRef.cast(ModRef('glbl_lib', 'clk_gate', modclsname='ClkGateMod'))
+            ModRef('glbl_lib', 'clk_gate', modclsname='ClkGateMod')
 
             Invalid Pattern:
 
             >>> ModRef.cast('lib.my:c-ls')
             Traceback (most recent call last):
             ..
             ValueError: 'lib.my:c-ls' does not match pattern 'lib.my[.MyMod]'
```

### Comparing `ucdp-0.3.0/src/ucdp/modtailored.py` & `ucdp-0.4.0/src/ucdp/modtailored.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,18 @@
 Tailored Module.
 
 """
 
 from abc import abstractmethod
 from typing import Any, ClassVar
 
-from caseconverter import snakecase
-
 from ._modbuilder import build
 from .modbase import BaseMod
 from .modfilelist import ModFileLists
-from .modutil import is_tb_from_modname
+from .modutil import get_libname, get_topmodname, is_tb_from_modname
 from .nameutil import join_names
 from .object import PrivateField
 
 
 class ATailoredMod(BaseMod):
     """
     Module Which Is Tailored For Every Use Case By The Parent Module, Mainly The Number And Names Of Ports.
@@ -130,22 +128,22 @@
         return modname
 
     @property
     def topmodname(self) -> str:
         """Top Module Name."""
         if self.parent:
             return self.parent.topmodname
-        return snakecase(self.__class__.__name__.removesuffix("Mod"))
+        return get_topmodname(self)
 
     @property
     def libname(self) -> str:
         """Library Name."""
         if self.parent:
             return self.parent.libname
-        return super().libname  # type: ignore[safe-super]
+        return get_libname(self.__class__)
 
     @property
     def is_tb(self) -> bool:
         """Determine if module belongs to Testbench or Design."""
         if self.parent:
             return self.parent.is_tb
         return is_tb_from_modname(self.modname)
```

### Comparing `ucdp-0.3.0/src/ucdp/modtb.py` & `ucdp-0.4.0/src/ucdp/modtb.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 """
 Testbench Module.
 """
 
 from abc import abstractmethod
 from collections.abc import Iterator
-from inspect import getfile
-from pathlib import Path
 from typing import Any, ClassVar
 
 from caseconverter import snakecase
 
 from ._modbuilder import build
 from .modbase import BaseMod
 from .modfilelist import ModFileLists
 from .moditer import ModPreIter
+from .modtopref import TopModRef
+from .modutil import get_libname, get_modname, get_topmodname
 from .object import Field
 from .test import Test
 
 
 class ATbMod(BaseMod):
     """
     Testbench Module.
@@ -115,33 +115,33 @@
         cls = self.__class__
         if dut is None:
             dut = cls.build_dut()
         if not name:
             basename = snakecase(cls.__name__.removesuffix("Mod"))
             name = f"{basename}_{dut.modname}"
         if cls.dut_mods:
-            if isinstance(dut, cls.dut_mods):
+            if not isinstance(dut, cls.dut_mods):
                 raise TypeError(f"{cls} can only test {cls.dut_mods} modules, but not {dut.__class__} module")
         super().__init__(parent=None, name=name, dut=dut, **kwargs)  # type: ignore[call-arg]
 
     @property
     def modname(self) -> str:
         """Module Name."""
-        modbasename = snakecase(self.__class__.__name__.removesuffix("Mod"))
+        modbasename = get_modname(self.__class__)
         return f"{modbasename}_{self.dut.modname}"
 
     @property
     def topmodname(self) -> str:
         """Top Module Name."""
-        return snakecase(self.__class__.__name__.removesuffix("Mod"))
+        return get_topmodname(self.__class__)
 
     @property
     def libname(self) -> str:
         """Library Name."""
-        return Path(getfile(self.__class__)).parts[-2]
+        return get_libname(self.__class__)
 
     @property
     def is_tb(self) -> bool:
         """Determine if module belongs to Testbench or Design."""
         return True
 
     @classmethod
@@ -155,17 +155,32 @@
         raise NotImplementedError
 
     @classmethod
     def search_duts(cls, mod) -> Iterator[BaseMod]:
         """
         Iterate over `topmod` and return modules which can be tested by this testbench.
         """
-        yield from ModPreIter(mod, filter_=lambda mod: isinstance(mod, cls.dut_mods))
+        yield from ModPreIter(mod, filter_=lambda mod: isinstance(mod, cls.dut_mods), unique=True)
 
-    def tests(self) -> Iterator[Test]:
+    @classmethod
+    def search_dut_topmodrefs(cls, mod) -> Iterator[TopModRef]:
+        """
+        Iterate over `topmod` and return `TopModRef` for modules which can be tested by this testbench.
+        """
+        tbref = cls.get_modref()
+        topref = mod.get_modref()
+        topqualname = mod.qualname
+        for dut in cls.search_duts(mod):
+            dutqualname = dut.qualname
+            if dutqualname != topqualname:
+                yield TopModRef(top=topref, sub=dutqualname, tb=tbref)
+            else:
+                yield TopModRef(top=topref, tb=tbref)
+
+    def get_tests(self) -> Iterator[Test]:
         """
         Yield Tests to be run on design.
         """
         yield from ()
 
     @abstractmethod
     def _build(self) -> None:
```

### Comparing `ucdp-0.3.0/src/ucdp/modtopref.py` & `ucdp-0.4.0/src/ucdp/modtopref.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,16 @@
             >>> import ucdp as u
             >>> u.TopModRef.cast('top_lib.top_mod')
             TopModRef(ModRef('top_lib', 'top_mod'))
             >>> u.TopModRef.cast('top_lib.top_mod-sub_lib.sub_mod')
             TopModRef(ModRef('top_lib', 'top_mod'), sub='sub_lib.sub_mod')
             >>> u.TopModRef.cast('mod_tb_lib.mod_tb#top_lib.top_mod')
             TopModRef(ModRef('top_lib', 'top_mod'), tb=ModRef('mod_tb_lib', 'mod_tb'))
+            >>> u.TopModRef.cast(TopModRef(ModRef('top_lib', 'top_mod')))
+            TopModRef(ModRef('top_lib', 'top_mod'))
 
             Invalid Pattern:
 
             >>> TopModRef.cast('lib.mod:c-ls.1')
             Traceback (most recent call last):
             ..
             ValueError: 'lib.mod:c-ls.1' does not match pattern '[tb_lib.tb#]top_lib.top[-sub_lib.sub]'
```

### Comparing `ucdp-0.3.0/src/ucdp/modutil.py` & `ucdp-0.4.0/src/ucdp/casting.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,38 +17,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""
-Module Utilities.
-
-"""
-
-from collections.abc import Iterator
-
-from .baseclassinfo import BaseClassInfo, get_baseclassinfos
 
 
-def get_modbaseinfos(cls_or_inst) -> Iterator[BaseClassInfo]:
-    """
-    Get Base Classes of `mod`.
-
-    Args:
-        cls_or_inst: Class or Instance
-    """
-    for baseclassinfo in get_baseclassinfos(cls_or_inst):
-        if baseclassinfo.libname == "ucdp":
-            break
-        yield baseclassinfo
-
+"""
+Casting.
+"""
 
-def is_tb_from_modname(modname: str) -> bool:
-    """
-    Determine if module is a testbench component by checking the name.
+from collections.abc import Iterable
 
-    Args:
-        modname: Module Name
-    """
-    return modname.endswith("_tb") or "_tb_" in modname
+Casting = Iterable[tuple[str, str]] | None
```

### Comparing `ucdp-0.3.0/src/ucdp/mux.py` & `ucdp-0.4.0/src/ucdp/mux.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Multiplexer."""
 
 from collections import defaultdict
 from collections.abc import Iterator
+from functools import cached_property
 
 from .assigns import Assign, Assigns, Drivers
 from .doc import Doc
 from .expr import Expr
 from .exprparser import ExprParser, Parseable
 from .ident import Ident, Idents
 from .object import Field, NamedObject, computed_field
@@ -54,20 +55,20 @@
     targets: Idents = Field(repr=False)
     namespace: Idents = Field(repr=False)
     drivers: Drivers = Field(repr=False, default_factory=dict)
     parser: ExprParser = Field(repr=False)
     doc: Doc = Doc()
 
     @computed_field(repr=False)
-    @property
+    @cached_property
     def __assigns(self) -> Assigns:
         return Assigns(targets=self.targets, sources=self.namespace, drivers=self.drivers)
 
     @computed_field(repr=False)
-    @property
+    @cached_property
     def __mux(self) -> dict[Expr, MuxBranch]:
         return defaultdict(dict)
 
     def set(self, sel: Parseable, cond: Parseable, out: Parseable, value: Parseable):
         """
         Set Multiplexer.
 
@@ -93,16 +94,16 @@
         condassigns.set(outexpr, valueexpr)
 
     def set_default(self, out: Parseable, value: Parseable):
         """
         Set Multiplexer.
 
         Args:
-            out (Expr): Output to be assigned
-            value (Expr): Value.
+            out: Output to be assigned
+            value: Value.
         """
         parse = self.parser.parse
         outexpr: BaseSignal = parse(out, only=BaseSignal)  # type: ignore[assignment]
         valueexpr = parse(value)
         self.__assigns.set_default(outexpr, valueexpr)
 
     def defaults(self) -> Iterator[Assign]:
```

### Comparing `ucdp-0.3.0/src/ucdp/namespace.py` & `ucdp-0.4.0/src/ucdp/namespace.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,59 +63,60 @@
         >>> namespace['d']
         Traceback (most recent call last):
         ...
         KeyError: 'd'
         >>> namespace.get_dym('d')
         Traceback (most recent call last):
         ...
-        ValueError: 'd' Known are 'a', 'b' and 'c'.
+        ValueError: 'd'. Known are 'a', 'b' and 'c'.
 
     Locking:
 
         >>> namespace.lock()
         >>> namespace.is_locked
         True
         >>> namespace['d'] = NamedObject('d', 7, 8)
         Traceback (most recent call last):
         ...
-        ValueError: Namespace is already locked
+        ucdp.exceptions.LockError: Namespace is already locked. Cannot add items anymore.
 
         >>> len(namespace)
         3
 """
 
 from collections.abc import Iterable
 from typing import Any
 
-from .exceptions import DuplicateError
+from .exceptions import DuplicateError, LockError
 from .nameutil import didyoumean
 from .object import NamedObject
 
 
 class Namespace(dict):
     """
     Namespace.
     """
 
     def __init__(self, items: Iterable[NamedObject] | None = None):
         super().__init__()
-        self.__locked = False
+        self.__is_locked = False
         if items:
             for item in items:
                 self[item.name] = item
 
     @property
     def is_locked(self) -> bool:
         """Locked."""
-        return self.__locked
+        return self.__is_locked
 
     def lock(self) -> None:
         """Lock."""
-        assert not self.__locked, f"{self} is already locked"
-        self.__locked = True
+        if self.__is_locked:
+            raise LockError("Namespace is already locked. Cannot lock again.")
+        self.__is_locked = True
 
     def add(self, item: NamedObject, exist_ok: bool = False):
         """Add."""
         try:
             self[item.name] = item
         except DuplicateError as exc:
             if not exist_ok:
@@ -123,23 +124,23 @@
 
     def get_dym(self, name: str) -> NamedObject:
         """Get NamedObject."""
         try:
             item = self[name]
         except KeyError as exc:
             dym = didyoumean(name, self.keys(), known=True)
-            raise ValueError(f"{exc!s}{dym}") from None
+            raise ValueError(f"{exc!s}.{dym}") from None
         return item
 
     def __setitem__(self, name, item):
         self._set_items(((name, item),))
 
     def _set_items(self, items: Iterable[tuple[str, NamedObject]]):
-        if self.__locked:
-            raise ValueError("Namespace is already locked")
+        if self.__is_locked:
+            raise LockError("Namespace is already locked. Cannot add items anymore.")
         for name, item in items:
             if item.name != name:
                 raise ValueError(f"{item} with must be stored at name '{item.name}' not at '{name}'")
             if item.name in self.keys():
                 if item is self[item.name]:
                     raise DuplicateError(f"{self[item.name]!r} already exists")
                 raise DuplicateError(f"Name '{item.name}' already taken by {self[item.name]!r}")
@@ -176,16 +177,16 @@
     def set_default(self, key, value=None) -> Any:
         """
         Set Default.
 
         If key is in the dictionary, return its value.
         If not, insert key with a value of default and return default. ``default`` defaults to None.
         """
-        if self.__locked:
-            raise ValueError("Namespace is already locked")
+        if self.__is_locked:
+            raise LockError("Namespace is already locked. Cannot add items anymore.")
         if key in self.keys():
             return self[key]
         self[key] = value
         return value
 
     def update(self, other: dict) -> None:  # type: ignore[override]
         """Update the dictionary with the key/value pairs from other."""
@@ -196,14 +197,14 @@
             return NotImplemented
         self._set_items(other.items())
         return self
 
     def __or__(self, other) -> "Namespace":
         if not isinstance(other, dict):
             return NotImplemented
-        if self.__locked:
-            raise ValueError("Namespace is already locked")
+        if self.__is_locked:
+            raise LockError("Namespace is already locked. Cannot add items anymore.")
         items = dict(self)
         items.update(other)
         namespace = Namespace()
         namespace._set_items(items.items())
         return namespace
```

### Comparing `ucdp-0.3.0/src/ucdp/nameutil.py` & `ucdp-0.4.0/src/ucdp/nameutil.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 from caseconverter import snakecase
 from fuzzywuzzy import process
 from humanfriendly.text import concatenate
 
 _FUZZY_MINRATIO: int = 80
 _RE_STARTNUM = re.compile(r"^[0-9]")
-_RE_SPLIT_PREFIX = re.compile(r"(?i)(?P<prefix>([a-z][a-z]?)_)(?P<basename>([a-z][a-z0-9_]*)?)\Z")
-_RE_SPLIT_SUFFIX = re.compile(r"(?i)(?P<basename>([a-z][a-z0-9_]*)?)(?P<suffix>_([a-z][a-z]?))\Z")
+_RE_SPLIT_PREFIX = re.compile(r"(?i)(?P<prefix>([a-z])_)(?P<basename>([a-z][a-z0-9_]*)?)\Z")
+_RE_SPLIT_SUFFIX = re.compile(r"(?i)(?P<basename>([a-z][a-z0-9_]*)?)(?P<suffix>_([a-z][o]?))\Z")
 
 
 @functools.lru_cache
 def split_prefix(name: str) -> tuple[str, str]:
     """
     Split Name Into Prefix and Basename.
 
@@ -55,16 +55,14 @@
 
             >>> split_prefix("i_count")
             ('i_', 'count')
             >>> split_prefix("u_count")
             ('u_', 'count')
             >>> split_prefix("I_VERY_LONG_NAME")
             ('I_', 'VERY_LONG_NAME')
-            >>> split_prefix("BT_VERY_LONG_NAME")
-            ('BT_', 'VERY_LONG_NAME')
             >>> split_prefix("")
             ('', '')
 
             The counterpart to this function is `join_names`.
     """
     mat = _RE_SPLIT_PREFIX.match(name)
     if mat:
```

### Comparing `ucdp-0.3.0/src/ucdp/note.py` & `ucdp-0.4.0/src/ucdp/note.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     note: str
 
     def __str__(self):
         return self.note
 
 
 OPEN = Note(note="OPEN")
-""" Open Note."""
+"""Open Note."""
 
 TODO = Note(note="TODO")
-""" Todo Note."""
+"""Todo Note."""
```

### Comparing `ucdp-0.3.0/src/ucdp/object.py` & `ucdp-0.4.0/src/ucdp/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             except KeyError:
                 global _CACHED_INSTANCES  # noqa: PLW0603
                 _CACHED_INSTANCES += 1
                 inst = self._cache[key] = super().__call__(*args, **kwargs)
         except TypeError as exc:
             try:
                 hash(self)
-            except TypeError:
+            except TypeError:  # pragma: no cover
                 raise TypeError(f"{self} is not constant.") from None
             # Determine what caused TypeError
             for idx, arg in enumerate(args):
                 try:
                     hash(arg)
                 except TypeError:  # noqa: PERF203
                     raise TypeError(f"{self}: {idx} argument {arg!r} is not constant.") from None
```

### Comparing `ucdp-0.3.0/src/ucdp/orientation.py` & `ucdp-0.4.0/src/ucdp/orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,19 @@
     _NAMEMAP: ClassVar[dict[int, str]] = {}
 
     mode: int
     """
     Integer representation.
     """
 
+    def __init__(self, mode):
+        if mode not in self._NAMEMAP:
+            raise ValueError(f"Invalid mode {mode}")
+        super().__init__(mode=mode)
+
     @property
     def name(self):
         """Name."""
         return self._NAMEMAP[self.mode]
 
     def __str__(self):
         return self._NAMEMAP[self.mode]
```

### Comparing `ucdp-0.3.0/src/ucdp/param.py` & `ucdp-0.4.0/src/ucdp/param.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,23 @@
         Param(ArrayType(UintType(16), 5), 'param_foo_data_p')
         Param(BitType(), 'param_foo_ack_p')
         Param(MType(), 'param_mode_p')
         Param(ArrayType(AType(), 3), 'param_bar_p')
         Param(ArrayType(BitType(), 3), 'param_bar_ack_p')
         Param(ArrayType(ArrayType(UintType(16), 5), 3), 'param_bar_data_p')
         Param(ArrayType(BitType(), 3), 'param_bar_req_p')
+
+    Value:
+
+        >>> for item in u.Param(u.UintType(6), "param_p").iter():
+        ...     print(repr(item))
+        Param(UintType(6), 'param_p')
+        >>> for item in u.Param(u.UintType(6), "param_p").iter(value=42):
+        ...     print(repr(item))
+        Param(UintType(6, default=42), 'param_p')
 """
 
 from collections.abc import Iterator
 from typing import Any
 
 from .ident import Ident, _iters
```

### Comparing `ucdp-0.3.0/src/ucdp/pathutil.py` & `ucdp-0.4.0/src/ucdp/pathutil.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/routepath.py` & `ucdp-0.4.0/src/ucdp/routepath.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/signal.py` & `ucdp-0.4.0/src/ucdp/signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         Port(ArrayType(AType(), 3), 'inp_bar_o', direction=OUT)
         Port(ArrayType(BitType(), 3), 'inp_bar_ack_i', direction=IN)
         Port(ArrayType(ArrayType(UintType(16), 5), 3), 'inp_bar_data_o', direction=OUT)
         Port(ArrayType(BitType(), 3), 'inp_bar_req_o', direction=OUT)
 
 """
 
+from .casting import Casting
 from .ident import Ident
 from .orientation import FWD, AOrientation, Direction
 from .typebase import BaseType
 
 
 class BaseSignal(Ident):
     """Base Class for All Signals ([Port][ucdp.signal.Port], [Signal][ucdp.signal.Signal]).
@@ -110,14 +111,18 @@
         doc: Documentation Container
         ifdef: IFDEF encapsulation
 
     """
 
     direction: AOrientation = FWD
 
+    def cast(self, other: Ident) -> Casting:
+        """Cast self=cast(other)."""
+        return self.type_.cast(other.type_)
+
 
 class Signal(BaseSignal):
     """
     Module Internal Signal.
 
     Args:
         type_: Type.
```

### Comparing `ucdp-0.3.0/src/ucdp/slices.py` & `ucdp-0.4.0/src/ucdp/slices.py`

 * *Files 22% similar despite different names*

```diff
@@ -119,37 +119,85 @@
     Traceback (most recent call last):
       ...
     ValueError: Invalid Slice Specification ''
     """
 
     left: Any
     right: Any
+    width: Any
 
-    def __init__(self, left: Any | None = None, right: Any | None = None) -> None:
+    def __init__(  # noqa: C901, PLR0912
+        self,
+        left: Any | None = None,
+        right: Any | None = None,
+        width: Any | None = None,
+        direction: SliceDirection | None = None,
+    ) -> None:
         if isinstance(left, str):
-            assert right is None, right
+            if right is not None:
+                raise ValueError("'right' must be None")
+            if width is not None:
+                raise ValueError("'width' must be None")
             mat = _RE_STRING.match(left)
             if mat:
                 left = int(mat.group("left"))
                 right = int(mat.group("right")) if mat.group("right") else None
             else:
                 raise ValueError(f"Invalid Slice Specification {left!r}") from None
-        if left is None:
+
+        # this is quite complex here - but left, right and width may be u.Expr and we want to have them minimal
+        if width is not None:
+            if left is None:
+                # 'width' given
+                if direction in (None, SliceDirection.DOWN):
+                    # downwards
+                    if right is None:
+                        right = 0
+                    if isinstance(width, int) and width == 1:
+                        left = right
+                    elif isinstance(right, int) and right == 0:
+                        left = width - 1
+                    else:
+                        left = width - 1 + right
+                elif right is None:
+                    left = 0
+                    right = width - 1
+                else:
+                    left = right - (width - 1)
+
+            elif right is None:
+                # left and width given
+                if direction in (None, SliceDirection.DOWN):
+                    # downwards
+                    right = left - (width - 1)
+                else:
+                    # upwards
+                    right = left + (width - 1)
+            else:
+                # 'left', 'right' and 'width' given
+                raise ValueError("'left', 'right' AND 'width' given, this is one too much")
+
+        elif left is None:
             left = right
+            width = 1
         elif right is None:
             right = left
-        super().__init__(left=left, right=right)  # type: ignore[call-arg]
+            width = 1
+        else:
+            width = self._calc_width(left, right)
+        _check_direction(left, right, direction)
+        super().__init__(left=left, right=right, width=width)  # type: ignore[call-arg]
 
-    @property
-    def width(self) -> int:
+    @staticmethod
+    def _calc_width(left: Any, right: Any) -> Any:
         """Slice Width."""
-        return abs(self.left - self.right) + 1
+        return abs(left - right) + 1
 
     @staticmethod
-    def cast(value, direction=None) -> "Slice":
+    def cast(value, direction: SliceDirection | None = None) -> "Slice":
         """
         Create :any:`Slice` from `value`.
 
         These three formats are supported:
 
         >>> Slice.cast("[15:4]")
         Slice('15:4')
@@ -176,15 +224,15 @@
           ...
         ValueError: Invalid Slice Specification None
         >>> Slice.cast("[4]", direction=DOWN)
         Slice('4')
         >>> Slice.cast("[4:15]", direction=DOWN)
         Traceback (most recent call last):
           ...
-        ValueError: Slice must be downwards but is 4:15
+        ValueError: Slice must be downwards but is upwards
         """
         slice_ = None
         if isinstance(value, Slice):
             slice_ = value
         elif isinstance(value, slice):
             slice_ = Slice(left=value.start, right=value.stop)
         elif isinstance(value, range):
@@ -193,19 +241,17 @@
         elif isinstance(value, int):
             slice_ = Slice(left=value)
         elif isinstance(value, str):
             mat = _RE_STRING.match(value)
             if mat:
                 left = int(mat.group("left"))
                 right = int(mat.group("right")) if mat.group("right") else None
-                slice_ = Slice(left=left, right=right)
+                slice_ = Slice(left=left, right=right, direction=direction)
         if slice_ is not None:
-            if direction:
-                if slice_.direction not in (None, direction):
-                    raise ValueError(f"Slice must be {direction.name.lower()}wards but is {slice_!s}")
+            _check_direction(slice_.left, slice_.right, direction)
             return slice_
         raise ValueError(f"Invalid Slice Specification {value!r}") from None
 
     @property
     def bits(self):
         """
         Colon separated bits.
@@ -244,30 +290,26 @@
         16
         >>> Slice(right=4).mask
         16
         """
         return ((2**self.width) - 1) << min(self.right, self.left)
 
     @property
-    def direction(self):
+    def direction(self) -> SliceDirection | None:
         """
         Direction.
 
         >>> Slice(left=4, right=8).direction
         <SliceDirection.UP: 1>
         >>> Slice(left=8, right=4).direction
         <SliceDirection.DOWN: 0>
         >>> Slice(left=4).direction
         >>> Slice(right=4).direction
         """
-        if self.left > self.right:
-            return SliceDirection.DOWN
-        if self.left < self.right:
-            return SliceDirection.UP
-        return None
+        return _get_direction(self.left, self.right)
 
     def extract(self, word):
         """
         Extract slice value from `word`.
 
         >>> slice = Slice(left=5, right=1)
         >>> slice.mask
@@ -294,7 +336,23 @@
         return NotImplemented
 
     def __iter__(self):
         if self.left > self.right:
             yield from range(self.left, self.right - 1, -1)
         else:
             yield from range(self.left, self.right + 1, 1)
+
+
+def _get_direction(left: Any, right: Any) -> SliceDirection | None:
+    if left > right:
+        return SliceDirection.DOWN
+    if left < right:
+        return SliceDirection.UP
+    return None
+
+
+def _check_direction(left: Any, right: Any, direction: SliceDirection | None):
+    slicedirection = _get_direction(left, right)
+    if direction and slicedirection and direction != slicedirection:
+        req = direction.name.lower()
+        act = slicedirection.name.lower()
+        raise ValueError(f"Slice must be {req}wards but is {act}wards")
```

### Comparing `ucdp-0.3.0/src/ucdp/test.py` & `ucdp-0.4.0/src/ucdp/test.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/top.py` & `ucdp-0.4.0/src/ucdp/top.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,36 +53,38 @@
             unique (bool): Just return module once and **NOT** all instances of it.
             post: Post-Order Iteration Strategy instead of Pre-Order Iteration Strategy.
         """
         if post:
             return ModPostIter(self.mod, filter_=filter_, stop=stop, maxlevel=maxlevel, unique=unique)
         return ModPreIter(self.mod, filter_=filter_, stop=stop, maxlevel=maxlevel, unique=unique)
 
-    def get_mods(self, namepats: Names | None = None, unique: bool = False):
+    def get_mods(self, namepats: Names | None = None, unique: bool = False, base: bool = False):
         """
         Return all modules matching `namepats`.
 
         Iterate top and all its submodules and return matching ones.
 
         Keyword Args:
             namepats: Iterable with name pattern (including `*` and `?`) or comma separated string
             unique (bool): Just return every module once.
+            base: namepats must match against module `basequalnames` instead of `qual_name`.
         """
-        return get_mods(self.mod, namepats=namepats, unique=unique)
+        return get_mods(self.mod, namepats=namepats, unique=unique, base=base)
 
-    def get_mod(self, namepats: Names):
+    def get_mod(self, namepats: Names, base: bool = False):
         """
         Return the one and just the one hardware module matching `namepats`.
 
         Iterate over `mod` and all its submodules and return matching one.
 
         Keyword Args:
             namepats: Iterable with name pattern (including `*` and `?`) or comma separated string
+            base: namepats must match against module `basequalnames` instead of `qual_name`.
         """
-        return get_mod(self.mod, namepats)
+        return get_mod(self.mod, namepats, base=base)
 
     def get_stat(self) -> dict[str, int]:
         """Get Statistics."""
         return {
             "Modules": len(self.get_mods(unique=True)),
             "Module-Instances": len(self.get_mods()),
             "LightObjects": _CACHED_INSTANCES,
```

### Comparing `ucdp-0.3.0/src/ucdp/typearray.py` & `ucdp-0.4.0/src/ucdp/typearray.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def __init__(self, itemtype: BaseType, depth: Any, left=0):
         super().__init__(itemtype=itemtype, depth=depth, left=left)  # type: ignore[call-arg]
 
     @property
     def slice_(self):
         """Get Slice of Matrix."""
-        return Slice(left=self.left, right=self.depth - 1)
+        return Slice(left=self.left, width=self.depth, direction=UP)
 
     def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`ArrayType` of the same depth and type.
```

### Comparing `ucdp-0.3.0/src/ucdp/typebase.py` & `ucdp-0.4.0/src/ucdp/typebase.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 """
 
 from abc import abstractmethod
 from typing import Any
 
 from pydantic import model_validator
 
+from .casting import Casting
 from .doc import Doc
 from .object import Light, Object
 from .slices import DOWN, Slice
 
 
 class BaseType(Object):
     """
@@ -61,21 +62,21 @@
         """
         Check For Valid Connection To `other`.
 
         This method has to be overwritten.
         """
         raise NotImplementedError
 
-    def cast(self, other: "BaseType"):
+    def cast(self, other: "BaseType") -> Casting:
         """
         How to cast an input of type `self` from a value of type `other`.
 
         `self = cast(other)`
         """
-        return NotImplemented
+        return None
 
     @property
     def bits(self):
         """
         Size in Bits.
 
         This method has to be overwritten.
@@ -183,16 +184,12 @@
 
     def __init__(self, width, **kwargs):
         super().__init__(width=width, **kwargs)
 
     @property
     def slice_(self):
         """Slice."""
-        right = self.right
-        # Ensure slim expressions
-        if isinstance(right, int) and right == 0:
-            return Slice(left=self.width - 1, right=0)
-        return Slice(left=right + self.width - 1, right=right)
+        return Slice(width=self.width, right=self.right)
 
 
 class ACompositeType(BaseType):
     """Base Class For All Composite Types."""
```

### Comparing `ucdp-0.3.0/src/ucdp/typeclkrst.py` & `ucdp-0.4.0/src/ucdp/typeclkrst.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/src/ucdp/typedescriptivestruct.py` & `ucdp-0.4.0/src/ucdp/typedescriptivestruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,9 +172,9 @@
             bwd += ibwd
             bid += ibid
         elif iorientation == FWD:
             fwd += itype_.bits
         elif iorientation == BWD:
             bwd += itype_.bits
         else:
-            bid += itype_.bits
+            raise AssertionError
     return fwd, bwd, bid
```

### Comparing `ucdp-0.3.0/src/ucdp/typeenum.py` & `ucdp-0.4.0/src/ucdp/typeenum.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,213 +30,20 @@
 * :any:`AEnumType` - Standard Enumeration
 * :any:`AGlobalEnumType` - A public enumeration which fills up through all instances.
 * :any:`DynamicEnumType` - A public enumeration which fills up per instance.
 * :any:`EnaType` - Native single bit with `ena` and `dis` enumeration, active-high
 * :any:`DisType` - Native single bit with `ena` and `dis` enumeration, low-high
 """
 
-from abc import abstractmethod
-from collections.abc import Callable
 from typing import Any
 
-from humanfriendly.text import concatenate
-from pydantic import model_validator
-
-from .consts import AUTO
-from .dict import Dict
-from .doc import Doc
-from .exceptions import LockError
-from .object import Field, Light, Object, PrivateField
-from .typebase import BaseScalarType
-from .typescalar import AScalarType, BitType, IntegerType
-
-
-class EnumItem(Object):
-    """
-    Enumeration NamedObject.
-
-    Args:
-        key (int): key value to be mapped.
-        value: Mapped value.
-
-    Keyword Args:
-        doc (Doc): Documentation Container
-
-    Enumeration items are typically created by :any:`EnumType._add`.
-    """
-
-    key: int
-    value: Any
-    doc: Doc = Doc()
-
-    _posargs: tuple[str, ...] = ("key", "value")
-
-    def __init__(self, key, value, **kwargs):
-        super().__init__(key=key, value=value, **kwargs)
-
-
-ItemFilter = Callable[[EnumItem], bool]
-
-
-class BaseEnumType(BaseScalarType, Dict):
-    """Base Type for all Enums."""
-
-    keytype: AScalarType = IntegerType()
-    valuetype: Any = None
-    default: Any = None
-    filter_: ItemFilter | None = Field(default=None, repr=False)
-    _locked: bool = PrivateField(default=False)
-
-    def _add(self, key, value, title: str | None = None, descr: str | None = None, comment: str | None = None) -> None:
-        """
-        Add NamedObject To Enumeration.
-
-        Args:
-            key (int): key value to be mapped.
-            value: Mapped value.
-
-        Keyword Args:
-            title (str): Full Spoken Name.
-            descr (str): Documentation Description.
-            comment (str): Source Code Comment.
-
-        :meta public:
-        """
-        if self._locked:
-            raise LockError(self)
-        items = self._items
-        if key is AUTO:
-            keys = items.keys()
-            key = max(keys) + 1 if keys else 0
-        self.keytype.check(key)
-        valuetype = self.valuetype
-        if valuetype:
-            valuetype.check(value)
-        if key in items.keys():
-            raise ValueError(f"key {key!r} already exists in {self}")
-        doc = Doc(title=title, descr=descr, comment=comment)
-        enumitem = EnumItem(key, value, doc=doc)
-        if not self.filter_ or self.filter_(enumitem):
-            items[key] = enumitem
-
-    @property
-    def width(self):
-        """Width in Bits."""
-        return self.keytype.width
-
-    def check(self, value, what="Value"):
-        """Check `value`."""
-        return self.keytype.check(value, what)
-
-    def encode(self, value, usedefault=False):
-        """Encode Value."""
-        if usedefault:
-            try:
-                return self.get_byvalue(value).key
-            except ValueError:
-                return self.default
-        return self.get_byvalue(value).key
-
-    def decode(self, value, usedefault=False):
-        """Decode Value."""
-        if usedefault:
-            try:
-                return self.get_bykey(value).value
-            except ValueError:
-                return self.get_bykey(self.default).value
-        else:
-            return self.get_bykey(value).value
-
-    @property
-    def is_full(self) -> bool:
-        """Return `True` if Enumeration Is Fully Encoded."""
-        return len(self) == (2 ** int(self.width))
-
-    def get_bykey(self, key) -> EnumItem:
-        """Return :any:`EnumItem` with key `key`."""
-        item = self.get(key)
-        if item is not None:
-            return item
-        keys = concatenate([repr(item) for item in self.keys()])
-        raise ValueError(f"{self} does not contain key {key!r}. Known keys are {keys}.")
-
-    def get_byvalue(self, value) -> EnumItem:
-        """Return :any:`EnumItem` with value `value`."""
-        for item in self.values():
-            if item.value == value:
-                return item
-        values = concatenate([repr(item.value) for item in self.values()])
-        raise ValueError(f"{self} does not contain value {value!r}. Known values are {values}.")
-
-    def get_value(self, key):
-        """Return `value` for `key`."""
-        return self.get_bykey(key).value
-
-    def get_key(self, value):
-        """Return `key` for `value`."""
-        return self.get_byvalue(value).key
-
-    def get_hex(self, value=None):
-        """Get Hex Value."""
-        if value is None:
-            value = self.default
-        return self.keytype.get_hex(value=value)
-
-    def is_connectable(self, other):
-        """Check For Valid Connection To `other`."""
-        return (
-            isinstance(other, BaseEnumType)
-            and self.keytype.is_connectable(other.keytype)
-            and self.valuetype == other.valuetype
-            and len(self) == len(other)
-            and self.keys() == other.keys()
-            and all(
-                selfitem.value == otheritem.value
-                for selfitem, otheritem in zip(self.values(), other.values(), strict=False)
-            )
-        ) or (self.keytype.is_connectable(other))
-
-    def __getitem__(self, slice_):
-        """Return Slice."""
-        return self.keytype[slice_]
-
-    @property
-    def min_(self):
-        """Minimal Value."""
-        return self.keytype.min_
-
-    @property
-    def max_(self):
-        """Maximal Value."""
-        return self.keytype.max_
-
-    @property
-    def bits(self):
-        """Size in Bits."""
-        return self.keytype.bits
-
-    # def cast(self, other):
-    #     """
-    #     How to cast an input of type `self` from a value of type `other`.
-
-    #     `self = cast(other)`
-    #     """
-    #     if isinstance(other, BaseEnumType) and self.keytype.is_connectable(other.keytype):
-    #         yield "", ""
-    #     return NotImplemented
-
-    @model_validator(mode="after")
-    def __post_init(self) -> "BaseEnumType":
-        if self.default is None:
-            self.__dict__["default"] = self.keytype.default
-        return self
-
-    @abstractmethod
-    def _build(self) -> None:
-        """Build Type."""
+from .object import Light
+from .typebase import AScalarType
+from .typebaseenum import BaseEnumType
+from .typescalar import BitType, IntegerType
 
 
 class AEnumType(BaseEnumType, Light):
     """
     Base class for all enumerations, behaves like a dictionary.
 
     Keyword Args:
@@ -492,15 +299,15 @@
     >>> MyType().new(filter_=lambda item: item.value != "cyclic")
     MyType()
     """
 
     def model_post_init(self, __context: Any) -> None:
         """Run Build."""
         self._build()
-        self._locked = True
+        self._is_locked = True
 
 
 class AGlobalEnumType(BaseEnumType, Light):
     """
     A singleton enumeration which can be filled outside `_build` and is **shared** between instances.
 
     >>> import ucdp as u
@@ -526,17 +333,19 @@
     ...     keytype: u.AScalarType = u.UintType(3)
     ...     def _build(self) -> None:
     ...         pass
     >>> ctrl = CtrlType()
     >>> ctrl._add(0, 'zero')
     Traceback (most recent call last):
       ...
-    ucdp.exceptions.LockError: CtrlType() is already locked for modification.
+    ucdp.exceptions.LockError: CtrlType(): Cannot add item 0='zero'.
     """
 
+    keytype: AScalarType = IntegerType()
+
     def add(self, key, value, title: str | None = None, descr: str | None = None, comment: str | None = None) -> None:
         """
         Add NamedObject To Enumeration.
 
         Args:
             key (int): key value to be mapped.
             value: Mapped value.
@@ -582,17 +391,19 @@
     ...     keytype: u.AScalarType = u.UintType(3)
     ...     def _build(self) -> None:
     ...         pass
     >>> ctrl = CtrlType()
     >>> ctrl._add(0, 'zero')
     Traceback (most recent call last):
       ...
-    ucdp.exceptions.LockError: CtrlType() is already locked for modification.
+    ucdp.exceptions.LockError: CtrlType(): Cannot add item 0='zero'.
     """
 
+    keytype: AScalarType = IntegerType()
+
     def add(self, key, value, title: str | None = None, descr: str | None = None, comment: str | None = None) -> None:
         """
         Add NamedObject To Enumeration.
 
         Args:
             key (int): key value to be mapped.
             value: Mapped value.
@@ -637,15 +448,15 @@
     title: str = "Enable"
 
     def _build(self) -> None:
         self._add(0, "dis", "disabled")
         self._add(1, "ena", "enabled")
 
     # def is_connectable(self, other):
-    #     """Return True if connectable to `other`."""
+    #    """Return True if connectable to `other`."""
     #     return (isinstance(other, BitType) and self.default == other.default) or super().is_connectable(other)
 
 
 class DisType(AEnumType):
     """
     Enable (positive logic).
```

### Comparing `ucdp-0.3.0/src/ucdp/typescalar.py` & `ucdp-0.4.0/src/ucdp/typescalar.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,16 +33,18 @@
 * :any:`SintType`
 """
 
 from typing import Any, ClassVar
 
 from humannum import hex_
 
+from .casting import Casting
 from .slices import DOWN, Slice
-from .typebase import AScalarType, AVecType
+from .typebase import AScalarType, AVecType, BaseType
+from .typebaseenum import BaseEnumType
 
 INTEGER_WIDTH: int = 32
 
 
 class IntegerType(AScalarType):
     """
     Native Signed 32-Bit Integer.
@@ -291,14 +293,28 @@
         A connection to an :any:`UintType()` of width is forbidden (requires a cast).
 
         >>> BitType().is_connectable(UintType(2))
         False
         """
         return isinstance(other, (BitType, UintType)) and int(other.width) == 1  # type: ignore[operator]
 
+    def cast(self, other: BaseType) -> Casting:
+        """
+        How to cast an input of type `self` from a value of type `other`.
+
+        `self = cast(other)`
+        """
+        if isinstance(other, (UintType, BitType, SintType, IntegerType)) and self.width == other.width:  # type: ignore[operator]
+            return [("", "")]
+
+        if isinstance(other, BaseEnumType) and self.width == other.keytype.width:  # type: ignore[operator]
+            return [("", "")]
+
+        return None
+
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == 1 and slice_.right == 0:
             return self
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
 
 
@@ -337,15 +353,15 @@
     BoolType(default=True)
     >>> u.BoolType()[32:31]
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 32:31 from BoolType()
     """
 
-    default: bool = False
+    default: Any = False
     width: ClassVar[int] = 1  # type: ignore[misc]
 
     @staticmethod
     def check(value, what="Value") -> bool:
         """
         Check `value` for type.
 
@@ -366,17 +382,18 @@
           ...
         ValueError: Value 2 is not a boolean
         >>> example.check(False)
         0
         >>> example.check(True)
         1
         """
-        if value not in (False, True):
-            raise ValueError(f"{what} {value} is not a boolean")
-        return value
+        # Note: we need identity check here
+        if int(value) in (0, 1):
+            return value
+        raise ValueError(f"{what} {value} is not a boolean")
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
         >>> import ucdp as u
         >>> u.BoolType().get_hex()
@@ -524,23 +541,27 @@
         A connection to an :any:`BitType()` is forbidden (requires a cast).
 
         >>> RailType().is_connectable(BitType())
         False
         """
         return isinstance(other, RailType)
 
-    # def cast(self, other):
-    #     """
-    #     How to cast an input of type `self` from a value of type `other`.
-
-    #     `self = cast(other)`
-    #     """
-    #     if isinstance(other, (BitType, UintType)) and other.width == 1:
-    #         yield "", ""
-    #     return NotImplemented
+    def cast(self, other: BaseType) -> Casting:
+        """
+        How to cast an input of type `self` from a value of type `other`.
+
+        `self = cast(other)`
+        """
+        if isinstance(other, (BitType, UintType)) and other.width == 1:  # type: ignore[operator]
+            return [("", "")]
+
+        if isinstance(other, BaseEnumType) and self.width == other.keytype.width:  # type: ignore[operator]
+            return [("", "")]
+
+        return None
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == 1 and slice_.right == 0:
             return self
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
 
@@ -666,23 +687,27 @@
         >>> UintType(1).is_connectable(BitType())
         True
         >>> UintType(1).is_connectable(SintType(1))
         False
         """
         return isinstance(other, (UintType, BitType)) and self.width == other.width  # type: ignore[operator]
 
-    # def cast(self, other):
-    #     """
-    #     How to cast an input of type `self` from a value of type `other`.
-
-    #     `self = cast(other)`
-    #     """
-    #     if isinstance(other, (SintType, IntegerType)) and self.width == other.width:
-    #         yield "", ""
-    #     return NotImplemented
+    def cast(self, other: BaseType) -> Casting:
+        """
+        How to cast an input of type `self` from a value of type `other`.
+
+        `self = cast(other)`
+        """
+        if isinstance(other, (SintType, IntegerType)) and self.width == other.width:  # type: ignore[operator]
+            return [("", "")]
+
+        if isinstance(other, BaseEnumType) and self.width == other.keytype.width:
+            return [("", "")]
+
+        return None
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == self.width and slice_.right == self.right:
             return self
         if slice_ in self.slice_:
             return UintType(slice_.width, default=slice_.extract(self.default))
@@ -817,23 +842,27 @@
         >>> SintType(1).is_connectable(BitType())
         False
         >>> SintType(1).is_connectable(UintType(1))
         False
         """
         return isinstance(other, (SintType, IntegerType)) and self.width == other.width  # type: ignore[operator]
 
-    # def cast(self, other):
-    #     """
-    #     How to cast an input of type `self` from a value of type `other`.
-
-    #     `self = cast(other)`
-    #     """
-    #     if isinstance(other, (UintType, BitType)) and self.width == other.width:
-    #         yield "", ""
-    #     return NotImplemented
+    def cast(self, other: BaseType) -> Casting:
+        """
+        How to cast an input of type `self` from a value of type `other`.
+
+        `self = cast(other)`
+        """
+        if isinstance(other, (UintType, BitType)) and self.width == other.width:  # type: ignore[operator]
+            return [("", "")]
+
+        if isinstance(other, BaseEnumType) and self.width == other.keytype.width:
+            return [("", "")]
+
+        return None
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == self.width and slice_.right == self.right:
             return self
         if slice_ in self.slice_:
             if slice_.left == self.slice_.left:
```

### Comparing `ucdp-0.3.0/src/ucdp/typestring.py` & `ucdp-0.4.0/src/ucdp/typestring.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     Native String.
 
     Example:
     >>> import ucdp as u
     >>> example = u.StringType()
     >>> example
     StringType()
+    >>> example = u.StringType(default='data')
+    >>> example
+    StringType(default='data')
+    >>> example[1:3]
+    StringType(default='at')
     """
 
     default: str = ""
 
     def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
@@ -59,8 +64,8 @@
         """
         return isinstance(other, StringType)
 
     def __getitem__(self, slice_):
         """
         Return Sliced Variant.
         """
-        return self.default[slice_]
+        return StringType(default=self.default[slice_])
```

### Comparing `ucdp-0.3.0/src/ucdp/typestruct.py` & `ucdp-0.4.0/src/ucdp/typestruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 
 class BaseStructType(Dict, ACompositeType):
     """Base Type for all Structs."""
 
     filter_: StructFilter | None = None
     _items: dict[Any, Any] = PrivateField(default_factory=dict)
-    _locked: bool = PrivateField(default=False)
+    _is_locked: bool = PrivateField(default=False)
 
     def _add(
         self,
         name: str,
         type_: BaseType,
         orientation: Orientation = FWD,
         title: str | None = None,
@@ -120,16 +120,16 @@
             title: Full Spoken Name.
             descr: Documentation Description.
             comment: Source Code Comment.
             ifdef: IFDEF encapsulation.
 
         :meta public:
         """
-        if self._locked:
-            raise LockError(self)
+        if self._is_locked:
+            raise LockError(f"{self}: Cannot add item {name!r}.")
         items = self._items
         if name not in items.keys():
             doc = doc_from_type(type_, title=title, descr=descr, comment=comment)
             structitem = StructItem(name, type_, orientation=orientation, doc=doc, ifdef=ifdef)
             if not self.filter_ or self.filter_(structitem):
                 items[name] = structitem
         else:
@@ -246,15 +246,15 @@
     StructItem('data', UintType(8))
     StructItem('valid', BitType())
     """
 
     def model_post_init(self, __context: Any) -> None:
         """Run Build."""
         self._build()
-        self._locked = True
+        self._is_locked = True
 
 
 class AGlobalStructType(BaseStructType, Light):
     """
     A singleton struct which can be filled outside `_build` and is **shared** between instances.
 
     >>> import ucdp as u
@@ -273,15 +273,15 @@
     >>> class BusType(u.AStructType):
     ...     def _build(self) -> None:
     ...         pass
     >>> bus = BusType()
     >>> bus._add('data', u.UintType(8))
     Traceback (most recent call last):
       ...
-    ucdp.exceptions.LockError: BusType() is already locked for modification.
+    ucdp.exceptions.LockError: BusType(): Cannot add item 'data'.
     """
 
     def add(
         self,
         name: str,
         type_: BaseType,
         orientation: Orientation = FWD,
@@ -346,15 +346,15 @@
     >>> class BusType(u.AStructType):
     ...     def _build(self) -> None:
     ...         pass
     >>> bus = BusType()
     >>> bus._add('data', u.UintType(8))
     Traceback (most recent call last):
       ...
-    ucdp.exceptions.LockError: BusType() is already locked for modification.
+    ucdp.exceptions.LockError: BusType(): Cannot add item 'data'.
     """
 
     def add(
         self,
         name: str,
         type_: BaseType,
         orientation: Orientation = FWD,
```

### Comparing `ucdp-0.3.0/src/ucdp/util.py` & `ucdp-0.4.0/src/ucdp/util.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/conftest.py` & `ucdp-0.4.0/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Pytest Configuration and Fixtures."""
 
+import os
 from pathlib import Path
+from unittest import mock
 
 import ucdp as u
 from pytest import fixture
 
 EXAMPLES_PATH = Path(u.__file__).parent / "examples"
 
 
@@ -34,7 +36,14 @@
 
 @fixture
 def example_param():
     """Add access to ``examples/param``."""
     example_path = EXAMPLES_PATH / "param"
     with u.extend_sys_path((example_path,)):
         yield example_path
+
+
+@fixture
+def prjroot(tmp_path):
+    """Project Environment."""
+    with mock.patch.dict(os.environ, {"PRJROOT": str(tmp_path)}):
+        yield tmp_path
```

### Comparing `ucdp-0.3.0/tests/test_baseclassinfo.py` & `ucdp-0.4.0/tests/test_baseclassinfo.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_buildproduct.py` & `ucdp-0.4.0/tests/test_buildproduct.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_config.py` & `ucdp-0.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_examples.py` & `ucdp-0.4.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_fileset.py` & `ucdp-0.4.0/tests/test_fileset.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,30 +19,33 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Test Module File Information."""
 
+from pathlib import Path
+
 import ucdp as u
 
 
 def test_basic(example_simple):
     """Basic Testing."""
     from uart_lib.uart import UartMod
 
     mod = UartMod()
 
     info = u.FileSet.from_mod(mod, "hdl")
+    prjroot = Path("$PRJROOT")
     assert info.target is None
     assert info.filepaths == (
-        u.LibPath(libname="glbl_lib", path=example_simple / "src" / "glbl_lib" / "clk_gate" / "rtl" / "clk_gate.sv"),
-        u.LibPath(libname="uart_lib", path=example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart_regf.sv"),
-        u.LibPath(libname="uart_lib", path=example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart_core.sv"),
-        u.LibPath(libname="uart_lib", path=example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart.sv"),
+        u.LibPath(libname="glbl_lib", path=prjroot / "glbl_lib" / "clk_gate" / "rtl" / "clk_gate.sv"),
+        u.LibPath(libname="uart_lib", path=prjroot / "uart_lib" / "uart" / "rtl" / "uart_regf.sv"),
+        u.LibPath(libname="uart_lib", path=prjroot / "uart_lib" / "uart" / "rtl" / "uart_core.sv"),
+        u.LibPath(libname="uart_lib", path=prjroot / "uart_lib" / "uart" / "rtl" / "uart.sv"),
     )
     assert info.inc_dirs == ()
 
     info = u.FileSet.from_mod(mod, "systemc")
     assert info.target is None
     assert info.filepaths == ()
     assert info.inc_dirs == ()
```

### Comparing `ucdp-0.3.0/tests/test_flipflop.py` & `ucdp-0.4.0/tests/test_flipflop.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_light_object.py` & `ucdp-0.4.0/tests/test_light_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Test :any:`LightObject`."""
 
+import re
+
 import ucdp as u
 from hypothesis import assume, given
 from hypothesis import strategies as st
 from pydantic import ValidationError
 from pytest import raises
 
 
@@ -158,7 +160,27 @@
 
 
 def test_not_hashable_kwarg():
     """Test Error Message on Non-Hashable Kwarg."""
     # TESTME
 
     #    NotHashableKwarg(["a", "b"])
+
+
+class NoHashLightObject(u.LightObject):
+    """Example LightObject."""
+
+    arg1: list[int]
+
+    def __init__(self, arg1):
+        super().__init__(arg1=arg1)
+
+
+def test_no_hash():
+    """Not Hashable."""
+    msg = "<class 'tests.test_light_object.NoHashLightObject'>: 0 argument [1, 2, 3] is not constant."
+    with raises(TypeError, match=re.escape(msg)):
+        NoHashLightObject([1, 2, 3])
+
+    msg = "<class 'tests.test_light_object.NoHashLightObject'>: 'arg1' argument [1, 2, 3] is not constant."
+    with raises(TypeError, match=re.escape(msg)):
+        NoHashLightObject(arg1=[1, 2, 3])
```

### Comparing `ucdp-0.3.0/tests/test_loader.py` & `ucdp-0.4.0/tests/test_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Test Loader and Top."""
 
+import re
+
 import ucdp as u
 from pytest import raises
 
 
 def test_load_simple(example_simple):
     """Simple Module."""
     top = u.load("glbl_lib.clk_gate")
@@ -90,14 +92,44 @@
         "<uart_lib.uart.UartCoreMod(inst='uart/u_core', libname='uart_lib', modname='uart_core')>",
         "<uart_lib.uart.UartMod(inst='uart', libname='uart_lib', modname='uart')>",
     ]
     assert (
         repr(top.get_mod("glbl_lib.clk_gate"))
         == "<glbl_lib.clk_gate.ClkGateMod(inst='uart/u_clk_gate', libname='glbl_lib', modname='clk_gate')>"
     )
+    assert [repr(mod) for mod in top.get_mods("glbl_lib.clk_gate")] == [
+        "<glbl_lib.clk_gate.ClkGateMod(inst='uart/u_clk_gate', libname='glbl_lib', modname='clk_gate')>",
+        "<glbl_lib.clk_gate.ClkGateMod(inst='uart/u_regf/u_clk_gate', libname='glbl_lib', modname='clk_gate')>",
+    ]
+    assert [repr(mod) for mod in top.get_mods("glbl_lib.regf")] == []
+    assert [repr(mod) for mod in top.get_mods("glbl_lib.regf", base=True)] == [
+        "<glbl_lib.regf.RegfMod(inst='uart/u_regf', libname='uart_lib', modname='uart_regf')>",
+    ]
+
+    msg = (
+        "'glbl_lib.regf' not found. Known are:\n  glbl_lib.clk_gate\n  uart_lib.uart\n  "
+        "uart_lib.uart_core\n  uart_lib.uart_regf"
+    )
+    with raises(ValueError, match=re.escape(msg)):
+        top.get_mod("glbl_lib.regf")
+
+    assert (
+        repr(top.get_mod("glbl_lib.regf", base=True))
+        == "<glbl_lib.regf.RegfMod(inst='uart/u_regf', libname='uart_lib', modname='uart_regf')>"
+    )
+
+    msg = (
+        "Found multiple hardware modules for 'uart_lib.*':\n  uart_lib.uart\n  uart_lib.uart_core\n  uart_lib.uart_regf"
+    )
+    with raises(ValueError, match=re.escape(msg)):
+        top.get_mod("uart_lib.*")
+
+    msg = "'glbl_lib.foo' not found. Known are:\n  glbl_lib.clk_gate\n  glbl_lib.regf\n  uart_lib.uart"
+    with raises(ValueError, match=re.escape(msg)):
+        top.get_mod("glbl_lib.foo", base=True)
 
 
 def test_load_complex_sub(example_simple):
     """Complexer Module with Sub module."""
     top = u.load("uart_lib.uart-glbl_lib.clk_gate")
     assert top.ref == u.TopModRef(u.ModRef("uart_lib", "uart"), sub="glbl_lib.clk_gate")
     assert (
```

### Comparing `ucdp-0.3.0/tests/test_modfilelist.py` & `ucdp-0.4.0/tests/test_modfilelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,27 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Test Module File Information."""
 
+from pathlib import Path
+
 import ucdp as u
 
 
 def test_basic(example_simple):
     """Basic Testing."""
     from fileliststandard import HdlFileList
     from uart_lib.uart import UartMod
 
     mod = UartMod()
-
-    filepath = example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart.sv"
+    prjroot = Path("$PRJROOT")
+    filepath = prjroot / "uart_lib" / "uart" / "rtl" / "uart.sv"
     modfilelist = u.resolve_modfilelist(mod, "hdl")
     assert modfilelist == HdlFileList(
         gen="full",
         filepaths=(filepath,),
         template_filepaths=(example_simple / "uart_lib" / "main.mako",),
     )
```

### Comparing `ucdp-0.3.0/tests/test_mux.py` & `ucdp-0.4.0/src/ucdp/_castingnamespace.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,18 +17,37 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""Test Multiplexer."""
 
+"""
+Casting Namespace.
 
-# TESTME
-# * use fixture for mux instance with reasonable namespace and parser
-# * test different sel and sel types (param, const, signal, port, expr, concat)
-# * test different cond and cond types (param, const, signal, port, range, expr)
-# * test different out and out types (param, const, signal, port, expr, slicing)
-# * test different value and value types (param, const, signal, port, expr, slicing)
-# * test default value handling
-# * test sels
+
+"""
+
+from .ident import Ident
+from .nameutil import join_names
+from .object import Object
+
+
+class CastingNamespace(Object):
+    """Namespace Helper for Type Casting."""
+
+    source: Ident
+
+    def __getitem__(self, key):
+        source = self.source
+        for subsource in source.iter():
+            if join_names(source.basename, key) == subsource.basename:
+                return subsource
+        raise KeyError(key)
+
+    def get_dym(self, name: str) -> Ident:
+        try:
+            item = self[name]
+        except KeyError as exc:
+            raise ValueError(f"{exc!s}.") from None
+        return item
```

### Comparing `ucdp-0.3.0/tests/test_namespace.py` & `ucdp-0.4.0/tests/test_namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Test Configuration."""
 
 # from collections import namedtuple
 
+import re
+
 import ucdp
 from hypothesis import assume, given
 from hypothesis import strategies as st
 from pytest import raises
 
 
 class MyObject(ucdp.NamedObject):
@@ -193,15 +195,15 @@
     assert namespace.get_dym(myobject1.name) == myobject1
     assert namespace.get_dym(myobject2.name) == myobject2
     with raises(ValueError) as excep:
         namespace.get_dym(str3)
 
     tmp_dict = {myobject1.name: myobject1, myobject2.name: myobject2}
     dym = ucdp.nameutil.didyoumean(str3, tmp_dict.keys(), known=True)
-    assert str(excep.value) == f"{str3!r}{dym}"
+    assert str(excep.value) == f"{str3!r}.{dym}"
 
 
 @given(
     int1=st.integers(),
     int2=st.integers(),
     int3=st.integers(),
     int4=st.integers(),
@@ -353,23 +355,27 @@
 
     # Add new Object
     namespace.add(myobject1)
     assert len(namespace) == 1
     assert namespace.is_locked is False
     namespace.lock()
     assert namespace.is_locked is True
-    with raises(AssertionError) as excep:
+
+    msg = "Namespace is already locked. Cannot lock again."
+    with raises(ucdp.LockError, match=re.escape(msg)):
         namespace.lock()
-    assert str(excep.value) == f"{namespace!r} is already locked"
-    with raises(ValueError) as excep:
+
+    msg = "Namespace is already locked. Cannot add items anymore."
+    with raises(ucdp.LockError, match=re.escape(msg)):
         namespace.add(myobject2)
-    assert str(excep.value) == "Namespace is already locked"
-    with raises(ValueError) as excep:
+
+    msg = "Namespace is already locked. Cannot add items anymore."
+    with raises(ucdp.LockError, match=re.escape(msg)):
         namespace.update({myobject2.name: myobject2})
-    assert str(excep.value) == "Namespace is already locked"
+
     assert len(namespace) == 1
 
 
 def test_ior():
     """Namespace IOR-Operator."""
     myobject1 = ucdp.NamedObject(name="str1")
     myobject2 = ucdp.NamedObject(name="str2")
@@ -380,17 +386,17 @@
 
     namespace |= {"str2": myobject2}
     assert tuple(namespace) == (myobject1, myobject2)
 
     namespace.lock()
     assert tuple(namespace) == (myobject1, myobject2)
 
-    with raises(ValueError) as excep:
+    msg = "Namespace is already locked. Cannot add items anymore."
+    with raises(ucdp.LockError, match=re.escape(msg)):
         namespace |= {"str3": myobject3}
-    assert str(excep.value) == "Namespace is already locked"
 
     assert tuple(namespace) == (myobject1, myobject2)
 
 
 def test_or():
     """Namespace IOR-Operator."""
     myobject1 = ucdp.NamedObject(name="str1")
@@ -403,12 +409,38 @@
     namespace2 = namespace | {"str2": myobject2}
     assert tuple(namespace) == (myobject1,)
     assert tuple(namespace2) == (myobject1, myobject2)
 
     namespace2.lock()
     assert tuple(namespace2) == (myobject1, myobject2)
 
-    with raises(ValueError) as excep:
+    msg = "Namespace is already locked. Cannot add items anymore."
+    with raises(ucdp.LockError, match=re.escape(msg)):
         namespace2 | {"str3": myobject3}
-    assert str(excep.value) == "Namespace is already locked"
 
     assert tuple(namespace2) == (myobject1, myobject2)
+
+
+def test_set_default():
+    """Namespace IOR-Operator."""
+    myobject1 = ucdp.NamedObject(name="str1")
+    myobject2 = ucdp.NamedObject(name="str2")
+    myobject3 = ucdp.NamedObject(name="str3")
+    namespace = ucdp.Namespace()
+    assert namespace.set_default("str1", myobject1) is myobject1
+    assert tuple(namespace) == (myobject1,)
+    assert namespace.set_default("str1", myobject1) is myobject1
+    assert tuple(namespace) == (myobject1,)
+
+    msg = "NamedObject(name='str3') with must be stored at name 'str3' not at 'str2'"
+    with raises(ValueError, match=re.escape(msg)):
+        namespace.set_default("str2", myobject3)
+
+    assert tuple(namespace) == (myobject1,)
+
+    namespace.lock()
+
+    msg = "Namespace is already locked. Cannot add items anymore."
+    with raises(ValueError, match=re.escape(msg)):
+        namespace.set_default("str2", myobject2)
+
+    assert tuple(namespace) == (myobject1,)
```

### Comparing `ucdp-0.3.0/tests/test_object.py` & `ucdp-0.4.0/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_pathutil.py` & `ucdp-0.4.0/tests/test_pathutil.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_routepath.py` & `ucdp-0.4.0/tests/test_routepath.py`

 * *Files 23% similar despite different names*

```diff
@@ -61,14 +61,24 @@
     assert str(path) == "cast(u_sub/clk_i)"
     assert path.path == "u_sub"
     assert path.expr == "clk_i"
     assert path.create is False
     assert path.cast is True
 
 
+def test_parsepath_optcast():
+    """'Optional Casting."""
+    path = u.parse_routepath("optcast(u_sub/clk_i)")
+    assert str(path) == "optcast(u_sub/clk_i)"
+    assert path.path == "u_sub"
+    assert path.expr == "clk_i"
+    assert path.create is False
+    assert path.cast is None
+
+
 def test_parsepath_create():
     """Creating."""
     path = u.parse_routepath("create(u_sub/clk_i)")
     assert str(path) == "create(u_sub/clk_i)"
     assert path.path == "u_sub"
     assert path.expr == "clk_i"
     assert path.create is True
@@ -97,7 +107,18 @@
     assert path.cast is False
 
 
 def test_create_cast():
     """Create and Casting."""
     with raises(u.ValidationError, match=re.escape("[opt]cast() and create() are mutally exclusive")):
         u.RoutePath(expr="clk_i", create=True, cast=True)
+
+
+def test_expr():
+    """Expression."""
+    expr = u.Signal(u.UintType(8), "sig_s")
+    path = u.parse_routepath(expr)
+    assert str(path) == "sig_s"
+    assert path.path is None
+    assert path.expr is expr
+    assert path.create is False
+    assert path.cast is False
```

### Comparing `ucdp-0.3.0/tests/test_typeenum.py` & `ucdp-0.4.0/tests/test_typeenum.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.3.0/tests/test_typescalar.py` & `ucdp-0.4.0/tests/test_typescalar.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,7 +197,22 @@
 
     var1 = u.SintType(12, default=8, right=4)
     assert var1.default == 8
     assert var1.width == 12
     assert var1.right == 4
     assert var1.slice_ == u.Slice("15:4")
     assert repr(var1) == "SintType(12, default=8, right=4)"
+
+
+def test_doc():
+    """Documentation."""
+    assert u.UintType(8).doc == u.Doc()
+
+    class MyUintType(u.UintType):
+        title: str = "mytitle"
+        descr: str = "mydescr"
+        comment: str = "mycomment"
+
+        def __init__(self):
+            super().__init__(8)
+
+    assert MyUintType().doc == u.Doc(title="mytitle", descr="mydescr", comment="mycomment")
```

### Comparing `ucdp-0.3.0/tests/test_typestruct.py` & `ucdp-0.4.0/tests/test_typestruct.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,39 +20,46 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
 Struct Type Testing.
-
 """
 
+import re
+
 import ucdp as u
 from pytest import raises
 
 
 def test_struct():
     """Struct."""
 
     class MyStructType(u.AStructType):
         """Struct."""
 
         def _build(self) -> None:
             self._add("data", u.UintType(8), title="title")
             self._add("valid", u.BitType(), descr="descr", ifdef="IFDEF")
             self._add("accept", u.BitType(), u.BWD, comment="comment")
-            with raises(ValueError) as exception:
+
+            msg = (
+                "name 'valid' already exists in test_struct.<locals>.MyStructType() "
+                "(StructItem('valid', BitType(), doc=Doc(descr='descr'), ifdef='IFDEF'))"
+            )
+            with raises(ValueError, match=re.escape(msg)):
                 self._add("valid", u.BitType())
-                assert str(exception.value) == "key 2 already exists in test_enum.<locals>.MyStructType()"
 
     struct = MyStructType()
-    with raises(u.LockError) as exception:
+
+    msg = "test_struct.<locals>.MyStructType(): Cannot add item 'lock'."
+    with raises(u.LockError, match=re.escape(msg)):
         struct._add("lock", u.BitType())
-        assert str(exception.value) == "key 2 already exists in test_enum.<locals>.MyStructType()"
+
     assert tuple(struct) == tuple(struct.keys())
     assert tuple(struct.keys()) == ("data", "valid", "accept")
     assert tuple(struct.values()) == (
         u.StructItem("data", u.UintType(8), doc=u.Doc(title="title")),
         u.StructItem("valid", u.BitType(), doc=u.Doc(descr="descr"), ifdef="IFDEF"),
         u.StructItem("accept", u.BitType(), orientation=u.BWD, doc=u.Doc(comment="comment")),
     )
@@ -123,7 +130,22 @@
     other = MyType()
     other.add("accept", u.BitType(), orientation=u.BWD)
 
     assert one is not other
     assert one != other
     assert tuple(one) == ("data", "valid")
     assert tuple(other) == ("accept",)
+
+
+def test_structitem():
+    """StructItem testing."""
+    doc = u.Doc(title="title", descr="descr", comment="comment")
+    item = u.StructItem(
+        "data",
+        u.UintType(8),
+        doc=doc,
+    )
+
+    assert item.doc is doc
+    assert item.title == "title"
+    assert item.descr == "descr"
+    assert item.comment == "comment"
```

### Comparing `ucdp-0.3.0/PKG-INFO` & `ucdp-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucdp
-Version: 0.3.0
+Version: 0.4.0
 Summary: Unified Chip Design Platform
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/nbiotcloud/ucdp
 Project-URL: Documentation, https://ucdp.readthedocs.io/en/latest/
 Project-URL: Bug tracker, https://github.com/nbiotcloud/ucdp/issues
 Requires-Python: <4.0,>=3.10.0
```

