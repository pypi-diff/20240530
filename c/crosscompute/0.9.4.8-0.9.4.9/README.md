# Comparing `tmp/crosscompute-0.9.4.8.tar.gz` & `tmp/crosscompute-0.9.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-0.9.4.8.tar", last modified: Fri May 19 19:43:47 2023, max compression
+gzip compressed data, was "crosscompute-0.9.4.9.tar", last modified: Sat May 20 03:27:31 2023, max compression
```

## Comparing `crosscompute-0.9.4.8.tar` & `crosscompute-0.9.4.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.130337 crosscompute-0.9.4.8/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4967 2023-05-19 19:43:47.130337 crosscompute-0.9.4.8/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.120337 crosscompute-0.9.4.8/crosscompute/
--rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-27 21:47:32.000000 crosscompute-0.9.4.8/crosscompute/__init__.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/__main__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.125337 crosscompute-0.9.4.8/crosscompute/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)    15561 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/LogoBrand-Horizontal-20230501.svg
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1630 2023-05-19 19:24:21.000000 crosscompute-0.9.4.8/crosscompute/assets/automation.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1006 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/base.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/button-panel.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      749 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      121 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)    13854 2023-05-19 19:17:25.000000 crosscompute-0.9.4.8/crosscompute/assets/configuration.yml
--rw-r--r--   0 rhh       (1000) rhh       (1000)      568 2023-05-19 19:41:05.000000 crosscompute-0.9.4.8/crosscompute/assets/default.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/embedded.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/favicon.ico
--rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/file-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/file-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      737 2023-05-19 19:41:05.000000 crosscompute-0.9.4.8/crosscompute/assets/flex.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)      108 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/frame-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       99 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/frame-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/image-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/image-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/json-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-05-16 21:06:41.000000 crosscompute-0.9.4.8/crosscompute/assets/json-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      408 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/link-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       98 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/link-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2556 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/live.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      323 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/markdown-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      148 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/markdown-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/pdf-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-05-16 21:07:00.000000 crosscompute-0.9.4.8/crosscompute/assets/pdf-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/pdf.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      660 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      118 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-05-15 19:34:28.000000 crosscompute-0.9.4.8/crosscompute/assets/root.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3275 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/step-body.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1021 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/step.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/string-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/string-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      479 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/string-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      128 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/string-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/table-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-05-16 21:07:09.000000 crosscompute-0.9.4.8/crosscompute/assets/table-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/text-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/text-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      131 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/text-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      144 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/text-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3287 2023-05-19 19:17:57.000000 crosscompute-0.9.4.8/crosscompute/constants.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-03-30 19:34:16.000000 crosscompute-0.9.4.8/crosscompute/dependencies.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2022-12-12 19:44:41.000000 crosscompute-0.9.4.8/crosscompute/exceptions.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.126337 crosscompute-0.9.4.8/crosscompute/macros/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/macros/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/macros/disk.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1551 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/macros/iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/macros/log.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-03-14 16:37:10.000000 crosscompute-0.9.4.8/crosscompute/macros/package.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/macros/security.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.127337 crosscompute-0.9.4.8/crosscompute/routers/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/routers/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6373 2023-05-19 19:39:24.000000 crosscompute-0.9.4.8/crosscompute/routers/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/file.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3451 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/root.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/stream.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      517 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/token.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.128337 crosscompute-0.9.4.8/crosscompute/routines/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-05-16 17:05:41.000000 crosscompute-0.9.4.8/crosscompute/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3401 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/authorization.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4806 2023-05-15 19:34:28.000000 crosscompute-0.9.4.8/crosscompute/routines/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3508 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/batch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    43690 2023-05-19 19:19:15.000000 crosscompute-0.9.4.8/crosscompute/routines/configuration.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    10401 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/database.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1333 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/interface.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1428 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/log.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2429 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/mutation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6177 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/printer.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6803 2023-05-15 19:34:28.000000 crosscompute-0.9.4.8/crosscompute/routines/server.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     9981 2023-05-19 19:39:37.000000 crosscompute-0.9.4.8/crosscompute/routines/step.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      699 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/uri.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    30435 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    28816 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/work.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.129336 crosscompute-0.9.4.8/crosscompute/scripts/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/scripts/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3870 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/scripts/configure.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3846 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/scripts/launch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/scripts/print.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/scripts/run.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/scripts/serve.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1403 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/settings.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.120337 crosscompute-0.9.4.8/crosscompute.egg-info/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     4967 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/PKG-INFO
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     3449 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/SOURCES.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/dependency_links.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      831 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/entry_points.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      427 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/requires.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       13 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/top_level.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2022-01-21 22:12:56.000000 crosscompute-0.9.4.8/crosscompute.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3257 2023-05-19 19:43:47.131337 crosscompute-0.9.4.8/setup.cfg
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.130337 crosscompute-0.9.4.8/tests/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      665 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/tests/test_constants.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/tests/test_macros_iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/tests/test_macros_security.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-27 21:47:32.000000 crosscompute-0.9.4.8/tests/test_routines_configuration.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2294 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/tests/test_routines_variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-27 21:47:32.000000 crosscompute-0.9.4.8/tests/test_routines_work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.346191 crosscompute-0.9.4.9/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4967 2023-05-20 03:27:31.346191 crosscompute-0.9.4.9/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.326191 crosscompute-0.9.4.9/crosscompute/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/__main__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.337191 crosscompute-0.9.4.9/crosscompute/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    15561 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/assets/LogoBrand-Horizontal-20230501.svg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1630 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/assets/automation.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1006 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/assets/base.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/button-panel.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/checkbox-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/checkbox-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      749 2023-05-18 16:36:35.000000 crosscompute-0.9.4.9/crosscompute/assets/checkbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      121 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/checkbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    13998 2023-05-20 03:25:16.000000 crosscompute-0.9.4.9/crosscompute/assets/configuration.yml
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      568 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/assets/default.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/embedded.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/favicon.ico
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/file-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/file-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      737 2023-05-18 03:23:16.000000 crosscompute-0.9.4.9/crosscompute/assets/flex.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      108 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/frame-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       99 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/frame-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/image-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/image-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/json-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/json-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      408 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/link-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       98 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/link-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2556 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/live.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      323 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/markdown-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      148 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/markdown-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/pdf-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/pdf-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/pdf.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/radio-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/radio-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      660 2023-05-18 15:46:32.000000 crosscompute-0.9.4.9/crosscompute/assets/radio-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      118 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/radio-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/root.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3275 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/step-body.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1028 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/assets/step.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/string-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/string-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      479 2023-05-18 19:24:46.000000 crosscompute-0.9.4.9/crosscompute/assets/string-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      128 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/string-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/table-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/table-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/text-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/assets/text-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      131 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/text-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      144 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/assets/text-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3331 2023-05-20 03:25:43.000000 crosscompute-0.9.4.9/crosscompute/constants.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/dependencies.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/exceptions.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.338191 crosscompute-0.9.4.9/crosscompute/macros/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/macros/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/macros/disk.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1551 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/macros/iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/macros/log.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      597 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/macros/package.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/macros/security.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.341191 crosscompute-0.9.4.9/crosscompute/routers/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/routers/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6373 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/routers/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/routers/file.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3451 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/routers/root.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-05-17 13:20:05.000000 crosscompute-0.9.4.9/crosscompute/routers/stream.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      517 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/routers/token.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.343191 crosscompute-0.9.4.9/crosscompute/routines/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3401 2023-05-18 03:23:16.000000 crosscompute-0.9.4.9/crosscompute/routines/authorization.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4806 2023-05-16 05:10:47.000000 crosscompute-0.9.4.9/crosscompute/routines/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3508 2023-05-18 03:23:16.000000 crosscompute-0.9.4.9/crosscompute/routines/batch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    43680 2023-05-20 03:17:27.000000 crosscompute-0.9.4.9/crosscompute/routines/configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    10401 2023-05-18 03:23:16.000000 crosscompute-0.9.4.9/crosscompute/routines/database.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1333 2023-05-17 07:19:39.000000 crosscompute-0.9.4.9/crosscompute/routines/interface.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1428 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/routines/log.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2429 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/routines/mutation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6177 2023-05-16 05:10:47.000000 crosscompute-0.9.4.9/crosscompute/routines/printer.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6803 2023-05-16 05:10:47.000000 crosscompute-0.9.4.9/crosscompute/routines/server.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    10524 2023-05-20 01:58:27.000000 crosscompute-0.9.4.9/crosscompute/routines/step.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      699 2023-05-17 06:49:42.000000 crosscompute-0.9.4.9/crosscompute/routines/uri.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    30435 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/routines/variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    28816 2023-05-17 09:02:06.000000 crosscompute-0.9.4.9/crosscompute/routines/work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.344191 crosscompute-0.9.4.9/crosscompute/scripts/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/scripts/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3870 2023-05-18 03:23:16.000000 crosscompute-0.9.4.9/crosscompute/scripts/configure.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3846 2023-05-18 03:23:16.000000 crosscompute-0.9.4.9/crosscompute/scripts/launch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/scripts/print.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/scripts/run.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/crosscompute/scripts/serve.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1403 2023-05-20 01:27:27.000000 crosscompute-0.9.4.9/crosscompute/settings.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.327191 crosscompute-0.9.4.9/crosscompute.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4967 2023-05-20 03:27:31.000000 crosscompute-0.9.4.9/crosscompute.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3449 2023-05-20 03:27:31.000000 crosscompute-0.9.4.9/crosscompute.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-20 03:27:31.000000 crosscompute-0.9.4.9/crosscompute.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      831 2023-05-20 03:27:31.000000 crosscompute-0.9.4.9/crosscompute.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      427 2023-05-20 03:27:31.000000 crosscompute-0.9.4.9/crosscompute.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-05-20 03:27:31.000000 crosscompute-0.9.4.9/crosscompute.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-16 05:34:11.000000 crosscompute-0.9.4.9/crosscompute.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3257 2023-05-20 03:27:31.347191 crosscompute-0.9.4.9/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:27:31.346191 crosscompute-0.9.4.9/tests/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      665 2023-05-18 17:52:57.000000 crosscompute-0.9.4.9/tests/test_constants.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      168 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/tests/test_macros_iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/tests/test_macros_security.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/tests/test_routines_configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2294 2023-05-17 07:00:02.000000 crosscompute-0.9.4.9/tests/test_routines_variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-05-01 17:04:24.000000 crosscompute-0.9.4.9/tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.4.8/LICENSE.md` & `crosscompute-0.9.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/PKG-INFO` & `crosscompute-0.9.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.8
+Version: 0.9.4.9
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://docs.crosscompute.com
```

### Comparing `crosscompute-0.9.4.8/README.md` & `crosscompute-0.9.4.9/README.md`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/LogoBrand-Horizontal-20230501.svg` & `crosscompute-0.9.4.9/crosscompute/assets/LogoBrand-Horizontal-20230501.svg`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/automation.html` & `crosscompute-0.9.4.9/crosscompute/assets/automation.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/base.html` & `crosscompute-0.9.4.9/crosscompute/assets/base.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/checkbox-input.html` & `crosscompute-0.9.4.9/crosscompute/assets/checkbox-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/checkbox-output-header.js` & `crosscompute-0.9.4.9/crosscompute/assets/checkbox-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/configuration.yml` & `crosscompute-0.9.4.9/crosscompute/assets/configuration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,40 @@
 # Documentation: https://docs.crosscompute.com
 # Forum: https://forum.crosscompute.com
 # Gallery: https://crosscompute.net
 
 # crosscompute version determines how this file is interpreted (required)
 crosscompute: 0.0.0
 
-# copyright declares who owns the rights to this work
-copyright_name: CrossCompute
-copyright_uri: https://crosscompute.com
-copyright_year: 2023
-attribution_text: >-
-  [![CrossCompute](/assets/logo.svg)]({copyright_uri}) © {copyright_year}.
-  Made with the
-  [CrossCompute Software Development Kit](https://docs.crosscompute.com).
-
 # name summarizes what your automation does
 name: Automation X
-
 # slug customizes the automation uri
 slug: automation-x
-
 # title sets the page title
 title: Automation X - Improve health, safety, quality of life
-
 # description explains why your automation is useful
 description: Improve health, safety, quality of life in our communities
-
 # version should increment after you make changes to your automation
 version: 0.0.0
 
+# copyright declares who owns the rights to this work
+copyright_name: CrossCompute
+copyright_uri: https://crosscompute.com
+copyright_year: 2023
+attribution_text: >-
+  [<img src="/assets/logo.svg" alt="{copyright_name}" loading="lazy">](
+  {copyright_uri}) © {copyright_year}. Made with the [CrossCompute Analytics
+  Software Development Kit](https://docs.crosscompute.com).
+
 # imports let you embed other automations in this automation
 imports:
   # id references this import in your templates when embedding;
   # path specifies the location of the automation file to import (required)
-  - id: automation-a
-    path: automation-a/automate.yml
+  - id: abc
+    path: abc/automate.yml
 
 # input is how your scripts get data from the user
 input:
 
   # input variables are provided to your scripts from the user or from batches
   variables:
     # id references this variable in your templates (required);
@@ -302,15 +298,17 @@
   # podman is a container engine (see https://podman.io);
   # unsafe means that the scripts will run directly on your machine
   engine: podman
 
   # image is the container used to run your scripts when using podman engine
   image: python
 
-  # packages are installed in the container when using podman engine
+  # packages are dependencies required by your scripts
+  # engine=unsafe will install the packages directly on your machine
+  # engine=podman will install the packages in the container image
   packages:
     # id is the name of the package as defined in the package manager
     # manager is the name of a package manager such as apt, dnf, npm, pip
     - id: matplotlib
       manager: pip
 
   # ports expose server processes running in your scripts
```

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/default.css` & `crosscompute-0.9.4.9/crosscompute/assets/default.css`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/favicon.ico` & `crosscompute-0.9.4.9/crosscompute/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/file-input-header.js` & `crosscompute-0.9.4.9/crosscompute/assets/file-input-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/flex.css` & `crosscompute-0.9.4.9/crosscompute/assets/flex.css`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/live.html` & `crosscompute-0.9.4.9/crosscompute/assets/live.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/radio-input.html` & `crosscompute-0.9.4.9/crosscompute/assets/radio-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/radio-output-header.js` & `crosscompute-0.9.4.9/crosscompute/assets/radio-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/step-body.js` & `crosscompute-0.9.4.9/crosscompute/assets/step-body.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/step.html` & `crosscompute-0.9.4.9/crosscompute/assets/step.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 {% block header_html %}
 {% if not for_embed and not for_print %}
 {% set absolute_automation_uri = root_uri + automation_definition.uri %}
 {% set absolute_batch_uri = absolute_automation_uri + batch_definition.uri %}
 <nav class="_breadcrumb" aria-label="breadcrumb">
 <ul>
-<li><a href="{{ root_uri or '/' }}">Root</a></li>
+<li><a href="{{ root_uri or '/' }}">Automations</a></li>
 <li><a href="{{ absolute_automation_uri }}">{{ automation_definition.name }}</a></li>
 <li>{{ batch_definition.name }}</li>
 <li>
 {% for a_step_name, variable_definitions in automation_definition.variable_definitions_by_step_name.items() if a_step_name != 'debug' and variable_definitions %}
 {% set is_this = a_step_name == step_name %}
 {% if is_this %}
 <b>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends live_template_path %} {% block header_html %} {% if not for_embed
 and not for_print %} {% set absolute_automation_uri = root_uri +
 automation_definition.uri %} {% set absolute_batch_uri =
 absolute_automation_uri + batch_definition.uri %}
-    * _R_o_o_t
+    * _A_u_t_o_m_a_t_i_o_n_s
     * _{_{_ _a_u_t_o_m_a_t_i_o_n___d_e_f_i_n_i_t_i_o_n_._n_a_m_e_ _}_}
     * {{ batch_definition.name }}
     * {% for a_step_name, variable_definitions in
       automation_definition.variable_definitions_by_step_name.items() if
       a_step_name != 'debug' and variable_definitions %} {% set is_this =
       a_step_name == step_name %} {% if is_this %} {{%% eennddiiff %%}} % if is_this
       %}aria-current="page"{% endif %}>{{ a_step_name }}
```

### Comparing `crosscompute-0.9.4.8/crosscompute/assets/table-output-header.js` & `crosscompute-0.9.4.9/crosscompute/assets/table-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/constants.py` & `crosscompute-0.9.4.9/crosscompute/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,17 @@
 AUTOMATION_NAME = 'Automation X'
 AUTOMATION_VERSION = '0.0.0'
 AUTOMATION_PATH = Path('automate.yml')
 COPYRIGHT_NAME = 'CrossCompute'
 COPYRIGHT_URI = 'https://crosscompute.com'
 COPYRIGHT_YEAR = datetime.now().year
 ATTRIBUTION_TEXT = '''
-[![CrossCompute](/assets/logo.svg)]({copyright_uri}) © {copyright_year}.
-Made with the
-[CrossCompute Software Development Kit](https://docs.crosscompute.com).
+[<img src="/assets/logo.svg" alt="{copyright_name}" loading="lazy">](
+{copyright_uri}) © {copyright_year}. Made with the [CrossCompute Analytics
+Software Development Kit](https://docs.crosscompute.com).
 '''.strip()
 LOGO_PATH = ASSETS_FOLDER / 'LogoBrand-Horizontal-20230501.svg'
 
 
 HOST = '127.0.0.1'
 PORT = 7000
 DISK_DEBOUNCE_IN_MILLISECONDS = 1600
```

### Comparing `crosscompute-0.9.4.8/crosscompute/dependencies.py` & `crosscompute-0.9.4.9/crosscompute/dependencies.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/exceptions.py` & `crosscompute-0.9.4.9/crosscompute/exceptions.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/macros/disk.py` & `crosscompute-0.9.4.9/crosscompute/macros/disk.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/macros/iterable.py` & `crosscompute-0.9.4.9/crosscompute/macros/iterable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/macros/log.py` & `crosscompute-0.9.4.9/crosscompute/macros/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/macros/package.py` & `crosscompute-0.9.4.9/crosscompute/macros/package.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/macros/security.py` & `crosscompute-0.9.4.9/crosscompute/macros/security.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routers/automation.py` & `crosscompute-0.9.4.9/crosscompute/routers/automation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routers/file.py` & `crosscompute-0.9.4.9/crosscompute/routers/file.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routers/root.py` & `crosscompute-0.9.4.9/crosscompute/routers/root.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routers/stream.py` & `crosscompute-0.9.4.9/crosscompute/routers/stream.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routers/token.py` & `crosscompute-0.9.4.9/crosscompute/routers/token.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/asset.py` & `crosscompute-0.9.4.9/crosscompute/routines/asset.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/authorization.py` & `crosscompute-0.9.4.9/crosscompute/routines/authorization.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/automation.py` & `crosscompute-0.9.4.9/crosscompute/routines/automation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/batch.py` & `crosscompute-0.9.4.9/crosscompute/routines/batch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/configuration.py` & `crosscompute-0.9.4.9/crosscompute/routines/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,16 +390,15 @@
     attribution_text = remove_single_paragraph(get_html_from_markdown(
         configuration.get('attribution_text', ATTRIBUTION_TEXT).format(
             name=name,
             copyright_name=copyright_name,
             copyright_uri=copyright_uri,
             copyright_year=copyright_year,
         ), extras=[
-            'target-blank-links',
-        ]))
+            'target-blank-links']))
     return {
         'name': name,
         'slug': slug,
         'title': configuration.get('title', name),
         'description': configuration.get('description', name),
         'version': configuration.get('version', AUTOMATION_VERSION),
         'uri': AUTOMATION_ROUTE.format(automation_slug=slug),
```

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/database.py` & `crosscompute-0.9.4.9/crosscompute/routines/database.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/interface.py` & `crosscompute-0.9.4.9/crosscompute/routines/interface.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/log.py` & `crosscompute-0.9.4.9/crosscompute/routines/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/mutation.py` & `crosscompute-0.9.4.9/crosscompute/routines/mutation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/printer.py` & `crosscompute-0.9.4.9/crosscompute/routines/printer.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/server.py` & `crosscompute-0.9.4.9/crosscompute/routines/server.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/step.py` & `crosscompute-0.9.4.9/crosscompute/routines/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,21 @@
         self.in_script = False
         self.template_parts = []
         super().__init__(*args, **kwargs)
 
     def handle_starttag(self, tag, attrs):
         if tag == 'script':
             self.in_script = True
-        attribute_strings = []
-        for k, v in attrs:
-            v = VARIABLE_ID_WHITELIST_PATTERN.sub(self.render_text, v)
-            attribute_strings.append(f'{k}="{v}"')
-        attributes_string = ' ' + ' '.join(
-            attribute_strings) if attribute_strings else ''
+        attributes_string = self.get_attributes_string(tag, attrs)
         self.template_parts.append(f'<{tag}{attributes_string}>')
 
+    def handle_startendtag(self, tag, attrs):
+        attributes_string = self.get_attributes_string(tag, attrs)
+        self.template_parts.append(f'<{tag}{attributes_string}/>')
+
     def handle_endtag(self, tag):
         if tag == 'script':
             self.in_script = False
         self.template_parts.append(f'</{tag}>')
 
     def handle_data(self, data):
         in_script = self.in_script
@@ -55,14 +54,28 @@
         self.template_parts.append(data)
 
     def process(self, text):
         self.template_parts = []
         self.feed(text)
         return ''.join(self.template_parts)
 
+    def get_attributes_string(self, tag, attrs):
+        keys = [_[0] for _ in attrs]
+        if tag == 'img' and 'loading' not in keys:
+            attrs.append(('loading', 'lazy'))
+        attribute_strings = []
+        for k, v in attrs:
+            if v is None:
+                attribute_string = k
+            else:
+                v = VARIABLE_ID_WHITELIST_PATTERN.sub(self.render_text, v)
+                attribute_string = f'{k}="{v}"'
+            attribute_strings.append(attribute_string)
+        return ' ' + ' '.join(attribute_strings) if attribute_strings else ''
+
 
 def get_automation_batch_step_uri(
         automation_definition, batch_definition, step_name):
     automation_uri = automation_definition.uri
     batch_uri = batch_definition.uri
     step_code = STEP_CODE_BY_NAME[step_name]
     step_uri = STEP_ROUTE.format(step_code=step_code)
```

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/uri.py` & `crosscompute-0.9.4.9/crosscompute/routines/uri.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/variable.py` & `crosscompute-0.9.4.9/crosscompute/routines/variable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/routines/work.py` & `crosscompute-0.9.4.9/crosscompute/routines/work.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/scripts/configure.py` & `crosscompute-0.9.4.9/crosscompute/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/scripts/launch.py` & `crosscompute-0.9.4.9/crosscompute/scripts/launch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/scripts/print.py` & `crosscompute-0.9.4.9/crosscompute/scripts/print.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/scripts/run.py` & `crosscompute-0.9.4.9/crosscompute/scripts/run.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/scripts/serve.py` & `crosscompute-0.9.4.9/crosscompute/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute/settings.py` & `crosscompute-0.9.4.9/crosscompute/settings.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute.egg-info/PKG-INFO` & `crosscompute-0.9.4.9/crosscompute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.8
+Version: 0.9.4.9
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://docs.crosscompute.com
```

### Comparing `crosscompute-0.9.4.8/crosscompute.egg-info/SOURCES.txt` & `crosscompute-0.9.4.9/crosscompute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/crosscompute.egg-info/entry_points.txt` & `crosscompute-0.9.4.9/crosscompute.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/setup.cfg` & `crosscompute-0.9.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute
-version = 0.9.4.8
+version = 0.9.4.9
 description = Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
```

### Comparing `crosscompute-0.9.4.8/tests/test_constants.py` & `crosscompute-0.9.4.9/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/tests/test_routines_configuration.py` & `crosscompute-0.9.4.9/tests/test_routines_configuration.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/tests/test_routines_variable.py` & `crosscompute-0.9.4.9/tests/test_routines_variable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.8/tests/test_routines_work.py` & `crosscompute-0.9.4.9/tests/test_routines_work.py`

 * *Files identical despite different names*

