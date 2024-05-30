# Comparing `tmp/genshin-1.6.3.tar.gz` & `tmp/genshin-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genshin-1.6.3.tar", last modified: Wed Apr 10 17:59:08 2024, max compression
+gzip compressed data, was "genshin-1.7.0.tar", last modified: Thu May 30 13:06:04 2024, max compression
```

## Comparing `genshin-1.6.3.tar` & `genshin-1.7.0.tar`

### file list

```diff
@@ -1,127 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.444755 genshin-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 17:59:04.000000 genshin-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 17:59:08.444755 genshin-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-10 17:59:04.000000 genshin-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.424755 genshin-1.6.3/genshin/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.428755 genshin-1.6.3/genshin/client/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.428755 genshin-1.6.3/genshin/client/components/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18522 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.428755 genshin-1.6.3/genshin/client/components/calculator/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/calculator/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/calculator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/client/components/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/genshin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/honkai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/starrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/gacha.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/client/components/geetest/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/geetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/geetest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/geetest/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/hoyolab.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/lineup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/teapot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/client/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/manager/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/manager/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/models/genshin/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/genshin/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/abyss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/tcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/lineup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/teapot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/honkai/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/battlesuit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/honkai/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/battlesuits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/hoyolab/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/private.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/miyoushe/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/miyoushe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/miyoushe/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/miyoushe/qrcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/starrail/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin/models/starrail/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/rogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin/paginators/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/paginators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/paginators/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/paginators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/extdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/geetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-10 17:59:04.000000 genshin-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:59:08.444755 genshin-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 17:59:04.000000 genshin-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:04.000000 genshin-1.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-10 17:59:04.000000 genshin-1.6.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-10 17:59:04.000000 genshin-1.6.3/tests/test_paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-30 13:06:00.000000 genshin-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-30 13:06:04.928471 genshin-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-30 13:06:00.000000 genshin-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.908470 genshin-1.7.0/genshin/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.912471 genshin-1.7.0/genshin/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.912471 genshin-1.7.0/genshin/client/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.912471 genshin-1.7.0/genshin/client/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/components/auth/subclients/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21107 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/components/calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/calculator/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/calculator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/components/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/genshin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/honkai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/starrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/hoyolab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/manager/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17675 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/manager/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/geetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/genshin/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/genshin/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/abyss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/tcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/honkai/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/battlesuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/honkai/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/battlesuits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/hoyolab/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/starrail/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/starrail/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/rogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/paginators/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/paginators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/paginators/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/paginators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/genshin/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/extdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/genshin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-30 13:06:00.000000 genshin-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:06:04.928471 genshin-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 13:06:00.000000 genshin-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:00.000000 genshin-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-30 13:06:00.000000 genshin-1.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 13:06:00.000000 genshin-1.7.0/tests/test_paginators.py
```

### Comparing `genshin-1.6.3/LICENSE` & `genshin-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/PKG-INFO` & `genshin-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.6.3
+Version: 1.7.0
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
@@ -28,17 +28,17 @@
 Provides-Extra: all
 Requires-Dist: browser-cookie3; extra == "all"
 Requires-Dist: rsa; extra == "all"
 Requires-Dist: click; extra == "all"
 Requires-Dist: qrcode[pil]; extra == "all"
 Provides-Extra: cookies
 Requires-Dist: browser-cookie3; extra == "cookies"
-Provides-Extra: geetest
-Requires-Dist: rsa; extra == "geetest"
-Requires-Dist: qrcode[pil]; extra == "geetest"
+Provides-Extra: auth
+Requires-Dist: rsa; extra == "auth"
+Requires-Dist: qrcode[pil]; extra == "auth"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 # genshin.py
 
 [![Downloads](https://pepy.tech/badge/genshin)](https://pepy.tech/project/genshin)
 [![PyPI package](https://img.shields.io/pypi/v/genshin)](https://pypi.org/project/genshin/)
```

### Comparing `genshin-1.6.3/README.md` & `genshin-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/__main__.py` & `genshin-1.7.0/genshin/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     data = await client.get_honkai_user(uid)
 
     click.secho("Stats:", fg="yellow")
     for k, v in data.stats.as_dict(lang=client.lang).items():
         if isinstance(v, dict):
             click.echo(f"{k}:")
-            for nested_k, nested_v in typing.cast("dict[str, object]", v).items():
+            for nested_k, nested_v in typing.cast("typing.Dict[str, object]", v).items():
                 click.echo(f"  {nested_k}: {click.style(str(nested_v), bold=True)}")
         else:
             click.echo(f"{k}: {click.style(str(v), bold=True)}")
 
 
 @genshin_group.command("stats")
 @click.argument("uid", type=int)
@@ -334,16 +334,16 @@
 @click.option("-a", "--account", default=None, prompt=True)
 @click.option("-p", "--password", default=None, prompt=True, hide_input=True)
 @click.option("--port", help="Webserver port.", type=int, default=5000)
 @asynchronous
 async def login(account: str, password: str, port: int) -> None:
     """Login with a password."""
     client = genshin.Client()
-    cookies = await client.login_with_password(account, password, port=port)
-    cookies = await genshin.complete_cookies(cookies)
+    result = await client.os_login_with_password(account, password, port=port)
+    cookies = await genshin.complete_cookies(result.dict())
 
     base: http.cookies.BaseCookie[str] = http.cookies.BaseCookie(cookies)
     click.echo(f"Your cookies are: {click.style(base.output(header='', sep=';'), bold=True)}")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `genshin-1.6.3/genshin/client/cache.py` & `genshin-1.7.0/genshin/client/cache.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/clients.py` & `genshin-1.7.0/genshin/client/clients.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """A simple HTTP client for API endpoints."""
 
 from .components import (
+    auth,
     calculator,
     chronicle,
     daily,
     diary,
     gacha,
-    geetest,
     hoyolab,
     lineup,
     teapot,
     transaction,
     wiki,
 )
 
@@ -24,10 +24,10 @@
     calculator.CalculatorClient,
     diary.DiaryClient,
     lineup.LineupClient,
     teapot.TeapotClient,
     wiki.WikiClient,
     gacha.WishClient,
     transaction.TransactionClient,
-    geetest.GeetestClient,
+    auth.AuthClient,
 ):
     """A simple HTTP client for API endpoints."""
```

### Comparing `genshin-1.6.3/genshin/client/compatibility.py` & `genshin-1.7.0/genshin/client/compatibility.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/base.py` & `genshin-1.7.0/genshin/client/components/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base ABC Client."""
 
 import abc
 import asyncio
 import base64
+import functools
 import json
 import logging
 import os
 import typing
 import urllib.parse
 import warnings
 
@@ -20,32 +21,48 @@
 from genshin.models import hoyolab as hoyolab_models
 from genshin.models import model as base_model
 from genshin.utility import concurrency, deprecation, ds
 
 __all__ = ["BaseClient"]
 
 
+T = typing.TypeVar("T")
+CallableT = typing.TypeVar("CallableT", bound="typing.Callable[..., object]")
+AsyncCallableT = typing.TypeVar("AsyncCallableT", bound="typing.Callable[..., typing.Awaitable[object]]")
+
+
 class BaseClient(abc.ABC):
     """Base ABC Client."""
 
-    __slots__ = ("cookie_manager", "cache", "_lang", "_region", "_default_game", "uids", "authkeys", "_hoyolab_id")
+    __slots__ = (
+        "cookie_manager",
+        "cache",
+        "_lang",
+        "_region",
+        "_default_game",
+        "uids",
+        "authkeys",
+        "_hoyolab_id",
+        "_accounts",
+    )
 
     USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36"  # noqa: E501
 
     logger: logging.Logger = logging.getLogger(__name__)
 
     cookie_manager: managers.BaseCookieManager
     cache: client_cache.BaseCache
     _lang: str
     _region: types.Region
     _default_game: typing.Optional[types.Game]
 
     uids: typing.Dict[types.Game, int]
     authkeys: typing.Dict[types.Game, str]
     _hoyolab_id: typing.Optional[int]
+    _accounts: typing.Dict[types.Game, hoyolab_models.GenshinAccount]
 
     def __init__(
         self,
         cookies: typing.Optional[managers.AnyCookieOrHeader] = None,
         *,
         authkey: typing.Optional[str] = None,
         lang: str = "en-us",
@@ -58,14 +75,15 @@
         debug: bool = False,
     ) -> None:
         self.cookie_manager = managers.BaseCookieManager.from_cookies(cookies)
         self.cache = cache or client_cache.StaticCache()
 
         self.uids = {}
         self.authkeys = {}
+        self._accounts = {}
 
         self.default_game = game
         self.lang = lang
         self.region = region
         self.authkey = authkey
         self.debug = debug
         self.proxy = proxy
@@ -490,14 +508,47 @@
         await self._update_cached_uids()
 
         if uid := self.uids.get(game):
             return uid
 
         raise errors.AccountNotFound(msg="No UID provided and account has no game account bound to it.")
 
+    async def _update_cached_accounts(self) -> None:
+        """Update cached fallback accounts."""
+        mixed_accounts = await self.get_game_accounts()
+
+        game_accounts: typing.Dict[types.Game, typing.List[hoyolab_models.GenshinAccount]] = {}
+        for account in mixed_accounts:
+            if not isinstance(account.game, types.Game):  # pyright: ignore[reportUnnecessaryIsInstance]
+                continue
+
+            game_accounts.setdefault(account.game, []).append(account)
+
+        self._accounts = {}
+        for game, accounts in game_accounts.items():
+            self._accounts[game] = next(
+                (acc for acc in accounts if acc.uid == self.uids.get(game)), max(accounts, key=lambda a: a.level)
+            )
+
+    @concurrency.prevent_concurrency
+    async def _get_account(self, game: types.Game) -> hoyolab_models.GenshinAccount:
+        """Get a cached fallback account."""
+        if (account := self._accounts.get(game)) and (uid := self.uids.get(game)) and account.uid == uid:
+            return account
+
+        await self._update_cached_accounts()
+
+        if account := self._accounts.get(game):
+            if (uid := self.uids.get(game)) and account.uid != uid:
+                raise errors.AccountNotFound(msg="There is no game account with such UID.")
+
+            return account
+
+        raise errors.AccountNotFound(msg="Account has no game account bound to it.")
+
     def _get_hoyolab_id(self) -> int:
         """Get a cached fallback hoyolab ID."""
         if self.hoyolab_id is not None:
             return self.hoyolab_id
 
         if self.cookie_manager.multi:
             raise RuntimeError("Hoyolab ID must be provided when using multi-cookie managers.")
@@ -530,7 +581,26 @@
 
         coros: typing.List[typing.Awaitable[None]] = []
         for key in routes.MI18N:
             for lang in langs:
                 coros.append(self._fetch_mi18n(key, lang, force=force))
 
         await asyncio.gather(*coros)
+
+
+def region_specific(region: types.Region) -> typing.Callable[[AsyncCallableT], AsyncCallableT]:
+    """Prevent function to be ran with unsupported regions."""
+
+    def decorator(func: AsyncCallableT) -> AsyncCallableT:
+        @functools.wraps(func)
+        async def wrapper(self: typing.Any, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
+
+            if not hasattr(self, "region"):
+                raise TypeError("Cannot use @region_specific on a plain function.")
+            if region != self.region:
+                raise RuntimeError("The method can only be used with client region set to " + region)
+
+            return await func(self, *args, **kwargs)
+
+        return typing.cast("AsyncCallableT", wrapper)
+
+    return decorator
```

### Comparing `genshin-1.6.3/genshin/client/components/calculator/calculator.py` & `genshin-1.7.0/genshin/client/components/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/calculator/client.py` & `genshin-1.7.0/genshin/client/components/calculator/client.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/chronicle/base.py` & `genshin-1.7.0/genshin/client/components/chronicle/base.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/chronicle/genshin.py` & `genshin-1.7.0/genshin/client/components/chronicle/genshin.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/chronicle/honkai.py` & `genshin-1.7.0/genshin/client/components/chronicle/honkai.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/chronicle/starrail.py` & `genshin-1.7.0/genshin/client/components/chronicle/starrail.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/daily.py` & `genshin-1.7.0/genshin/client/components/daily.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import functools
 import typing
 import uuid
 
 import aiohttp.typedefs
 
-from genshin import constants, paginators, types, utility
+from genshin import constants, paginators, types
 from genshin.client import cache, routes
 from genshin.client.components import base
 from genshin.client.manager import managers
 from genshin.models.genshin import daily as models
 from genshin.utility import ds as ds_utility
 
 __all__ = ["DailyRewardClient"]
@@ -50,31 +50,30 @@
         url = (base_url / endpoint).update_query(**base_url.query)
 
         if self.region == types.Region.OVERSEAS:
             params["lang"] = lang or self.lang
             headers["referer"] = "https://act.hoyolab.com/"
 
         elif self.region == types.Region.CHINESE:
-            uid = await self._get_uid(game)
+            account = await self._get_account(game)
 
-            params["uid"] = uid
-            params["region"] = utility.recognize_server(uid, game)
+            params["uid"] = account.uid
+            params["region"] = account.server
 
-            # most of the extra headers are likely just placebo
-            headers["x-rpc-app_version"] = "2.34.1"
+            # These headers are optional but left here because they might affect geetest trigger rate
+            headers["x-rpc-app_version"] = "2.70.1"
             headers["x-rpc-client_type"] = "5"
             headers["x-rpc-device_id"] = str(uuid.uuid4())
             headers["x-rpc-sys_version"] = "12"
             headers["x-rpc-platform"] = "android"
             headers["x-rpc-channel"] = "miyousheluodi"
             headers["x-rpc-device_model"] = str(self.hoyolab_id) or ""
-            headers["referer"] = (
-                "https://webstatic.mihoyo.com/bbs/event/signin-ys/index.html?"
-                "bbs_auth_required=true&act_id=e202009291139501&utm_source=bbs&utm_medium=mys&utm_campaign=icon"
-            )
+
+            if game == types.Game.GENSHIN:
+                headers["x-rpc-signgame"] = "hk4e"
 
             headers["ds"] = ds_utility.generate_dynamic_secret(constants.DS_SALT["cn_signin"])
 
         else:
             raise TypeError(f"{self.region!r} is not a valid region.")
 
         if challenge:
```

### Comparing `genshin-1.6.3/genshin/client/components/diary.py` & `genshin-1.7.0/genshin/client/components/diary.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/gacha.py` & `genshin-1.7.0/genshin/client/components/gacha.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/geetest/client.py` & `genshin-1.7.0/genshin/client/manager/managers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,563 +1,512 @@
-"""Geetest client component."""
+"""Cookie managers for making authenticated requests."""
 
-import asyncio
-import json
+from __future__ import annotations
+
+import abc
+import functools
+import http.cookies
 import logging
-import random
 import typing
-from string import ascii_letters, digits
+import warnings
 
 import aiohttp
-import aiohttp.web
-import qrcode
-import qrcode.image.pil
-from qrcode.constants import ERROR_CORRECT_L
+import aiohttp.typedefs
+import yarl
 
-from genshin import constants, errors
-from genshin.client import routes
-from genshin.client.components import base
-from genshin.client.manager.cookie import fetch_cookie_token_by_game_token, fetch_stoken_by_game_token
-from genshin.models.miyoushe.qrcode import QRCodeCheckResult, QRCodeCreationResult, QRCodeStatus
-from genshin.utility import ds as ds_utility
-from genshin.utility import geetest as geetest_utility
+from genshin import errors, types
+from genshin.client import ratelimit
+from genshin.utility import fs as fs_utility
 
-from . import server
+from ...constants import MIYOUSHE_GEETEST_RETCODES
 
-__all__ = ["GeetestClient"]
+_LOGGER = logging.getLogger(__name__)
 
-LOGGER_ = logging.getLogger(__name__)
+__all__ = [
+    "BaseCookieManager",
+    "CookieManager",
+    "InternationalCookieManager",
+    "RotatingCookieManager",
+    "parse_cookie",
+]
 
+CookieOrHeader = typing.Union["http.cookies.BaseCookie[typing.Any]", typing.Mapping[typing.Any, typing.Any], str]
+AnyCookieOrHeader = typing.Union[CookieOrHeader, typing.Sequence[CookieOrHeader]]
 
-class GeetestClient(base.BaseClient):
-    """Geetest client component."""
+T = typing.TypeVar("T")
+CallableT = typing.TypeVar("CallableT", bound="typing.Callable[..., object]")
+AsyncCallableT = typing.TypeVar("AsyncCallableT", bound="typing.Callable[..., typing.Awaitable[object]]")
+MaybeSequence = typing.Union[T, typing.Sequence[T]]
 
-    async def _web_login(
-        self,
-        account: str,
-        password: str,
-        *,
-        tokenType: typing.Optional[int] = 6,
-        geetest: typing.Optional[typing.Dict[str, typing.Any]] = None,
-    ) -> typing.Dict[str, typing.Any]:
-        """Login with a password using web endpoint.
 
-        Returns either data from aigis header or cookies.
-        """
-        headers = {**geetest_utility.WEB_LOGIN_HEADERS}
-        if geetest:
-            mmt_data = geetest["data"]
-            session_id = geetest["session_id"]
-            headers["x-rpc-aigis"] = geetest_utility.get_aigis_header(session_id, mmt_data)
-
-        payload = {
-            "account": geetest_utility.encrypt_geetest_credentials(account, self._region),
-            "password": geetest_utility.encrypt_geetest_credentials(password, self._region),
-            "token_type": tokenType,
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.WEB_LOGIN_URL.get_url(),
-                json=payload,
-                headers=headers,
-            ) as r:
-                data = await r.json()
-                cookies = {cookie.key: cookie.value for cookie in r.cookies.values()}
-
-        if data["retcode"] == -3101:
-            # Captcha triggered
-            aigis = json.loads(r.headers["x-rpc-aigis"])
-            aigis["data"] = json.loads(aigis["data"])
-            return aigis
+def parse_cookie(cookie: typing.Optional[CookieOrHeader]) -> typing.Dict[str, str]:
+    """Parse a cookie or header into a cookie mapping."""
+    if cookie is None:
+        return {}
 
-        if not data["data"]:
-            errors.raise_for_retcode(data)
+    if isinstance(cookie, str):
+        cookie = http.cookies.SimpleCookie(cookie)
 
-        if data["data"].get("stoken"):
-            cookies["stoken"] = data["data"]["stoken"]
+    return {str(k): v.value if isinstance(v, http.cookies.Morsel) else str(v) for k, v in cookie.items()}
 
-        self.set_cookies(cookies)
 
-        return cookies
+def get_cookie_identifier(cookie: typing.Mapping[str, str]) -> typing.Optional[str]:
+    """Get a unique identifier for a cookie."""
+    for name, value in cookie.items():
+        if name in ("ltuid", "account_id", "ltuid_v2", "account_id_v2"):
+            return value
 
-    async def _cn_login_by_password(
-        self,
-        account: str,
-        password: str,
-        *,
-        geetest: typing.Optional[typing.Dict[str, typing.Any]] = None,
-    ) -> typing.Dict[str, typing.Any]:
-        """
-        Login with account and password using Miyoushe loginByPassword endpoint.
+    # fallback non-digit identifier
+    for name, value in cookie.items():
+        if name in ("ltmid_v2", "account_mid_v2"):
+            return value
+
+    return None
+
+
+class BaseCookieManager(abc.ABC):
+    """A cookie manager for making requests."""
+
+    _proxy: typing.Optional[yarl.URL] = None
+
+    @classmethod
+    def from_cookies(cls, cookies: typing.Optional[AnyCookieOrHeader] = None) -> BaseCookieManager:
+        """Create an arbitrary cookie manager implementation instance."""
+        if not cookies:
+            return CookieManager()
+
+        if isinstance(cookies, typing.Sequence) and not isinstance(cookies, str):
+            return RotatingCookieManager(cookies)
+
+        return CookieManager(cookies)
+
+    @classmethod
+    def from_browser_cookies(cls, browser: typing.Optional[str] = None) -> CookieManager:
+        """Create a cookie manager with browser cookies."""
+        manager = CookieManager()
+        manager.set_browser_cookies(browser)
+
+        return manager
+
+    @property
+    def available(self) -> bool:
+        """Whether the authentication cookies are available."""
+        return True
+
+    @property
+    def multi(self) -> bool:
+        """Whether the cookie manager contains multiple cookies and therefore should not cache private data."""
+        return False
 
-        Returns data from aigis header or cookies.
+    @property
+    def user_id(self) -> typing.Optional[int]:
+        """The id of the user that owns cookies.
+
+        Returns None if not found or not applicable.
         """
-        headers = {
-            **geetest_utility.CN_LOGIN_HEADERS,
-            "ds": ds_utility.generate_dynamic_secret(constants.DS_SALT["cn_signin"]),
-        }
-        if geetest:
-            mmt_data = geetest["data"]
-            session_id = geetest["session_id"]
-            headers["x-rpc-aigis"] = geetest_utility.get_aigis_header(session_id, mmt_data)
-
-        payload = {
-            "account": geetest_utility.encrypt_geetest_credentials(account, self._region),
-            "password": geetest_utility.encrypt_geetest_credentials(password, self._region),
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.CN_WEB_LOGIN_URL.get_url(),
-                json=payload,
-                headers=headers,
-            ) as r:
-                data = await r.json()
-
-        if data["retcode"] == -3102:
-            # Captcha triggered
-            aigis = json.loads(r.headers["x-rpc-aigis"])
-            aigis["data"] = json.loads(aigis["data"])
-            return aigis
+        return None
 
-        if not data["data"]:
-            errors.raise_for_retcode(data)
+    @property
+    def proxy(self) -> typing.Optional[yarl.URL]:
+        """Proxy for http(s) requests."""
+        return self._proxy
+
+    @proxy.setter
+    def proxy(self, proxy: typing.Optional[aiohttp.typedefs.StrOrURL]) -> None:
+        if proxy is None:
+            self._proxy = None
+            return
+
+        proxy = yarl.URL(proxy)
+        if str(proxy.scheme) not in ("https", "http", "ws", "wss"):
+            raise ValueError("Proxy URL must have a valid scheme.")
+
+        self._proxy = proxy
+
+    def create_session(self, **kwargs: typing.Any) -> aiohttp.ClientSession:
+        """Create a client session."""
+        return aiohttp.ClientSession(
+            cookie_jar=aiohttp.DummyCookieJar(),
+            **kwargs,
+        )
 
-        cookies = {cookie.key: cookie.value for cookie in r.cookies.values()}
+    @ratelimit.handle_ratelimits()
+    async def _request(
+        self,
+        method: str,
+        str_or_url: aiohttp.typedefs.StrOrURL,
+        cookies: typing.MutableMapping[str, str],
+        **kwargs: typing.Any,
+    ) -> typing.Any:
+        """Make a request towards any json resource."""
+        async with self.create_session() as session:
+            async with session.request(method, str_or_url, proxy=self.proxy, cookies=cookies, **kwargs) as response:
+                if response.content_type != "application/json":
+                    content = await response.text()
+                    raise errors.GenshinException(msg="Recieved a response with an invalid content type:\n" + content)
+
+                data = await response.json()
+
+                if not self.multi:
+                    new_cookies = parse_cookie(response.cookies)
+                    new_keys = new_cookies.keys() - cookies.keys()
+                    if new_keys:
+                        cookies.update(new_cookies)
+                        _LOGGER.debug("Updating cookies for %s: %s", get_cookie_identifier(cookies), new_keys)
+
+        errors.check_for_geetest(data)
+
+        if data["retcode"] in MIYOUSHE_GEETEST_RETCODES:
+            raise errors.MiyousheGeetestError(data, {k: morsel.value for k, morsel in response.cookies.items()})
 
-        self.set_cookies(cookies)
-        return cookies
+        if data["retcode"] == 0:
+            return data["data"]
 
-    async def _app_login(
+        errors.raise_for_retcode(data)
+
+    @abc.abstractmethod
+    async def request(
         self,
-        account: str,
-        password: str,
+        url: aiohttp.typedefs.StrOrURL,
         *,
-        geetest: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        ticket: typing.Optional[typing.Dict[str, typing.Any]] = None,
-    ) -> typing.Dict[str, typing.Any]:
-        """Login with a password using HoYoLab app endpoint.
+        method: str = "GET",
+        params: typing.Optional[typing.Mapping[str, typing.Any]] = None,
+        data: typing.Any = None,
+        json: typing.Any = None,
+        cookies: typing.Optional[aiohttp.typedefs.LooseCookies] = None,
+        headers: typing.Optional[aiohttp.typedefs.LooseHeaders] = None,
+        **kwargs: typing.Any,
+    ) -> typing.Any:
+        """Make an authenticated request."""
 
-        Returns data from aigis header or action_ticket or cookies.
-        """
-        headers = {
-            **geetest_utility.APP_LOGIN_HEADERS,
-            "ds": ds_utility.generate_dynamic_secret(constants.DS_SALT["app_login"]),
-        }
-        if geetest:
-            mmt_data = geetest["data"]
-            session_id = geetest["session_id"]
-            headers["x-rpc-aigis"] = geetest_utility.get_aigis_header(session_id, mmt_data)
-
-        if ticket:
-            ticket["verify_str"] = json.dumps(ticket["verify_str"])
-            headers["x-rpc-verify"] = json.dumps(ticket)
-
-        payload = {
-            "account": geetest_utility.encrypt_geetest_credentials(account, self._region),
-            "password": geetest_utility.encrypt_geetest_credentials(password, self._region),
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.APP_LOGIN_URL.get_url(),
-                json=payload,
-                headers=headers,
-            ) as r:
-                data = await r.json()
-
-        if data["retcode"] == -3101:
-            # Captcha triggered
-            aigis = json.loads(r.headers["x-rpc-aigis"])
-            aigis["data"] = json.loads(aigis["data"])
-            return aigis
-
-        if data["retcode"] == -3239:
-            # Email verification required
-            verify = json.loads(r.headers["x-rpc-verify"])
-            verify["verify_str"] = json.loads(verify["verify_str"])
-            return verify
-
-        if not data["data"]:
-            errors.raise_for_retcode(data)
-
-        cookies = {
-            "stoken": data["data"]["token"]["token"],
-            "ltuid_v2": data["data"]["user_info"]["aid"],
-            "ltmid_v2": data["data"]["user_info"]["mid"],
-            "account_id_v2": data["data"]["user_info"]["aid"],
-            "account_mid_v2": data["data"]["user_info"]["mid"],
-        }
-        self.set_cookies(cookies)
 
-        return cookies
+class CookieManager(BaseCookieManager):
+    """Standard implementation of the cookie manager."""
 
-    async def _send_verification_email(
+    _cookies: typing.Dict[str, str]
+
+    def __init__(
         self,
-        ticket: typing.Dict[str, typing.Any],
-        *,
-        geetest: typing.Optional[typing.Dict[str, typing.Any]] = None,
-    ) -> typing.Union[None, typing.Dict[str, typing.Any]]:
-        """Send verification email.
+        cookies: typing.Optional[CookieOrHeader] = None,
+    ) -> None:
+        self.cookies = parse_cookie(cookies)
 
-        Returns None if success, aigis headers (mmt/aigis) otherwise.
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.cookies})"
+
+    @property
+    def cookies(self) -> typing.MutableMapping[str, str]:
+        """Cookies used for authentication."""
+        return self._cookies
+
+    @cookies.setter
+    def cookies(self, cookies: typing.Optional[CookieOrHeader]) -> None:
+        if not cookies:
+            self._cookies = {}
+            return
+
+        self._cookies = parse_cookie(cookies)
+
+    @property
+    def available(self) -> bool:
+        return bool(self._cookies)
+
+    @property
+    def multi(self) -> bool:
+        return False
+
+    @property
+    def jar(self) -> http.cookies.SimpleCookie:
+        """SimpleCookie containing the cookies."""
+        return http.cookies.SimpleCookie(self.cookies)
+
+    @property
+    def header(self) -> str:
+        """Header representation of cookies.
+
+        This representation is reparsable by the manager.
         """
-        headers = {**geetest_utility.EMAIL_SEND_HEADERS}
-        if geetest:
-            mmt_data = geetest["data"]
-            session_id = geetest["session_id"]
-            headers["x-rpc-aigis"] = geetest_utility.get_aigis_header(session_id, mmt_data)
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.SEND_VERIFICATION_CODE_URL.get_url(),
-                json={
-                    "action_type": "verify_for_component",
-                    "action_ticket": ticket["verify_str"]["ticket"],
-                },
-                headers=headers,
-            ) as r:
-                data = await r.json()
-
-        if data["retcode"] == -3101:
-            # Captcha triggered
-            aigis = json.loads(r.headers["x-rpc-aigis"])
-            aigis["data"] = json.loads(aigis["data"])
-            return aigis
+        return self.jar.output(header="", sep=";").strip()
 
-        if data["retcode"] != 0:
-            errors.raise_for_retcode(data)
+    def set_cookies(
+        self,
+        cookies: typing.Optional[CookieOrHeader] = None,
+        **kwargs: typing.Any,
+    ) -> typing.MutableMapping[str, str]:
+        """Parse and set cookies."""
+        if not bool(cookies) ^ bool(kwargs):
+            raise TypeError("Cannot use both positional and keyword arguments at once")
 
-        return None
+        self.cookies = parse_cookie(cookies or kwargs)
+        return self.cookies
+
+    def set_browser_cookies(self, browser: typing.Optional[str] = None) -> typing.Mapping[str, str]:
+        """Extract cookies from your browser and set them as client cookies.
+
+        Available browsers: chrome, chromium, opera, edge, firefox.
+        """
+        self.cookies = parse_cookie(fs_utility.get_browser_cookies(browser))
+        return self.cookies
+
+    @property
+    def user_id(self) -> typing.Optional[int]:
+        """The id of the user that owns cookies.
 
-    async def _verify_email(self, code: str, ticket: typing.Dict[str, typing.Any]) -> None:
-        """Verify email."""
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.VERIFY_EMAIL_URL.get_url(),
-                json={
-                    "action_type": "verify_for_component",
-                    "action_ticket": ticket["verify_str"]["ticket"],
-                    "email_captcha": code,
-                    "verify_method": 2,
-                },
-                headers=geetest_utility.EMAIL_VERIFY_HEADERS,
-            ) as r:
-                data = await r.json()
+        Returns None if cookies are not set.
+        """
+        for name, value in self.cookies.items():
+            if name in ("ltuid", "account_id", "ltuid_v2", "account_id_v2"):
+                if not value:
+                    raise ValueError(f"{name} can not be an empty string.")
 
-        if data["retcode"] != 0:
-            errors.raise_for_retcode(data)
+                return int(value)
 
         return None
 
-    async def _send_mobile_otp(
+    async def request(
         self,
-        mobile: str,
+        url: aiohttp.typedefs.StrOrURL,
         *,
-        geetest: typing.Optional[typing.Dict[str, typing.Any]] = None,
-    ) -> typing.Dict[str, typing.Any] | None:
-        """Attempt to send OTP to the provided mobile number.
+        method: str = "GET",
+        **kwargs: typing.Any,
+    ) -> typing.Any:
+        """Make an authenticated request."""
+        return await self._request(method, url, cookies=self.cookies, **kwargs)
 
-        May return aigis headers if captcha is triggered, None otherwise.
-        """
-        headers = {
-            **geetest_utility.CN_LOGIN_HEADERS,
-            "ds": ds_utility.generate_dynamic_secret(constants.DS_SALT["cn_signin"]),
-        }
-        if geetest:
-            mmt_data = geetest["data"]
-            session_id = geetest["session_id"]
-            headers["x-rpc-aigis"] = geetest_utility.get_aigis_header(session_id, mmt_data)
-
-        payload = {
-            "mobile": geetest_utility.encrypt_geetest_credentials(mobile, self._region),
-            "area_code": geetest_utility.encrypt_geetest_credentials("+86", self._region),
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.MOBILE_OTP_URL.get_url(),
-                json=payload,
-                headers=headers,
-            ) as r:
-                data = await r.json()
-
-        if data["retcode"] == -3101:
-            # Captcha triggered
-            aigis = json.loads(r.headers["x-rpc-aigis"])
-            aigis["data"] = json.loads(aigis["data"])
-            return aigis
 
-        if not data["data"]:
-            errors.raise_for_retcode(data)
+class CookieSequence(typing.Sequence[typing.Mapping[str, str]]):
+    MAX_USES: int = 30
 
-        return None
+    # {id: ({cookie}, uses), ...}
+    _cookies: typing.Dict[str, typing.Tuple[typing.Dict[str, str], int]]
 
-    async def _login_with_mobile_otp(self, mobile: str, otp: str) -> typing.Dict[str, typing.Any]:
-        """Login with OTP and mobile number.
+    def __init__(self, cookies: typing.Optional[typing.Sequence[CookieOrHeader]] = None) -> None:
+        self.cookies = [parse_cookie(cookie) for cookie in cookies or []]
 
-        Returns cookies if OTP matches the one sent, raises an error otherwise.
-        """
-        headers = {
-            **geetest_utility.CN_LOGIN_HEADERS,
-            "ds": ds_utility.generate_dynamic_secret(constants.DS_SALT["cn_signin"]),
-        }
-
-        payload = {
-            "mobile": geetest_utility.encrypt_geetest_credentials(mobile, self._region),
-            "area_code": geetest_utility.encrypt_geetest_credentials("+86", self._region),
-            "captcha": otp,
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.MOBILE_LOGIN_URL.get_url(),
-                json=payload,
-                headers=headers,
-            ) as r:
-                data = await r.json()
+    @property
+    def cookies(self) -> typing.Sequence[typing.Mapping[str, str]]:
+        """Cookies used for authentication"""
+        cookies = sorted(self._cookies.values(), key=lambda x: 0 if x[1] >= self.MAX_USES else x[1], reverse=True)
+        return [cookies for cookies, _ in cookies]
 
-        if not data["data"]:
-            errors.raise_for_retcode(data)
+    @cookies.setter
+    def cookies(self, cookies: typing.Optional[typing.Sequence[CookieOrHeader]]) -> None:
+        if not cookies:
+            self._cookies = {}
+            return
 
-        cookies = {cookie.key: cookie.value for cookie in r.cookies.values()}
-        self.set_cookies(cookies)
+        self._cookies = {}
+        for cookie in cookies:
+            cookie = parse_cookie(cookie)
 
-        return cookies
+            account_id = get_cookie_identifier(cookie)
+            if not account_id or not account_id.isdigit():
+                raise ValueError(f"Cookies must contain a valid identifier: {cookie}")
 
-    async def _create_qrcode(self) -> QRCodeCreationResult:
-        """Create a QR code for login."""
-        device_id = "".join(random.choices(ascii_letters + digits, k=64))
-        app_id = "8"
-        payload = {
-            "app_id": app_id,
-            "device": device_id,
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.CREATE_QRCODE_URL.get_url(),
-                json=payload,
-            ) as r:
-                data = await r.json()
-
-        if not data["data"]:
-            errors.raise_for_retcode(data)
-
-        url: str = data["data"]["url"]
-        return QRCodeCreationResult(
-            app_id=app_id,
-            ticket=url.split("ticket=")[1],
-            device_id=device_id,
-            url=url,
-        )
+            if account_id in self._cookies:
+                raise ValueError(f"Cannot use the same identifier for multiple cookies: {account_id}.")
 
-    async def _check_qrcode(self, app_id: str, device_id: str, ticket: str) -> QRCodeCheckResult:
-        """Check the status of a QR code login."""
-        payload = {
-            "app_id": app_id,
-            "device": device_id,
-            "ticket": ticket,
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(
-                routes.CHECK_QRCODE_URL.get_url(),
-                json=payload,
-            ) as r:
-                data = await r.json()
+            self._cookies[account_id] = (cookie, 0)
 
-        if not data["data"]:
-            errors.raise_for_retcode(data)
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} len={len(self._cookies)}>"
 
-        return QRCodeCheckResult(**data["data"])
+    def __getitem__(self, index: int) -> typing.Mapping[str, str]:  # type: ignore # I can't be fucked with slices
+        return self.cookies[index]
 
-    async def login_with_password(
-        self,
-        account: str,
-        password: str,
-        *,
-        port: int = 5000,
-        tokenType: typing.Optional[int] = 6,
-        geetest_solver: typing.Optional[
-            typing.Callable[
-                [typing.Dict[str, typing.Any]],
-                typing.Awaitable[typing.Dict[str, typing.Any]],
-            ]
-        ] = None,
-    ) -> typing.Dict[str, str]:
-        """Login with a password via web endpoint.
+    def __len__(self) -> int:
+        return len(self.cookies)
 
-        Note that this will start a webserver if captcha is
-        triggered and `geetest_solver` is not passed.
-        """
-        result = await self._web_login(account, password, tokenType=tokenType)
+    def __iter__(self) -> typing.Iterator[typing.Mapping[str, str]]:
+        return iter(self.cookies)
 
-        if "session_id" not in result:
-            # Captcha not triggered
-            return result
 
-        if geetest_solver:
-            geetest = await geetest_solver(result)
-        else:
-            geetest = await server.solve_geetest(result, port=port)
+class RotatingCookieManager(BaseCookieManager):
+    """Cookie Manager with rotating cookies."""
 
-        return await self._web_login(account, password, tokenType=tokenType, geetest=geetest)
+    _cookies: CookieSequence
 
-    async def cn_login_by_password(
+    def __init__(self, cookies: typing.Optional[typing.Sequence[CookieOrHeader]] = None) -> None:
+        self.set_cookies(cookies)
+
+    @property
+    def cookies(self) -> typing.Sequence[typing.Mapping[str, str]]:
+        """Cookies used for authentication"""
+        return self._cookies
+
+    @cookies.setter
+    def cookies(self, cookies: typing.Optional[typing.Sequence[CookieOrHeader]]) -> None:
+        self._cookies.cookies = cookies  # type: ignore # mypy does not understand property setters
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} len={len(self._cookies)}>"
+
+    @property
+    def available(self) -> bool:
+        return bool(self._cookies)
+
+    @property
+    def multi(self) -> bool:
+        return True
+
+    def set_cookies(
         self,
-        account: str,
-        password: str,
-        *,
-        port: int = 5000,
-        geetest_solver: typing.Optional[
-            typing.Callable[
-                [typing.Dict[str, typing.Any]],
-                typing.Awaitable[typing.Dict[str, typing.Any]],
-            ]
-        ] = None,
-    ) -> typing.Dict[str, str]:
-        """Login with a password via Miyoushe loginByPassword endpoint.
+        cookies: typing.Optional[typing.Sequence[CookieOrHeader]] = None,
+    ) -> typing.Sequence[typing.Mapping[str, str]]:
+        """Parse and set cookies."""
+        self._cookies = CookieSequence(cookies)
+        return self.cookies
 
-        Note that this will start a webserver if captcha is triggered and `geetest_solver` is not passed.
-        """
-        result = await self._cn_login_by_password(account, password)
+    async def request(
+        self,
+        url: aiohttp.typedefs.StrOrURL,
+        *,
+        method: str = "GET",
+        **kwargs: typing.Any,
+    ) -> typing.Any:
+        """Make an authenticated request."""
+        if not self.cookies:
+            raise RuntimeError("Tried to make a request before setting cookies")
+
+        for account_id, (cookie, uses) in self._cookies._cookies.copy().items():
+            try:
+                data = await self._request(method, url, cookies=cookie, **kwargs)
+            except errors.TooManyRequests:
+                _LOGGER.debug("Putting cookie %s on cooldown.", account_id)
+                self._cookies._cookies[account_id] = (cookie, self._cookies.MAX_USES)
+            except errors.InvalidCookies:
+                warnings.warn(f"Deleting invalid cookie {cookie}")
+                # prevent race conditions
+                if account_id in self._cookies._cookies:
+                    del self._cookies._cookies[account_id]
+            else:
+                self._cookies._cookies[account_id] = (cookie, 1 if uses >= self._cookies.MAX_USES else uses + 1)
+                return data
 
-        if "session_id" not in result:
-            # Captcha not triggered
-            return result
+        msg = "All cookies have hit their request limit of 30 accounts per day."
+        raise errors.TooManyRequests({"retcode": 10101}, msg)
 
-        if geetest_solver:
-            geetest = await geetest_solver(result)
-        else:
-            geetest = await server.solve_geetest(result, port=port)
 
-        return await self._cn_login_by_password(account, password, geetest=geetest)
+class InternationalCookieManager(BaseCookieManager):
+    """Cookie Manager with international rotating cookies."""
 
-    async def check_mobile_number_validity(self, mobile: str) -> bool:
-        """Check if a mobile number is valid (it's registered on Miyoushe).
+    _cookies: typing.Mapping[types.Region, CookieSequence]
 
-        Returns True if the mobile number is valid, False otherwise.
-        """
-        async with aiohttp.ClientSession() as session:
-            async with session.get(
-                routes.CHECK_MOBILE_VALIDITY_URL.get_url(),
-                params={"mobile": mobile},
-            ) as r:
-                data = await r.json()
+    def __init__(self, cookies: typing.Optional[typing.Mapping[str, MaybeSequence[CookieOrHeader]]] = None) -> None:
+        self.set_cookies(cookies)
 
-        return data["data"]["status"] != data["data"]["is_registable"]
+    @property
+    def cookies(self) -> typing.Mapping[types.Region, typing.Sequence[typing.Mapping[str, str]]]:
+        """Cookies used for authentication"""
+        return self._cookies
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}>"
+
+    @property
+    def available(self) -> bool:
+        return bool(self._cookies)
+
+    @property
+    def multi(self) -> bool:
+        return True
 
-    async def login_with_mobile_number(
+    def set_cookies(
         self,
-        mobile: str,
-    ) -> typing.Dict[str, str]:
-        """Login with mobile number, returns cookies.
-
-        Only works for Chinese region (Miyoushe) users, do not include area code (+86) in the mobile number.
-        Steps:
-        1. Sends OTP to the provided mobile number.
-        1-1. If captcha is triggered, prompts the user to solve it.
-        2. Lets user enter the OTP.
-        3. Logs in with the OTP.
-        4. Returns cookies.
-        """
-        result = await self._send_mobile_otp(mobile)
+        cookies: typing.Optional[typing.Mapping[str, MaybeSequence[CookieOrHeader]]] = None,
+    ) -> typing.Mapping[types.Region, typing.Sequence[typing.Mapping[str, str]]]:
+        """Parse and set cookies."""
+        self._cookies = {}
+        if not cookies:
+            return {}
+
+        for region, regional_cookies in cookies.items():
+            if not isinstance(regional_cookies, typing.Sequence):
+                regional_cookies = [regional_cookies]
+
+            self._cookies[types.Region(region)] = CookieSequence(regional_cookies)
+
+        return self.cookies
 
-        if result is not None and "session_id" in result:
-            # Captcha triggered
-            geetest = await server.solve_geetest(result)
-            await self._send_mobile_otp(mobile, geetest=geetest)
-
-        otp = await server.enter_otp()
-        cookies = await self._login_with_mobile_otp(mobile, otp)
-        return cookies
+    def guess_region(self, url: yarl.URL) -> types.Region:
+        """Guess the region from the URL."""
+        assert url.host is not None
 
-    async def login_with_app_password(
+        if "os" in url.host or "os" in url.path:
+            return types.Region.OVERSEAS
+
+        if "takumi" in url.host:
+            return types.Region.CHINESE
+
+        if "sg" in url.host:
+            return types.Region.OVERSEAS
+
+        return types.Region.CHINESE
+
+    async def request(
         self,
-        account: str,
-        password: str,
+        url: aiohttp.typedefs.StrOrURL,
         *,
-        port: int = 5000,
-        geetest_solver: typing.Optional[
-            typing.Callable[
-                [typing.Dict[str, typing.Any]],
-                typing.Awaitable[typing.Dict[str, typing.Any]],
-            ]
-        ] = None,
-    ) -> typing.Dict[str, str]:
-        """Login with a password via HoYoLab app endpoint.
-
-        Note that this will start a webserver if either of the
-        following happens:
-
-        1. Captcha is triggered and `geetest_solver` is not passed.
-        2. Email verification is triggered (can happen if you
-        first login with a new device).
-        """
-        result = await self._app_login(account, password)
-
-        if "session_id" in result:
-            # Captcha triggered
-            if geetest_solver:
-                geetest = await geetest_solver(result)
+        method: str = "GET",
+        **kwargs: typing.Any,
+    ) -> typing.Any:
+        """Make an authenticated request."""
+        if not self.cookies:
+            raise RuntimeError("Tried to make a request before setting cookies")
+
+        region = self.guess_region(yarl.URL(url))
+
+        # TODO: less copy-paste
+        for account_id, (cookie, uses) in self._cookies[region]._cookies.copy().items():
+            try:
+                data = await self._request(method, url, cookies=cookie, **kwargs)
+            except errors.TooManyRequests:
+                _LOGGER.debug("Putting cookie %s on cooldown.", account_id)
+                self._cookies[region]._cookies[account_id] = (cookie, self._cookies[region].MAX_USES)
+            except errors.InvalidCookies:
+                warnings.warn(f"Deleting invalid cookie {cookie}")
+                # prevent race conditions
+                if account_id in self._cookies[region]._cookies:
+                    del self._cookies[region]._cookies[account_id]
             else:
-                geetest = await server.solve_geetest(result, port=port)
+                self._cookies[region]._cookies[account_id] = (
+                    cookie,
+                    1 if uses >= self._cookies[region].MAX_USES else uses + 1,
+                )
+                return data
 
-            result = await self._app_login(account, password, geetest=geetest)
+        msg = "All cookies have hit their request limit of 30 accounts per day."
+        raise errors.TooManyRequests({"retcode": 10101}, msg)
 
-        if "risk_ticket" in result:
-            # Email verification required
-            mmt = await self._send_verification_email(result)
-            if mmt:
-                if geetest_solver:
-                    geetest = await geetest_solver(mmt)
-                else:
-                    geetest = await server.solve_geetest(mmt, port=port)
 
-                await self._send_verification_email(result, geetest=geetest)
+def no_multi(func: CallableT) -> CallableT:
+    """Prevent function to be ran with a multi-cookie manager."""
 
-            await server.verify_email(self, result, port=port)
-            result = await self._app_login(account, password, ticket=result)
+    @functools.wraps(func)
+    def wrapper(self: typing.Any, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
+        if not hasattr(self, "cookie_manager"):
+            raise TypeError("Cannot use @no_multi on a plain function.")
+        if self.cookie_manager.multi:
+            raise RuntimeError(f"Cannot use {func.__name__} with multi-cookie managers - data is private.")
 
-        return result
+        return func(self, *args, **kwargs)
 
-    async def login_with_qrcode(self) -> typing.Dict[str, str]:
-        """Login with QR code, only available for Miyoushe users.
+    return typing.cast("CallableT", wrapper)
 
-        Returns cookies.
-        """
-        creation_result = await self._create_qrcode()
-        qrcode_: qrcode.image.pil.PilImage = qrcode.make(creation_result.url, error_correction=ERROR_CORRECT_L)  # type: ignore
-        qrcode_.show()
-
-        scanned = False
-        while True:
-            check_result = await self._check_qrcode(
-                creation_result.app_id, creation_result.device_id, creation_result.ticket
-            )
-            if check_result.status == QRCodeStatus.SCANNED and not scanned:
-                LOGGER_.info("QR code scanned")
-                scanned = True
-            elif check_result.status == QRCodeStatus.CONFIRMED:
-                LOGGER_.info("QR code login confirmed")
-                break
 
-            await asyncio.sleep(2)
+def requires_cookie_token(func: AsyncCallableT) -> AsyncCallableT:
+    """Prevent function to be ran without a cookie_token."""
 
-        raw_data = check_result.payload.raw
-        assert raw_data is not None
+    @functools.wraps(func)
+    async def wrapper(self: typing.Any, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
+        if not hasattr(self, "cookie_manager"):
+            raise TypeError("Cannot use @requires_cookie_token on a plain function.")
+        if self.cookie_manager.multi:
+            raise RuntimeError(f"Cannot use {func.__name__} with multi-cookie managers - data is private.")
+        if isinstance(self.cookie_manager, CookieManager):
+            contained = set(self.cookie_manager.cookies.keys())
+            if "cookie_token" not in contained and "cookie_token_v2" not in contained:
+                raise errors.InvalidCookies(msg="Missing cookie_token cookie.")
 
-        cookie_token = await fetch_cookie_token_by_game_token(
-            game_token=raw_data.game_token, account_id=raw_data.account_id
-        )
-        stoken = await fetch_stoken_by_game_token(game_token=raw_data.game_token, account_id=int(raw_data.account_id))
+        return await func(self, *args, **kwargs)
 
-        cookies = {
-            "stoken_v2": stoken.token,
-            "stuid": stoken.aid,
-            "mid": stoken.mid,
-            "cookie_token": cookie_token,
-        }
-        self.set_cookies(cookies)
-        return cookies
+    return typing.cast("AsyncCallableT", wrapper)
```

### Comparing `genshin-1.6.3/genshin/client/components/hoyolab.py` & `genshin-1.7.0/genshin/client/components/hoyolab.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/lineup.py` & `genshin-1.7.0/genshin/client/components/lineup.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/teapot.py` & `genshin-1.7.0/genshin/client/components/teapot.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/components/transaction.py` & `genshin-1.7.0/genshin/client/components/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             authkey=authkey,
             params=dict(end_id=end_id, size=20),
         )
 
         transactions: typing.List[models.BaseTransaction] = []
         for trans in data["list"]:
             model = models.ItemTransaction if "name" in trans else models.Transaction
-            model = typing.cast("type[models.BaseTransaction]", model)
+            model = typing.cast("typing.Type[models.BaseTransaction]", model)
             transactions.append(model(**trans, kind=kind, lang=lang or self.lang))
 
         return transactions
 
     def transaction_log(
         self,
         kind: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
```

### Comparing `genshin-1.6.3/genshin/client/components/wiki.py` & `genshin-1.7.0/genshin/client/components/wiki.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/manager/cookie.py` & `genshin-1.7.0/genshin/client/manager/cookie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Cookie completion.
 
-Available convertions:
+Available conversions:
 
 - fetch_cookie_with_cookie
     - cookie_token -> cookie_token
     - cookie_token -> ltoken
     - stoken -> cookie_token
     - stoken -> ltoken
     - stoken -> login_ticket
 - fetch_cookie_token_info
     - cookie_token -> cookie_token
     - login_ticket -> cookie_token
 - fetch_cookie_with_stoken_v2
     - stoken (v2) + mid -> ltoken_v2 (token_type=2)
     - stoken (v2) + mid -> cookie_token_v2 (token_type=4)
+- fetch_cookie_token_with_game_token
+    - game_token -> cookie_token
+- fetch_stoken_with_game_token
+    - game_token -> stoken
 """
 
 from __future__ import annotations
 
 import random
 import typing
 import uuid
@@ -25,41 +29,27 @@
 
 import aiohttp
 import aiohttp.typedefs
 
 from genshin import constants, errors, types
 from genshin.client import routes
 from genshin.client.manager import managers
-from genshin.models.miyoushe.cookie import StokenResult
+from genshin.models.auth.cookie import StokenResult
 from genshin.utility import ds as ds_utility
 
 __all__ = [
     "complete_cookies",
-    "fetch_cookie_token_by_game_token",
     "fetch_cookie_token_info",
+    "fetch_cookie_token_with_game_token",
     "fetch_cookie_with_cookie",
     "fetch_cookie_with_stoken_v2",
-    "fetch_stoken_by_game_token",
+    "fetch_stoken_with_game_token",
     "refresh_cookie_token",
 ]
 
-STOKEN_BY_GAME_TOKEN_HEADERS = {
-    "x-rpc-app_version": "2.41.0",
-    "x-rpc-aigis": "",
-    "Content-Type": "application/json",
-    "Accept": "application/json",
-    "x-rpc-game_biz": "bbs_cn",
-    "x-rpc-sys_version": "11",
-    "x-rpc-device_name": "GenshinUid_login_device_lulu",
-    "x-rpc-device_model": "GenshinUid_login_device_lulu",
-    "x-rpc-app_id": "bll8iq97cem8",
-    "x-rpc-client_type": "2",
-    "User-Agent": "okhttp/4.8.0",
-}
-
 
 async def fetch_cookie_with_cookie(
     cookies: managers.CookieOrHeader,
     *,
     source: typing.Literal["CookieToken", "SToken"],
     target: typing.Literal["CookieAccountInfo", "LToken", "ActionTicket"],
     region: types.Region = types.Region.OVERSEAS,
@@ -184,16 +174,16 @@
 
     if refresh:
         cookies = await refresh_cookie_token(cookies, region=region)  # type: ignore[assignment]
 
     return cookies
 
 
-async def fetch_cookie_token_by_game_token(*, game_token: str, account_id: str) -> str:
-    """Fetch cookie token by game token, which is obtained by scanning a QR code."""
+async def fetch_cookie_token_with_game_token(*, game_token: str, account_id: str) -> str:
+    """Fetch cookie token with game token, which can be obtained by scanning a QR code."""
     url = routes.GET_COOKIE_TOKEN_BY_GAME_TOKEN_URL.get_url()
     params = {
         "game_token": game_token,
         "account_id": account_id,
     }
 
     async with aiohttp.ClientSession() as session:
@@ -202,26 +192,26 @@
 
     if not data["data"]:
         errors.raise_for_retcode(data)
 
     return data["data"]["cookie_token"]
 
 
-async def fetch_stoken_by_game_token(*, game_token: str, account_id: int) -> StokenResult:
-    """Fetch cookie token by game token, which is obtained by scanning a QR code."""
+async def fetch_stoken_with_game_token(*, game_token: str, account_id: int) -> StokenResult:
+    """Fetch cookie token with game token, which can be obtained by scanning a QR code."""
     url = routes.GET_STOKEN_BY_GAME_TOKEN_URL.get_url()
     payload = {
         "account_id": account_id,
         "game_token": game_token,
     }
     headers = {
         "DS": ds_utility.generate_passport_ds(body=payload),
         "x-rpc-device_id": uuid.uuid4().hex,
         "x-rpc-device_fp": "".join(random.choices(ascii_letters + digits, k=13)),
-        **STOKEN_BY_GAME_TOKEN_HEADERS,
+        "x-rpc-app_id": "bll8iq97cem8",
     }
 
     async with aiohttp.ClientSession() as session:
         async with session.post(url, json=payload, headers=headers) as r:
             data = await r.json()
 
     if not data["data"]:
```

### Comparing `genshin-1.6.3/genshin/client/ratelimit.py` & `genshin-1.7.0/genshin/client/ratelimit.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/client/routes.py` & `genshin-1.7.0/genshin/client/routes.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,33 +13,34 @@
     "BBS_REFERER_URL",
     "BBS_URL",
     "CALCULATOR_URL",
     "CHECK_QRCODE_URL",
     "CN_WEB_LOGIN_URL",
     "COMMUNITY_URL",
     "COOKIE_V2_REFRESH_URL",
+    "CREATE_MMT_URL",
     "CREATE_QRCODE_URL",
     "DETAIL_LEDGER_URL",
     "GACHA_URL",
     "GET_COOKIE_TOKEN_BY_GAME_TOKEN_URL",
     "GET_STOKEN_BY_GAME_TOKEN_URL",
     "HK4E_URL",
     "INFO_LEDGER_URL",
     "LINEUP_URL",
     "MI18N",
     "RECORD_URL",
     "REWARD_URL",
-    "Route",
     "TAKUMI_URL",
     "TEAPOT_URL",
     "VERIFY_EMAIL_URL",
     "WEBAPI_URL",
     "WEBSTATIC_URL",
     "WEB_LOGIN_URL",
     "YSULOG_URL",
+    "Route",
 ]
 
 
 class BaseRoute(abc.ABC):
     """A route which provides useful metadata."""
 
 
@@ -180,16 +181,16 @@
 REWARD_URL = GameRoute(
     overseas=dict(
         genshin="https://sg-hk4e-api.hoyolab.com/event/sol?act_id=e202102251931481",
         honkai3rd="https://sg-public-api.hoyolab.com/event/mani?act_id=e202110291205111",
         hkrpg="https://sg-public-api.hoyolab.com/event/luna/os?act_id=e202303301540311",
     ),
     chinese=dict(
-        genshin="https://api-takumi.mihoyo.com/event/bbs_sign_reward/?act_id=e202009291139501",
-        honkai3rd="https://api-takumi.mihoyo.com/event/luna/?act_id=e202207181446311",
+        genshin="https://api-takumi.mihoyo.com/event/luna/?act_id=e202311201442471",
+        honkai3rd="https://api-takumi.mihoyo.com/event/luna/?act_id=e202306201626331",
         hkrpg="https://api-takumi.mihoyo.com/event/luna/?act_id=e202304121516551",
     ),
 )
 
 CODE_URL = GameRoute(
     overseas=dict(
         genshin="https://sg-hk4e-api.hoyoverse.com/common/apicdkey/api/webExchangeCdkey",
@@ -233,7 +234,56 @@
 
 CHECK_MOBILE_VALIDITY_URL = Route("https://webapi.account.mihoyo.com/Api/is_mobile_registrable")
 MOBILE_OTP_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-verifier/verifier/createLoginCaptcha")
 MOBILE_LOGIN_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-passport/web/loginByMobileCaptcha")
 
 CREATE_QRCODE_URL = Route("https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/fetch")
 CHECK_QRCODE_URL = Route("https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/query")
+
+CREATE_MMT_URL = Route(
+    "https://api-takumi-record.mihoyo.com/game_record/app/card/wapi/createVerification?is_high=false"
+)
+
+GAME_RISKY_CHECK_URL = InternationalRoute(
+    overseas="https://api-account-os.hoyoverse.com/account/risky/api/check",
+    chinese="https://gameapi-account.mihoyo.com/account/risky/api/check",
+)
+
+SHIELD_LOGIN_URL = GameRoute(
+    overseas=dict(
+        genshin="https://hk4e-sdk-os.hoyoverse.com/hk4e_global/mdk/shield/api/login",
+        honkai3rd="https://bh3-sdk-os.hoyoverse.com/bh3_os/mdk/shield/api/login",
+        hkrpg="https://hkrpg-sdk-os.hoyoverse.com/hkrpg_global/mdk/shield/api/login",
+        nap="https://nap-sdk-os.hoyoverse.com/nap_global/mdk/shield/api/login",
+    ),
+    chinese=dict(
+        genshin="https://hk4e-sdk.mihoyo.com/hk4e_cn/mdk/shield/api/login",
+        honkai3rd="https://api-sdk.mihoyo.com/bh3_cn/mdk/shield/api/login",
+        hkrpg="https://hkrpg-sdk.mihoyo.com/hkrpg_cn/mdk/shield/api/login",
+        nap="https://nap-sdk.mihoyo.com/nap_cn/mdk/shield/api/login",
+    ),
+)
+
+PRE_GRANT_TICKET_URL = InternationalRoute(
+    overseas="https://api-account-os.hoyoverse.com/account/device/api/preGrantByTicket",
+    chinese="https://gameapi-account.mihoyo.com/account/device/api/preGrantByTicket",
+)
+
+DEVICE_GRANT_URL = InternationalRoute(
+    overseas="https://api-account-os.hoyoverse.com/account/device/api/grant",
+    chinese="https://gameapi-account.mihoyo.com/account/device/api/grant",
+)
+
+GAME_LOGIN_URL = GameRoute(
+    overseas=dict(
+        genshin="https://hk4e-sdk-os.hoyoverse.com/hk4e_global/combo/granter/login/v2/login",
+        honkai3rd="https://bh3-sdk-os.hoyoverse.com/bh3_os/combo/granter/login/v2/login",
+        hkrpg="https://hkrpg-sdk-os.hoyoverse.com/hkrpg_global/combo/granter/login/v2/login",
+        nap="https://nap-sdk-os.hoyoverse.com/nap_global/combo/granter/login/v2/login",
+    ),
+    chinese=dict(
+        genshin="https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/granter/login/v2/login",
+        honkai3rd="https://api-sdk.mihoyo.com/bh3_cn/combo/granter/login/v2/login",
+        hkrpg="https://hkrpg-sdk.mihoyo.com/hkrpg_cn/combo/granter/login/v2/login",
+        nap="https://nap-sdk.mihoyo.com/nap_cn/combo/granter/login/v2/login",
+    ),
+)
```

### Comparing `genshin-1.6.3/genshin/errors.py` & `genshin-1.7.0/genshin/errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Errors received from the API."""
 
 import typing
 
 __all__ = [
+    "ERRORS",
     "AccountNotFound",
     "AlreadyClaimed",
     "AuthkeyException",
     "AuthkeyTimeout",
     "CookieException",
     "DataNotPublic",
-    "ERRORS",
     "GeetestTriggered",
     "GenshinException",
     "InvalidAuthkey",
     "InvalidCookies",
+    "MiyousheGeetestError",
     "RedemptionClaimed",
     "RedemptionCooldown",
     "RedemptionException",
     "RedemptionInvalid",
     "TooManyRequests",
     "check_for_geetest",
     "raise_for_retcode",
@@ -182,14 +183,66 @@
 
 class WrongOTP(GenshinException):
     """Wrong OTP code."""
 
     msg = "The provided OTP code is wrong."
 
 
+class MiyousheGeetestError(GenshinException):
+    """Geetest triggered during Miyoushe API request."""
+
+    def __init__(
+        self,
+        response: typing.Dict[str, typing.Any],
+        cookies: typing.Mapping[str, str],
+    ) -> None:
+        self.cookies = cookies
+        super().__init__(response)
+
+    msg = "Geetest triggered during Miyoushe API request."
+
+
+class OTPRateLimited(GenshinException):
+    """Too many OTP messages sent for the number.
+
+    The limit is 40 messages/day/number.
+    """
+
+    retcode = -119
+    msg = "Too many OTP messages sent for the number."
+
+
+class IncorrectGameAccount(GenshinException):
+    """Game account is incorrect."""
+
+    retcode = -216
+    msg = "Game account is incorrect."
+
+
+class IncorrectGamePassword(GenshinException):
+    """Game password is incorrect."""
+
+    retcode = -202
+    msg = "Game password is incorrect."
+
+
+class AccountDoesNotExist(GenshinException):
+    """Account does not exist."""
+
+    retcode = -3203
+    msg = "Account does not exist."
+
+
+class VerificationCodeRateLimited(GenshinException):
+    """Too many verification code requests for the account."""
+
+    retcode = -3206
+    msg = "Too many verification code requests for the account."
+
+
 _TGE = typing.Type[GenshinException]
 _errors: typing.Dict[int, typing.Union[_TGE, str, typing.Tuple[_TGE, typing.Optional[str]]]] = {
     # misc hoyolab
     -100: InvalidCookies,
     -108: "Invalid language.",
     -110: VisitsTooFrequently,
     # game record
@@ -231,15 +284,23 @@
     -5003: AlreadyClaimed,
     # chinese
     1008: AccountNotFound,
     -1104: "This action must be done in the app.",
     # account
     -3208: AccountLoginFail,
     -3202: AccountHasLocked,
+    -3203: AccountDoesNotExist,
     -3205: WrongOTP,
+    -3206: VerificationCodeRateLimited,
+    # Miyoushe
+    -119: OTPRateLimited,
+    -3006: "Request too frequent.",  # OTP endpoint
+    # Game login
+    -216: IncorrectGameAccount,
+    -202: IncorrectGamePassword,
 }
 
 ERRORS: typing.Dict[int, typing.Tuple[_TGE, typing.Optional[str]]] = {
     retcode: ((exc, None) if isinstance(exc, type) else (GenshinException, exc) if isinstance(exc, str) else exc)
     for retcode, exc in _errors.items()
 }
```

### Comparing `genshin-1.6.3/genshin/models/genshin/calculator.py` & `genshin-1.7.0/genshin/models/genshin/calculator.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/character.py` & `genshin-1.7.0/genshin/models/genshin/character.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/chronicle/abyss.py` & `genshin-1.7.0/genshin/models/genshin/chronicle/abyss.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/chronicle/activities.py` & `genshin-1.7.0/genshin/models/genshin/chronicle/activities.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/chronicle/characters.py` & `genshin-1.7.0/genshin/models/genshin/chronicle/characters.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/chronicle/notes.py` & `genshin-1.7.0/genshin/models/genshin/chronicle/notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
         import pydantic.v1 as pydantic
     except ImportError:
         import pydantic
 
 from genshin.models.model import Aliased, APIModel
 
 __all__ = [
+    "ArchonQuest",
+    "ArchonQuestProgress",
+    "ArchonQuestStatus",
     "AttendanceReward",
     "AttendanceRewardStatus",
     "DailyTasks",
     "Expedition",
     "Notes",
     "TaskReward",
     "TaskRewardStatus",
@@ -121,14 +124,39 @@
     claimed_commission_reward: bool = Aliased("is_extra_task_reward_received")
 
     task_rewards: typing.Sequence[TaskReward]
     attendance_rewards: typing.Sequence[AttendanceReward]
     attendance_visible: bool
 
 
+class ArchonQuestStatus(str, enum.Enum):
+    """Archon quest status."""
+
+    ONGOING = "StatusOngoing"
+    NOT_OPEN = "StatusNotOpen"
+
+
+class ArchonQuest(APIModel):
+    """Archon Quest."""
+
+    id: int
+    status: ArchonQuestStatus
+    chapter_num: str
+    chapter_title: str
+
+
+class ArchonQuestProgress(APIModel):
+    """Archon Quest Progress."""
+
+    list: typing.Sequence[ArchonQuest]
+    mainlines_finished: bool = Aliased("is_finish_all_mainline")
+    archon_quest_unlocked: bool = Aliased("is_open_archon_quest")
+    interchapters_finished: bool = Aliased("is_finish_all_interchapter")
+
+
 class Notes(APIModel):
     """Real-Time notes."""
 
     current_resin: int
     max_resin: int
     remaining_resin_recovery_time: datetime.timedelta = Aliased("resin_recovery_time")
 
@@ -144,14 +172,16 @@
     max_resin_discounts: int = Aliased("resin_discount_num_limit")
 
     remaining_transformer_recovery_time: typing.Optional[TransformerTimedelta]
 
     expeditions: typing.Sequence[Expedition]
     max_expeditions: int = Aliased("max_expedition_num")
 
+    archon_quest_progress: ArchonQuestProgress
+
     @property
     def resin_recovery_time(self) -> datetime.datetime:
         """The time when resin will be recovered."""
         return datetime.datetime.now().astimezone() + self.remaining_resin_recovery_time
 
     @property
     def realm_currency_recovery_time(self) -> datetime.datetime:
```

### Comparing `genshin-1.6.3/genshin/models/genshin/chronicle/stats.py` & `genshin-1.7.0/genshin/models/genshin/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/chronicle/tcg.py` & `genshin-1.7.0/genshin/models/genshin/chronicle/tcg.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/constants.py` & `genshin-1.7.0/genshin/models/genshin/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/daily.py` & `genshin-1.7.0/genshin/models/genshin/daily.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/diary.py` & `genshin-1.7.0/genshin/models/genshin/diary.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/gacha.py` & `genshin-1.7.0/genshin/models/genshin/gacha.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/lineup.py` & `genshin-1.7.0/genshin/models/genshin/lineup.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/teapot.py` & `genshin-1.7.0/genshin/models/genshin/teapot.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     post_id: str
     title: str
     content: str
     images: typing.List[str] = Aliased("imgs")
     created_at: datetime.datetime
     stats: TeapotReplicaStats
-    lang: str
+    lang: str  # type: ignore
 
     author: TeapotReplicaAuthor
 
     view_type: int
     sub_type: int
     blueprint: TeapotReplicaBlueprint
     video: typing.Optional[str]
```

### Comparing `genshin-1.6.3/genshin/models/genshin/transaction.py` & `genshin-1.7.0/genshin/models/genshin/transaction.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/genshin/wiki.py` & `genshin-1.7.0/genshin/models/genshin/wiki.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/honkai/battlesuit.py` & `genshin-1.7.0/genshin/models/honkai/battlesuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 BATTLESUIT_TYPES = {
     "ShengWu": "BIO",
     "JiXie": "MECH",
     "YiNeng": "PSY",
     "LiangZi": "QUA",
     "XuShu": "IMG",
+    "Xingchen": "SD",
 }
 ICON_BASE = "https://upload-os-bbs.mihoyo.com/game_record/honkai3rd/global/SpriteOutput/"
 
 
 class Battlesuit(APIModel, Unique):
     """Represents a battlesuit without equipment or level."""
```

### Comparing `genshin-1.6.3/genshin/models/honkai/chronicle/battlesuits.py` & `genshin-1.7.0/genshin/models/honkai/chronicle/battlesuits.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/honkai/chronicle/modes.py` & `genshin-1.7.0/genshin/models/honkai/chronicle/modes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     except ImportError:
         import pydantic
 
 from genshin.models.honkai import battlesuit
 from genshin.models.model import Aliased, APIModel, Unique
 
 __all__ = [
-    "Boss",
     "ELF",
+    "Boss",
     "ElysianRealm",
     "MemorialArena",
     "MemorialBattle",
     "OldAbyss",
     "SuperstringAbyss",
 ]
```

### Comparing `genshin-1.6.3/genshin/models/honkai/chronicle/stats.py` & `genshin-1.7.0/genshin/models/honkai/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/honkai/constants.py` & `genshin-1.7.0/genshin/models/honkai/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/hoyolab/announcements.py` & `genshin-1.7.0/genshin/models/hoyolab/announcements.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     extra_remind: bool
 
     start_time: datetime.datetime
     end_time: datetime.datetime
     tag_start_time: datetime.datetime
     tag_end_time: datetime.datetime
 
-    lang: str
+    lang: str  # type: ignore
     has_content: bool
```

### Comparing `genshin-1.6.3/genshin/models/hoyolab/record.py` & `genshin-1.7.0/genshin/models/hoyolab/record.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/model.py` & `genshin-1.7.0/genshin/models/model.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/starrail/character.py` & `genshin-1.7.0/genshin/models/starrail/character.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/starrail/chronicle/challenge.py` & `genshin-1.7.0/genshin/models/starrail/chronicle/challenge.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/starrail/chronicle/characters.py` & `genshin-1.7.0/genshin/models/starrail/chronicle/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Starrail chronicle character."""
 
+import enum
 import typing
 from typing import Any, Mapping, Optional, Sequence
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
 else:
     try:
         import pydantic.v1 as pydantic
     except ImportError:
         import pydantic
 
-from genshin.models.model import APIModel
+from genshin.models.model import Aliased, APIModel
 
 from .. import character
 
 __all__ = [
     "CharacterProperty",
     "ModifyRelicProperty",
     "PropertyInfo",
@@ -24,17 +25,30 @@
     "Relic",
     "RelicProperty",
     "Skill",
     "SkillStage",
     "StarRailDetailCharacter",
     "StarRailDetailCharacters",
     "StarRailEquipment",
+    "StarRailPath",
 ]
 
 
+class StarRailPath(enum.IntEnum):
+    """StarRail character path."""
+
+    DESTRUCTION = 1
+    THE_HUNT = 2
+    ERUDITION = 3
+    HARMONY = 4
+    NIHILITY = 5
+    PRESERVATION = 6
+    ABUNDANCE = 7
+
+
 class StarRailEquipment(APIModel):
     """Character equipment."""
 
     id: int
     level: int
     rank: int
     name: str
@@ -143,15 +157,15 @@
 
     image: str
     equip: Optional[StarRailEquipment]
     relics: Sequence[Relic]
     ornaments: Sequence[Relic]
     ranks: Sequence[Rank]
     properties: Sequence[CharacterProperty]
-    base_type: int
+    path: StarRailPath = Aliased("base_type")
     figure_path: str
     skills: Sequence[Skill]
 
 
 class ModifyRelicProperty(APIModel):
     """Modify relic property."""
```

### Comparing `genshin-1.6.3/genshin/models/starrail/chronicle/notes.py` & `genshin-1.7.0/genshin/models/starrail/chronicle/notes.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/starrail/chronicle/rogue.py` & `genshin-1.7.0/genshin/models/starrail/chronicle/rogue.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/models/starrail/chronicle/stats.py` & `genshin-1.7.0/genshin/models/starrail/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/paginators/api.py` & `genshin-1.7.0/genshin/paginators/api.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/paginators/base.py` & `genshin-1.7.0/genshin/paginators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 T = typing.TypeVar("T")
 
 
 async def flatten(iterable: typing.AsyncIterable[T]) -> typing.Sequence[T]:
     """Flatten an async iterable."""
     if isinstance(iterable, Paginator):
-        return await iterable.flatten()
+        return await iterable.flatten()  # type: ignore
 
     return [x async for x in iterable]
 
 
 async def aiterate(iterable: typing.Iterable[T]) -> typing.AsyncIterator[T]:
     """Turn a plain iterable into an async iterator."""
     for i in iterable:
```

### Comparing `genshin-1.6.3/genshin/types.py` & `genshin-1.7.0/genshin/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,10 +29,13 @@
 
     HONKAI = "honkai3rd"
     """Honkai Impact 3rd"""
 
     STARRAIL = "hkrpg"
     """Honkai Star Rail"""
 
+    ZZZ = "nap"
+    """Zenless Zone Zero"""
+
 
 IDOr = typing.Union[int, UniqueT]
 """Allows partial objects."""
```

### Comparing `genshin-1.6.3/genshin/utility/concurrency.py` & `genshin-1.7.0/genshin/utility/concurrency.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/utility/deprecation.py` & `genshin-1.7.0/genshin/utility/deprecation.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/utility/ds.py` & `genshin-1.7.0/genshin/utility/ds.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 import random
 import string
 import time
 import typing
 
 from genshin import constants, types
 
-__all__ = ["generate_cn_dynamic_secret", "generate_dynamic_secret", "generate_passport_ds", "get_ds_headers"]
+__all__ = [
+    "generate_cn_dynamic_secret",
+    "generate_create_geetest_ds",
+    "generate_dynamic_secret",
+    "generate_passport_ds",
+    "get_ds_headers",
+]
 
 
 def generate_dynamic_secret(salt: str = constants.DS_SALT[types.Region.OVERSEAS]) -> str:
     """Create a new overseas dynamic secret."""
     t = int(time.time())
     r = "".join(random.choices(string.ascii_letters, k=6))
     h = hashlib.md5(f"salt={salt}&t={t}&r={r}".encode()).hexdigest()
@@ -66,7 +72,16 @@
     salt = constants.DS_SALT["cn_passport"]
     t = int(time.time())
     r = "".join(random.sample(string.ascii_letters, 6))
     b = json.dumps(body)
     h = hashlib.md5(f"salt={salt}&t={t}&r={r}&b={b}&q=".encode()).hexdigest()
     result = f"{t},{r},{h}"
     return result
+
+
+def generate_create_geetest_ds() -> str:
+    """Create a dynamic secret for Miyoushe createVerification API endpoint."""
+    salt = constants.DS_SALT[types.Region.CHINESE]
+    t = int(time.time())
+    r = random.randint(100000, 200000)
+    h = hashlib.md5(f"salt={salt}&t={t}&r={r}&b=&q=is_high=false".encode()).hexdigest()
+    return f"{t},{r},{h}"
```

### Comparing `genshin-1.6.3/genshin/utility/extdb.py` & `genshin-1.7.0/genshin/utility/extdb.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/utility/fs.py` & `genshin-1.7.0/genshin/utility/fs.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/utility/logfile.py` & `genshin-1.7.0/genshin/utility/logfile.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin/utility/uid.py` & `genshin-1.7.0/genshin/utility/uid.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/genshin.egg-info/PKG-INFO` & `genshin-1.7.0/genshin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.6.3
+Version: 1.7.0
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
@@ -28,17 +28,17 @@
 Provides-Extra: all
 Requires-Dist: browser-cookie3; extra == "all"
 Requires-Dist: rsa; extra == "all"
 Requires-Dist: click; extra == "all"
 Requires-Dist: qrcode[pil]; extra == "all"
 Provides-Extra: cookies
 Requires-Dist: browser-cookie3; extra == "cookies"
-Provides-Extra: geetest
-Requires-Dist: rsa; extra == "geetest"
-Requires-Dist: qrcode[pil]; extra == "geetest"
+Provides-Extra: auth
+Requires-Dist: rsa; extra == "auth"
+Requires-Dist: qrcode[pil]; extra == "auth"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 # genshin.py
 
 [![Downloads](https://pepy.tech/badge/genshin)](https://pepy.tech/project/genshin)
 [![PyPI package](https://img.shields.io/pypi/v/genshin)](https://pypi.org/project/genshin/)
```

### Comparing `genshin-1.6.3/genshin.egg-info/SOURCES.txt` & `genshin-1.7.0/genshin.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -25,31 +25,41 @@
 genshin/client/components/diary.py
 genshin/client/components/gacha.py
 genshin/client/components/hoyolab.py
 genshin/client/components/lineup.py
 genshin/client/components/teapot.py
 genshin/client/components/transaction.py
 genshin/client/components/wiki.py
+genshin/client/components/auth/__init__.py
+genshin/client/components/auth/client.py
+genshin/client/components/auth/server.py
+genshin/client/components/auth/subclients/__init__.py
+genshin/client/components/auth/subclients/app.py
+genshin/client/components/auth/subclients/game.py
+genshin/client/components/auth/subclients/web.py
 genshin/client/components/calculator/__init__.py
 genshin/client/components/calculator/calculator.py
 genshin/client/components/calculator/client.py
 genshin/client/components/chronicle/__init__.py
 genshin/client/components/chronicle/base.py
 genshin/client/components/chronicle/client.py
 genshin/client/components/chronicle/genshin.py
 genshin/client/components/chronicle/honkai.py
 genshin/client/components/chronicle/starrail.py
-genshin/client/components/geetest/__init__.py
-genshin/client/components/geetest/client.py
-genshin/client/components/geetest/server.py
 genshin/client/manager/__init__.py
 genshin/client/manager/cookie.py
 genshin/client/manager/managers.py
 genshin/models/__init__.py
 genshin/models/model.py
+genshin/models/auth/__init__.py
+genshin/models/auth/cookie.py
+genshin/models/auth/geetest.py
+genshin/models/auth/qrcode.py
+genshin/models/auth/responses.py
+genshin/models/auth/verification.py
 genshin/models/genshin/__init__.py
 genshin/models/genshin/calculator.py
 genshin/models/genshin/character.py
 genshin/models/genshin/constants.py
 genshin/models/genshin/daily.py
 genshin/models/genshin/diary.py
 genshin/models/genshin/gacha.py
@@ -71,34 +81,31 @@
 genshin/models/honkai/chronicle/battlesuits.py
 genshin/models/honkai/chronicle/modes.py
 genshin/models/honkai/chronicle/stats.py
 genshin/models/hoyolab/__init__.py
 genshin/models/hoyolab/announcements.py
 genshin/models/hoyolab/private.py
 genshin/models/hoyolab/record.py
-genshin/models/miyoushe/__init__.py
-genshin/models/miyoushe/cookie.py
-genshin/models/miyoushe/qrcode.py
 genshin/models/starrail/__init__.py
 genshin/models/starrail/character.py
 genshin/models/starrail/chronicle/__init__.py
 genshin/models/starrail/chronicle/base.py
 genshin/models/starrail/chronicle/challenge.py
 genshin/models/starrail/chronicle/characters.py
 genshin/models/starrail/chronicle/notes.py
 genshin/models/starrail/chronicle/rogue.py
 genshin/models/starrail/chronicle/stats.py
 genshin/paginators/__init__.py
 genshin/paginators/api.py
 genshin/paginators/base.py
 genshin/utility/__init__.py
+genshin/utility/auth.py
 genshin/utility/concurrency.py
 genshin/utility/deprecation.py
 genshin/utility/ds.py
 genshin/utility/extdb.py
 genshin/utility/fs.py
-genshin/utility/geetest.py
 genshin/utility/logfile.py
 genshin/utility/uid.py
 tests/__init__.py
 tests/conftest.py
 tests/test_paginators.py
```

### Comparing `genshin-1.6.3/pyproject.toml` & `genshin-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/setup.py` & `genshin-1.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Run setuptools."""
 
 from setuptools import find_packages, setup
 
 setup(
     name="genshin",
-    version="1.6.3",
+    version="1.7.0",
     author="thesadru",
     author_email="thesadru@gmail.com",
     description="An API wrapper for Genshin Impact.",
     keywords="hoyoverse mihoyo genshin genshin-impact honkai".split(),
     url="https://github.com/thesadru/genshin.py",
     project_urls={
         "Documentation": "https://thesadru.github.io/genshin.py",
@@ -16,15 +16,15 @@
     },
     packages=find_packages(exclude=["tests.*"]),
     python_requires=">=3.8",
     install_requires=["aiohttp", "pydantic"],
     extras_require={
         "all": ["browser-cookie3", "rsa", "click", "qrcode[pil]"],
         "cookies": ["browser-cookie3"],
-        "geetest": ["rsa", "qrcode[pil]"],
+        "auth": ["rsa", "qrcode[pil]"],
         "cli": ["click"],
     },
     include_package_data=True,
     package_data={"genshin": ["py.typed"]},
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `genshin-1.6.3/tests/conftest.py` & `genshin-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.3/tests/test_paginators.py` & `genshin-1.7.0/tests/test_paginators.py`

 * *Files identical despite different names*

