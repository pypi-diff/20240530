# Comparing `tmp/ccpstencil-0.3.0.tar.gz` & `tmp/ccpstencil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpstencil-0.3.0.tar", last modified: Tue May 28 17:41:07 2024, max compression
+gzip compressed data, was "ccpstencil-0.4.0.tar", last modified: Thu May 30 09:51:22 2024, max compression
```

## Comparing `ccpstencil-0.3.0.tar` & `ccpstencil-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.232651 ccpstencil-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-28 17:41:07.232651 ccpstencil-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.220651 ccpstencil-0.3.0/ccpstencil/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.224651 ccpstencil-0.3.0/ccpstencil/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.224651 ccpstencil-0.3.0/ccpstencil/cli/ccp_stencil/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/cli/ccp_stencil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/cli/ccp_stencil/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/cli/ccp_stencil/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.224651 ccpstencil-0.3.0/ccpstencil/context/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/context/_alviss.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/context/_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/context/_kwarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.224651 ccpstencil-0.3.0/ccpstencil/jinjaext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/jinjaext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.224651 ccpstencil-0.3.0/ccpstencil/jinjaext/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/jinjaext/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/jinjaext/extensions/_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.224651 ccpstencil-0.3.0/ccpstencil/jinjaext/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/jinjaext/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/jinjaext/filters/_base64.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/renderer/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/renderer/_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/renderer/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/renderer/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/renderer/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/shortcuts/_render_stencil.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/stencils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil/structs/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/interfaces/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/interfaces/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/structs/interfaces/_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil/template/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/template/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/template/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/template/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/ccpstencil/utils/_guessers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/ccpstencil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-28 17:41:07.000000 ccpstencil-0.3.0/ccpstencil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-28 17:41:07.000000 ccpstencil-0.3.0/ccpstencil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:41:07.000000 ccpstencil-0.3.0/ccpstencil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 17:41:07.000000 ccpstencil-0.3.0/ccpstencil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 17:41:07.000000 ccpstencil-0.3.0/ccpstencil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 17:41:07.000000 ccpstencil-0.3.0/ccpstencil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:41:07.232651 ccpstencil-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:41:07.228651 ccpstencil-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-28 17:40:55.000000 ccpstencil-0.3.0/tests/test_some_basic_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.204393 ccpstencil-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-30 09:51:22.204393 ccpstencil-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.196393 ccpstencil-0.4.0/ccpstencil/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.196393 ccpstencil-0.4.0/ccpstencil/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.196393 ccpstencil-0.4.0/ccpstencil/cli/ccp_stencil/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/cli/ccp_stencil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/cli/ccp_stencil/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/cli/ccp_stencil/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.196393 ccpstencil-0.4.0/ccpstencil/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/context/_alviss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/context/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/context/_kwarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.196393 ccpstencil-0.4.0/ccpstencil/jinjaext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/jinjaext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/jinjaext/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/jinjaext/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/jinjaext/extensions/_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/jinjaext/extensions/_skip_if.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/jinjaext/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/jinjaext/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/jinjaext/filters/_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/renderer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/renderer/_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/renderer/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/renderer/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/renderer/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/shortcuts/_render_stencil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/stencils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/structs/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/interfaces/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/interfaces/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/structs/interfaces/_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.200393 ccpstencil-0.4.0/ccpstencil/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/template/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/template/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/template/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.204393 ccpstencil-0.4.0/ccpstencil/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/ccpstencil/utils/_guessers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.204393 ccpstencil-0.4.0/ccpstencil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-30 09:51:22.000000 ccpstencil-0.4.0/ccpstencil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:51:22.000000 ccpstencil-0.4.0/ccpstencil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:51:22.000000 ccpstencil-0.4.0/ccpstencil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 09:51:22.000000 ccpstencil-0.4.0/ccpstencil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 09:51:22.000000 ccpstencil-0.4.0/ccpstencil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 09:51:22.000000 ccpstencil-0.4.0/ccpstencil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:51:22.204393 ccpstencil-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:51:22.204393 ccpstencil-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/tests/test_skip_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 09:51:12.000000 ccpstencil-0.4.0/tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.3.0/LICENSE` & `ccpstencil-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/PKG-INFO` & `ccpstencil-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.3.0
+Version: 0.4.0
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.3.0/README.md` & `ccpstencil-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/cli/ccp_stencil/_runner.py` & `ccpstencil-0.4.0/ccpstencil/cli/ccp_stencil/_runner.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/cli/ccp_stencil/main.py` & `ccpstencil-0.4.0/ccpstencil/cli/ccp_stencil/main.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/context/_alviss.py` & `ccpstencil-0.4.0/ccpstencil/context/_alviss.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/context/_dict.py` & `ccpstencil-0.4.0/ccpstencil/context/_dict.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/jinjaext/extensions/_embed.py` & `ccpstencil-0.4.0/ccpstencil/jinjaext/extensions/_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/renderer/_base.py` & `ccpstencil-0.4.0/ccpstencil/renderer/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,21 +121,30 @@
     @template.setter
     def template(self, value: ITemplate):
         if not self._is_valid_template(value):
             raise InvalidTemplateTypeForRendererError(f'Template of {value.__class__.__name__} type does not work with a {self.__class__.__name__} Renderer')
         value.set_renderer(self)
         self._template = value
 
-    @abc.abstractmethod
     def render(self):
-        """This should just be called by subclasses via super().render() in
-        order to run preflight and common stuff, but the empty return value
-        should be ignored.
-        """
         self._pre_flight()
+        try:
+            rendered_string = self._render_as_string()
+            return self._output_rendered_results(rendered_string)
+        except CancelRendering:
+            log.info(f'Rendering cancelled by skip_if tag')
+            return None
+
+    @abc.abstractmethod
+    def _output_rendered_results(self, rendered_string: str):
+        pass
+
+    @abc.abstractmethod
+    def _render_as_string(self) -> str:
+        pass
 
     @property
     def jinja_environment(self) -> jinja2.Environment:
         return self._env
 
     def is_template_loadable(self, template_name: str) -> bool:
         try:
```

### Comparing `ccpstencil-0.3.0/ccpstencil/renderer/_file.py` & `ccpstencil-0.4.0/ccpstencil/renderer/_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,13 +15,23 @@
         if isinstance(output_file, str):
             output_file = Path(output_file)
         self._output_file: Path = output_file
         self._overwrite = overwrite
         super().__init__(context, template, **kwargs)
 
     def render(self) -> str:
+        return super().render()
+
+    def _output_rendered_results(self, rendered_string: str) -> str:
+        results = super().render()
+        if results is None:
+            return f'Skipped: {self._output_file.absolute()}'
+
         if self._output_file.exists() and not self._overwrite:
-            raise OutputFileExistsError(f'The target output file already exists and overwriting is disabled: {self._output_file.absolute()}')
+            raise OutputFileExistsError(f'The target output file already exists and overwriting is'
+                                        f' disabled: {self._output_file.absolute()}')
         self._output_file.parent.mkdir(parents=True, exist_ok=True)
+
         with open(self._output_file, 'w') as fout:
-            fout.write(super().render())
+            fout.write(results)
         return str(self._output_file.absolute())
+
```

### Comparing `ccpstencil-0.3.0/ccpstencil/structs/_errors.py` & `ccpstencil-0.4.0/ccpstencil/structs/_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
     'RenderError',
     'NoTemplateSetError',
     'InvalidContextTypeForRendererError',
     'InvalidTemplateTypeForRendererError',
     'OutputFileExistsError',
     'EmbedFileNotFound',
+
+    'CancelRendering',
 ]
 
 
 class StencilError(Exception):
     pass
 
 
@@ -49,7 +51,11 @@
 
 class OutputFileExistsError(RenderError, FileExistsError):
     pass
 
 
 class EmbedFileNotFound(RenderError, FileNotFoundError):
     pass
+
+
+class CancelRendering(Exception):
+    pass
```

### Comparing `ccpstencil-0.3.0/ccpstencil/structs/interfaces/_renderer.py` & `ccpstencil-0.4.0/ccpstencil/structs/interfaces/_renderer.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/template/_file.py` & `ccpstencil-0.4.0/ccpstencil/template/_file.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil/utils/_guessers.py` & `ccpstencil-0.4.0/ccpstencil/utils/_guessers.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/ccpstencil.egg-info/PKG-INFO` & `ccpstencil-0.4.0/ccpstencil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpstencil
-Version: 0.3.0
+Version: 0.4.0
 Summary: An Alviss powered Template renderer where the context input can be files and entire directory structures can be rendered.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ccpstencil-0.3.0/ccpstencil.egg-info/SOURCES.txt` & `ccpstencil-0.4.0/ccpstencil.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ccpstencil/context/__init__.py
 ccpstencil/context/_alviss.py
 ccpstencil/context/_dict.py
 ccpstencil/context/_kwarg.py
 ccpstencil/jinjaext/__init__.py
 ccpstencil/jinjaext/extensions/__init__.py
 ccpstencil/jinjaext/extensions/_embed.py
+ccpstencil/jinjaext/extensions/_skip_if.py
 ccpstencil/jinjaext/filters/__init__.py
 ccpstencil/jinjaext/filters/_base64.py
 ccpstencil/renderer/__init__.py
 ccpstencil/renderer/_base.py
 ccpstencil/renderer/_dir.py
 ccpstencil/renderer/_file.py
 ccpstencil/renderer/_stdout.py
@@ -43,8 +44,9 @@
 ccpstencil/template/_base.py
 ccpstencil/template/_file.py
 ccpstencil/template/_string.py
 ccpstencil/utils/__init__.py
 ccpstencil/utils/_guessers.py
 tests/test_embed.py
 tests/test_filters.py
+tests/test_skip_if.py
 tests/test_some_basic_stuff.py
```

### Comparing `ccpstencil-0.3.0/pyproject.toml` & `ccpstencil-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/tests/test_embed.py` & `ccpstencil-0.4.0/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/tests/test_filters.py` & `ccpstencil-0.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ccpstencil-0.3.0/tests/test_some_basic_stuff.py` & `ccpstencil-0.4.0/tests/test_some_basic_stuff.py`

 * *Files identical despite different names*

