# Comparing `tmp/ccpstencil-0.5.0.tar.gz` & `tmp/ccpstencil-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpstencil-0.5.0.tar", last modified: Thu May 30 11:50:14 2024, max compression
+gzip compressed data, was "ccpstencil-0.5.1.tar", last modified: Thu May 30 12:24:38 2024, max compression
```

## Comparing `ccpstencil-0.5.0.tar` & `ccpstencil-0.5.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.566635 ccpstencil-0.5.0/ccpstencil/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/cli/ccp_stencil/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/cli/ccp_stencil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/cli/ccp_stencil/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/cli/ccp_stencil/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/context/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/context/_alviss.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/context/_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/context/_kwarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/jinjaext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/jinjaext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/jinjaext/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/jinjaext/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/jinjaext/extensions/_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/jinjaext/extensions/_skip_if.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/jinjaext/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/jinjaext/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/jinjaext/filters/_base64.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.570635 ccpstencil-0.5.0/ccpstencil/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/renderer/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/renderer/_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/renderer/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/renderer/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/renderer/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/ccpstencil/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/shortcuts/_render_stencil.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/stencils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/ccpstencil/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/ccpstencil/structs/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/interfaces/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/interfaces/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/structs/interfaces/_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/ccpstencil/template/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/template/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/template/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/template/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/ccpstencil/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/ccpstencil/utils/_guessers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/ccpstencil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 11:50:14.000000 ccpstencil-0.5.0/ccpstencil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 11:50:14.000000 ccpstencil-0.5.0/ccpstencil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:50:14.000000 ccpstencil-0.5.0/ccpstencil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 11:50:14.000000 ccpstencil-0.5.0/ccpstencil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 11:50:14.000000 ccpstencil-0.5.0/ccpstencil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 11:50:14.000000 ccpstencil-0.5.0/ccpstencil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:14.574635 ccpstencil-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/tests/test_skip_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 11:50:03.000000 ccpstencil-0.5.0/tests/test_some_basic_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.022874 ccpstencil-0.5.1/ccpstencil/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/_alviss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/context/_kwarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/jinjaext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_skip_if.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.026874 ccpstencil-0.5.1/ccpstencil/jinjaext/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/jinjaext/filters/_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/renderer/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/shortcuts/_render_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/stencils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/structs/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/structs/interfaces/_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/template/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.030875 ccpstencil-0.5.1/ccpstencil/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/ccpstencil/utils/_guessers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/ccpstencil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 12:24:37.000000 ccpstencil-0.5.1/ccpstencil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:24:38.034875 ccpstencil-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_skip_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 12:24:29.000000 ccpstencil-0.5.1/tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.5.0/LICENSE` & `ccpstencil-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/PKG-INFO` & `ccpstencil-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.5.0
+Version: 0.5.1
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.5.0/README.md` & `ccpstencil-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/cli/ccp_stencil/_runner.py` & `ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 __all__ = [
     'StencilRunner',
 ]
+import os
+import sys
 from ccptools.structs import *
 from ccpstencil.stencils import *
 import logging
 log = logging.getLogger(__file__)
 
 
 class StencilRunner:
@@ -16,15 +18,23 @@
 
         self.input: Optional[str] = None
         self.additional_arg_list: List[str] = []
 
         self.output: Optional[str] = None
         self.no_overwrite: bool = False
 
+    def _make_cwd_importable(self):
+        cwd = os.getcwd()
+        if self.verbose:
+            log.debug(f'os.getcwd()={cwd}')
+        if cwd not in sys.path:
+            sys.path.append(cwd)
+
     def run(self):
+        self._make_cwd_importable()
         rnd = self.get_renderer()
         rnd.template = self.get_template()
         rnd.context = self.get_context()
         rnd.render()
 
     def get_template(self) -> ITemplate:
         if self.template:
```

### Comparing `ccpstencil-0.5.0/ccpstencil/cli/ccp_stencil/main.py` & `ccpstencil-0.5.1/ccpstencil/cli/ccp_stencil/main.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/context/_alviss.py` & `ccpstencil-0.5.1/ccpstencil/context/_alviss.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/context/_dict.py` & `ccpstencil-0.5.1/ccpstencil/context/_dict.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/jinjaext/extensions/_embed.py` & `ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/jinjaext/extensions/_skip_if.py` & `ccpstencil-0.5.1/ccpstencil/jinjaext/extensions/_skip_if.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/renderer/_base.py` & `ccpstencil-0.5.1/ccpstencil/renderer/_base.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/renderer/_file.py` & `ccpstencil-0.5.1/ccpstencil/renderer/_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self._overwrite = overwrite
         super().__init__(context, template, **kwargs)
 
     def render(self) -> str:
         return super().render()
 
     def _output_rendered_results(self, rendered_string: str) -> str:
-        results = super().render()
+        results = self._render_as_string()
         if results is None:
             return f'Skipped: {self._output_file.absolute()}'
 
         if self._output_file.exists() and not self._overwrite:
             raise OutputFileExistsError(f'The target output file already exists and overwriting is'
                                         f' disabled: {self._output_file.absolute()}')
         self._output_file.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `ccpstencil-0.5.0/ccpstencil/renderer/_string.py` & `ccpstencil-0.5.1/ccpstencil/renderer/_string.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/structs/_errors.py` & `ccpstencil-0.5.1/ccpstencil/structs/_errors.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/structs/interfaces/_renderer.py` & `ccpstencil-0.5.1/ccpstencil/structs/interfaces/_renderer.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/template/_file.py` & `ccpstencil-0.5.1/ccpstencil/template/_file.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil/utils/_guessers.py` & `ccpstencil-0.5.1/ccpstencil/utils/_guessers.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/ccpstencil.egg-info/PKG-INFO` & `ccpstencil-0.5.1/ccpstencil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.5.0
+Version: 0.5.1
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.5.0/ccpstencil.egg-info/SOURCES.txt` & `ccpstencil-0.5.1/ccpstencil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/pyproject.toml` & `ccpstencil-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/tests/test_embed.py` & `ccpstencil-0.5.1/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/tests/test_filters.py` & `ccpstencil-0.5.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/tests/test_skip_if.py` & `ccpstencil-0.5.1/tests/test_skip_if.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.5.0/tests/test_some_basic_stuff.py` & `ccpstencil-0.5.1/tests/test_some_basic_stuff.py`

 * *Files identical despite different names*

