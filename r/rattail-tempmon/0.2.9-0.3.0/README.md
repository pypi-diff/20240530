# Comparing `tmp/rattail-tempmon-0.2.9.tar.gz` & `tmp/rattail_tempmon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattail-tempmon-0.2.9.tar", last modified: Tue May 16 22:40:56 2023, max compression
+gzip compressed data, was "rattail_tempmon-0.3.0.tar", last modified: Thu May 30 16:14:50 2024, max compression
```

## Comparing `rattail-tempmon-0.2.9.tar` & `rattail_tempmon-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/
--rw-r--r--   0 lance     (1000) lance     (1000)     4505 2023-05-16 22:40:30.000000 rattail-tempmon-0.2.9/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 04:36:35.000000 rattail-tempmon-0.2.9/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      252 2016-12-11 04:16:13.000000 rattail-tempmon-0.2.9/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1096 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      371 2017-07-07 04:37:44.000000 rattail-tempmon-0.2.9/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.754131 rattail-tempmon-0.2.9/rattail_tempmon/
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2017-07-07 04:37:15.000000 rattail-tempmon-0.2.9/rattail_tempmon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-16 22:40:33.000000 rattail-tempmon-0.2.9/rattail_tempmon/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7834 2023-02-12 04:24:45.000000 rattail-tempmon-0.2.9/rattail_tempmon/client.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5401 2017-11-19 04:01:12.000000 rattail-tempmon-0.2.9/rattail_tempmon/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2076 2017-07-07 04:36:51.000000 rattail-tempmon-0.2.9/rattail_tempmon/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.754131 rattail-tempmon-0.2.9/rattail_tempmon/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1082 2017-07-07 04:37:01.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.758131 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2015-01-27 18:37:50.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/README
--rw-r--r--   0 lance     (1000) lance     (1000)     1958 2017-08-08 23:46:47.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/env.py
--rw-r--r--   0 lance     (1000) lance     (1000)      640 2017-08-05 17:53:32.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/script.py.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.774131 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)      728 2018-09-28 17:24:26.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py
--rw-r--r--   0 lance     (1000) lance     (1000)      600 2018-09-29 00:08:14.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py
--rw-r--r--   0 lance     (1000) lance     (1000)      639 2017-08-05 17:53:37.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py
--rw-r--r--   0 lance     (1000) lance     (1000)      587 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1383 2018-10-19 22:29:06.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     3462 2016-12-05 21:23:41.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1039 2018-10-20 00:16:00.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1847 2018-10-19 18:52:07.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py
--rw-r--r--   0 lance     (1000) lance     (1000)      778 2018-09-28 17:18:35.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2695 2019-01-26 00:47:51.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16559 2023-02-08 16:54:09.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5516 2019-06-13 17:06:43.000000 rattail-tempmon-0.2.9/rattail_tempmon/emails.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.778131 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.778131 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5156 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/tempmon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2095 2019-01-26 00:39:09.000000 rattail-tempmon-0.2.9/rattail_tempmon/problems.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13667 2019-05-05 16:34:10.000000 rattail-tempmon-0.2.9/rattail_tempmon/server.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2729 2018-10-23 15:22:14.000000 rattail-tempmon-0.2.9/rattail_tempmon/settings.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.742131 rattail-tempmon-0.2.9/rattail_tempmon/templates/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/
--rw-r--r--   0 lance     (1000) lance     (1000)      249 2018-02-07 23:48:07.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_client_offline.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      873 2018-09-11 23:41:05.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      339 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_error.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      268 2016-12-10 18:35:21.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_good_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.754131 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1096 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     2046 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      449 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       24 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1295 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1015 2023-05-16 18:21:17.000000 rattail-tempmon-0.2.9/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4693 2024-05-30 16:14:06.000000 rattail_tempmon-0.3.0/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 04:36:35.000000 rattail_tempmon-0.3.0/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      252 2016-12-11 04:16:13.000000 rattail_tempmon-0.3.0/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1165 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      371 2017-07-07 04:37:44.000000 rattail_tempmon-0.3.0/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.410177 rattail_tempmon-0.3.0/rattail_tempmon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2017-07-07 04:37:15.000000 rattail_tempmon-0.3.0/rattail_tempmon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2024-05-30 16:14:12.000000 rattail_tempmon-0.3.0/rattail_tempmon/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7834 2023-02-12 04:24:45.000000 rattail_tempmon-0.3.0/rattail_tempmon/client.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8796 2024-05-29 12:27:05.000000 rattail_tempmon-0.3.0/rattail_tempmon/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2076 2017-07-07 04:36:51.000000 rattail_tempmon-0.3.0/rattail_tempmon/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.410177 rattail_tempmon-0.3.0/rattail_tempmon/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1082 2017-07-07 04:37:01.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.410177 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2015-01-27 18:37:50.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/README
+-rw-r--r--   0 lance     (1000) lance     (1000)     1958 2017-08-08 23:46:47.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/env.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      640 2017-08-05 17:53:32.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/script.py.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)      728 2018-09-28 17:24:26.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      600 2018-09-29 00:08:14.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      639 2017-08-05 17:53:37.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      587 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1383 2018-10-19 22:29:06.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     3462 2016-12-05 21:23:41.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1039 2018-10-20 00:16:00.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1847 2018-10-19 18:52:07.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      778 2018-09-28 17:18:35.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2695 2019-01-26 00:47:51.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16559 2023-02-08 16:54:09.000000 rattail_tempmon-0.3.0/rattail_tempmon/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5516 2019-06-13 17:06:43.000000 rattail_tempmon-0.3.0/rattail_tempmon/emails.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/rattail_tempmon/hotcooler/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/hotcooler/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/rattail_tempmon/hotcooler/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/hotcooler/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5156 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/hotcooler/importing/tempmon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2095 2019-01-26 00:39:09.000000 rattail_tempmon-0.3.0/rattail_tempmon/problems.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13667 2019-05-05 16:34:10.000000 rattail_tempmon-0.3.0/rattail_tempmon/server.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2729 2018-10-23 15:22:14.000000 rattail_tempmon-0.3.0/rattail_tempmon/settings.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.410177 rattail_tempmon-0.3.0/rattail_tempmon/templates/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/
+-rw-r--r--   0 lance     (1000) lance     (1000)      249 2018-02-07 23:48:07.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_client_offline.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      873 2018-09-11 23:41:05.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      339 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_error.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      268 2016-12-10 18:35:21.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_good_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1165 2024-05-30 16:14:50.000000 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     2046 2024-05-30 16:14:50.000000 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-05-30 16:14:50.000000 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      520 2024-05-30 16:14:50.000000 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       24 2024-05-30 16:14:50.000000 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2024-05-30 16:14:50.000000 rattail_tempmon-0.3.0/rattail_tempmon.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1367 2024-05-30 16:14:50.414177 rattail_tempmon-0.3.0/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1015 2023-05-16 18:21:17.000000 rattail_tempmon-0.3.0/setup.py
```

### Comparing `rattail-tempmon-0.2.9/CHANGES.rst` & `rattail_tempmon-0.3.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 
 CHANGELOG
 =========
 
+0.3.0 (2024-05-30)
+------------------
+
+* Migrate all commands to use ``typer``.
+
+
+0.2.10 (2023-11-30)
+-------------------
+
+* Update subcommand entry point group names, per wuttjamaican.
+
+
 0.2.9 (2023-05-16)
 ------------------
 
 * Replace ``setup.py`` contents with ``setup.cfg``.
 
 
 0.2.8 (2023-02-12)
```

### Comparing `rattail-tempmon-0.2.9/COPYING.txt` & `rattail_tempmon-0.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/PKG-INFO` & `rattail_tempmon-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-tempmon
-Version: 0.2.9
+Version: 0.3.0
 Summary: Retail Software Framework - Temperature monitoring add-on
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,17 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
+Requires-Dist: rattail[db]
+Requires-Dist: six
+Requires-Dist: sqlsoup
 
 
 rattail-tempmon
 ===============
 
 Rattail is a retail software framework, released under the GNU General Public
 License.
```

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/__init__.py` & `rattail_tempmon-0.3.0/rattail_tempmon/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/client.py` & `rattail_tempmon-0.3.0/rattail_tempmon/client.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/config.py` & `rattail_tempmon-0.3.0/rattail_tempmon/config.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/__init__.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/env.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/script.py.mako` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/db/model.py` & `rattail_tempmon-0.3.0/rattail_tempmon/db/model.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/emails.py` & `rattail_tempmon-0.3.0/rattail_tempmon/emails.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/tempmon.py` & `rattail_tempmon-0.3.0/rattail_tempmon/hotcooler/importing/tempmon.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/problems.py` & `rattail_tempmon-0.3.0/rattail_tempmon/problems.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/server.py` & `rattail_tempmon-0.3.0/rattail_tempmon/server.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/settings.py` & `rattail_tempmon-0.3.0/rattail_tempmon/settings.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako` & `rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako` & `rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako` & `rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako` & `rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako` & `rattail_tempmon-0.3.0/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon.egg-info/PKG-INFO` & `rattail_tempmon-0.3.0/rattail_tempmon.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-tempmon
-Version: 0.2.9
+Version: 0.3.0
 Summary: Retail Software Framework - Temperature monitoring add-on
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,17 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
+Requires-Dist: rattail[db]
+Requires-Dist: six
+Requires-Dist: sqlsoup
 
 
 rattail-tempmon
 ===============
 
 Rattail is a retail software framework, released under the GNU General Public
 License.
```

### Comparing `rattail-tempmon-0.2.9/rattail_tempmon.egg-info/SOURCES.txt` & `rattail_tempmon-0.3.0/rattail_tempmon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.9/setup.cfg` & `rattail_tempmon-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 	rattail[db]
 	six
 	sqlsoup
 packages = find:
 include_package_data = True
 
 [options.entry_points]
-rattail.commands = 
+rattail.subcommands = 
 	export-hotcooler = rattail_tempmon.commands:ExportHotCooler
 	purge-tempmon = rattail_tempmon.commands:PurgeTempmon
 	tempmon-client = rattail_tempmon.commands:TempmonClient
 	tempmon-problems = rattail_tempmon.commands:TempmonProblems
 	tempmon-server = rattail_tempmon.commands:TempmonServer
+rattail.typer_imports = 
+	rattail_tempmon = rattail_tempmon.commands
 rattail.config.extensions = 
 	tempmon = rattail_tempmon.config:TempmonConfigExtension
 rattail.emails = 
 	rattail_tempmon = rattail_tempmon.emails
 
 [egg_info]
 tag_build =
```

### Comparing `rattail-tempmon-0.2.9/setup.py` & `rattail_tempmon-0.3.0/setup.py`

 * *Files identical despite different names*

