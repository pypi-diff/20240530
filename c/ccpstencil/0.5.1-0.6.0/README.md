# Comparing `tmp/ccpstencil-0.5.1.tar.gz` & `tmp/ccpstencil-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpstencil-0.5.1.tar", last modified: Thu May 30 12:24:38 2024, max compression
+gzip compressed data, was "ccpstencil-0.6.0.tar", last modified: Thu May 30 13:53:36 2024, max compression
```

## Comparing `ccpstencil-0.5.1.tar` & `ccpstencil-0.6.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.022874 ccpstencil-0.5.1/ccpstencil/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/context/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/_alviss.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/_kwarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/jinjaext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_skip_if.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/jinjaext/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/filters/_base64.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/shortcuts/_render_stencil.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/stencils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/structs/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/template/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/utils/_guessers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/ccpstencil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_skip_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_some_basic_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.470872 ccpstencil-0.6.0/ccpstencil/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.470872 ccpstencil-0.6.0/ccpstencil/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/_alviss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/context/_kwarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/jinjaext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_setfilename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_skip_if.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/jinjaext/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/jinjaext/filters/_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.474871 ccpstencil-0.6.0/ccpstencil/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/renderer/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/shortcuts/_render_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/stencils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/structs/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/structs/interfaces/_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/template/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/ccpstencil/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/ccpstencil/utils/_guessers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/ccpstencil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 13:53:36.000000 ccpstencil-0.6.0/ccpstencil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:53:36.482871 ccpstencil-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:53:36.478871 ccpstencil-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_skip_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 13:53:27.000000 ccpstencil-0.6.0/tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.5.1/LICENSE` & `ccpstencil-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/PKG-INFO` & `ccpstencil-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.5.1
+Version: 0.6.0
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.5.1/README.md` & `ccpstencil-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/_runner.py` & `ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/_runner.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/main.py` & `ccpstencil-0.6.0/ccpstencil/cli/ccp_stencil/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
     parser.add_argument('-v', '--verbose', action="store_true", help='Spits out DEBUG level logs')
 
     parser.add_argument('-i', '--input', nargs='?', help='Alviss file with input context (YAML or JSON)')
 
     parser.add_argument('-a', '--arg', action='append', help='Add additional Context arguments from the command line, e.g. -a foo=bar')
 
-    parser.add_argument('-o', '--output', help='File to write the results to (otherwise its just printed to stdout)',
+    parser.add_argument('-o', '--output', help='Path or file to write the results to (otherwise its just printed to stdout).'
+                                               ' If this is only a path, the name of the rendered file will be the same as the input template.',
                               default='', nargs='?')
     parser.add_argument('--no-overwrite', action="store_true", help='Makes sore existing output files are not overwritten')
 
     input_group = parser.add_mutually_exclusive_group(required=True)
     input_group.add_argument('-t', '--template', default='',
                              help='Template file to render')
     input_group.add_argument('-s', '--string-template', default='',
```

### Comparing `ccpstencil-0.5.1/ccpstencil/context/_alviss.py` & `ccpstencil-0.6.0/ccpstencil/context/_alviss.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil/context/_dict.py` & `ccpstencil-0.6.0/ccpstencil/context/_dict.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_embed.py` & `ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_embed.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 __all__ = [
     'EmbedExtension',
 ]
 
-import os
-from jinja2 import nodes, TemplateSyntaxError
+from jinja2 import nodes
 from jinja2.ext import Extension
-from ccptools.structs import *
+from ccpstencil.structs import *
+
 
 class EmbedExtension(Extension):
     tags = {'embed'}
 
     def __init__(self, environment):
         super().__init__(environment)
         environment.extend(stencil_renderer=None)
 
+    @property
+    def renderer(self) -> IRenderer:
+        return self.environment.stencil_renderer  # noqa
+
     def parse(self, parser):
         lineno = next(parser.stream).lineno
         args = [parser.parse_expression()]
         source_file = parser.filename
         kwargs = [nodes.Keyword('source_file', nodes.Const(source_file))]
         while parser.stream.skip_if('comma'):
             key = parser.stream.expect('name').value
@@ -25,25 +29,20 @@
             value = parser.parse_expression()
             kwargs.append(nodes.Keyword(key, value))
 
         return nodes.CallBlock(self.call_method('_render_embed', args, kwargs), [], [], []).set_lineno(lineno)
 
     def _render_embed(self, file_path, source_file: Optional[str] = None, indent: int = 0,
                       alviss: bool = False, env: bool = False,  caller=None, **kwargs):
-        # file_path = os.path.abspath(file_path)
-
-        c = caller()
-
-        caller_source = c.strip()
 
         # Check if file_path is a variable in the context
         if hasattr(file_path, '__call__'):
             file_path = file_path()
 
-        content = self.environment.stencil_renderer.get_embed(file_path, alviss=alviss, env=env)
+        content = self.renderer.get_embed(file_path, alviss=alviss, env=env)
 
         # Detect the current line's indentation level
         if indent:
             indent_str = ' '*indent
         else:
             indent_str = ''
```

### Comparing `ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_skip_if.py` & `ccpstencil-0.6.0/ccpstencil/jinjaext/extensions/_skip_if.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil/renderer/_base.py` & `ccpstencil-0.6.0/ccpstencil/renderer/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             self.template = template
         if kwargs:
             log.warning(f'Unrecognized kwargs for {self.__class__.__name__}: {kwargs}')
         self._search_paths: List[Path] = []
         self._load_search_paths()
         self._env: jinja2.Environment = self._make_environment()
         self._load_filters()
+        self._output_file_name: Optional[str] = None
 
     def _make_environment(self) -> jinja2.Environment:
         env = jinja2.Environment(
             lstrip_blocks=True,
             trim_blocks=True,
             keep_trailing_newline=True,
             undefined=jinja2.ChainableUndefined,
@@ -180,7 +181,23 @@
             return quickloader.render_load(abs_file_path,
                                            skip_env_loading=not env,
                                            skip_fidelius=not fidelius)
 
         else:
             with open(abs_file_path, 'r', newline=None) as fin:
                 return fin.read()
+
+    @property
+    def output_file_name(self) -> Optional[str]:
+        if self._output_file_name:
+            return self._output_file_name
+
+        if self._template:
+            from ccpstencil.template import FileTemplate
+            if isinstance(self._template, FileTemplate):
+                return self._template.get_file_path().name
+
+        return None
+
+    @output_file_name.setter
+    def output_file_name(self, value: str):
+        self._output_file_name = value or None
```

### Comparing `ccpstencil-0.5.1/ccpstencil/renderer/_file.py` & `ccpstencil-0.6.0/ccpstencil/renderer/_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,34 +4,60 @@
 
 from ccpstencil.structs import *
 from pathlib import Path
 from ._string import *
 
 
 class FileRenderer(StringRenderer):
-    def __init__(self, output_file: Union[str, Path],
+    def __init__(self, output_path: Union[str, Path],
                  context: Optional[IContext] = None, template: Optional[ITemplate] = None,
                  overwrite: bool = True,
                  **kwargs):
-        if isinstance(output_file, str):
-            output_file = Path(output_file)
-        self._output_file: Path = output_file
+        if isinstance(output_path, str):
+            output_path = Path(output_path)
+        self._output_path: Path = output_path
+        if not self._output_path.is_dir():
+            self.output_file_name = self._output_path.name
+            self._output_path = self._output_path.parent
+
         self._overwrite = overwrite
         super().__init__(context, template, **kwargs)
 
     def render(self) -> str:
         return super().render()
 
     def _output_rendered_results(self, rendered_string: str) -> str:
         results = self._render_as_string()
+        fout_path = self.output_file()
         if results is None:
-            return f'Skipped: {self._output_file.absolute()}'
+            return f'Skipped: {fout_path.absolute()}'
 
-        if self._output_file.exists() and not self._overwrite:
+        if fout_path.exists() and not self._overwrite:
             raise OutputFileExistsError(f'The target output file already exists and overwriting is'
-                                        f' disabled: {self._output_file.absolute()}')
-        self._output_file.parent.mkdir(parents=True, exist_ok=True)
+                                        f' disabled: {fout_path.absolute()}')
+        fout_path.parent.mkdir(parents=True, exist_ok=True)
 
-        with open(self._output_file, 'w') as fout:
+        with open(fout_path, 'w') as fout:
             fout.write(results)
-        return str(self._output_file.absolute())
+        return str(fout_path.absolute())
 
+    def output_file(self) -> Path:
+        name = self.output_file_name
+        if name is None:
+            raise NoOutputFileNameError('no output file name set or found')
+        return self._output_path / Path(self.output_file_name)
+
+    @property
+    def output_file_name(self) -> Optional[str]:
+        if self._output_file_name:
+            return self._output_file_name
+
+        if self._template:
+            from ccpstencil.template import FileTemplate
+            if isinstance(self._template, FileTemplate):
+                return self._template.get_file_path().name
+
+        return None
+
+    @output_file_name.setter
+    def output_file_name(self, value: str):
+        self._output_file_name = value
```

### Comparing `ccpstencil-0.5.1/ccpstencil/renderer/_string.py` & `ccpstencil-0.6.0/ccpstencil/renderer/_string.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil/structs/_errors.py` & `ccpstencil-0.6.0/ccpstencil/structs/_errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     'ContextError',
 
     'RenderError',
     'NoTemplateSetError',
     'InvalidContextTypeForRendererError',
     'InvalidTemplateTypeForRendererError',
     'OutputFileExistsError',
+    'NoOutputFileNameError',
     'EmbedFileNotFound',
 
     'CancelRendering',
 ]
 
 
 class StencilError(Exception):
@@ -49,13 +50,17 @@
     pass
 
 
 class OutputFileExistsError(RenderError, FileExistsError):
     pass
 
 
+class NoOutputFileNameError(RenderError, ValueError):
+    pass
+
+
 class EmbedFileNotFound(RenderError, FileNotFoundError):
     pass
 
 
 class CancelRendering(Exception):
     pass
```

### Comparing `ccpstencil-0.5.1/ccpstencil/structs/interfaces/_renderer.py` & `ccpstencil-0.6.0/ccpstencil/structs/interfaces/_renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,7 +44,17 @@
     @abc.abstractmethod
     def is_template_loadable(self, template_name: str) -> bool:
         pass
 
     @abc.abstractmethod
     def get_embed(self, file_path: str, source_file: Optional[str] = None, alviss: bool = False, env: bool = False) -> str:
         pass
+
+    @property
+    @abc.abstractmethod
+    def output_file_name(self) -> str:
+        pass
+
+    @output_file_name.setter
+    @abc.abstractmethod
+    def output_file_name(self, value: str):
+        pass
```

### Comparing `ccpstencil-0.5.1/ccpstencil/template/_file.py` & `ccpstencil-0.6.0/ccpstencil/template/_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 
 class FileTemplate(_BaseTemplate):
     def __init__(self, file_path: T_PATH, **kwargs):
         super().__init__(**kwargs)
         self._file_path: T_PATH = file_path
 
     def _read_file(self) -> str:
-        if isinstance(self._file_path, str):
-            as_path = Path(self._file_path)
-        else:
-            as_path = self._file_path
+        as_path = self.get_file_path()
+
         if not as_path.exists():
             raise TemplateNotFoundError(f'File {as_path} does not exist')
 
         with open(as_path, 'r') as fin:
             return fin.read()
 
+    def get_file_path(self) -> Path:
+        if isinstance(self._file_path, str):
+            return Path(self._file_path)
+        return self._file_path
+
     def get_jinja_template(self) -> jinja2.Template:
         if isinstance(self._file_path, str):
             try:
                 return self.renderer.jinja_environment.get_template(self._file_path)
             except jinja2.exceptions.TemplateNotFound:
                 pass
         template_string = self._read_file()
```

### Comparing `ccpstencil-0.5.1/ccpstencil/utils/_guessers.py` & `ccpstencil-0.6.0/ccpstencil/utils/_guessers.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/ccpstencil.egg-info/PKG-INFO` & `ccpstencil-0.6.0/ccpstencil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.5.1
+Version: 0.6.0
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.5.1/ccpstencil.egg-info/SOURCES.txt` & `ccpstencil-0.6.0/ccpstencil.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ccpstencil/context/__init__.py
 ccpstencil/context/_alviss.py
 ccpstencil/context/_dict.py
 ccpstencil/context/_kwarg.py
 ccpstencil/jinjaext/__init__.py
 ccpstencil/jinjaext/extensions/__init__.py
 ccpstencil/jinjaext/extensions/_embed.py
+ccpstencil/jinjaext/extensions/_setfilename.py
 ccpstencil/jinjaext/extensions/_skip_if.py
 ccpstencil/jinjaext/filters/__init__.py
 ccpstencil/jinjaext/filters/_base64.py
 ccpstencil/renderer/__init__.py
 ccpstencil/renderer/_base.py
 ccpstencil/renderer/_dir.py
 ccpstencil/renderer/_file.py
```

### Comparing `ccpstencil-0.5.1/pyproject.toml` & `ccpstencil-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/tests/test_embed.py` & `ccpstencil-0.6.0/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/tests/test_filters.py` & `ccpstencil-0.6.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/tests/test_skip_if.py` & `ccpstencil-0.6.0/tests/test_skip_if.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.1/tests/test_some_basic_stuff.py` & `ccpstencil-0.6.0/tests/test_some_basic_stuff.py`

 * *Files identical despite different names*

