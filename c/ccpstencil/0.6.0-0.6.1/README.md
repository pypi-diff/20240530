# Comparing `tmp/ccpstencil-0.6.0.tar.gz` & `tmp/ccpstencil-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpstencil-0.6.0.tar", last modified: Thu May 30 13:53:36 2024, max compression
+gzip compressed data, was "ccpstencil-0.6.1.tar", last modified: Thu May 30 14:42:54 2024, max compression
```

## Comparing `ccpstencil-0.6.0.tar` & `ccpstencil-0.6.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.470872 ccpstencil-0.6.0/ccpstencil/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.470872 ccpstencil-0.6.0/ccpstencil/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/context/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/_alviss.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/_kwarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/jinjaext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_setfilename.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_skip_if.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/jinjaext/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/filters/_base64.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/shortcuts/_render_stencil.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/stencils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/structs/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/template/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/utils/_guessers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/ccpstencil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_skip_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_some_basic_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.736187 ccpstencil-0.6.1/ccpstencil/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.736187 ccpstencil-0.6.1/ccpstencil/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.736187 ccpstencil-0.6.1/ccpstencil/cli/ccp_stencil/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/cli/ccp_stencil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/cli/ccp_stencil/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/cli/ccp_stencil/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.736187 ccpstencil-0.6.1/ccpstencil/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/context/_alviss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/context/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/context/_kwarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.736187 ccpstencil-0.6.1/ccpstencil/jinjaext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.740187 ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/_setfilename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/_skip_if.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.740187 ccpstencil-0.6.1/ccpstencil/jinjaext/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/jinjaext/filters/_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.740187 ccpstencil-0.6.1/ccpstencil/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/renderer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/renderer/_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/renderer/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/renderer/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/renderer/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.740187 ccpstencil-0.6.1/ccpstencil/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/shortcuts/_render_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/stencils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.740187 ccpstencil-0.6.1/ccpstencil/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.740187 ccpstencil-0.6.1/ccpstencil/structs/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/interfaces/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/interfaces/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/structs/interfaces/_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/ccpstencil/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/template/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/template/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/template/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/ccpstencil/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/ccpstencil/utils/_guessers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/ccpstencil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 14:42:54.000000 ccpstencil-0.6.1/ccpstencil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 14:42:54.000000 ccpstencil-0.6.1/ccpstencil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:42:54.000000 ccpstencil-0.6.1/ccpstencil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 14:42:54.000000 ccpstencil-0.6.1/ccpstencil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 14:42:54.000000 ccpstencil-0.6.1/ccpstencil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 14:42:54.000000 ccpstencil-0.6.1/ccpstencil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:54.744187 ccpstencil-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/tests/test_skip_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 14:42:40.000000 ccpstencil-0.6.1/tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.6.0/LICENSE` & `ccpstencil-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/PKG-INFO` & `ccpstencil-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.6.0
+Version: 0.6.1
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.6.0/README.md` & `ccpstencil-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/_runner.py` & `ccpstencil-0.6.1/ccpstencil/cli/ccp_stencil/_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,17 @@
             sys.path.append(cwd)
 
     def run(self):
         self._make_cwd_importable()
         rnd = self.get_renderer()
         rnd.template = self.get_template()
         rnd.context = self.get_context()
-        rnd.render()
+        res = rnd.render()
+        if self.output:
+            print(f'Wrote file: {res}')
 
     def get_template(self) -> ITemplate:
         if self.template:
             return FileTemplate(self.template)
         else:
             return StringTemplate(self.string_template)
```

### Comparing `ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/main.py` & `ccpstencil-0.6.1/ccpstencil/cli/ccp_stencil/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     parser.add_argument('-v', '--verbose', action="store_true", help='Spits out DEBUG level logs')
 
     parser.add_argument('-i', '--input', nargs='?', help='Alviss file with input context (YAML or JSON)')
 
     parser.add_argument('-a', '--arg', action='append', help='Add additional Context arguments from the command line, e.g. -a foo=bar')
 
     parser.add_argument('-o', '--output', help='Path or file to write the results to (otherwise its just printed to stdout).'
-                                               ' If this is only a path, the name of the rendered file will be the same as the input template.',
+                                               ' If this is a path (ends with /), the name of the rendered file will be the same as the input template.',
                               default='', nargs='?')
     parser.add_argument('--no-overwrite', action="store_true", help='Makes sore existing output files are not overwritten')
 
     input_group = parser.add_mutually_exclusive_group(required=True)
     input_group.add_argument('-t', '--template', default='',
                              help='Template file to render')
     input_group.add_argument('-s', '--string-template', default='',
```

### Comparing `ccpstencil-0.6.0/ccpstencil/context/_alviss.py` & `ccpstencil-0.6.1/ccpstencil/context/_alviss.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/context/_dict.py` & `ccpstencil-0.6.1/ccpstencil/context/_dict.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_embed.py` & `ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_setfilename.py` & `ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/_setfilename.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_skip_if.py` & `ccpstencil-0.6.1/ccpstencil/jinjaext/extensions/_skip_if.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/renderer/_base.py` & `ccpstencil-0.6.1/ccpstencil/renderer/_base.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/renderer/_file.py` & `ccpstencil-0.6.1/ccpstencil/renderer/_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 __all__ = [
     'FileRenderer',
 ]
 
 from ccpstencil.structs import *
 from pathlib import Path
 from ._string import *
+import logging
+log = logging.getLogger(__file__)
 
 
 class FileRenderer(StringRenderer):
     def __init__(self, output_path: Union[str, Path],
                  context: Optional[IContext] = None, template: Optional[ITemplate] = None,
                  overwrite: bool = True,
                  **kwargs):
+        self._overwrite = overwrite
+        super().__init__(context, template, **kwargs)
+        is_dir = False
+        log.debug(f'{output_path=}')
         if isinstance(output_path, str):
+            if output_path.endswith('\\') or output_path.endswith('/'):
+                is_dir = True
             output_path = Path(output_path)
-        self._output_path: Path = output_path
-        if not self._output_path.is_dir():
-            self.output_file_name = self._output_path.name
-            self._output_path = self._output_path.parent
 
-        self._overwrite = overwrite
-        super().__init__(context, template, **kwargs)
+        if not is_dir:
+            self.output_file_name = str(output_path.name)
+            self._output_path = output_path.parent
+        else:
+            self._output_path = output_path
+
+        log.debug(f'{self._output_path=}')
+        log.debug(f'{self.output_file_name=}')
 
     def render(self) -> str:
         return super().render()
 
     def _output_rendered_results(self, rendered_string: str) -> str:
         results = self._render_as_string()
         fout_path = self.output_file()
@@ -56,8 +66,8 @@
             if isinstance(self._template, FileTemplate):
                 return self._template.get_file_path().name
 
         return None
 
     @output_file_name.setter
     def output_file_name(self, value: str):
-        self._output_file_name = value
+        self._output_file_name = value
```

### Comparing `ccpstencil-0.6.0/ccpstencil/renderer/_string.py` & `ccpstencil-0.6.1/ccpstencil/renderer/_string.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/structs/_errors.py` & `ccpstencil-0.6.1/ccpstencil/structs/_errors.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/structs/interfaces/_renderer.py` & `ccpstencil-0.6.1/ccpstencil/structs/interfaces/_renderer.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/template/_file.py` & `ccpstencil-0.6.1/ccpstencil/template/_file.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil/utils/_guessers.py` & `ccpstencil-0.6.1/ccpstencil/utils/_guessers.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/ccpstencil.egg-info/PKG-INFO` & `ccpstencil-0.6.1/ccpstencil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.6.0
+Version: 0.6.1
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.6.0/ccpstencil.egg-info/SOURCES.txt` & `ccpstencil-0.6.1/ccpstencil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/pyproject.toml` & `ccpstencil-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/tests/test_embed.py` & `ccpstencil-0.6.1/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/tests/test_filters.py` & `ccpstencil-0.6.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/tests/test_skip_if.py` & `ccpstencil-0.6.1/tests/test_skip_if.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.6.0/tests/test_some_basic_stuff.py` & `ccpstencil-0.6.1/tests/test_some_basic_stuff.py`

 * *Files identical despite different names*

