# Comparing `tmp/mayan-importer-3.4.tar.gz` & `tmp/mayan-importer-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-3.4.tar", last modified: Wed May 29 21:24:09 2024, max compression
+gzip compressed data, was "mayan-importer-3.5.tar", last modified: Thu May 30 20:31:52 2024, max compression
```

## Comparing `mayan-importer-3.4.tar` & `mayan-importer-3.5.tar`

### file list

```diff
@@ -1,96 +1,95 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.493307 mayan-importer-3.4/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6853 2024-05-27 19:32:10.000000 mayan-importer-3.4/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.4/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.4/MANIFEST.in
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9743 2024-05-29 21:24:09.493307 mayan-importer-3.4/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.4/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.484307 mayan-importer-3.4/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.4/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/admin.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.484307 mayan-importer-3.4/importer/api_views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-26 15:20:06.000000 mayan-importer-3.4/importer/api_views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      377 2024-05-26 15:33:08.000000 mayan-importer-3.4/importer/api_views/api_view_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3132 2024-05-26 15:36:43.000000 mayan-importer-3.4/importer/api_views/import_setup_api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1398 2024-05-26 15:51:28.000000 mayan-importer-3.4/importer/api_views/import_setup_item_api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7839 2024-05-14 04:09:13.000000 mayan-importer-3.4/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7165 2024-05-03 23:02:13.000000 mayan-importer-3.4/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      146 2024-05-29 21:22:31.000000 mayan-importer-3.4/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1759 2024-05-14 04:09:13.000000 mayan-importer-3.4/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/exceptions.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.485308 mayan-importer-3.4/importer/forms/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.4/importer/forms/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      327 2024-05-04 21:13:39.000000 mayan-importer-3.4/importer/forms/filer_forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.4/importer/forms/form_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.4/importer/forms/import_setup_forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.4/importer/forms/import_setup_item_forms.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.485308 mayan-importer-3.4/importer/icons/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.4/importer/icons/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.4/importer/icons/import_setup_filer_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.4/importer/icons/import_setup_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.4/importer/icons/import_setup_item_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8765 2024-05-27 18:10:36.000000 mayan-importer-3.4/importer/importers.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.486307 mayan-importer-3.4/importer/links/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.4/importer/links/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.4/importer/links/import_setup_filer_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.4/importer/links/import_setup_item_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.4/importer/links/import_setup_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.4/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.489307 mayan-importer-3.4/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.4/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.4/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.4/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.4/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/migrations/0017_delete_importsetuplog.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/migrations/0018_auto_20240401_0808.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.4/importer/migrations/0019_auto_20240402_1101.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.4/importer/migrations/0020_auto_20240502_1907.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2343 2024-05-26 15:35:26.000000 mayan-importer-3.4/importer/migrations/0021_migrate_state_codes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.4/importer/migrations/0022_auto_20240503_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.4/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.490307 mayan-importer-3.4/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       91 2024-05-04 07:48:41.000000 mayan-importer-3.4/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4150 2024-05-27 18:07:50.000000 mayan-importer-3.4/importer/models/import_setup_item_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.4/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6055 2024-05-09 22:12:23.000000 mayan-importer-3.4/importer/models/import_setup_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-04 06:55:15.000000 mayan-importer-3.4/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3256 2024-05-04 19:50:33.000000 mayan-importer-3.4/importer/models/model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.4/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.491307 mayan-importer-3.4/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.4/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.4/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      695 2024-05-04 07:00:01.000000 mayan-importer-3.4/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1294 2024-05-04 07:47:44.000000 mayan-importer-3.4/importer/tests/test_filer_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8230 2024-05-04 06:59:12.000000 mayan-importer-3.4/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7720 2024-05-04 07:46:59.000000 mayan-importer-3.4/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11506 2024-05-14 04:09:13.000000 mayan-importer-3.4/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6309 2024-05-04 07:46:59.000000 mayan-importer-3.4/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5860 2024-05-26 15:51:08.000000 mayan-importer-3.4/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.492307 mayan-importer-3.4/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.4/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-04 21:13:39.000000 mayan-importer-3.4/importer/views/import_setup_filer_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.4/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.4/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-29 21:24:09.493307 mayan-importer-3.4/mayan_importer.egg-info/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9743 2024-05-29 21:24:09.000000 mayan-importer-3.4/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2974 2024-05-29 21:24:09.000000 mayan-importer-3.4/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-29 21:24:09.000000 mayan-importer-3.4/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-29 21:24:09.000000 mayan-importer-3.4/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-29 21:24:09.000000 mayan-importer-3.4/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-29 21:24:09.000000 mayan-importer-3.4/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-29 21:24:09.493307 mayan-importer-3.4/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3036 2024-05-29 21:23:59.000000 mayan-importer-3.4/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.907819 mayan-importer-3.5/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6853 2024-05-27 19:32:10.000000 mayan-importer-3.5/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.5/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.5/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9743 2024-05-30 20:31:52.907819 mayan-importer-3.5/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.5/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.885820 mayan-importer-3.5/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.5/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/admin.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.886820 mayan-importer-3.5/importer/api_views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-26 15:20:06.000000 mayan-importer-3.5/importer/api_views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      377 2024-05-26 15:33:08.000000 mayan-importer-3.5/importer/api_views/api_view_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3132 2024-05-26 15:36:43.000000 mayan-importer-3.5/importer/api_views/import_setup_api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1398 2024-05-26 15:51:28.000000 mayan-importer-3.5/importer/api_views/import_setup_item_api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7839 2024-05-14 04:09:13.000000 mayan-importer-3.5/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7165 2024-05-03 23:02:13.000000 mayan-importer-3.5/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1759 2024-05-14 04:09:13.000000 mayan-importer-3.5/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/exceptions.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.888820 mayan-importer-3.5/importer/forms/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.5/importer/forms/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      327 2024-05-04 21:13:39.000000 mayan-importer-3.5/importer/forms/filer_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.5/importer/forms/form_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.5/importer/forms/import_setup_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.5/importer/forms/import_setup_item_forms.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.889820 mayan-importer-3.5/importer/icons/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.5/importer/icons/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.5/importer/icons/import_setup_filer_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.5/importer/icons/import_setup_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.5/importer/icons/import_setup_item_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8765 2024-05-27 18:10:36.000000 mayan-importer-3.5/importer/importers.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.890820 mayan-importer-3.5/importer/links/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.5/importer/links/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.5/importer/links/import_setup_filer_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.5/importer/links/import_setup_item_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.5/importer/links/import_setup_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.5/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.901820 mayan-importer-3.5/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.5/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.5/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.5/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.5/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.5/importer/migrations/0019_auto_20240402_1101.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.5/importer/migrations/0020_auto_20240502_1907.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2343 2024-05-26 15:35:26.000000 mayan-importer-3.5/importer/migrations/0021_migrate_state_codes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.5/importer/migrations/0022_auto_20240503_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.5/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.902819 mayan-importer-3.5/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       91 2024-05-04 07:48:41.000000 mayan-importer-3.5/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4150 2024-05-27 18:07:50.000000 mayan-importer-3.5/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.5/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6055 2024-05-09 22:12:23.000000 mayan-importer-3.5/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-04 06:55:15.000000 mayan-importer-3.5/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3256 2024-05-04 19:50:33.000000 mayan-importer-3.5/importer/models/model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.5/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.904819 mayan-importer-3.5/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.5/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.5/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      695 2024-05-04 07:00:01.000000 mayan-importer-3.5/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1294 2024-05-04 07:47:44.000000 mayan-importer-3.5/importer/tests/test_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8230 2024-05-04 06:59:12.000000 mayan-importer-3.5/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7720 2024-05-04 07:46:59.000000 mayan-importer-3.5/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11506 2024-05-14 04:09:13.000000 mayan-importer-3.5/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6309 2024-05-04 07:46:59.000000 mayan-importer-3.5/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5860 2024-05-26 15:51:08.000000 mayan-importer-3.5/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.905820 mayan-importer-3.5/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.5/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-04 21:13:39.000000 mayan-importer-3.5/importer/views/import_setup_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.5/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.5/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-30 20:31:52.907819 mayan-importer-3.5/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9743 2024-05-30 20:31:52.000000 mayan-importer-3.5/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2949 2024-05-30 20:31:52.000000 mayan-importer-3.5/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-30 20:31:52.000000 mayan-importer-3.5/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-30 20:31:52.000000 mayan-importer-3.5/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-30 20:31:52.000000 mayan-importer-3.5/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-30 20:31:52.000000 mayan-importer-3.5/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-30 20:31:52.907819 mayan-importer-3.5/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3036 2024-05-29 21:30:12.000000 mayan-importer-3.5/setup.py
```

### Comparing `mayan-importer-3.4/HISTORY.rst` & `mayan-importer-3.5/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/LICENSE` & `mayan-importer-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/PKG-INFO` & `mayan-importer-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.4
+Version: 3.5
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.4/README.rst` & `mayan-importer-3.5/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/api_views/import_setup_api_views.py` & `mayan-importer-3.5/importer/api_views/import_setup_api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/api_views/import_setup_item_api_views.py` & `mayan-importer-3.5/importer/api_views/import_setup_item_api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/apps.py` & `mayan-importer-3.5/importer/apps.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/classes.py` & `mayan-importer-3.5/importer/classes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/events.py` & `mayan-importer-3.5/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/forms/import_setup_forms.py` & `mayan-importer-3.5/importer/forms/import_setup_forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/forms/import_setup_item_forms.py` & `mayan-importer-3.5/importer/forms/import_setup_item_forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/icons/import_setup_icons.py` & `mayan-importer-3.5/importer/icons/import_setup_icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/icons/import_setup_item_icons.py` & `mayan-importer-3.5/importer/icons/import_setup_item_icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/importers.py` & `mayan-importer-3.5/importer/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/links/import_setup_filer_links.py` & `mayan-importer-3.5/importer/links/import_setup_filer_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/links/import_setup_item_links.py` & `mayan-importer-3.5/importer/links/import_setup_item_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/links/import_setup_links.py` & `mayan-importer-3.5/importer/links/import_setup_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/literals.py` & `mayan-importer-3.5/importer/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0001_initial.py` & `mayan-importer-3.5/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.5/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.5/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.5/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.5/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.5/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.5/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.5/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.5/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.5/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.5/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.5/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0018_auto_20240401_0808.py` & `mayan-importer-3.5/importer/migrations/0018_auto_20240401_0808.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0019_auto_20240402_1101.py` & `mayan-importer-3.5/importer/migrations/0019_auto_20240402_1101.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0020_auto_20240502_1907.py` & `mayan-importer-3.5/importer/migrations/0020_auto_20240502_1907.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0021_migrate_state_codes.py` & `mayan-importer-3.5/importer/migrations/0021_migrate_state_codes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/migrations/0022_auto_20240503_0853.py` & `mayan-importer-3.5/importer/migrations/0022_auto_20240503_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/models/import_setup_item_model_mixins.py` & `mayan-importer-3.5/importer/models/import_setup_item_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/models/import_setup_item_models.py` & `mayan-importer-3.5/importer/models/import_setup_item_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/models/import_setup_model_mixins.py` & `mayan-importer-3.5/importer/models/import_setup_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/models/import_setup_models.py` & `mayan-importer-3.5/importer/models/import_setup_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/models/model_mixins.py` & `mayan-importer-3.5/importer/models/model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/permissions.py` & `mayan-importer-3.5/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/queues.py` & `mayan-importer-3.5/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/serializers.py` & `mayan-importer-3.5/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tasks.py` & `mayan-importer-3.5/importer/tasks.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/importers.py` & `mayan-importer-3.5/importer/tests/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/literals.py` & `mayan-importer-3.5/importer/tests/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/test_filer_views.py` & `mayan-importer-3.5/importer/tests/test_filer_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/test_import_setup_api.py` & `mayan-importer-3.5/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.5/importer/tests/test_import_setup_item_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.5/importer/tests/test_import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/tests/test_import_setup_views.py` & `mayan-importer-3.5/importer/tests/test_import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/urls.py` & `mayan-importer-3.5/importer/urls.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/views/import_setup_filer_views.py` & `mayan-importer-3.5/importer/views/import_setup_filer_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/views/import_setup_item_views.py` & `mayan-importer-3.5/importer/views/import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/importer/views/import_setup_views.py` & `mayan-importer-3.5/importer/views/import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.4/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.5/mayan_importer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.4
+Version: 3.5
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.4/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.5/mayan_importer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.rst
 setup.cfg
 setup.py
 importer/__init__.py
 importer/admin.py
 importer/apps.py
 importer/classes.py
-importer/dependencies.py
 importer/events.py
 importer/exceptions.py
 importer/importers.py
 importer/literals.py
 importer/permissions.py
 importer/queues.py
 importer/serializers.py
```

### Comparing `mayan-importer-3.4/setup.py` & `mayan-importer-3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='3.4',
+    version='3.5',
     zip_safe=False,
 )
```

