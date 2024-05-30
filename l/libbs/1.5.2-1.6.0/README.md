# Comparing `tmp/libbs-1.5.2.tar.gz` & `tmp/libbs-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.5.2.tar", last modified: Wed May 29 21:20:55 2024, max compression
+gzip compressed data, was "libbs-1.6.0.tar", last modified: Thu May 30 05:48:05 2024, max compression
```

## Comparing `libbs-1.5.2.tar` & `libbs-1.6.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-29 21:20:51.000000 libbs-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:20:55.293996 libbs-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-29 21:20:51.000000 libbs-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.281996 libbs-1.5.2/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.285996 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32864 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.289996 libbs-1.5.2/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-29 21:20:51.000000 libbs-1.5.2/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 21:20:55.000000 libbs-1.5.2/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 21:20:55.293996 libbs-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 21:20:51.000000 libbs-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:20:55.293996 libbs-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-29 21:20:51.000000 libbs-1.5.2/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-29 21:20:51.000000 libbs-1.5.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-29 21:20:51.000000 libbs-1.5.2/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.156632 libbs-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 05:47:58.000000 libbs-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-30 05:48:05.156632 libbs-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-30 05:47:58.000000 libbs-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.144632 libbs-1.6.0/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.144632 libbs-1.6.0/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.148632 libbs-1.6.0/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.152632 libbs-1.6.0/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.152632 libbs-1.6.0/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.152632 libbs-1.6.0/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.152632 libbs-1.6.0/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32896 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.152632 libbs-1.6.0/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30613 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.156632 libbs-1.6.0/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-30 05:47:58.000000 libbs-1.6.0/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.156632 libbs-1.6.0/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-30 05:48:05.000000 libbs-1.6.0/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-30 05:48:05.000000 libbs-1.6.0/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:48:05.000000 libbs-1.6.0/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 05:48:05.000000 libbs-1.6.0/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 05:48:05.000000 libbs-1.6.0/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 05:48:05.000000 libbs-1.6.0/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 05:48:05.156632 libbs-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 05:47:58.000000 libbs-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:48:05.156632 libbs-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-05-30 05:47:58.000000 libbs-1.6.0/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-30 05:47:58.000000 libbs-1.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-30 05:47:58.000000 libbs-1.6.0/tests/test_decompilers.py
```

### Comparing `libbs-1.5.2/LICENSE` & `libbs-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/PKG-INFO` & `libbs-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.5.2
+Version: 1.6.0
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -85,7 +85,19 @@
 ```python
 for func_addr, light_func in deci.functions.items():
     full_function = deci.function[func_addr]
 ```
 
 Notice, when using the `items` function the function is `light`, meaning it does not contain stack vars and other 
 info. This also means using `keys`, `values`, or `list` on an artifact dictionary will have the same affect. 
+
+### Serializing Artifacts
+All artifacts are serializable to the TOML and JSON formats. Serialization is done like so:
+```python
+from libbs.artifacts import Function
+import json
+
+my_func = Function(name="my_func", addr=0x4000, size=0x10)
+json_str = my_func.dumps(fmt="json")
+loaded_dict = json.loads(json_str) # now loadable through normal JSON parsing
+loaded_func = Function.loads(json_str, fmt="json")
+```
```

### Comparing `libbs-1.5.2/README.md` & `libbs-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,7 +61,19 @@
 ```python
 for func_addr, light_func in deci.functions.items():
     full_function = deci.function[func_addr]
 ```
 
 Notice, when using the `items` function the function is `light`, meaning it does not contain stack vars and other 
 info. This also means using `keys`, `values`, or `list` on an artifact dictionary will have the same affect. 
+
+### Serializing Artifacts
+All artifacts are serializable to the TOML and JSON formats. Serialization is done like so:
+```python
+from libbs.artifacts import Function
+import json
+
+my_func = Function(name="my_func", addr=0x4000, size=0x10)
+json_str = my_func.dumps(fmt="json")
+loaded_dict = json.loads(json_str) # now loadable through normal JSON parsing
+loaded_func = Function.loads(json_str, fmt="json")
+```
```

### Comparing `libbs-1.5.2/libbs/__main__.py` & `libbs-1.6.0/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/api/artifact_dict.py` & `libbs-1.6.0/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/api/artifact_lifter.py` & `libbs-1.6.0/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/api/decompiler_interface.py` & `libbs-1.6.0/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/api/type_parser.py` & `libbs-1.6.0/libbs/api/type_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 errorlog.setLevel(logging.ERROR)
 
 
 l = logging.getLogger(__name__)
 
 
 class CType:
-    def __init__(self,
-                 type_=None,
-                 size=0,
-                 is_primitive=True,
-                 is_array=False,
-                 is_ptr=False,
-                 is_unknown=False
-                 ):
+    def __init__(
+        self,
+        type_=None,
+        size=0,
+        is_primitive=True,
+        is_array=False,
+        is_ptr=False,
+        is_unknown=False
+    ):
         self.type = type_
         self._size = size
 
         self.is_primitive = is_primitive
         self.is_array = is_array
         self.is_ptr = is_ptr
         self.is_unknown = is_unknown
@@ -66,26 +67,26 @@
     """
     Most of this code is ripped from angr's sim_type:
     https://github.com/angr/angr/blob/master/angr/sim_type.py
 
     It is highly simplified and drops a lot of support for real declaration parsing (like a struct dec).
     Instead, we just use it to parse types.
     """
-    def __init__(self,
-                 sizeof_ptr=8,
-                 sizeof_long=8,
-                 sizeof_double=8,
-                 sizeof_int=4,
-                 sizeof_float=4,
-                 sizeof_short=2,
-                 sizeof_char=1,
-                 sizeof_bool=1,
-                 extra_types=None
-                 ):
-
+    def __init__(
+        self,
+        sizeof_ptr=8,
+        sizeof_long=8,
+        sizeof_double=8,
+        sizeof_int=4,
+        sizeof_float=4,
+        sizeof_short=2,
+        sizeof_char=1,
+        sizeof_bool=1,
+        extra_types=None
+    ):
         # sizes
         self.sizeof_ptr = sizeof_ptr
         self.sizeof_long = sizeof_long
         self.sizeof_double = sizeof_double
         self.sizeof_int = sizeof_int
         self.sizeof_float = sizeof_float
         self.sizeof_short = sizeof_short
@@ -101,14 +102,15 @@
             optimize=False,
             errorlog=errorlog
         )
         self.ALL_TYPES = {}
         self.BASIC_TYPES = {}
         self.STDINT_TYPES = {}
         self.extra_types = extra_types or {}
+        self.SIZE_TO_TYPES = {}
         self._init_all_types()
 
     def _init_all_types(self):
         self.BASIC_TYPES = {
             "char": CType(type_="char", size=self.sizeof_char),
             "signed char": CType(type_="signed char", size=self.sizeof_char),
             "unsigned char": CType(type_="unsigned char", size=self.sizeof_char),
@@ -162,15 +164,19 @@
             "dword": CType(type_="dword", size=4),
             "int64_t": CType(type_="int64_t", size=8),
             "uint64_t": CType(type_="uint64_t", size=8),
         }
         self.ALL_TYPES.update(self.STDINT_TYPES)
         self.ALL_TYPES.update(self.extra_types)
 
-    def parse_type(self, defn, preprocess=True, predefined_types=None, arch=None):  # pylint:disable=unused-argument
+        for name, ctype in self.ALL_TYPES.items():
+            if name.startswith("unsigned"):
+                self.SIZE_TO_TYPES[ctype.size] = ctype
+
+    def parse_type(self, defn, preprocess=True, predefined_types=None, arch=None) -> Optional[CType]:  # pylint:disable=unused-argument
         """
         Parse a simple type expression into a SimType
 
         >>> self.parse_type('int *')
         """
         return self.parse_type_with_name(defn, preprocess=preprocess, predefined_types=predefined_types, arch=arch)[0]
 
@@ -323,7 +329,23 @@
                 return self._decl_to_type(c.expr.type, extra_types=extra_types).size
             else:
                 raise ValueError("Unary op %s" % c.op)
         elif type(c) is pycparser.c_ast.Cast:
             return self._parse_const(c.expr, extra_types=extra_types)
         else:
             raise ValueError(c)
+
+    def size_to_type(self, size: int) -> CType:
+        if not size:
+            raise ValueError("A type size must be greater than 0")
+
+        ctype = self.SIZE_TO_TYPES.get(size, None)
+        if ctype is None:
+            # one of two possible things have happend here:
+            # 1. this is a type that is larger than the simple types, in which case it's an array
+            # 2. this is a type with a non-aligned size, in which case we default to an array as well
+            array_size = size // self.sizeof_char
+            ctype = self.parse_type(f"char[{array_size}]")
+            if ctype is None:
+                raise RuntimeError(f"Failed to create a CType of array size {array_size}")
+
+        return ctype
```

### Comparing `libbs-1.5.2/libbs/api/utils.py` & `libbs-1.6.0/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/artifacts/__init__.py` & `libbs-1.6.0/libbs/artifacts/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .artifact import Artifact, TomlHexEncoder
+from .formatting import TomlHexEncoder, ArtifactFormat
+from .artifact import Artifact
 from .comment import Comment
 from .decompilation import Decompilation
 from .enum import Enum
 from .func import Function, FunctionHeader, FunctionArgument
 from .global_variable import GlobalVariable
 from .patch import Patch
 from .stack_variable import StackVariable
```

### Comparing `libbs-1.5.2/libbs/artifacts/enum.py` & `libbs-1.6.0/libbs/artifacts/enum.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,36 @@
 from collections import OrderedDict
 from typing import Dict
 
-import toml
-
 from .artifact import Artifact
 
 
 class Enum(Artifact):
     __slots__ = Artifact.__slots__ + (
         "name",
         "members",
     )
 
-    def __init__(self, name, members: Dict[str, int], last_change=None):
-        super(Enum, self).__init__(last_change=last_change)
+    def __init__(
+        self,
+        name: str = None,
+        members: Dict[str, int] = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
         self.name = name
         # sorts map by the int value
-        self.members = OrderedDict(sorted(members.items(), key=lambda kv: kv[1]))
+        self.members = self._order_members(members) if members else None
 
     def __str__(self):
         return f"<Enum: {self.name} member_count={len(self.members)}>"
 
-    def __repr__(self):
-        return self.__str__()
-
-    @classmethod
-    def parse(cls, s):
-        en = Enum(None, {})
-        en.__setstate__(toml.loads(s))
-        return en
-
-    @classmethod
-    def load_many(cls, enums_toml):
-        for enum_toml in enums_toml.values():
-            enum = Enum(None, {})
-            try:
-                enum.__setstate__(enum_toml)
-            except TypeError:
-                # skip all incorrect ones
-                continue
-            yield enum
-
-    @classmethod
-    def dump_many(cls, enums):
-        enums_ = {}
-
-        for name, enum in enums.items():
-            enums_[name] = enum.__getstate__()
-        return enums_
-
-    def copy(self):
-        return Enum(
-            self.name,
-            self.members.copy(),
-            last_change=self.last_change
-        )
+    @staticmethod
+    def _order_members(members):
+        return OrderedDict(sorted(members.items(), key=lambda kv: kv[1]))
 
     def nonconflict_merge(self, enum2: "Enum", **kwargs):
         enum1: Enum = self.copy()
         if not enum2 or enum1 == enum2:
             return enum1.copy()
 
         master_state = kwargs.get("master_state", None)
```

### Comparing `libbs-1.5.2/libbs/artifacts/func.py` & `libbs-1.6.0/libbs/artifacts/func.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Dict, Optional
 
-import toml
-
-from .artifact import Artifact, TomlHexEncoder
+from .artifact import Artifact
 from .stack_variable import StackVariable
 
 
 #
 # Function Header Classes
 #
 
@@ -14,86 +12,77 @@
     __slots__ = Artifact.__slots__ + (
         "offset",
         "name",
         "type",
         "size",
     )
 
-    def __init__(self, offset, name, type_, size, last_change=None):
-        super(FunctionArgument, self).__init__(last_change=last_change)
+    def __init__(
+        self,
+        offset: int = None,
+        name: str = None,
+        type_: str = None,
+        size: int = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
         self.offset = offset
         self.name = name
         self.type = type_
         self.size = size
 
     def __str__(self):
         return f"<FuncArg: {self.type} {self.name}; @{self.offset}>"
 
-    def __repr__(self):
-        return self.__str__()
-
-    @classmethod
-    def parse(cls, s):
-        fa = FunctionArgument(None, None, None, None)
-        fa.__setstate__(toml.loads(s))
-        return fa
-
-    def copy(self):
-        return FunctionArgument(self.offset, self.name, self.type, self.size, last_change=self.last_change)
-
 
 class FunctionHeader(Artifact):
     __slots__ = Artifact.__slots__ + (
         "name",
         "addr",
         "type",
         "args"
     )
 
-    def __init__(self, name, addr, type_=None, args=None, last_change=None):
-        super(FunctionHeader, self).__init__(last_change=last_change)
+    def __init__(
+        self,
+        name: str = None,
+        addr: int = None,
+        type_: str = None,
+        args: Optional[Dict[int, FunctionArgument]] = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
         self.name = name
         self.addr = addr
         self.type = type_
-        self.args: Dict[str, FunctionArgument] = args or {}
+        self.args: Dict = args or {}
 
     def __str__(self):
-        return f"<FuncHeader: {self.type} {self.name}(args={len(self.args)}); @{hex(self.addr)}>"
-
-    def __repr__(self):
-        return self.__str__()
+        return f"<FuncHeader: {self.type} {self.name}(args={len(self.args or {})}); @{hex(self.addr)}>"
 
     def __getstate__(self):
-        args = {str(idx): arg.__getstate__() for idx, arg in self.args.items()} if self.args else {}
-
-        return {
-            "last_change": self.last_change,
-            "name": self.name,
-            "addr": self.addr,
-            "type": self.type,
-            "args": args if len(args) > 0 else None,
-        }
+        data_dict = super().__getstate__()
+        args_dict = data_dict["args"]
+        if args_dict is None:
+            return data_dict
+
+        new_args_dict = {hex(k): v.__getstate__() for k, v in args_dict.items()}
+        data_dict["args"] = new_args_dict
+        return data_dict
 
     def __setstate__(self, state):
-        self.last_change = state.get("last_change", None)
-        self.name = state.get("name", None)
-        self.addr = state["addr"]
-        self.type = state.get("type", None)
-        args = state.get("args", {})
-        self.args = {int(idx, 16): FunctionArgument.parse(toml.dumps(arg, encoder=TomlHexEncoder())) for idx, arg in args.items()}
-
-    @classmethod
-    def parse(cls, s):
-        loaded_s = toml.loads(s)
-        if len(loaded_s) <= 0:
-            return None
-
-        fh = FunctionHeader(None, None)
-        fh.__setstate__(toml.loads(s))
-        return fh
+        args_dict = state.pop("args", {})
+        new_args_dict = {}
+        for k, v in args_dict.items():
+            fa = FunctionArgument()
+            fa.__setstate__(v)
+            new_args_dict[int(k, 0)] = fa
+
+        self.args = new_args_dict
+        super().__setstate__(state)
 
     def diff(self, other, **kwargs) -> Dict:
         diff_dict = {}
         # early exit if the two do not match type
         if not isinstance(other, FunctionHeader):
             for k in ["name", "addr", "type"]:
                 diff_dict[k] = {
@@ -128,19 +117,14 @@
             if idx in diff_dict["args"]:
                 continue
 
             diff_dict["args"][idx] = self.invert_diff(other_arg.diff(None))
 
         return diff_dict
 
-    def copy(self):
-        fh = FunctionHeader(self.name, self.addr, type_=self.type, last_change=self.last_change)
-        fh.args = {k: v.copy() for k, v in self.args.items()}
-        return fh
-
     def reset_last_change(self):
         if self.args:
             for arg in self.args.values():
                 arg.reset_last_change()
 
     def overwrite_merge(self, obj2: "Artifact", **kwargs):
         fh2: "FunctionHeader" = obj2
@@ -196,74 +180,88 @@
     2. Header
     3. Stack Vars
 
     The metadata contains info on changes and size. The header holds the return type,
     and arguments (including their types). The stack vars contain StackVariables.
     """
 
-    __slots__ = (
-        "last_change",
+    __slots__ = Artifact.__slots__ + (
         "addr",
         "size",
         "header",
         "stack_vars",
         "dec_obj",
     )
 
-    def __init__(self, addr, size, header=None, stack_vars=None, dec_obj=None, last_change=None):
-        super(Function, self).__init__(last_change=last_change)
-        self.addr: int = addr
-        self.size: int = size
-        self.header: Optional[FunctionHeader] = header
+    def __init__(
+        self,
+        addr: int = None,
+        size: int = None,
+        name: str = None,
+        header: Optional[FunctionHeader] = None,
+        stack_vars: Optional[Dict[int, StackVariable]] = None,
+        dec_obj: Optional[object] = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+        self.addr = addr
+        self.size = size
+        self.header = header
+        self.name = name
         self.stack_vars: Dict[int, StackVariable] = stack_vars or {}
 
         # a special property which can only be set while running inside the decompiler.
         # contains a reference to the decompiler object associated with this function.
         self.dec_obj = dec_obj
 
     def __str__(self):
         if self.header:
             return f"<Function: {self.header.type} {self.name}(args={len(self.args)}); @{hex(self.addr)} " \
                    f"vars={len(self.stack_vars)} len={hex(self.size)}>"
 
         return f"<Function: @{hex(self.addr)} len={hex(self.size)}>"
 
-    def __repr__(self):
-        return self.__str__()
-
     def __getstate__(self):
         header = self.header.__getstate__() if self.header else None
-        stack_vars = {hex(offset): stack_var.__getstate__() for offset, stack_var in self.stack_vars.items()} if \
-            self.stack_vars else {}
-
-        return {
-            "metadata": {
-                "addr": self.addr,
-                "size": self.size,
-                "last_change": self.last_change
-            },
-            "header": header,
-            "stack_vars": stack_vars if len(stack_vars) > 0 else None
-        }
+        stack_vars = {
+            hex(offset): stack_var.__getstate__() for offset, stack_var in self.stack_vars.items()
+        } if self.stack_vars else None
+
+        state = super().__getstate__()
+        state["header"] = header
+        state["stack_vars"] = stack_vars
+        return state
 
     def __setstate__(self, state):
-        if not isinstance(state["metadata"]["addr"], int):
-            raise TypeError("Unsupported type %s for addr." % type(state["metadata"]["addr"]))
-
-        metadata, header, stack_vars = state["metadata"], state.get("header", None), state.get("stack_vars", {})
-
-        self.addr = metadata["addr"]
-        self.size = metadata["size"]
-        self.last_change = metadata.get("last_change", None)
+        # XXX: this is a backport of the old state format. Remove this after a few releases.
+        if "metadata" in state:
+            metadata: Dict = state.pop("metadata")
+            metadata.update(state)
+            state = metadata
+
+        header_dat = state.pop("header", None)
+        if header_dat:
+            header = FunctionHeader()
+            header.__setstate__(header_dat)
+        else:
+            header = None
+        self.header = header
 
-        self.header = FunctionHeader.parse(toml.dumps(header, encoder=TomlHexEncoder())) if header else None
+        stack_vars_dat = state.pop("stack_vars", {})
+        if stack_vars_dat:
+            stack_vars = {}
+            for off, stack_var in stack_vars_dat.items():
+                sv = StackVariable()
+                sv.__setstate__(stack_var)
+                stack_vars[int(off, 0)] = sv
+        else:
+            stack_vars = None
+        self.stack_vars = stack_vars or {}
 
-        self.stack_vars = {
-            int(off, 16): StackVariable.parse(toml.dumps(stack_var, encoder=TomlHexEncoder())) for off, stack_var in stack_vars.items()
-        } if stack_vars else {}
+        super().__setstate__(state)
 
     def diff(self, other, **kwargs) -> Dict:
         diff_dict = {}
         if not isinstance(other, Function):
             # metadata
             for k in ["addr", "size"]:
                 diff_dict[k] = {
@@ -309,33 +307,14 @@
             if off in diff_dict["stack_vars"]:
                 continue
 
             diff_dict["stack_vars"][off] = self.invert_diff(other_var.diff(None))
 
         return diff_dict
 
-    def copy(self):
-        func = Function(self.addr, self.size, last_change=self.last_change, dec_obj=self.dec_obj)
-        func.header = self.header.copy() if self.header else None
-        func.stack_vars = {k: v.copy() for k, v in self.stack_vars.items()}
-
-        return func
-
-    @classmethod
-    def parse(cls, s):
-        func = Function(None, None)
-        func.__setstate__(s)
-        return func
-
-    @classmethod
-    def load(cls, func_toml):
-        f = Function(None, None)
-        f.__setstate__(func_toml)
-        return f
-
     def reset_last_change(self):
         if self.header:
             self.header.reset_last_change()
 
         if self.stack_vars:
             for sv in self.stack_vars.values():
                 sv.reset_last_change()
@@ -393,16 +372,13 @@
     def name(self):
         return self.header.name if self.header else None
 
     @name.setter
     def name(self, value):
         # create a header if one does not exist for this function
         if not self.header:
-            self.header = FunctionHeader(None, self.addr)
+            self.header = FunctionHeader(name=None, addr=self.addr)
         self.header.name = value
 
     @property
     def args(self):
-        return self.header.args
-
-    def set_stack_var(self, name, off: int, off_type: int, size: int, type_, last_change):
-        self.stack_vars[off] = StackVariable(off, off_type, name, type_, size, self.addr, last_change=last_change)
+        return self.header.args if self.header else {}
```

### Comparing `libbs-1.5.2/libbs/artifacts/struct.py` & `libbs-1.6.0/libbs/artifacts/struct.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import toml
 
-from .artifact import Artifact, TomlHexEncoder
+from .artifact import Artifact
+from . import TomlHexEncoder
 
 import logging
 l = logging.getLogger(name=__name__)
 
 
 class StructMember(Artifact):
     """
@@ -16,89 +17,82 @@
     __slots__ = Artifact.__slots__ + (
         "name",
         "offset",
         "type",
         "size",
     )
 
-    def __init__(self, name, offset, type_, size, last_change=None):
-        super(StructMember, self).__init__(last_change=last_change)
+    def __init__(
+        self,
+        name: str = None,
+        offset: int = None,
+        type_: Optional[str] = None,
+        size: int = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
         self.name: str = name
         self.offset: int = offset
         self.type: str = type_
         self.size: int = size
 
     def __str__(self):
         return f"<StructMember: {self.type} {self.name}; @{hex(self.offset)}>"
 
-    def __repr__(self):
-        return self.__str__()
-
-    @classmethod
-    def parse(cls, s):
-        sm = StructMember(None, None, None, None)
-        sm.__setstate__(toml.loads(s))
-        return sm
-
-    def copy(self):
-        sm = StructMember(
-            self.name,
-            self.offset,
-            self.type,
-            self.size
-        )
-
-        return sm
-
 
 class Struct(Artifact):
     """
     Describes a struct
     """
 
     __slots__ = Artifact.__slots__ + (
         "name",
         "size",
         "members",
     )
 
-    def __init__(self, name: str, size: int, members: Dict[int, StructMember], last_change=None):
-        super(Struct, self).__init__(last_change=last_change)
+    def __init__(
+        self,
+        name: str = None,
+        size: int = None,
+        members: Dict[int, StructMember] = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
         self.name = name
         self.size = size or 0
-        self.members: Dict[int, StructMember] = members
+        self.members: Dict[int, StructMember] = members or {}
 
     def __str__(self):
         return f"<Struct: {self.name} membs={len(self.members)} ({hex(self.size)})>"
 
-    def __repr__(self):
-        return self.__str__()
-
     def __getstate__(self):
-        return {
-            "metadata": {
-                "name": self.name, "size": self.size, "last_change": self.last_change
-            },
-
-            "members": {
-                hex(offset): member.__getstate__() for offset, member in self.members.items()
-            }
+        data_dict = super().__getstate__()
+        data_dict["members"] = {
+            hex(offset): member.__getstate__() for offset, member in self.members.items()
         }
 
-    def __setstate__(self, state):
-        metadata = state["metadata"]
-        members = state["members"]
-
-        self.name = metadata["name"]
-        self.size = metadata["size"]
-        self.last_change = metadata.get("last_change", None)
+        return data_dict
 
-        self.members = {
-            int(off, 16): StructMember.parse(toml.dumps(member, encoder=TomlHexEncoder())) for off, member in members.items()
-        }
+    def __setstate__(self, state):
+        # XXX: this is a backport of the old state format. Remove this after a few releases.
+        if "metadata" in state:
+            metadata: Dict = state.pop("metadata")
+            metadata.update(state)
+            state = metadata
+
+        members_dat = state.pop("members", None)
+        if members_dat:
+            for off, member in members_dat.items():
+                sm = StructMember()
+                sm.__setstate__(member)
+                self.members[int(off, 0)] = sm
+        else:
+            self.members = {}
+        super().__setstate__(state)
 
     def add_struct_member(self, mname, moff, mtype, size):
         self.members[moff] = StructMember(mname, moff, mtype, size)
 
     def diff(self, other, **kwargs) -> Dict:
         diff_dict = {}
         if not isinstance(other, Struct):
@@ -127,31 +121,14 @@
             if off in diff_dict["members"]:
                 continue
 
             diff_dict["members"][off] = self.invert_diff(other_mem.diff(None))
 
         return diff_dict
 
-    def copy(self):
-        members = {offset: member.copy() for offset, member in self.members.items()}
-        struct = Struct(self.name, self.size, members, last_change=self.last_change)
-        return struct
-
-    @classmethod
-    def parse(cls, s):
-        struct = Struct(None, None, None)
-        struct.__setstate__(s)
-        return struct
-
-    @classmethod
-    def load(cls, struct_toml):
-        s = Struct(None, None, None)
-        s.__setstate__(struct_toml)
-        return s
-
     def nonconflict_merge(self, struct2: "Struct", **kwargs) -> "Struct":
         struct1: "Struct" = self.copy()
         if not struct2 or struct1 == struct2:
             return struct1
 
         struct_diff = struct1.diff(struct2)
         merge_struct = struct1
```

### Comparing `libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.6.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.6.0/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/angr/compat.py` & `libbs-1.6.0/libbs/decompilers/angr/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,72 +110,76 @@
 
     # pylint: disable=unused-argument
     def handle_func_arg_renamed(self, func, offset, old_name, new_name):
         decompilation = self.interface.decompile_function(func)
         func_args = AngrInterface.func_args_as_libbs_args(decompilation)
         self.interface.function_header_changed(
             FunctionHeader(
-                None,
-                func.addr,
+                name=None,
+                addr=func.addr,
                 type_=None,
-                args={offset: FunctionArgument(offset, new_name, None, func_args[offset].size)},
+                args={
+                    offset: FunctionArgument(offset=offset, name=new_name, type_=None, size=func_args[offset].size)
+                },
             )
         )
 
         return True
 
     # pylint: disable=unused-argument
     def handle_func_arg_retyped(self, func, offset, old_type, new_type):
         decompilation = self.interface.decompile_function(func)
         func_args = AngrInterface.func_args_as_libbs_args(decompilation)
         self.interface.function_header_changed(
             FunctionHeader(
-                None,
-                func.addr,
+                name=None,
+                addr=func.addr,
                 type_=None,
-                args={offset: FunctionArgument(offset, None, new_type, func_args[offset].size)},
+                args={
+                    offset: FunctionArgument(offset=offset, name=None, type_=new_type, size=func_args[offset].size)
+                },
             )
         )
 
         return True
 
     # pylint: disable=unused-argument,no-self-use
     def handle_global_var_renamed(self, address, old_name, new_name):
         self.interface.global_variable_changed(
-            GlobalVariable(address, new_name, type_=None)
+            GlobalVariable(addr=address, name=new_name, type_=None)
         )
         return True
 
     # pylint: disable=unused-argument,no-self-use
     def handle_global_var_retyped(self, address, old_type, new_type):
         self.interface.global_variable_changed(
-            GlobalVariable(address, None, type_=new_type)
+            GlobalVariable(addr=address, name=None, type_=new_type)
         )
         return True
 
     # pylint: disable=unused-argument
     def handle_function_renamed(self, func, old_name, new_name):
         if func is None:
             return False
 
-        self.interface.function_header_changed(FunctionHeader(new_name, func.addr))
+        self.interface.function_header_changed(FunctionHeader(name=new_name, addr=func.addr))
         return True
 
     # pylint: disable=unused-argument,no-self-use
     def handle_function_retyped(self, func, old_type, new_type):
         if func is None:
             return False
 
-        self.interface.function_header_changed(FunctionHeader(None, func.addr, type_=new_type))
+        self.interface.function_header_changed(FunctionHeader(name=None, addr=func.addr, type_=new_type))
         return True
 
     # pylint: disable=unused-argument
     def handle_comment_changed(self, address, old_cmt, new_cmt, created: bool, decomp: bool):
         # comments are only possible in functions in AM
         func_addr = self.interface.get_closest_function(address)
         if func_addr is None:
             return False
 
         self.interface.comment_changed(
-            Comment(address, new_cmt, func_addr=func_addr, decompiled=True), deleted=not new_cmt
+            Comment(addr=address, comment=new_cmt, func_addr=func_addr, decompiled=True), deleted=not new_cmt
         )
         return True
```

### Comparing `libbs-1.5.2/libbs/decompilers/angr/interface.py` & `libbs-1.6.0/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.6.0/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/binja/hooks.py` & `libbs-1.6.0/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/binja/interface.py` & `libbs-1.6.0/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.6.0/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.6.0/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/ghidra/hooks.py` & `libbs-1.6.0/libbs/decompilers/ghidra/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/ghidra/interface.py` & `libbs-1.6.0/libbs/decompilers/ghidra/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,24 +271,24 @@
         stack_variables = {}
         if stack_variable_info:
             stack_variables = {
                 offset: StackVariable(offset, name, typestr, size, addr) for offset, name, typestr, size in
                 stack_variable_info
             }
 
-        arg_variable_info: Optional[List[Tuple[int, str, str, int]]] = self.ghidra.bridge.remote_eval(
+        arg_variable_info: Optional[List[Tuple[str, str, int]]] = self.ghidra.bridge.remote_eval(
             "[(sym.getName(), str(sym.getDataType()), sym.getSize()) "
             "for sym in dec.getHighFunction().getLocalSymbolMap().getSymbols() "
             "if sym.isParameter()]",
             dec=dec
         )
         args = {}
         if arg_variable_info:
             args = {
-                i: FunctionArgument(i, info[0], info[1], info[2], addr) for i, info in enumerate(arg_variable_info)
+                i: FunctionArgument(offset=i, name=info[0], type_=info[1], size=info[2]) for i, info in enumerate(arg_variable_info)
             }
 
         # grab the return type of the function from ghidra
         type_ = self.ghidra.bridge.remote_eval(
             "dec.getHighFunction().getFunctionPrototype().getReturnType().getName()",
             dec=dec
         )
@@ -714,16 +714,16 @@
         return bs_stack_var
 
     def _gfunc_to_bsfunc(self, gfunc: "GhidraFunction"):
         if gfunc is None:
             return None
 
         bs_func = Function(
-            gfunc.getEntryPoint().getOffset(), gfunc.getBody().getNumAddresses(),
-            header=FunctionHeader(gfunc.getName(), gfunc.getEntryPoint().getOffset()),
+            addr=gfunc.getEntryPoint().getOffset(), size=gfunc.getBody().getNumAddresses(),
+            header=FunctionHeader(name=gfunc.getName(), addr=gfunc.getEntryPoint().getOffset()),
         )
         return bs_func
 
     def _ghidra_decompile(self, func: "GhidraFunction") -> "DecompileResult":
         """
         TODO: this needs to be cached!
         @param func:
```

### Comparing `libbs-1.5.2/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.6.0/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/ida/compat.py` & `libbs-1.6.0/libbs/decompilers/ida/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     for func_addr in func_addrs:
         # skip non-text segments
         if idc.get_segm_name(func_addr) in blacklisted_segs:
             continue
 
         func_name = get_func_name(func_addr)
         func_size = get_func_size(func_addr)
-        func = Function(func_addr, func_size)
+        func = Function(addr=func_addr, size=func_size)
         func.name = func_name
         funcs[func_addr] = func
 
     return funcs
 
 
 @execute_write
```

### Comparing `libbs-1.5.2/libbs/decompilers/ida/hooks.py` & `libbs-1.6.0/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/decompilers/ida/interface.py` & `libbs-1.6.0/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/logger.py` & `libbs-1.6.0/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/plugin_installer.py` & `libbs-1.6.0/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/ui/__init__.py` & `libbs-1.6.0/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/ui/qt_objects.py` & `libbs-1.6.0/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs/ui/utils.py` & `libbs-1.6.0/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/libbs.egg-info/PKG-INFO` & `libbs-1.6.0/libbs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.5.2
+Version: 1.6.0
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -85,7 +85,19 @@
 ```python
 for func_addr, light_func in deci.functions.items():
     full_function = deci.function[func_addr]
 ```
 
 Notice, when using the `items` function the function is `light`, meaning it does not contain stack vars and other 
 info. This also means using `keys`, `values`, or `list` on an artifact dictionary will have the same affect. 
+
+### Serializing Artifacts
+All artifacts are serializable to the TOML and JSON formats. Serialization is done like so:
+```python
+from libbs.artifacts import Function
+import json
+
+my_func = Function(name="my_func", addr=0x4000, size=0x10)
+json_str = my_func.dumps(fmt="json")
+loaded_dict = json.loads(json_str) # now loadable through normal JSON parsing
+loaded_func = Function.loads(json_str, fmt="json")
+```
```

### Comparing `libbs-1.5.2/libbs.egg-info/SOURCES.txt` & `libbs-1.6.0/libbs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 libbs/api/type_parser.py
 libbs/api/utils.py
 libbs/artifacts/__init__.py
 libbs/artifacts/artifact.py
 libbs/artifacts/comment.py
 libbs/artifacts/decompilation.py
 libbs/artifacts/enum.py
+libbs/artifacts/formatting.py
 libbs/artifacts/func.py
 libbs/artifacts/global_variable.py
 libbs/artifacts/patch.py
 libbs/artifacts/stack_variable.py
 libbs/artifacts/struct.py
 libbs/decompiler_stubs/__init__.py
 libbs/decompiler_stubs/ida_libbs.py
```

### Comparing `libbs-1.5.2/setup.cfg` & `libbs-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/tests/test_cli.py` & `libbs-1.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.5.2/tests/test_decompilers.py` & `libbs-1.6.0/tests/test_decompilers.py`

 * *Files identical despite different names*

