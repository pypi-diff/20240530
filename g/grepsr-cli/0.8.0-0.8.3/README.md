# Comparing `tmp/grepsr_cli-0.8.0.tar.gz` & `tmp/grepsr_cli-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grepsr_cli-0.8.0.tar", last modified: Wed May 22 03:04:12 2024, max compression
+gzip compressed data, was "grepsr_cli-0.8.3.tar", last modified: Thu May 30 10:20:01 2024, max compression
```

## Comparing `grepsr_cli-0.8.0.tar` & `grepsr_cli-0.8.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-05-22 03:01:49.000000 grepsr_cli-0.8.0/.version
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/CHANGELOG.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/LICENSE.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/MANIFEST.in
--rw-r--r--   0 zznix     (1000) zznix     (1000)     3593 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3061 2024-05-21 03:15:08.000000 grepsr_cli-0.8.0/README.md
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/grepsr_cli.egg-info/
--rw-r--r--   0 zznix     (1000) zznix     (1000)     3593 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/entry_points.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/requires.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/top_level.txt
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.004200 grepsr_cli-0.8.0/grepsrcli/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/controllers/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/controllers/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.8.0/grepsrcli/controllers/base.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    19297 2024-05-21 05:07:27.000000 grepsr_cli-0.8.0/grepsrcli/controllers/crawler.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/controllers/generate.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/controllers/report.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/core/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.8.0/grepsrcli/core/aws_s3.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.8.0/grepsrcli/core/config.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/exc.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/input_prompts.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.8.0/grepsrcli/core/message_log.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/report_api.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.8.0/grepsrcli/core/sdk_setup.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     5713 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/core/test_local.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    16893 2024-05-21 04:05:06.000000 grepsr_cli-0.8.0/grepsrcli/core/utils.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/ext/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/ext/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-04-25 17:32:12.000000 grepsr_cli-0.8.0/grepsrcli/main.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/plugins/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/plugins/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/grepsrcli/templates/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/autocomplete.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/autocomplete_zsh.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/composer.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/node_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2084 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/templates/php_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3458 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/templates/php_brp_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2087 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/templates/php_vc_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/py_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/requirements-dev.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/requirements.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/setup.cfg
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/setup.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/tests/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      615 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/tests/test_grepsrcli.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.8.0/tests/test_unit.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.286144 grepsr_cli-0.8.3/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-05-30 10:19:41.000000 grepsr_cli-0.8.3/.version
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-05-07 09:17:11.000000 grepsr_cli-0.8.3/CHANGELOG.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/LICENSE.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/MANIFEST.in
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3593 2024-05-30 10:20:01.286144 grepsr_cli-0.8.3/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3061 2024-05-21 03:15:08.000000 grepsr_cli-0.8.3/README.md
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.286144 grepsr_cli-0.8.3/grepsr_cli.egg-info/
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3593 2024-05-30 10:20:01.000000 grepsr_cli-0.8.3/grepsr_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-05-30 10:20:01.000000 grepsr_cli-0.8.3/grepsr_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-05-30 10:20:01.000000 grepsr_cli-0.8.3/grepsr_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-05-30 10:20:01.000000 grepsr_cli-0.8.3/grepsr_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-05-30 10:20:01.000000 grepsr_cli-0.8.3/grepsr_cli.egg-info/requires.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-05-30 10:20:01.000000 grepsr_cli-0.8.3/grepsr_cli.egg-info/top_level.txt
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.278144 grepsr_cli-0.8.3/grepsrcli/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.278144 grepsr_cli-0.8.3/grepsrcli/controllers/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/controllers/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.8.3/grepsrcli/controllers/base.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    19339 2024-05-30 09:46:16.000000 grepsr_cli-0.8.3/grepsrcli/controllers/crawler.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/controllers/generate.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/controllers/report.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.282144 grepsr_cli-0.8.3/grepsrcli/core/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/core/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.8.3/grepsrcli/core/aws_s3.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.8.3/grepsrcli/core/config.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/core/exc.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/core/input_prompts.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.8.3/grepsrcli/core/message_log.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/core/report_api.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.8.3/grepsrcli/core/sdk_setup.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     6624 2024-05-29 06:09:25.000000 grepsr_cli-0.8.3/grepsrcli/core/test_local.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    17231 2024-05-30 09:36:48.000000 grepsr_cli-0.8.3/grepsrcli/core/utils.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.282144 grepsr_cli-0.8.3/grepsrcli/ext/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/ext/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-05-29 03:43:30.000000 grepsr_cli-0.8.3/grepsrcli/main.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.282144 grepsr_cli-0.8.3/grepsrcli/plugins/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/plugins/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.282144 grepsr_cli-0.8.3/grepsrcli/templates/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/templates/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/templates/autocomplete.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/templates/autocomplete_zsh.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/templates/composer.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/templates/node_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2081 2024-05-27 06:36:35.000000 grepsr_cli-0.8.3/grepsrcli/templates/php_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3459 2024-05-27 06:36:51.000000 grepsr_cli-0.8.3/grepsrcli/templates/php_brp_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2088 2024-05-27 06:36:43.000000 grepsr_cli-0.8.3/grepsrcli/templates/php_vc_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/grepsrcli/templates/py_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/requirements-dev.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-05-07 09:17:11.000000 grepsr_cli-0.8.3/requirements.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-05-30 10:20:01.286144 grepsr_cli-0.8.3/setup.cfg
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.8.3/setup.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-30 10:20:01.286144 grepsr_cli-0.8.3/tests/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      615 2024-05-07 09:17:11.000000 grepsr_cli-0.8.3/tests/test_grepsrcli.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.8.3/tests/test_unit.py
```

### Comparing `grepsr_cli-0.8.0/CHANGELOG.md` & `grepsr_cli-0.8.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/PKG-INFO` & `grepsr_cli-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.8.0
+Version: 0.8.3
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `grepsr_cli-0.8.0/README.md` & `grepsr_cli-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsr_cli.egg-info/PKG-INFO` & `grepsr_cli-0.8.3/grepsr_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.8.0
+Version: 0.8.3
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `grepsr_cli-0.8.0/grepsr_cli.egg-info/SOURCES.txt` & `grepsr_cli-0.8.3/grepsr_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/controllers/base.py` & `grepsr_cli-0.8.3/grepsrcli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/controllers/crawler.py` & `grepsr_cli-0.8.3/grepsrcli/controllers/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     return_parsed_url,
     insert_all_chained_dependencies,
     generate_plugin_name,
     string_to_list,
     first_found_numbers,
     get_current_branch_name,
     cmd_shell_exec,
+    get_extension,
 )
 from ..core.test_local import TestLocal
 from ..core.message_log import Log
 from ..core.aws_s3 import S3
 
 class CrawlerBase(Controller):
     class Meta:
@@ -76,20 +77,20 @@
     )
     def test(self):
         plugin_name = self.app.pargs.plugin_name
         main_fn_params = self.app.pargs.params
         main_fn_params_file = self.app.pargs.params_file
         is_multi_proc = self.app.pargs.multi_proc_mode
 
-        platforms = ['php', 'php_next']
+        platforms = ['php', 'php_next', 'node']
         for platform in platforms:
             if platform in self.config:
                 plugin_path = get_plugin_path(plugin_name, type=platform)
                 if plugin_path:
-                    base_path = pathlib.Path(get_plugin_path(plugin_name, type=platform)).parent
+                    base_path = pathlib.Path(plugin_path).parent
                     try:
                         TestLocal(type=platform, base_path=base_path, plugin_name=plugin_name, params=main_fn_params, params_file=main_fn_params_file, is_multi_proc=is_multi_proc)
                     except json.JSONDecodeError as e:
                         self.app.log.error(f"Error decoding params as JSON. {e}")
                         self.app.exit_code = 10
                     except FileNotFoundError as e:
                         self.app.log.error(f"Params file: `{main_fn_params_file}` not found. {e}")
@@ -302,15 +303,15 @@
             if not plugin_dir_path:
                 self.app.log.error(f'Could not find plugin: {plugin_name}')
                 continue
 
             plugin_info = get_plugin_info(plugin_dir_path)
             if plugin_info:
                 base_class = plugin_info['base_class']
-                if not base_class.startswith('Vtx_Service_Plugin'):
+                if base_class and not base_class.startswith('Vtx_Service_Plugin'):
                     if base_class not in plugin_info['dependencies']:
                         msg = f'Plugin extends {base_class} but does not declare it as a dependency.'
                         self.app.log.warning(msg)
                         if ask_user_input_YN(f'[Experimental] Do you want to automatically add dependencies?') == 'Y':
                             insert_all_chained_dependencies(plugin_name)
                         go_fwd = ask_user_input_YN(f'Do you want to continue?')
                         if go_fwd == 'N':
@@ -348,15 +349,15 @@
                 try:
                     proc = subprocess.run(cmd, shell=True, check=True, timeout=100, cwd=root_repo_dir)
                 except subprocess.TimeoutExpired:
                     self.app.log.error(f'timed out on syncing rep for {plugin_name}')
                     continue
                 
                 if not does_plugin_have_modifications(plugin_name, root_repo_dir):
-                    plugin_abs_path = path.join(plugin_dir_path, plugin_name + '.php')
+                    plugin_abs_path = path.join(plugin_dir_path, plugin_name + '.' + get_extension(type=crawler_type))
                     self.app.log.warning(f'No changes detected for {plugin_name}. Adding newline')
                     write_text(plugin_abs_path, read_text(plugin_abs_path) + "\n")
                     
                 version_info = update_version_file(plugin_dir_path, major_flag, minor_flag)
                 if plugin_info and version_info == '0.0.1':
                     # if its already deployed then the service probabily works fine.
                     # if its the first deploy, we annoy the user.
```

### Comparing `grepsr_cli-0.8.0/grepsrcli/controllers/generate.py` & `grepsr_cli-0.8.3/grepsrcli/controllers/generate.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/controllers/report.py` & `grepsr_cli-0.8.3/grepsrcli/controllers/report.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/aws_s3.py` & `grepsr_cli-0.8.3/grepsrcli/core/aws_s3.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/config.py` & `grepsr_cli-0.8.3/grepsrcli/core/config.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/message_log.py` & `grepsr_cli-0.8.3/grepsrcli/core/message_log.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/report_api.py` & `grepsr_cli-0.8.3/grepsrcli/core/report_api.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/sdk_setup.py` & `grepsr_cli-0.8.3/grepsrcli/core/sdk_setup.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/test_local.py` & `grepsr_cli-0.8.3/grepsrcli/core/test_local.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
                     self.test_script_php(env=True)
                 else:
                     self.test_script_php(env=False)
             else:
                 self.test_script_php(env=False)
         elif self.type == "php_next":
             self.test_script_php_next()
+        elif self.type == 'node':
+            self.test_script_node()
 
     def test_script_php(self, env=False):
         if self.is_multi_proc is None:
             # only use the value of multiprocess if it is not passed explicitly from cmd line
             try:
                 self.is_multi_proc = 1 if self.type_config['multiprocess'] == True else 0
             except KeyError:
@@ -98,15 +100,16 @@
             sh_contents.append(f'source {original_entrypoints[0]} {sdk_args} {pipe_params}')
             write_text(custom_shell_file_local, '\n'.join(sh_contents))
 
             bash_cmd = f'source /tmp/{custom_shell_file}'
 
         commands = [
                 'docker run -t --network="host" --rm',
-                f'-v {self.base_path}:/home/grepsr/vortex-plugins/{path.basename(self.base_path)}',
+                # f'-v {self.base_path}:/home/grepsr/vortex-plugins/{path.basename(self.base_path)}',
+                f'-v {self.base_path}:/home/grepsr/vortex-plugins/vortex-plugins-services',
                 f'-v {self.tmp_path}:/tmp',
                 f'-e APP_ENV={self.config["app_env"]}',
                 " ".join(env_vars),
                 f'--entrypoint=""' if not only_service else '',
                 docker_image_name,
                 f'bash -ci "{bash_cmd}"' if not only_service else sdk_args,
         ]
@@ -120,9 +123,27 @@
         command = f'''docker run -t -i --network="host" --rm \
                      -v {self.base_path}:/home/grepsr/vortex-backend-next/scraper-plugins \
                      -v {self.tmp_path}:/tmp \
                      -e APP_ENV={self.config['app_env']} \
                      {self.type_config['sdk_image']} -s {self.plugin_name} '''
         system(command)
 
-    def test_script_local(self):
-        pass
+    def test_script_node(self):
+        env_vars = []
+        if self.type_config.get('env'):
+            env_vars = [
+                f'-e {env_var}={self.type_config["env"][env_var]}' for env_var in self.type_config["env"].keys()
+            ]
+        docker_image_name = self.type_config["sdk_image"]
+        commands = [
+            'docker run --rm -it --init --network="host"',
+            f'-v {self.base_path}:/home/grepsr/crawler/',
+            f'-v {self.tmp_path}:/tmp/',
+            " ".join(env_vars),
+            f'-e APP_ENV={self.config["app_env"]}',
+            f'-e SERVICE_NAME={self.plugin_name}',
+            docker_image_name,
+        ]
+
+        command = ' '.join([command for command in commands if command])
+        # print(command, flush=True)
+        system(command)
```

### Comparing `grepsr_cli-0.8.0/grepsrcli/core/utils.py` & `grepsr_cli-0.8.3/grepsrcli/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,28 @@
 
         for base_paths in base_paths_list:
             if base_paths is not None and _generate_plugin_path(plugin_name, base_paths):
                 return _generate_plugin_path(plugin_name, base_paths)
         Log.error("Plugin name not found.")
         return False
 
+def get_extension(type='php'):
+    if type == 'php':
+        return 'php'
+    elif type == 'node':
+        return 'js'
+    elif type == 'py':
+        return 'py'
+    elif type == 'php_next':
+        return 'php'
+    elif type == 'node_next':
+        return 'js'
+    else:
+        Log.error("No extension for this type")
+        return ''
 
 def create_boilerplate(folder_path, boilerplate, data, extention,):
     """ to create boilerplate for a given path
 
     Args:
         folder_path (str): the destination path
         boilerplate (str): the name of the boilerplate
```

### Comparing `grepsr_cli-0.8.0/grepsrcli/main.py` & `grepsr_cli-0.8.3/grepsrcli/main.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/templates/autocomplete_zsh.jinja2` & `grepsr_cli-0.8.3/grepsrcli/templates/autocomplete_zsh.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/templates/node_boilerplate.jinja2` & `grepsr_cli-0.8.3/grepsrcli/templates/node_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/grepsrcli/templates/php_boilerplate.jinja2` & `grepsr_cli-0.8.3/grepsrcli/templates/php_boilerplate.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 <?php
+
 /**
  * Name: {{host_name | default(plugin_name)}}{{ ' - ' ~ scrape_category if scrape_category else ''}}
  * Description: {{host_name | default(plugin_name)}}{{ ' - ' ~ scrape_category if scrape_category else ''}}
  * PID: {{pid}} force
  */
 
 class {{plugin_name}} extends Vtx_Service_Plugin {
@@ -39,16 +40,15 @@
         $this->setHeaders('Upgrade-Insecure-Requests', '1');
         $this->setHeaders('User-Agent', 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.67 Safari/537.36');
 
         //$this->setCurlOption(CURLOPT_CONNECTTIMEOUT, 180);
         //$this->setCurlOption(CURLOPT_TIMEOUT, 180);
     }
 
-    public function main($params)
-    {
+    public function main($params) {
 	    echo("Crawling : " . $this->domainUrl . PHP_EOL);
 	    $this->dataSet->setPageName(get_class($this) .'_%s' , [ date('Ymd') ]);
         $this->dataSet->setColHeaders($this->colHeaders);
 	    $this->newSession();
 	    $this->switchProxy();
 
         //$this->loadDocument($this->baseUrl);
```

### Comparing `grepsr_cli-0.8.0/grepsrcli/templates/php_brp_boilerplate.jinja2` & `grepsr_cli-0.8.3/grepsrcli/templates/php_brp_boilerplate.jinja2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 <?php
+
 /**
  * Name: {{host_name | default(plugin_name)}}
  * Description: {{host_name | default(plugin_name)}}
  * PID: {{pid}} force
  * Dependencies: brp_locations
  */
```

### Comparing `grepsr_cli-0.8.0/grepsrcli/templates/php_vc_boilerplate.jinja2` & `grepsr_cli-0.8.3/grepsrcli/templates/php_vc_boilerplate.jinja2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 <?php
+
 /**
  * Name: {{host_name | default(plugin_name)}}
  * Description: {{host_name | default(plugin_name)}}
  * PID: {{pid}} force
  * Dependencies: vericred_service_main
  */
```

### Comparing `grepsr_cli-0.8.0/grepsrcli/templates/py_boilerplate.jinja2` & `grepsr_cli-0.8.3/grepsrcli/templates/py_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/setup.py` & `grepsr_cli-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/tests/test_grepsrcli.py` & `grepsr_cli-0.8.3/tests/test_grepsrcli.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.8.0/tests/test_unit.py` & `grepsr_cli-0.8.3/tests/test_unit.py`

 * *Files identical despite different names*

