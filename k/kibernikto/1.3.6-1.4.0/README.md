# Comparing `tmp/kibernikto-1.3.6.tar.gz` & `tmp/kibernikto-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibernikto-1.3.6.tar", last modified: Sat Mar 30 17:14:25 2024, max compression
+gzip compressed data, was "kibernikto-1.4.0.tar", last modified: Thu May 30 12:42:04 2024, max compression
```

## Comparing `kibernikto-1.3.6.tar` & `kibernikto-1.4.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.217633 kibernikto-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-30 17:14:15.000000 kibernikto-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-30 17:14:15.000000 kibernikto-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-03-30 17:14:25.213633 kibernikto-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-03-30 17:14:15.000000 kibernikto-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/bots/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/ai_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/bots/cybernoone/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/cybernoone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/cybernoone/_cybernoone.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/redactor_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/bots/vertihvostka/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/vertihvostka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/bots/vertihvostka/_vertihvostka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/cmd/__start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/data/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.209632 kibernikto-1.3.6/kibernikto/data/pg/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/data/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/data/pg/_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/data/pg/_postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.213633 kibernikto-1.3.6/kibernikto/interactors/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/interactors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/interactors/openai_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/interactors/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.213633 kibernikto-1.3.6/kibernikto/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/plugins/_img_summarizator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/plugins/_kibernikto_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/plugins/_weblink_summarizator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/plugins/_youtube_summarizator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.213633 kibernikto-1.3.6/kibernikto/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/_executor_corral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/_message_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/comprehensive_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/single_group_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/telegram_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/telegram/whisper_openai_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.213633 kibernikto-1.3.6/kibernikto/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/ai_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/psycopg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-30 17:14:15.000000 kibernikto-1.3.6/kibernikto/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:14:25.213633 kibernikto-1.3.6/kibernikto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-03-30 17:14:25.000000 kibernikto-1.3.6/kibernikto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-30 17:14:25.000000 kibernikto-1.3.6/kibernikto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 17:14:25.000000 kibernikto-1.3.6/kibernikto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-30 17:14:25.000000 kibernikto-1.3.6/kibernikto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-30 17:14:25.000000 kibernikto-1.3.6/kibernikto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-30 17:14:25.000000 kibernikto-1.3.6/kibernikto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-30 17:14:15.000000 kibernikto-1.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 17:14:25.217633 kibernikto-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-30 17:14:15.000000 kibernikto-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.065114 kibernikto-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 12:41:55.000000 kibernikto-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 12:41:55.000000 kibernikto-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-30 12:42:04.061114 kibernikto-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-30 12:41:55.000000 kibernikto-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.053114 kibernikto-1.4.0/kibernikto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/bots/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/ai_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/bots/cybernoone/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/cybernoone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/cybernoone/_cybernoone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/redactor_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/bots/vertihvostka/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/vertihvostka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/bots/vertihvostka/_vertihvostka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/cmd/__start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/data/pg/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/data/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/data/pg/_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/data/pg/_postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.057114 kibernikto-1.4.0/kibernikto/interactors/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/interactors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/interactors/openai_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/interactors/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.061114 kibernikto-1.4.0/kibernikto/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/plugins/_img_summarizator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/plugins/_kibernikto_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/plugins/_weblink_summarizator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/plugins/_youtube_summarizator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.061114 kibernikto-1.4.0/kibernikto/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/_executor_corral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/comprehensive_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.061114 kibernikto-1.4.0/kibernikto/telegram/pre_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/pre_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/pre_processors/_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/pre_processors/_gladia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/single_group_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/telegram_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/telegram/whisper_openai_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.061114 kibernikto-1.4.0/kibernikto/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/ai_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/psycopg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-30 12:41:55.000000 kibernikto-1.4.0/kibernikto/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:42:04.061114 kibernikto-1.4.0/kibernikto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-30 12:42:04.000000 kibernikto-1.4.0/kibernikto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 12:42:04.000000 kibernikto-1.4.0/kibernikto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:42:04.000000 kibernikto-1.4.0/kibernikto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 12:42:04.000000 kibernikto-1.4.0/kibernikto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 12:42:04.000000 kibernikto-1.4.0/kibernikto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 12:42:04.000000 kibernikto-1.4.0/kibernikto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 12:41:55.000000 kibernikto-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:42:04.065114 kibernikto-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 12:41:55.000000 kibernikto-1.4.0/setup.py
```

### Comparing `kibernikto-1.3.6/LICENSE` & `kibernikto-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/PKG-INFO` & `kibernikto-1.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,20 @@
-Metadata-Version: 2.1
-Name: kibernikto
-Version: 1.3.6
-Summary: Easily run telegram bots connected to AI models.
-Home-page: https://github.com/solovieff/kibernikto
-Author-email: solovieff.nnov@gmail.com
-License: GPL-3.0 license
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiogram==3.1.1
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: openai==1.3.0
-Requires-Dist: youtube_transcript_api==0.6.1
-Requires-Dist: pytube==15.0
-Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: emoji-country-flag==1.3.2
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: pydantic-settings
-Requires-Dist: pydub
-Requires-Dist: psycopg==3.1.18
-Requires-Dist: psycopg[binary]==3.1.18
-Requires-Dist: psycopg-pool==3.2
-Requires-Dist: dict2xml==1.7.5
-Requires-Dist: fujson==0.1.1
-
 # kibernikto
 
 Kibernikto is an app/lib to easily run telegram bots connected to AI models with additional features.  
-Kibernikto bots can be easily extended to be used outised telegram.
+Kibernikto bots can be easily extended to be used outside telegram.  
+Core and bots can be used as a core libs for creating ai-bot based apps.  
 
-- voice messages recognition
-- youtube video summary
-- webpage summary
-- image recognition
-- function tools easy integration (anthropic xml format supported!)
+- ✍️ telegram conversations with different AIs in groups or privately (including hidden second-level AI-redactors)
+- 🔉 voice messages recognition
+- 👂 interviews and meetings (up to 2 hours) analysis right in Telegram using Gladia.io 
+- 🎞 youtube video summarization
+- 🔗 webpage summarization
+- 📸 image recognition
+- 🫡 openai function tools easy [integration](https://github.com/solovieff/kibernikto-planner). No more pain. ~~(anthropic xml format supported, too! looks like they changed it again)~~
 
 Given an image Kibernikto will publish it to a free image hosting service and then process as a link.
 
 By default `single_group_dispatcher` is used with a following rules:
 
 - One Kibernikto instance **can privately talk only to one** (`TG_MASTER_ID`) user and work with **one group chat
   ** (`TG_FRIEND_GROUP_ID`).
@@ -49,16 +22,16 @@
 If you want your bot to be able to work with **any user or group**, use `comprehensive_dispatcher`. You will need the
 following `additional` env parameters if you want to restrict user/group ids.
 Do not add it to your env if you want anyone
 to
 be able to use yr Kibernikto instance:
 
 ```dotenv
-TG_MASTER_IDS=[199720543]
-TG_FRIEND_GROUP_IDS=[-813228576]
+TG_MASTER_IDS=[XXXXXXXXX]
+TG_FRIEND_GROUP_IDS=[-XXXXXXXXX]
 ```
 
 or
 
 ``kibernikto --env_file_path=local.env --bot_type=kibernikto --dispatcher=multiuser``
 
 Kibernikto can post-process messages returned by one AI using another AI (for now it's a hardcoded 2 step chain).
@@ -121,61 +94,100 @@
 Other AI behaviour options:
 
 ```dotenv
 OPENAI_MAX_TOKENS=800  
 OPENAI_WHO_AM_I=Answer all questions as {0}, the majestic lord of the universes with all the knowledge of our small planet.  
 ```
 
-WeblinkSummaryPlugin and YoutubePlugin.
+**Telegram**
+
+```dotenv
+# Telegram configuration
+TG_BOT_KEY=XXXXXXXXXX:XXXxxxXXXxxxxXXXxxx  
+TG_BOT_MAX_HISTORY=8  
+TG_FRIEND_GROUP_ID=-XXXXXXXXXX  
+# Your telegram ID. For example 122349243. Forward your message to @idstickerbot to get it.  
+TG_MASTER_ID=XXXXXXXXX
+# Kibernikto reacts to direct replies or when sees the following words. 
+# Preserving pydantic-settings list format.  
+TG_REACTION_CALLS=["киберникто","государь"]  
+# sometimes Kibernikto sends stickers for fun together with his answers  
+TG_STICKER_LIST=["CAACAgIAAxkBAAEKqsplQ8BRyPbGj_B_K4ujCLsDAe-l7wAC8AIAAs-71A7mCrGe-zzi0DME","CAACAgIAAxkBAAEIgoxkMaHv1maOeEne8CYAAY5s4kJ1e4wAAo4JAAIItxkCXSMuZ6bo59gvBA"]
+```
+
+
+- **WeblinkSummaryPlugin and YoutubePlugin**
 
 ```dotenv
 # If no key is provided, youtube videos and webpages will be ignored.
 SUMMARIZATION_OPENAI_API_KEY=yr-key
 SUMMARIZATION_OPENAI_API_BASE_URL=https://api.openai.com/v1  
 SUMMARIZATION_OPENAI_API_MODEL=gpt-4-turbo-preview
 ```
 
-ImageSummaryPlugin to process images.
+- **ImageSummaryPlugin to process images.**
 
 ```dotenv
 # If no key is provided, images will not be processed.
 IMAGE_SUMMARIZATION_OPENAI_API_KEY=yr-key
 IMAGE_SUMMARIZATION_OPENAI_API_MODEL=gpt-4-vision-preview
 IMAGE_SUMMARIZATION_OPENAI_API_BASE_URL=https://api.openai.com/v1
 
 # You can get your key here: https://imgbb.com. If you do no set up this variable, default one will be used.  
 # This is needed to store images send to the bot.  
 IMAGE_STORAGE_API_KEY = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
 ```
 
-Voice messages processing
+- **Voice messages** processing using **OpenAI**:
 
 ```dotenv
 # If no key is provided, voice messages will not be processed.
+VOICE_PROCESSOR=openai
 VOICE_OPENAI_API_KEY=yr-key
 VOICE_OPENAI_API_MODEL=whisper-1
 VOICE_OPENAI_API_BASE_URL=https://api.openai.com/v1
-VOICE_PROCESSOR=openai
-VOICE_FILE_LOCATION=/tmp/tg_voices
+VOICE_FILE_LOCATION=/tmp
 ```
+    
+- **Voice messages** processing using [gladia.io](https://gladia.io):  
+**Gladia** Audio Intelligence API, is designed to enable any company to easily 
+embed top-quality Audio AI into their applications, whatever the tech stack.  
+    
+As whisper api is limited to 25 megs, [gladia.io](https://glaudia.io) helps to process bigger files.    
+
+Kibernikto treats voice messages with duration less than `VOICE_MIN_COMPLEX_SECONDS` as usual AI interaction ones.
+For longer durations Kibernikto will return detailed audio 
+analysis including summary etc.  
+
+Perfect solution for analyzing interviews and meeting.  
+Gladia price policies are also very affordable.
+
+```dotenv
+VOICE_PROCESSOR=gladia
+VOICE_GLADIA_API_KEY=yr-gladia-key
+VOICE_GLADIA_SUMMARIZATION_TYPE=concise
+VOICE_MIN_COMPLEX_SECONDS=300
+```    
+   
+- **Smart voice messages** processing using both [gladia.io](https://gladia.io) and OpenAI:  
 
-Telegram
-
+Whisper api is a bit faster and looks better to use just for talking with your bot.
 ```dotenv
-# Telegram configuration
-TG_BOT_KEY=XXXXXXXXXX:XXXxxxXXXxxxxXXXxxx  
-TG_BOT_MAX_HISTORY=8  
-TG_FRIEND_GROUP_ID=-XXXXXXXXXX  
-# Your telegram ID. For example 122349243. Forward your message to @idstickerbot to get it.  
-TG_MASTER_ID=XXXXXXXXX
-# Kibernikto reacts to direct replies or when sees the following words. 
-# Preserving pydantic-settings list format.  
-TG_REACTION_CALLS=["киберникто","государь"]  
-# sometimes Kibernikto sends stickers for fun together with his answers  
-TG_STICKER_LIST=["CAACAgIAAxkBAAEKqsplQ8BRyPbGj_B_K4ujCLsDAe-l7wAC8AIAAs-71A7mCrGe-zzi0DME","CAACAgIAAxkBAAEIgoxkMaHv1maOeEne8CYAAY5s4kJ1e4wAAo4JAAIItxkCXSMuZ6bo59gvBA"]
+VOICE_PROCESSOR=**auto**
+
+VOICE_OPENAI_API_KEY=yr-key
+VOICE_OPENAI_API_MODEL=whisper-1
+VOICE_OPENAI_API_BASE_URL=https://api.openai.com/v1
+VOICE_FILE_LOCATION=/tmp
+
+#starting this audio length Kibernikto will start using Gladia and deeper analysis
+VOICE_MIN_COMPLEX_SECONDS=300
+VOICE_GLADIA_API_KEY=yr-gladia-key
+VOICE_GLADIA_SUMMARIZATION_TYPE=concise
+VOICE_GLADIA_CONTEXT=We have before us an interview for the position of office manager
 ```
 
 For the full list of variables, see `env_examples` folder.
 
 # redactor mode
 
 To run Kibernikto with additional redactor for each response change the `bot_type` to "vertihvostka":    
@@ -196,14 +208,15 @@
 
 To create and operate your bot: https://t.me/BotFather  
 To obtain group/user ids etc: https://t.me/getidsbot  
 To obtain sticker ids: https://t.me/idstickerbot  
 To get familiar with basic OpenAI principles: https://openai.com  
 Basics on Gpt-4 vision: https://gptpluginz.com/gpt-4-vision-api  
 To find out more on models and multi-model api details: https://vsegpt.ru/Docs/Models  
+Audio analysis: https://gladia.io  
 Website to text and other helpful tools https://toolsyep.com  
 Free image hosting: https://imgbb.com
 
 # code details
 
 *(ignore it if dont plan to create yr own plugins or Kibernikto bots using Kibernikto as a library)*
```

### Comparing `kibernikto-1.3.6/kibernikto/bots/ai_settings.py` & `kibernikto-1.4.0/kibernikto/bots/ai_settings.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/bots/cybernoone/_cybernoone.py` & `kibernikto-1.4.0/kibernikto/bots/cybernoone/_cybernoone.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 
 
 class Kibernikto(TelegramBot):
     """
     Basic implementation of Telegram bot can be used as an example.
     """
 
-    def __init__(self, master_id: str, username: str, config: OpenAiExecutorConfig):
+    def __init__(self, master_id: str, username: str, config: OpenAiExecutorConfig, key=NOT_GIVEN):
         """
         :param master_id: telegram admin id
         :param username: telegram username
         :param config: ai bot config
         """
+        self.key = key
         super().__init__(config=config, username=username, master_id=master_id)
 
     async def heed_and_reply(self, message, author=NOT_GIVEN, save_to_history=True):
         try:
             return await super().heed_and_reply(message, author, save_to_history=save_to_history)
         except KiberniktoPluginException as e:
             return f" {e.plugin_name} не сработал!\n\n {str(e)}"
```

### Comparing `kibernikto-1.3.6/kibernikto/bots/redactor_settings.py` & `kibernikto-1.4.0/kibernikto/bots/redactor_settings.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/bots/vertihvostka/_vertihvostka.py` & `kibernikto-1.4.0/kibernikto/bots/vertihvostka/_vertihvostka.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/cmd/__start.py` & `kibernikto-1.4.0/kibernikto/cmd/__start.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/data/pg/_connectors.py` & `kibernikto-1.4.0/kibernikto/data/pg/_connectors.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/interactors/openai_executor.py` & `kibernikto-1.4.0/kibernikto/interactors/openai_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from collections import deque
 from enum import Enum
 from typing import List
 
 from openai import AsyncOpenAI
 from openai._types import NOT_GIVEN
 from openai.types.chat import ChatCompletion, ChatCompletionMessage
-from openai.types.edit import Choice
+from openai.types.chat.chat_completion import Choice
+
 from pydantic import BaseModel
 
 from kibernikto.bots.ai_settings import AI_SETTINGS
 from kibernikto.interactors.tools import Toolbox
 from kibernikto.plugins import KiberniktoPlugin
 from kibernikto.utils import ai_tools
 
@@ -136,22 +137,23 @@
             temperature=self.full_config.temperature
         )
         response_message: ChatCompletionMessage = completion.choices[0].message
 
         return response_message
 
     async def _run_for_messages(self, full_prompt, author=NOT_GIVEN):
+        tools_to_use = self.tools_definitions if self.tools_definitions else NOT_GIVEN
 
         completion: ChatCompletion = await self.client.chat.completions.create(
             model=self.model,
             messages=full_prompt,
             max_tokens=AI_SETTINGS.OPENAI_MAX_TOKENS,
             temperature=AI_SETTINGS.OPENAI_TEMPERATURE,
             user=author,
-            tools=self.tools_definitions
+            tools=tools_to_use
         )
         choice: Choice = completion.choices[0]
 
         return choice
 
     async def heed_and_reply(self, message: str, author=NOT_GIVEN, save_to_history=True):
         """
@@ -170,15 +172,15 @@
             else:
                 return plugins_result
 
         this_message = dict(content=f"{user_message}", role=OpenAIRoles.user.value)
 
         await self._aware_overflow()
 
-        prompt = [self.about_me] + list(self.messages) + [this_message]
+        prompt = [self.get_cur_system_message()] + list(self.messages) + [this_message]
 
         logging.debug(f"sending {prompt}")
 
         choice: Choice = await self._run_for_messages(prompt, author)
         response_message: ChatCompletionMessage = choice.message
 
         if ai_tools.is_function_call(choice=choice, xml=self.xml_tools):
@@ -190,14 +192,17 @@
 
         return response_message.content
 
     def reset_if_usercall(self, message):
         if self.reset_call in message:
             self._reset()
 
+    def get_cur_system_message(self):
+        return self.about_me
+
     def _reset(self):
         # never gets full, +1 for system
         self.messages = deque(maxlen=self.max_messages + 1)
 
         wai = self.full_config.who_am_i.format(self.full_config.name)
 
         # weirdo
```

### Comparing `kibernikto-1.3.6/kibernikto/interactors/tools.py` & `kibernikto-1.4.0/kibernikto/interactors/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 def get_tools_from_module(python_module, permitted_names=[]):
     tools = []
     for tool_name, tool_module in getmembers(python_module, ismodule):
         # print(f"\nfound {tool_name}")
         if permitted_names and not tool_name in permitted_names:
             continue
         for function_name, function in getmembers(tool_module, isfunction):
+
             if tool_name in function_name:
                 if function_name.endswith("_tool"):
                     definition = function()
                 else:
                     implementation = function
         tools.append(Toolbox(function_name=tool_name, definition=definition, implementation=implementation))
     return tools
```

### Comparing `kibernikto-1.3.6/kibernikto/plugins/_img_summarizator.py` & `kibernikto-1.4.0/kibernikto/plugins/_img_summarizator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     MESSAGE: str = _DEFAULT_TEXT
 
 
 DEFAULT_SETTINGS = ImagePluginSettings()
 
 
 class ImageSummaryPlugin(KiberniktoPlugin):
-    index = 1
+    index = 100
     """
     This plugin is used to get information about the given image.
     """
 
     @staticmethod
     def applicable():
         return DEFAULT_SETTINGS.OPENAI_API_KEY is not None
```

### Comparing `kibernikto-1.3.6/kibernikto/plugins/_kibernikto_plugin.py` & `kibernikto-1.4.0/kibernikto/plugins/_kibernikto_plugin.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/plugins/_weblink_summarizator.py` & `kibernikto-1.4.0/kibernikto/plugins/_weblink_summarizator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     WEBLINK_MESSAGE: str = _DEFAULT_TEXT
 
 
 DEFAULT_SETTINGS = WeblinkPluginSettings()
 
 
 class WeblinkSummaryPlugin(KiberniktoPlugin):
-    index = 100
+    index = 10000
     """
     This plugin is used to get weblink transcript and then get text summary from it.
     It uses toolsyep to get text repr of the website
     """
 
     @staticmethod
     def applicable():
```

### Comparing `kibernikto-1.3.6/kibernikto/plugins/_youtube_summarizator.py` & `kibernikto-1.4.0/kibernikto/plugins/_youtube_summarizator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     VIDEO_MESSAGE: str = _DEFAULT_TEXT
 
 
 DEFAULT_SETTINGS = YoutubePluginSettings()
 
 
 class YoutubePlugin(KiberniktoPlugin):
-    index = 0
+    index = 1000
 
     @staticmethod
     def applicable():
         return DEFAULT_SETTINGS.OPENAI_API_KEY is not None
 
     """
     This plugin is used to get video transcript and then get text summary from it.
@@ -118,15 +118,15 @@
     match = re.match(youtube_regex, url)
     return bool(match)
 
 
 def _get_video_from_text(text) -> YouTube:
     any_link, other_text = _extract_link(text)
     if any_link is None or not _is_youtube_url(any_link):
-        return None
+        return None, None
 
     other_text = text.replace(any_link, "").strip()
     youtube_video = YouTube(f'{any_link}')
     return youtube_video, other_text
 
 
 def _get_video_transcript(video_id, langcode='ru'):
```

### Comparing `kibernikto-1.3.6/kibernikto/telegram/_executor_corral.py` & `kibernikto-1.4.0/kibernikto/telegram/_executor_corral.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import sys
 import traceback
 from typing import Dict, Type, List
 
+from openai._types import NOT_GIVEN
+
 from kibernikto.plugins import KiberniktoPlugin
 
 from kibernikto.utils.environment import print_plugin_banner, print_plugin_off
 from pydantic import BaseModel
 
 from .telegram_bot import TelegramBot
 from kibernikto.interactors import OpenAiExecutorConfig
@@ -45,15 +47,15 @@
         await bot.client.close()
 
 
 def get_ai_executor(key_id: int):
     bot = __BOTS.get(key_id)
 
     if not bot:
-        bot = _new_executor()
+        bot = _new_executor(str(key_id))
         _apply_plugins(bot)
         __BOTS[key_id] = bot
     return bot
 
 
 def _apply_plugins(bot: TelegramBot):
     def apply_plugin(plugin: KiberniktoPlugin):
@@ -72,18 +74,19 @@
                 logging.error(str(plugin_error))
                 traceback.print_exc(file=sys.stdout)
                 logging.error("PLUGINS WERE NOT LOADED!")
         else:
             print_plugin_off(plugin_class)
 
 
-def _new_executor():
+def _new_executor(key_id: str = NOT_GIVEN):
     """
     creates new ai bot executor connected to AI API
     :return:
     :rtype:
     """
     _configuration = __EXECUTOR_CONFIG.model_copy(deep=True)
     bot = __BOT_CLASS(username=_configuration.username,
                       master_id=_configuration.master_id,
-                      config=_configuration.config)
+                      config=_configuration.config,
+                      key=key_id)
     return bot
```

### Comparing `kibernikto-1.3.6/kibernikto/telegram/single_group_dispatcher.py` & `kibernikto-1.4.0/kibernikto/telegram/single_group_dispatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,67 +4,84 @@
 import random
 import sys
 import traceback
 from random import choice
 from typing import List
 
 from aiogram import Bot, Dispatcher, types, enums, F
+from aiogram.filters import and_f
 from aiogram.types import User
 from pydantic_settings import BaseSettings
 
 from kibernikto.interactors import OpenAiExecutorConfig
 from kibernikto.interactors.tools import Toolbox
 from kibernikto.plugins import KiberniktoPlugin
 from kibernikto.utils.environment import print_plugin_banner, print_plugin_off
 from kibernikto.utils.text import split_text_by_sentences, split_text_into_chunks_by_sentences
-from ._message_preprocessors import get_message_text
+from kibernikto.telegram.pre_processors import TelegramMessagePreprocessor
 from .telegram_bot import TelegramBot
 
+
 class TelegramSettings(BaseSettings):
     TG_BOT_KEY: str
     TG_MASTER_ID: int
     TG_FRIEND_GROUP_ID: int
     TG_MAX_MESSAGE_LENGTH: int = 4096
     TG_CHUNK_SENTENCES: int = 7
     TG_REACTION_CALLS: List[str] = ['honda', 'киберникто']
+    TG_STICKER_LIST: List[str] = ["CAACAgIAAxkBAAELx29l_2OsQzpRWhmXTIMBM4yekypTOwACdgkAAgi3GQI1Wnpqru6xgTQE"]
     TG_SAY_HI: bool = False
-    TG_STICKER_LIST: List[str] = ()
 
 
 TELEGRAM_SETTINGS = TelegramSettings()
 
 smart_bot_class = None
 
 # Telegram bot
 tg_bot: Bot = None
 bot_me: User = None
 dp = Dispatcher()
-
+preprocessor = TelegramMessagePreprocessor()
 # Open AI bot instances.
 # TODO: upper level class to create
 FRIEND_GROUP_BOT: TelegramBot | None = None
 PRIVATE_BOT: TelegramBot | None = None
 
 TOOLS: List[Toolbox] = []
 MAX_TG_MESSAGE_LEN = 4096
 
 commands = {}
 
 
-def start(bot_class, tools=[]):
+def start(bot_class, tools=[], msg_preprocessor=None):
     """
     runs the executor polling the dispatcher for incoming messages
 
+    :param tools: tools available for bots created by this dispatcher
+    :type tools: List[Toolbox]
     :param bot_class: the bot class to use
+    :type bot_class: Type[TelegramBot]
+    :param msg_preprocessor: if we want to use custom message preprocessor
+    :type msg_preprocessor: Type[TelegramMessagePreprocessor]
+
     :return:
     """
     global smart_bot_class
     global tg_bot
     global TOOLS
+    global preprocessor
+    if msg_preprocessor:
+        preprocessor = msg_preprocessor
     TOOLS = tools
+
+    print("\t")
+    print('\t%-15s%-15s' % ("tg master:", TELEGRAM_SETTINGS.TG_MASTER_ID))
+    print('\t%-15s%-15s' % ("tg group:", TELEGRAM_SETTINGS.TG_FRIEND_GROUP_ID))
+    print('\t%-15s%-15s' % ("dispatcher:", 'single-user-and-group'))
+
     smart_bot_class = bot_class
     dp.startup.register(on_startup)
     tg_bot = Bot(token=TELEGRAM_SETTINGS.TG_BOT_KEY)
     dp.run_polling(tg_bot, skip_updates=True)
 
 
 async def on_startup(bot: Bot):
@@ -117,35 +134,39 @@
 
     # say hi to everyone
     await tg_bot.send_sticker(
         sticker=sticker_id,
         chat_id=chat_id)
 
 
-@dp.message(F.chat.type == enums.ChatType.PRIVATE)
+@dp.message(and_f(F.chat.type == enums.ChatType.PRIVATE, ~F.text.startswith('/')))
 async def private_message(message: types.Message):
     if not PRIVATE_BOT.check_master(message.from_user.id, message.md_text):
         reply_text = f"Я не отвечаю на вопросы в личных беседах с незакомыми людьми (если это конечно не мой Господин " \
                      f"Создатель снизошёл до меня). Я передам ваше соообщение мастеру."
         await tg_bot.send_message(TELEGRAM_SETTINGS.TG_MASTER_ID, f"{message.from_user.username}: {message.md_text}")
     else:
         await tg_bot.send_chat_action(message.chat.id, 'typing')
-        user_text = await get_message_text(message, tg_bot)
+        user_text = await preprocessor.process_tg_message(message, tg_bot)
+        if user_text is None:
+            return None  # do not reply
         await tg_bot.send_chat_action(message.chat.id, 'typing')
         reply_text = await PRIVATE_BOT.heed_and_reply(message=user_text)
     chunks = split_text_by_sentences(reply_text, TELEGRAM_SETTINGS.TG_MAX_MESSAGE_LENGTH)
     for chunk in chunks:
         await message.reply(text=chunk)
 
 
 @dp.message(F.chat.id == TELEGRAM_SETTINGS.TG_FRIEND_GROUP_ID)
 async def group_message(message: types.Message):
     if is_reply(message) or FRIEND_GROUP_BOT.should_react(message.md_text):
         await tg_bot.send_chat_action(message.chat.id, 'typing')
-        user_text = await get_message_text(message, tg_bot)
+        user_text = await preprocessor.process_tg_message(message, tg_bot)
+        if user_text is None:
+            return None  # do not reply
         logging.getLogger().info(f"group_message: from {message.from_user.full_name} in {message.chat.title} processed")
 
         await tg_bot.send_chat_action(message.chat.id, 'typing')
         # not using author not to send usernames to openai :)
         reply_text = await FRIEND_GROUP_BOT.heed_and_reply(user_text)  # author=message.from_user.full_name
         await asyncio.sleep(random.uniform(0, 2))
         chunks = split_text_into_chunks_by_sentences(reply_text,
```

### Comparing `kibernikto-1.3.6/kibernikto/telegram/telegram_bot.py` & `kibernikto-1.4.0/kibernikto/telegram/telegram_bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from openai._types import NOT_GIVEN
+
 from kibernikto.interactors import OpenAIExecutor, OpenAiExecutorConfig
 
 
 class TelegramBot(OpenAIExecutor):
-    def __init__(self, config: OpenAiExecutorConfig, master_id, username):
+    def __init__(self, config: OpenAiExecutorConfig, master_id, username, key=NOT_GIVEN):
+        self.key = key
         self.master_id = master_id
         self.username = username
         super().__init__(config=config)
 
     def should_react(self, message_text):
         if not message_text:
             return False
```

### Comparing `kibernikto-1.3.6/kibernikto/telegram/whisper_openai_v1.py` & `kibernikto-1.4.0/kibernikto/telegram/whisper_openai_v1.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/utils/ai_tools.py` & `kibernikto-1.4.0/kibernikto/utils/ai_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import json
 import logging
 import pprint
 import uuid
 from json import JSONDecodeError
 from typing import Callable, List
 
@@ -14,63 +15,69 @@
 from ..interactors.tools import Toolbox
 
 
 def tool_to_claude_dict(tool: Toolbox):
     tool_dict = tool.definition
     tool_func = tool_dict['function']
     parameters = []
-    for prop in tool_func['parameters']['properties'].items():
-        name, prop_params = prop
-        parameters.append({
-            'name': name,
-            'description': prop_params.get('description', name),
-            'type': prop_params['type']
-        })
+    if 'parameters' in tool_func and 'properties' in tool_func['parameters']:
+        for prop in tool_func['parameters']['properties'].items():
+            name, prop_params = prop
+            parameters.append({
+                'name': name,
+                'description': prop_params.get('description', name),
+                'type': prop_params['type']
+            })
     claude_dict = {"tool_name": tool_func['name'],
                    "description": tool_func['description'],
                    "parameters": {"parameter": parameters}
                    }
 
     return claude_dict
 
 
 def is_function_call(choice: Choice, xml=False):
     if not xml:
         return choice.finish_reason == "tool_calls"
     else:
-        if 'function_name' in choice.message.content and 'parameters' in choice.message.content:
+        if 'function_name' in choice.message.content and 'call_id' in choice.message.content:
             try:
                 logging.warning(choice.message.content)
                 function_string = choice.message.content.replace('\n', ' ').replace('\r', '')
                 call_dict = parse_json_garbage(function_string)
                 # call_dict = json.loads(json_string)
                 pprint.pprint(call_dict)
             except JSONDecodeError as err:
                 logging.error(str(err))
                 return False
             new_ai_tool_call = ChatCompletionMessageToolCall(
-                id=str(uuid.uuid4()),
+                id=str(call_dict['call_id']),
                 type="function",
                 function=Function(name=call_dict['function_name'],
                                   arguments=json.dumps(call_dict['parameters'])
                                   ))
             choice.message.tool_calls = [new_ai_tool_call]
             return True
     return False
 
 
 async def execute_tool_call_function(tool_call: ChatCompletionMessageToolCall,
-                                     function_impl: Callable):
+                                     function_impl: Callable, additional_params: dict = {}):
     tool_call_function: Function = tool_call.function
     fn_name = tool_call_function.name
     arguments: str = tool_call_function.arguments
 
     dict_args = json.loads(arguments)
-    logging.info(f"running {fn_name}")
-    pprint.pprint(dict_args)
+
+    impl_params = inspect.getfullargspec(function_impl)[0]
+
+    for key in additional_params:
+        if key in impl_params:
+            dict_args[key] = additional_params[key]
+    logging.info(f"running {fn_name} with params {dict_args}")
     try:
         result = await function_impl(**dict_args)
     except Exception as e:
         result = str(e)
     return result
 
 
@@ -139,14 +146,15 @@
     call_example = """
                 {
                     "function_name": $TOOL_NAME,
                     "parameters": {
                         "$PARAM_NAME": $PARAM_VALUE
                         ...
                     },
+                    "call_id": $RANDOM
                 }
             """
     tools_content = f"""
     In this environment you have access to a set of tools you can use to answer the user's question. 
     To let me know you want to call a tool return only tool call description JSON without any comments.
     Like this:
     {call_example}\n
```

### Comparing `kibernikto-1.3.6/kibernikto/utils/audio.py` & `kibernikto-1.4.0/kibernikto/utils/audio.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/utils/environment.py` & `kibernikto-1.4.0/kibernikto/utils/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,14 @@
     if REDACTOR_SETTINGS.OPENAI_API_KEY is not None:
         print("\t")
         print('\t%-15s%-15s' % ("redact model:", REDACTOR_SETTINGS.OPENAI_API_MODEL))
         print('\t%-15s%-15s' % ("redact host:", REDACTOR_SETTINGS.OPENAI_BASE_URL))
     else:
         print('\t%-15s%-15s' % ("redactor:", 'disabled'))
 
-    from kibernikto.telegram.single_group_dispatcher import TELEGRAM_SETTINGS
-    print("\t")
-    print('\t%-15s%-15s' % ("tg master:", TELEGRAM_SETTINGS.TG_MASTER_ID))
-    print('\t%-15s%-15s' % ("tg group:", TELEGRAM_SETTINGS.TG_FRIEND_GROUP_ID))
-
 
 def print_plugin_banner(kbnktp_plgn: KiberniktoPlugin):
     print("\t")
     plgn_name = kbnktp_plgn.__class__.__name__
     print('\t%-15s%-15s' % (f"{plgn_name} model: ", kbnktp_plgn.model))
     print('\t%-15s%-15s' % (f"{plgn_name} host: ", kbnktp_plgn.base_url))
 
@@ -47,14 +42,17 @@
     logging.basicConfig(
         format='%(levelname)-8s %(asctime)s %(name)s:%(filename)s:%(lineno)d %(message)s',
         datefmt='%Y-%m-%d:%H:%M:%S',
         level=logging.DEBUG)
     logger = logging.getLogger('openai')
     logger.setLevel(logging.INFO)
 
+    logger = logging.getLogger('aiosqlite')
+    logger.setLevel(logging.ERROR)
+
     logger = logging.getLogger('httpcore')
     logger.setLevel(logging.INFO)
 
     logger = logging.getLogger('httpx')
     logger.setLevel(logging.INFO)
 
     logger = logging.getLogger('asyncio')
```

### Comparing `kibernikto-1.3.6/kibernikto/utils/image.py` & `kibernikto-1.4.0/kibernikto/utils/image.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/utils/psycopg.py` & `kibernikto-1.4.0/kibernikto/utils/psycopg.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto/utils/text.py` & `kibernikto-1.4.0/kibernikto/utils/text.py`

 * *Files identical despite different names*

### Comparing `kibernikto-1.3.6/kibernikto.egg-info/PKG-INFO` & `kibernikto-1.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: kibernikto
-Version: 1.3.6
+Version: 1.4.0
 Summary: Easily run telegram bots connected to AI models.
 Home-page: https://github.com/solovieff/kibernikto
 Author-email: solovieff.nnov@gmail.com
 License: GPL-3.0 license
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiogram==3.1.1
+Requires-Dist: aiogram==3.5.0
+Requires-Dist: aiofiles==23.2.1
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: openai==1.3.0
+Requires-Dist: openai==1.3.6
 Requires-Dist: youtube_transcript_api==0.6.1
 Requires-Dist: pytube==15.0
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: emoji-country-flag==1.3.2
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: pydantic-settings
 Requires-Dist: pydub
@@ -27,21 +28,24 @@
 Requires-Dist: psycopg-pool==3.2
 Requires-Dist: dict2xml==1.7.5
 Requires-Dist: fujson==0.1.1
 
 # kibernikto
 
 Kibernikto is an app/lib to easily run telegram bots connected to AI models with additional features.  
-Kibernikto bots can be easily extended to be used outised telegram.
+Kibernikto bots can be easily extended to be used outside telegram.  
+Core and bots can be used as a core libs for creating ai-bot based apps.  
 
-- voice messages recognition
-- youtube video summary
-- webpage summary
-- image recognition
-- function tools easy integration (anthropic xml format supported!)
+- ✍️ telegram conversations with different AIs in groups or privately (including hidden second-level AI-redactors)
+- 🔉 voice messages recognition
+- 👂 interviews and meetings (up to 2 hours) analysis right in Telegram using Gladia.io 
+- 🎞 youtube video summarization
+- 🔗 webpage summarization
+- 📸 image recognition
+- 🫡 openai function tools easy [integration](https://github.com/solovieff/kibernikto-planner). No more pain. ~~(anthropic xml format supported, too! looks like they changed it again)~~
 
 Given an image Kibernikto will publish it to a free image hosting service and then process as a link.
 
 By default `single_group_dispatcher` is used with a following rules:
 
 - One Kibernikto instance **can privately talk only to one** (`TG_MASTER_ID`) user and work with **one group chat
   ** (`TG_FRIEND_GROUP_ID`).
@@ -49,16 +53,16 @@
 If you want your bot to be able to work with **any user or group**, use `comprehensive_dispatcher`. You will need the
 following `additional` env parameters if you want to restrict user/group ids.
 Do not add it to your env if you want anyone
 to
 be able to use yr Kibernikto instance:
 
 ```dotenv
-TG_MASTER_IDS=[199720543]
-TG_FRIEND_GROUP_IDS=[-813228576]
+TG_MASTER_IDS=[XXXXXXXXX]
+TG_FRIEND_GROUP_IDS=[-XXXXXXXXX]
 ```
 
 or
 
 ``kibernikto --env_file_path=local.env --bot_type=kibernikto --dispatcher=multiuser``
 
 Kibernikto can post-process messages returned by one AI using another AI (for now it's a hardcoded 2 step chain).
@@ -121,61 +125,100 @@
 Other AI behaviour options:
 
 ```dotenv
 OPENAI_MAX_TOKENS=800  
 OPENAI_WHO_AM_I=Answer all questions as {0}, the majestic lord of the universes with all the knowledge of our small planet.  
 ```
 
-WeblinkSummaryPlugin and YoutubePlugin.
+**Telegram**
+
+```dotenv
+# Telegram configuration
+TG_BOT_KEY=XXXXXXXXXX:XXXxxxXXXxxxxXXXxxx  
+TG_BOT_MAX_HISTORY=8  
+TG_FRIEND_GROUP_ID=-XXXXXXXXXX  
+# Your telegram ID. For example 122349243. Forward your message to @idstickerbot to get it.  
+TG_MASTER_ID=XXXXXXXXX
+# Kibernikto reacts to direct replies or when sees the following words. 
+# Preserving pydantic-settings list format.  
+TG_REACTION_CALLS=["киберникто","государь"]  
+# sometimes Kibernikto sends stickers for fun together with his answers  
+TG_STICKER_LIST=["CAACAgIAAxkBAAEKqsplQ8BRyPbGj_B_K4ujCLsDAe-l7wAC8AIAAs-71A7mCrGe-zzi0DME","CAACAgIAAxkBAAEIgoxkMaHv1maOeEne8CYAAY5s4kJ1e4wAAo4JAAIItxkCXSMuZ6bo59gvBA"]
+```
+
+
+- **WeblinkSummaryPlugin and YoutubePlugin**
 
 ```dotenv
 # If no key is provided, youtube videos and webpages will be ignored.
 SUMMARIZATION_OPENAI_API_KEY=yr-key
 SUMMARIZATION_OPENAI_API_BASE_URL=https://api.openai.com/v1  
 SUMMARIZATION_OPENAI_API_MODEL=gpt-4-turbo-preview
 ```
 
-ImageSummaryPlugin to process images.
+- **ImageSummaryPlugin to process images.**
 
 ```dotenv
 # If no key is provided, images will not be processed.
 IMAGE_SUMMARIZATION_OPENAI_API_KEY=yr-key
 IMAGE_SUMMARIZATION_OPENAI_API_MODEL=gpt-4-vision-preview
 IMAGE_SUMMARIZATION_OPENAI_API_BASE_URL=https://api.openai.com/v1
 
 # You can get your key here: https://imgbb.com. If you do no set up this variable, default one will be used.  
 # This is needed to store images send to the bot.  
 IMAGE_STORAGE_API_KEY = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
 ```
 
-Voice messages processing
+- **Voice messages** processing using **OpenAI**:
 
 ```dotenv
 # If no key is provided, voice messages will not be processed.
+VOICE_PROCESSOR=openai
 VOICE_OPENAI_API_KEY=yr-key
 VOICE_OPENAI_API_MODEL=whisper-1
 VOICE_OPENAI_API_BASE_URL=https://api.openai.com/v1
-VOICE_PROCESSOR=openai
-VOICE_FILE_LOCATION=/tmp/tg_voices
+VOICE_FILE_LOCATION=/tmp
 ```
+    
+- **Voice messages** processing using [gladia.io](https://gladia.io):  
+**Gladia** Audio Intelligence API, is designed to enable any company to easily 
+embed top-quality Audio AI into their applications, whatever the tech stack.  
+    
+As whisper api is limited to 25 megs, [gladia.io](https://glaudia.io) helps to process bigger files.    
+
+Kibernikto treats voice messages with duration less than `VOICE_MIN_COMPLEX_SECONDS` as usual AI interaction ones.
+For longer durations Kibernikto will return detailed audio 
+analysis including summary etc.  
+
+Perfect solution for analyzing interviews and meeting.  
+Gladia price policies are also very affordable.
+
+```dotenv
+VOICE_PROCESSOR=gladia
+VOICE_GLADIA_API_KEY=yr-gladia-key
+VOICE_GLADIA_SUMMARIZATION_TYPE=concise
+VOICE_MIN_COMPLEX_SECONDS=300
+```    
+   
+- **Smart voice messages** processing using both [gladia.io](https://gladia.io) and OpenAI:  
 
-Telegram
-
+Whisper api is a bit faster and looks better to use just for talking with your bot.
 ```dotenv
-# Telegram configuration
-TG_BOT_KEY=XXXXXXXXXX:XXXxxxXXXxxxxXXXxxx  
-TG_BOT_MAX_HISTORY=8  
-TG_FRIEND_GROUP_ID=-XXXXXXXXXX  
-# Your telegram ID. For example 122349243. Forward your message to @idstickerbot to get it.  
-TG_MASTER_ID=XXXXXXXXX
-# Kibernikto reacts to direct replies or when sees the following words. 
-# Preserving pydantic-settings list format.  
-TG_REACTION_CALLS=["киберникто","государь"]  
-# sometimes Kibernikto sends stickers for fun together with his answers  
-TG_STICKER_LIST=["CAACAgIAAxkBAAEKqsplQ8BRyPbGj_B_K4ujCLsDAe-l7wAC8AIAAs-71A7mCrGe-zzi0DME","CAACAgIAAxkBAAEIgoxkMaHv1maOeEne8CYAAY5s4kJ1e4wAAo4JAAIItxkCXSMuZ6bo59gvBA"]
+VOICE_PROCESSOR=**auto**
+
+VOICE_OPENAI_API_KEY=yr-key
+VOICE_OPENAI_API_MODEL=whisper-1
+VOICE_OPENAI_API_BASE_URL=https://api.openai.com/v1
+VOICE_FILE_LOCATION=/tmp
+
+#starting this audio length Kibernikto will start using Gladia and deeper analysis
+VOICE_MIN_COMPLEX_SECONDS=300
+VOICE_GLADIA_API_KEY=yr-gladia-key
+VOICE_GLADIA_SUMMARIZATION_TYPE=concise
+VOICE_GLADIA_CONTEXT=We have before us an interview for the position of office manager
 ```
 
 For the full list of variables, see `env_examples` folder.
 
 # redactor mode
 
 To run Kibernikto with additional redactor for each response change the `bot_type` to "vertihvostka":    
@@ -196,14 +239,15 @@
 
 To create and operate your bot: https://t.me/BotFather  
 To obtain group/user ids etc: https://t.me/getidsbot  
 To obtain sticker ids: https://t.me/idstickerbot  
 To get familiar with basic OpenAI principles: https://openai.com  
 Basics on Gpt-4 vision: https://gptpluginz.com/gpt-4-vision-api  
 To find out more on models and multi-model api details: https://vsegpt.ru/Docs/Models  
+Audio analysis: https://gladia.io  
 Website to text and other helpful tools https://toolsyep.com  
 Free image hosting: https://imgbb.com
 
 # code details
 
 *(ignore it if dont plan to create yr own plugins or Kibernikto bots using Kibernikto as a library)*
```

### Comparing `kibernikto-1.3.6/kibernikto.egg-info/SOURCES.txt` & `kibernikto-1.4.0/kibernikto.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 kibernikto/plugins/__init__.py
 kibernikto/plugins/_img_summarizator.py
 kibernikto/plugins/_kibernikto_plugin.py
 kibernikto/plugins/_weblink_summarizator.py
 kibernikto/plugins/_youtube_summarizator.py
 kibernikto/telegram/__init__.py
 kibernikto/telegram/_executor_corral.py
-kibernikto/telegram/_message_preprocessors.py
 kibernikto/telegram/comprehensive_dispatcher.py
 kibernikto/telegram/single_group_dispatcher.py
 kibernikto/telegram/telegram_bot.py
 kibernikto/telegram/whisper_openai_v1.py
+kibernikto/telegram/pre_processors/__init__.py
+kibernikto/telegram/pre_processors/_default.py
+kibernikto/telegram/pre_processors/_gladia.py
 kibernikto/utils/__init__.py
 kibernikto/utils/ai_tools.py
 kibernikto/utils/audio.py
 kibernikto/utils/environment.py
 kibernikto/utils/image.py
 kibernikto/utils/psycopg.py
 kibernikto/utils/text.py
```

### Comparing `kibernikto-1.3.6/setup.py` & `kibernikto-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 with open(path.join(HERE, "requirements.txt")) as f:
     required = f.read().splitlines()
 
 setup(
     name="kibernikto",
-    version="1.3.6",
+    version="1.4.0",
     packages=find_packages(),
     install_requires=required,
     url='https://github.com/solovieff/kibernikto',
     license='GPL-3.0 license',
     author_email='solovieff.nnov@gmail.com',
     description='Easily run telegram bots connected to AI models.',
     long_description=long_description,
```

