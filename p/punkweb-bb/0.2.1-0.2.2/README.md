# Comparing `tmp/punkweb_bb-0.2.1.tar.gz` & `tmp/punkweb_bb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.2.1.tar", last modified: Wed May 29 04:58:56 2024, max compression
+gzip compressed data, was "punkweb_bb-0.2.2.tar", last modified: Wed May 29 20:22:44 2024, max compression
```

## Comparing `punkweb_bb-0.2.1.tar` & `punkweb_bb-0.2.2.tar`

### file list

```diff
@@ -1,282 +1,289 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.1/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.1/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     4369 2024-05-09 06:47:11.000000 punkweb_bb-0.2.1/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.1/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/guests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    13931 2024-05-29 01:02:42.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1025 2024-05-29 04:36:57.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3565 2024-05-29 01:15:02.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      748 2024-05-28 21:07:24.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    25276 2024-05-29 01:17:40.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.2.1/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.2.1/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.1/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.1/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.1/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.1/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.1/punkweb_bb/guests.py
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.1/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/0003_alter_thread_options.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.1/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     6348 2024-05-29 01:02:41.000000 punkweb_bb-0.2.1/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.1/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.1/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.1/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      561 2024-05-29 04:36:54.000000 punkweb_bb-0.2.1/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.1/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/category-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      711 2024-05-28 20:02:41.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1873 2024-05-29 01:04:59.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10470 2024-05-29 04:55:52.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2781 2024-05-29 04:30:06.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     3012 2024-05-29 04:30:15.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      736 2024-05-29 04:44:03.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     5848 2024-05-29 04:30:44.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10276 2024-05-29 04:43:11.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-29 04:30:51.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/can_delete.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/can_edit.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/can_post.py
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.1/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2587 2024-05-29 01:15:01.000000 punkweb_bb-0.2.1/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-05-28 21:06:17.000000 punkweb_bb-0.2.1/punkweb_bb/utils.py
--rw-r--r--   0 pork      (1000) pork      (1000)    17400 2024-05-29 01:17:40.000000 punkweb_bb-0.2.1/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    14409 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-29 04:58:04.000000 punkweb_bb-0.2.1/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.2/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.2/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     4441 2024-05-29 05:09:26.000000 punkweb_bb-0.2.2/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.2/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     4182 2024-05-29 19:50:24.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3531 2024-05-29 19:49:57.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    15235 2024-05-29 20:18:30.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1025 2024-05-29 04:36:57.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3565 2024-05-29 01:15:02.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2086 2024-05-29 20:11:36.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    25276 2024-05-29 01:17:40.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2821 2024-05-29 19:50:23.000000 punkweb_bb-0.2.2/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1372 2024-05-29 19:49:56.000000 punkweb_bb-0.2.2/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.2/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.2/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.2/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.2/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.2/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.2/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0003_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1821 2024-05-29 19:48:54.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/0004_groupstyle.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2000 2024-05-29 19:48:57.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.2/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     6962 2024-05-29 20:18:29.000000 punkweb_bb-0.2.2/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.2/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.2/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.2/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      561 2024-05-29 04:36:54.000000 punkweb_bb-0.2.2/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.2/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.388550 punkweb_bb-0.2.2/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/category-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      735 2024-05-29 20:09:34.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1870 2024-05-29 20:15:36.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.396550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.388550 punkweb_bb-0.2.2/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.400550 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10526 2024-05-29 20:04:35.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2804 2024-05-29 20:04:57.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3035 2024-05-29 20:06:01.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      759 2024-05-29 20:07:16.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     5842 2024-05-29 20:09:18.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10390 2024-05-29 20:13:22.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-29 04:30:51.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      712 2024-05-29 20:12:20.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-29 20:03:41.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      626 2024-05-29 19:57:45.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/can_delete.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/can_edit.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/can_post.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/shoutbox_bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      257 2024-05-29 20:12:14.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/styled_group_name.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      202 2024-05-29 20:03:14.000000 punkweb_bb-0.2.2/punkweb_bb/templatetags/styled_username.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.2/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2587 2024-05-29 01:15:01.000000 punkweb_bb-0.2.2/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1223 2024-05-29 20:11:35.000000 punkweb_bb-0.2.2/punkweb_bb/utils.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    17400 2024-05-29 01:17:40.000000 punkweb_bb-0.2.2/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.2/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 20:22:44.392550 punkweb_bb-0.2.2/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     5095 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    14803 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-29 20:22:44.000000 punkweb_bb-0.2.2/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-29 20:22:44.404550 punkweb_bb-0.2.2/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-29 20:22:30.000000 punkweb_bb-0.2.2/setup.py
```

### Comparing `punkweb_bb-0.2.1/LICENSE` & `punkweb_bb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/PKG-INFO` & `punkweb_bb-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.2.1
+Version: 0.2.2
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -31,15 +31,15 @@
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
 - [SCEditor](https://www.sceditor.com/)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
-- Python 3.11+
+- Python 3.9+
 - Django 4.2+
 - django-precise-bbcode 1.2+
 - Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
 ## Installation
@@ -107,14 +107,15 @@
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
   "FAVICON": "punkweb_bb/favicon.ico",
+  "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
 ```
```

### Comparing `punkweb_bb-0.2.1/README.md` & `punkweb_bb-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
 - [SCEditor](https://www.sceditor.com/)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
-- Python 3.11+
+- Python 3.9+
 - Django 4.2+
 - django-precise-bbcode 1.2+
 - Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
 ## Installation
@@ -89,14 +89,15 @@
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
   "FAVICON": "punkweb_bb/favicon.ico",
+  "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
 ```
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,36 +1,39 @@
 magic:    0xa70d0d0a
-moddate:  0x126b1066 (Fri Apr  5 21:20:18 2024 UTC)
-files sz: 2493
+moddate:  0xff865766 (Wed May 29 19:50:23 2024 UTC)
+files sz: 2821
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a056d065a066d075a076d085a086d095a090100640064046c
-      0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a100100020065
-      016a110000000000000000650ba6010000ab010000000000000000020047
-      0064058400640665016a120000000000000000a6030000ab030000000000
-      000000a6000000ab0000000000000000005a13020065016a110000000000
-      000000650ca6010000ab0100000000000000000200470064078400640865
-      016a120000000000000000a6030000ab030000000000000000a6000000ab
-      0000000000000000005a14020065016a110000000000000000650fa60100
-      00ab0100000000000000000200470064098400640a65016a120000000000
+      036c046d055a056d065a066d075a076d085a086d095a096d0a5a0a010064
+      0064046c0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d
+      125a120100020065016a130000000000000000650ca6010000ab01000000
+      00000000000200470064058400640665016a140000000000000000a60300
+      00ab030000000000000000a6000000ab0000000000000000005a15020065
+      016a130000000000000000650da6010000ab010000000000000000020047
+      0064078400640865016a140000000000000000a6030000ab030000000000
+      000000a6000000ab0000000000000000005a16020065016a130000000000
+      0000006511a6010000ab0100000000000000000200470064098400640a65
+      016a140000000000000000a6030000ab030000000000000000a6000000ab
+      0000000000000000005a17020065016a1300000000000000006512a60100
+      00ab01000000000000000002004700640b8400640c65016a140000000000
       000000a6030000ab030000000000000000a6000000ab0000000000000000
-      005a15020065016a1100000000000000006510a6010000ab010000000000
-      00000002004700640b8400640c65016a120000000000000000a6030000ab
-      030000000000000000a6000000ab0000000000000000005a16020065016a
-      110000000000000000650da6010000ab0100000000000000000200470064
-      0d8400640e65016a120000000000000000a6030000ab0300000000000000
-      00a6000000ab0000000000000000005a17020065016a1100000000000000
-      00650ea6010000ab01000000000000000002004700640f8400641065016a
-      120000000000000000a6030000ab030000000000000000a6000000ab0000
-      000000000000005a1864115300
+      005a18020065016a130000000000000000650fa6010000ab010000000000
+      00000002004700640d8400640e65016a140000000000000000a6030000ab
+      030000000000000000a6000000ab0000000000000000005a19020065016a
+      1300000000000000006510a6010000ab0100000000000000000200470064
+      0f8400641065016a140000000000000000a6030000ab0300000000000000
+      00a6000000ab0000000000000000005a1a020065016a1300000000000000
+      00650ea6010000ab0100000000000000000200470064118400641265016a
+      140000000000000000a6030000ab030000000000000000a6000000ab0000
+      000000000000005a1b64135300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('admin',))
                  6 IMPORT_NAME              0 (django.contrib)
                  8 IMPORT_FROM              1 (admin)
                 10 STORE_NAME               1 (admin)
@@ -40,214 +43,240 @@
                 16 LOAD_CONST               2 (('mark_safe',))
                 18 IMPORT_NAME              2 (django.utils.safestring)
                 20 IMPORT_FROM              3 (mark_safe)
                 22 STORE_NAME               3 (mark_safe)
                 24 POP_TOP
    
      4          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm'))
+                28 LOAD_CONST               3 (('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm'))
                 30 IMPORT_NAME              4 (punkweb_bb.admin_forms)
                 32 IMPORT_FROM              5 (BoardProfileAdminModelForm)
                 34 STORE_NAME               5 (BoardProfileAdminModelForm)
                 36 IMPORT_FROM              6 (CategoryAdminModelForm)
                 38 STORE_NAME               6 (CategoryAdminModelForm)
-                40 IMPORT_FROM              7 (PostAdminModelForm)
-                42 STORE_NAME               7 (PostAdminModelForm)
-                44 IMPORT_FROM              8 (SubcategoryAdminModelForm)
-                46 STORE_NAME               8 (SubcategoryAdminModelForm)
-                48 IMPORT_FROM              9 (ThreadAdminModelForm)
-                50 STORE_NAME               9 (ThreadAdminModelForm)
-                52 POP_TOP
-   
-    11          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               4 (('BoardProfile', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
-                58 IMPORT_NAME             10 (punkweb_bb.models)
-                60 IMPORT_FROM             11 (BoardProfile)
-                62 STORE_NAME              11 (BoardProfile)
-                64 IMPORT_FROM             12 (Category)
-                66 STORE_NAME              12 (Category)
-                68 IMPORT_FROM             13 (Post)
-                70 STORE_NAME              13 (Post)
-                72 IMPORT_FROM             14 (Shout)
-                74 STORE_NAME              14 (Shout)
-                76 IMPORT_FROM             15 (Subcategory)
-                78 STORE_NAME              15 (Subcategory)
-                80 IMPORT_FROM             16 (Thread)
-                82 STORE_NAME              16 (Thread)
-                84 POP_TOP
-   
-    14          86 PUSH_NULL
-                88 LOAD_NAME                1 (admin)
-                90 LOAD_ATTR               17 (register)
-               100 LOAD_NAME               11 (BoardProfile)
-               102 PRECALL                  1
-               106 CALL                     1
-   
-    15         116 PUSH_NULL
-               118 LOAD_BUILD_CLASS
-               120 LOAD_CONST               5 (<code object BoardProfileModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 14>)
-               122 MAKE_FUNCTION            0
-               124 LOAD_CONST               6 ('BoardProfileModelAdmin')
-               126 LOAD_NAME                1 (admin)
-               128 LOAD_ATTR               18 (ModelAdmin)
-               138 PRECALL                  3
-               142 CALL                     3
-   
-    14         152 PRECALL                  0
-               156 CALL                     0
-   
-    15         166 STORE_NAME              19 (BoardProfileModelAdmin)
-   
-    34         168 PUSH_NULL
-               170 LOAD_NAME                1 (admin)
-               172 LOAD_ATTR               17 (register)
-               182 LOAD_NAME               12 (Category)
-               184 PRECALL                  1
-               188 CALL                     1
-   
-    35         198 PUSH_NULL
-               200 LOAD_BUILD_CLASS
-               202 LOAD_CONST               7 (<code object CategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 34>)
-               204 MAKE_FUNCTION            0
-               206 LOAD_CONST               8 ('CategoryModelAdmin')
-               208 LOAD_NAME                1 (admin)
-               210 LOAD_ATTR               18 (ModelAdmin)
-               220 PRECALL                  3
-               224 CALL                     3
-   
-    34         234 PRECALL                  0
-               238 CALL                     0
-   
-    35         248 STORE_NAME              20 (CategoryModelAdmin)
-   
-    48         250 PUSH_NULL
-               252 LOAD_NAME                1 (admin)
-               254 LOAD_ATTR               17 (register)
-               264 LOAD_NAME               15 (Subcategory)
-               266 PRECALL                  1
-               270 CALL                     1
-   
-    49         280 PUSH_NULL
-               282 LOAD_BUILD_CLASS
-               284 LOAD_CONST               9 (<code object SubcategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 48>)
-               286 MAKE_FUNCTION            0
-               288 LOAD_CONST              10 ('SubcategoryModelAdmin')
-               290 LOAD_NAME                1 (admin)
-               292 LOAD_ATTR               18 (ModelAdmin)
-               302 PRECALL                  3
-               306 CALL                     3
-   
-    48         316 PRECALL                  0
-               320 CALL                     0
-   
-    49         330 STORE_NAME              21 (SubcategoryModelAdmin)
-   
-    64         332 PUSH_NULL
-               334 LOAD_NAME                1 (admin)
-               336 LOAD_ATTR               17 (register)
-               346 LOAD_NAME               16 (Thread)
-               348 PRECALL                  1
-               352 CALL                     1
-   
-    65         362 PUSH_NULL
-               364 LOAD_BUILD_CLASS
-               366 LOAD_CONST              11 (<code object ThreadModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 64>)
-               368 MAKE_FUNCTION            0
-               370 LOAD_CONST              12 ('ThreadModelAdmin')
-               372 LOAD_NAME                1 (admin)
-               374 LOAD_ATTR               18 (ModelAdmin)
-               384 PRECALL                  3
-               388 CALL                     3
-   
-    64         398 PRECALL                  0
-               402 CALL                     0
-   
-    65         412 STORE_NAME              22 (ThreadModelAdmin)
-   
-    91         414 PUSH_NULL
-               416 LOAD_NAME                1 (admin)
-               418 LOAD_ATTR               17 (register)
-               428 LOAD_NAME               13 (Post)
-               430 PRECALL                  1
-               434 CALL                     1
-   
-    92         444 PUSH_NULL
-               446 LOAD_BUILD_CLASS
-               448 LOAD_CONST              13 (<code object PostModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 91>)
-               450 MAKE_FUNCTION            0
-               452 LOAD_CONST              14 ('PostModelAdmin')
-               454 LOAD_NAME                1 (admin)
-               456 LOAD_ATTR               18 (ModelAdmin)
-               466 PRECALL                  3
-               470 CALL                     3
-   
-    91         480 PRECALL                  0
-               484 CALL                     0
-   
-    92         494 STORE_NAME              23 (PostModelAdmin)
-   
-   106         496 PUSH_NULL
-               498 LOAD_NAME                1 (admin)
-               500 LOAD_ATTR               17 (register)
-               510 LOAD_NAME               14 (Shout)
-               512 PRECALL                  1
-               516 CALL                     1
-   
-   107         526 PUSH_NULL
-               528 LOAD_BUILD_CLASS
-               530 LOAD_CONST              15 (<code object ShoutModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 106>)
-               532 MAKE_FUNCTION            0
-               534 LOAD_CONST              16 ('ShoutModelAdmin')
-               536 LOAD_NAME                1 (admin)
-               538 LOAD_ATTR               18 (ModelAdmin)
-               548 PRECALL                  3
-               552 CALL                     3
-   
-   106         562 PRECALL                  0
-               566 CALL                     0
-   
-   107         576 STORE_NAME              24 (ShoutModelAdmin)
-               578 LOAD_CONST              17 (None)
-               580 RETURN_VALUE
+                40 IMPORT_FROM              7 (GroupStyleAdminModelForm)
+                42 STORE_NAME               7 (GroupStyleAdminModelForm)
+                44 IMPORT_FROM              8 (PostAdminModelForm)
+                46 STORE_NAME               8 (PostAdminModelForm)
+                48 IMPORT_FROM              9 (SubcategoryAdminModelForm)
+                50 STORE_NAME               9 (SubcategoryAdminModelForm)
+                52 IMPORT_FROM             10 (ThreadAdminModelForm)
+                54 STORE_NAME              10 (ThreadAdminModelForm)
+                56 POP_TOP
+   
+    12          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               4 (('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread'))
+                62 IMPORT_NAME             11 (punkweb_bb.models)
+                64 IMPORT_FROM             12 (BoardProfile)
+                66 STORE_NAME              12 (BoardProfile)
+                68 IMPORT_FROM             13 (Category)
+                70 STORE_NAME              13 (Category)
+                72 IMPORT_FROM             14 (GroupStyle)
+                74 STORE_NAME              14 (GroupStyle)
+                76 IMPORT_FROM             15 (Post)
+                78 STORE_NAME              15 (Post)
+                80 IMPORT_FROM             16 (Shout)
+                82 STORE_NAME              16 (Shout)
+                84 IMPORT_FROM             17 (Subcategory)
+                86 STORE_NAME              17 (Subcategory)
+                88 IMPORT_FROM             18 (Thread)
+                90 STORE_NAME              18 (Thread)
+                92 POP_TOP
+   
+    23          94 PUSH_NULL
+                96 LOAD_NAME                1 (admin)
+                98 LOAD_ATTR               19 (register)
+               108 LOAD_NAME               12 (BoardProfile)
+               110 PRECALL                  1
+               114 CALL                     1
+   
+    24         124 PUSH_NULL
+               126 LOAD_BUILD_CLASS
+               128 LOAD_CONST               5 (<code object BoardProfileModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 23>)
+               130 MAKE_FUNCTION            0
+               132 LOAD_CONST               6 ('BoardProfileModelAdmin')
+               134 LOAD_NAME                1 (admin)
+               136 LOAD_ATTR               20 (ModelAdmin)
+               146 PRECALL                  3
+               150 CALL                     3
+   
+    23         160 PRECALL                  0
+               164 CALL                     0
+   
+    24         174 STORE_NAME              21 (BoardProfileModelAdmin)
+   
+    43         176 PUSH_NULL
+               178 LOAD_NAME                1 (admin)
+               180 LOAD_ATTR               19 (register)
+               190 LOAD_NAME               13 (Category)
+               192 PRECALL                  1
+               196 CALL                     1
+   
+    44         206 PUSH_NULL
+               208 LOAD_BUILD_CLASS
+               210 LOAD_CONST               7 (<code object CategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 43>)
+               212 MAKE_FUNCTION            0
+               214 LOAD_CONST               8 ('CategoryModelAdmin')
+               216 LOAD_NAME                1 (admin)
+               218 LOAD_ATTR               20 (ModelAdmin)
+               228 PRECALL                  3
+               232 CALL                     3
+   
+    43         242 PRECALL                  0
+               246 CALL                     0
+   
+    44         256 STORE_NAME              22 (CategoryModelAdmin)
+   
+    57         258 PUSH_NULL
+               260 LOAD_NAME                1 (admin)
+               262 LOAD_ATTR               19 (register)
+               272 LOAD_NAME               17 (Subcategory)
+               274 PRECALL                  1
+               278 CALL                     1
+   
+    58         288 PUSH_NULL
+               290 LOAD_BUILD_CLASS
+               292 LOAD_CONST               9 (<code object SubcategoryModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 57>)
+               294 MAKE_FUNCTION            0
+               296 LOAD_CONST              10 ('SubcategoryModelAdmin')
+               298 LOAD_NAME                1 (admin)
+               300 LOAD_ATTR               20 (ModelAdmin)
+               310 PRECALL                  3
+               314 CALL                     3
+   
+    57         324 PRECALL                  0
+               328 CALL                     0
+   
+    58         338 STORE_NAME              23 (SubcategoryModelAdmin)
+   
+    73         340 PUSH_NULL
+               342 LOAD_NAME                1 (admin)
+               344 LOAD_ATTR               19 (register)
+               354 LOAD_NAME               18 (Thread)
+               356 PRECALL                  1
+               360 CALL                     1
+   
+    74         370 PUSH_NULL
+               372 LOAD_BUILD_CLASS
+               374 LOAD_CONST              11 (<code object ThreadModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 73>)
+               376 MAKE_FUNCTION            0
+               378 LOAD_CONST              12 ('ThreadModelAdmin')
+               380 LOAD_NAME                1 (admin)
+               382 LOAD_ATTR               20 (ModelAdmin)
+               392 PRECALL                  3
+               396 CALL                     3
+   
+    73         406 PRECALL                  0
+               410 CALL                     0
+   
+    74         420 STORE_NAME              24 (ThreadModelAdmin)
+   
+   100         422 PUSH_NULL
+               424 LOAD_NAME                1 (admin)
+               426 LOAD_ATTR               19 (register)
+               436 LOAD_NAME               15 (Post)
+               438 PRECALL                  1
+               442 CALL                     1
+   
+   101         452 PUSH_NULL
+               454 LOAD_BUILD_CLASS
+               456 LOAD_CONST              13 (<code object PostModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 100>)
+               458 MAKE_FUNCTION            0
+               460 LOAD_CONST              14 ('PostModelAdmin')
+               462 LOAD_NAME                1 (admin)
+               464 LOAD_ATTR               20 (ModelAdmin)
+               474 PRECALL                  3
+               478 CALL                     3
+   
+   100         488 PRECALL                  0
+               492 CALL                     0
+   
+   101         502 STORE_NAME              25 (PostModelAdmin)
+   
+   115         504 PUSH_NULL
+               506 LOAD_NAME                1 (admin)
+               508 LOAD_ATTR               19 (register)
+               518 LOAD_NAME               16 (Shout)
+               520 PRECALL                  1
+               524 CALL                     1
+   
+   116         534 PUSH_NULL
+               536 LOAD_BUILD_CLASS
+               538 LOAD_CONST              15 (<code object ShoutModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 115>)
+               540 MAKE_FUNCTION            0
+               542 LOAD_CONST              16 ('ShoutModelAdmin')
+               544 LOAD_NAME                1 (admin)
+               546 LOAD_ATTR               20 (ModelAdmin)
+               556 PRECALL                  3
+               560 CALL                     3
+   
+   115         570 PRECALL                  0
+               574 CALL                     0
+   
+   116         584 STORE_NAME              26 (ShoutModelAdmin)
+   
+   128         586 PUSH_NULL
+               588 LOAD_NAME                1 (admin)
+               590 LOAD_ATTR               19 (register)
+               600 LOAD_NAME               14 (GroupStyle)
+               602 PRECALL                  1
+               606 CALL                     1
+   
+   129         616 PUSH_NULL
+               618 LOAD_BUILD_CLASS
+               620 LOAD_CONST              17 (<code object GroupStyleModelAdmin, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 128>)
+               622 MAKE_FUNCTION            0
+               624 LOAD_CONST              18 ('GroupStyleModelAdmin')
+               626 LOAD_NAME                1 (admin)
+               628 LOAD_ATTR               20 (ModelAdmin)
+               638 PRECALL                  3
+               642 CALL                     3
+   
+   128         652 PRECALL                  0
+               656 CALL                     0
+   
+   129         666 STORE_NAME              27 (GroupStyleModelAdmin)
+               668 LOAD_CONST              19 (None)
+               670 RETURN_VALUE
    consts
       0
       ('admin',)
       ('mark_safe',)
-      ('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm')
-      ('BoardProfile', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread')
+      ('BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm')
+      ('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a0664035a0764045a
             08640584005a0964065300
-          14           0 RESUME                   0
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfileModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          16          10 LOAD_NAME                3 (BoardProfileAdminModelForm)
+          25          10 LOAD_NAME                3 (BoardProfileAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          17          14 LOAD_CONST               1 (('user',))
+          26          14 LOAD_CONST               1 (('user',))
                       16 STORE_NAME               5 (list_display)
          
-          18          18 LOAD_CONST               2 (('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser'))
+          27          18 LOAD_CONST               2 (('created_at', 'user__is_active', 'user__is_staff', 'user__is_superuser'))
                       20 STORE_NAME               6 (list_filter)
          
-          24          22 LOAD_CONST               3 (('user__username', 'user__email'))
+          33          22 LOAD_CONST               3 (('user__username', 'user__email'))
                       24 STORE_NAME               7 (search_fields)
          
-          28          26 LOAD_CONST               4 (('signature_rendered',))
+          37          26 LOAD_CONST               4 (('signature_rendered',))
                       28 STORE_NAME               8 (readonly_fields)
          
-          30          30 LOAD_CONST               5 (<code object signature_rendered, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 30>)
+          39          30 LOAD_CONST               5 (<code object signature_rendered, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py", line 39>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               9 (signature_rendered)
                       36 LOAD_CONST               6 (None)
                       38 RETURN_VALUE
          consts
             'BoardProfileModelAdmin'
             ('user',)
@@ -258,67 +287,67 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c016a0100000000000000006a0200
                   00000000000000a6010000ab0100000000000000005300
-                30           0 RESUME                   0
+                39           0 RESUME                   0
                
-                31           2 LOAD_GLOBAL              1 (NULL + mark_safe)
+                40           2 LOAD_GLOBAL              1 (NULL + mark_safe)
                             14 LOAD_FAST                1 (obj)
                             16 LOAD_ATTR                1 (signature)
                             26 LOAD_ATTR                2 (rendered)
                             36 PRECALL                  1
                             40 CALL                     1
                             50 RETURN_VALUE
                consts
                   None
                names      ('mark_safe', 'signature', 'rendered')
                varnames   ('self', 'obj')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
                name       'signature_rendered'
-               firstlineno 30
+               firstlineno 39
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'BoardProfileAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields', 'readonly_fields', 'signature_rendered')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'BoardProfileModelAdmin'
-         firstlineno 14
+         firstlineno 23
          lnotab 0x0a0204010401040604040402
       'BoardProfileModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a066403640469015a
             0764055300
-          34           0 RESUME                   0
+          43           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CategoryModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          36          10 LOAD_NAME                3 (CategoryAdminModelForm)
+          45          10 LOAD_NAME                3 (CategoryAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          37          14 LOAD_CONST               1 (('name', 'order'))
+          46          14 LOAD_CONST               1 (('name', 'order'))
                       16 STORE_NAME               5 (list_display)
          
-          41          18 LOAD_CONST               2 (('name', 'description'))
+          50          18 LOAD_CONST               2 (('name', 'description'))
                       20 STORE_NAME               6 (search_fields)
          
-          45          22 LOAD_CONST               3 ('slug')
+          54          22 LOAD_CONST               3 ('slug')
                       24 LOAD_CONST               4 (('name',))
                       26 BUILD_MAP                1
                       28 STORE_NAME               7 (prepopulated_fields)
                       30 LOAD_CONST               5 (None)
                       32 RETURN_VALUE
          consts
             'CategoryModelAdmin'
@@ -329,44 +358,44 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'CategoryAdminModelForm', 'form', 'list_display', 'search_fields', 'prepopulated_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'CategoryModelAdmin'
-         firstlineno 34
+         firstlineno 43
          lnotab 0x0a02040104040404
       'CategoryModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a0664035a07640464
             0569015a0864065300
-          48           0 RESUME                   0
+          57           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SubcategoryModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          50          10 LOAD_NAME                3 (SubcategoryAdminModelForm)
+          59          10 LOAD_NAME                3 (SubcategoryAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          51          14 LOAD_CONST               1 (('name', 'category', 'order'))
+          60          14 LOAD_CONST               1 (('name', 'category', 'order'))
                       16 STORE_NAME               5 (list_display)
          
-          56          18 LOAD_CONST               2 (('category',))
+          65          18 LOAD_CONST               2 (('category',))
                       20 STORE_NAME               6 (list_filter)
          
-          57          22 LOAD_CONST               3 (('name', 'description'))
+          66          22 LOAD_CONST               3 (('name', 'description'))
                       24 STORE_NAME               7 (search_fields)
          
-          61          26 LOAD_CONST               4 ('slug')
+          70          26 LOAD_CONST               4 ('slug')
                       28 LOAD_CONST               5 (('name',))
                       30 BUILD_MAP                1
                       32 STORE_NAME               8 (prepopulated_fields)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'SubcategoryModelAdmin'
@@ -378,41 +407,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'SubcategoryAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields', 'prepopulated_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'SubcategoryModelAdmin'
-         firstlineno 48
+         firstlineno 57
          lnotab 0x0a020401040504010404
       'SubcategoryModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0265035a0464015a0564025a0664035a07640453
             00
-          64           0 RESUME                   0
+          73           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          66          10 LOAD_NAME                3 (ThreadAdminModelForm)
+          75          10 LOAD_NAME                3 (ThreadAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          67          14 LOAD_CONST               1 (('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
+          76          14 LOAD_CONST               1 (('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
                       16 STORE_NAME               5 (list_display)
          
-          76          18 LOAD_CONST               2 (('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
+          85          18 LOAD_CONST               2 (('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed'))
                       20 STORE_NAME               6 (list_filter)
          
-          83          22 LOAD_CONST               3 (('user__username', 'user__email', 'title', 'content'))
+          92          22 LOAD_CONST               3 (('user__username', 'user__email', 'title', 'content'))
                       24 STORE_NAME               7 (search_fields)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'ThreadModelAdmin'
             ('title', 'subcategory', 'user', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed')
             ('subcategory', 'created_at', 'last_post_created_at', 'is_pinned', 'is_closed')
@@ -420,90 +449,127 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'ThreadAdminModelForm', 'form', 'list_display', 'list_filter', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'ThreadModelAdmin'
-         firstlineno 64
+         firstlineno 73
          lnotab 0x0a02040104090407
       'ThreadModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0265035a0464015a0564025a0664035300
-          91           0 RESUME                   0
+         100           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-          93          10 LOAD_NAME                3 (PostAdminModelForm)
+         102          10 LOAD_NAME                3 (PostAdminModelForm)
                       12 STORE_NAME               4 (form)
          
-          94          14 LOAD_CONST               1 (('thread', 'user', 'created_at'))
+         103          14 LOAD_CONST               1 (('thread', 'user', 'created_at'))
                       16 STORE_NAME               5 (list_display)
          
-          99          18 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
+         108          18 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
                       20 STORE_NAME               6 (search_fields)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'PostModelAdmin'
             ('thread', 'user', 'created_at')
             ('user__username', 'user__email', 'content')
             None
          names      ('__name__', '__module__', '__qualname__', 'PostAdminModelForm', 'form', 'list_display', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'PostModelAdmin'
-         firstlineno 91
+         firstlineno 100
          lnotab 0x0a0204010405
       'PostModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a0464035300
-         106           0 RESUME                   0
+         115           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ShoutModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         108          10 LOAD_CONST               1 (('user', 'created_at'))
+         117          10 LOAD_CONST               1 (('user', 'created_at'))
                       12 STORE_NAME               3 (list_display)
          
-         112          14 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
+         121          14 LOAD_CONST               2 (('user__username', 'user__email', 'content'))
                       16 STORE_NAME               4 (search_fields)
                       18 LOAD_CONST               3 (None)
                       20 RETURN_VALUE
          consts
             'ShoutModelAdmin'
             ('user', 'created_at')
             ('user__username', 'user__email', 'content')
             None
          names      ('__name__', '__module__', '__qualname__', 'list_display', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
          name       'ShoutModelAdmin'
-         firstlineno 106
+         firstlineno 115
          lnotab 0x0a020404
       'ShoutModelAdmin'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
+         code 0x970065005a0164005a0265035a0464015a0564025a0664035300
+         128           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('GroupStyleModelAdmin')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         130          10 LOAD_NAME                3 (GroupStyleAdminModelForm)
+                      12 STORE_NAME               4 (form)
+         
+         131          14 LOAD_CONST               1 (('group', 'priority'))
+                      16 STORE_NAME               5 (list_display)
+         
+         135          18 LOAD_CONST               2 (('group__name', 'username_style'))
+                      20 STORE_NAME               6 (search_fields)
+                      22 LOAD_CONST               3 (None)
+                      24 RETURN_VALUE
+         consts
+            'GroupStyleModelAdmin'
+            ('group', 'priority')
+            ('group__name', 'username_style')
+            None
+         names      ('__name__', '__module__', '__qualname__', 'GroupStyleAdminModelForm', 'form', 'list_display', 'search_fields')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
+         name       'GroupStyleModelAdmin'
+         firstlineno 128
+         lnotab 0x0a0204010404
+      'GroupStyleModelAdmin'
       None
-   names      ('django.contrib', 'admin', 'django.utils.safestring', 'mark_safe', 'punkweb_bb.admin_forms', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'register', 'ModelAdmin', 'BoardProfileModelAdmin', 'CategoryModelAdmin', 'SubcategoryModelAdmin', 'ThreadModelAdmin', 'PostModelAdmin', 'ShoutModelAdmin')
+   names      ('django.contrib', 'admin', 'django.utils.safestring', 'mark_safe', 'punkweb_bb.admin_forms', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'GroupStyleAdminModelForm', 'PostAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Shout', 'Subcategory', 'Thread', 'register', 'ModelAdmin', 'BoardProfileModelAdmin', 'CategoryModelAdmin', 'SubcategoryModelAdmin', 'ThreadModelAdmin', 'PostModelAdmin', 'ShoutModelAdmin', 'GroupStyleModelAdmin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c021c0720031e0124ff0e0102131e0124ff0e01020d1e
-      0124ff0e01020f1e0124ff0e01021a1e0124ff0e01020e1e0124ff0e01
+      0x00ff02010c010c022008240b1e0124ff0e0102131e0124ff0e01020d1e
+      0124ff0e01020f1e0124ff0e01021a1e0124ff0e01020e1e0124ff0e0102
+      0c1e0124ff0e01
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,134 +1,148 @@
 magic:    0xa70d0d0a
-moddate:  0x94ab0d66 (Wed Apr  3 19:18:44 2024 UTC)
-files sz: 1128
+moddate:  0xe4865766 (Wed May 29 19:49:56 2024 UTC)
+files sz: 1372
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a066d075a070100640064036c086d095a0901000200470064
-      048400640565016a0a0000000000000000a6030000ab0300000000000000
-      005a0b0200470064068400640765016a0a0000000000000000a6030000ab
-      0300000000000000005a0c0200470064088400640965016a0a0000000000
-      000000a6030000ab0300000000000000005a0d02004700640a8400640b65
-      016a0a0000000000000000a6030000ab0300000000000000005a0e020047
-      00640c8400640d65016a0a0000000000000000a6030000ab030000000000
-      0000005a0f640e5300
+      055a056d065a066d075a076d085a080100640064036c096d0a5a0a010002
+      00470064048400640565016a0b0000000000000000a6030000ab03000000
+      00000000005a0c0200470064068400640765016a0b0000000000000000a6
+      030000ab0300000000000000005a0d0200470064088400640965016a0b00
+      00000000000000a6030000ab0300000000000000005a0e02004700640a84
+      00640b65016a0b0000000000000000a6030000ab0300000000000000005a
+      0f02004700640c8400640d65016a0b0000000000000000a6030000ab0300
+      000000000000005a1002004700640e8400640f65016a0b00000000000000
+      00a6030000ab0300000000000000005a1164105300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('forms',))
                  6 IMPORT_NAME              0 (django)
                  8 IMPORT_FROM              1 (forms)
                 10 STORE_NAME               1 (forms)
                 12 POP_TOP
    
      3          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('BoardProfile', 'Category', 'Post', 'Subcategory', 'Thread'))
+                16 LOAD_CONST               2 (('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Subcategory', 'Thread'))
                 18 IMPORT_NAME              2 (punkweb_bb.models)
                 20 IMPORT_FROM              3 (BoardProfile)
                 22 STORE_NAME               3 (BoardProfile)
                 24 IMPORT_FROM              4 (Category)
                 26 STORE_NAME               4 (Category)
-                28 IMPORT_FROM              5 (Post)
-                30 STORE_NAME               5 (Post)
-                32 IMPORT_FROM              6 (Subcategory)
-                34 STORE_NAME               6 (Subcategory)
-                36 IMPORT_FROM              7 (Thread)
-                38 STORE_NAME               7 (Thread)
-                40 POP_TOP
+                28 IMPORT_FROM              5 (GroupStyle)
+                30 STORE_NAME               5 (GroupStyle)
+                32 IMPORT_FROM              6 (Post)
+                34 STORE_NAME               6 (Post)
+                36 IMPORT_FROM              7 (Subcategory)
+                38 STORE_NAME               7 (Subcategory)
+                40 IMPORT_FROM              8 (Thread)
+                42 STORE_NAME               8 (Thread)
+                44 POP_TOP
    
-     4          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('BBCodeEditorWidget',))
-                46 IMPORT_NAME              8 (punkweb_bb.widgets)
-                48 IMPORT_FROM              9 (BBCodeEditorWidget)
-                50 STORE_NAME               9 (BBCodeEditorWidget)
-                52 POP_TOP
+    11          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               3 (('BBCodeEditorWidget',))
+                50 IMPORT_NAME              9 (punkweb_bb.widgets)
+                52 IMPORT_FROM             10 (BBCodeEditorWidget)
+                54 STORE_NAME              10 (BBCodeEditorWidget)
+                56 POP_TOP
    
-     7          54 PUSH_NULL
-                56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               4 (<code object BoardProfileAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 7>)
-                60 MAKE_FUNCTION            0
-                62 LOAD_CONST               5 ('BoardProfileAdminModelForm')
-                64 LOAD_NAME                1 (forms)
-                66 LOAD_ATTR               10 (ModelForm)
-                76 PRECALL                  3
-                80 CALL                     3
-                90 STORE_NAME              11 (BoardProfileAdminModelForm)
+    14          58 PUSH_NULL
+                60 LOAD_BUILD_CLASS
+                62 LOAD_CONST               4 (<code object BoardProfileAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 14>)
+                64 MAKE_FUNCTION            0
+                66 LOAD_CONST               5 ('BoardProfileAdminModelForm')
+                68 LOAD_NAME                1 (forms)
+                70 LOAD_ATTR               11 (ModelForm)
+                80 PRECALL                  3
+                84 CALL                     3
+                94 STORE_NAME              12 (BoardProfileAdminModelForm)
    
-    16          92 PUSH_NULL
-                94 LOAD_BUILD_CLASS
-                96 LOAD_CONST               6 (<code object CategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 16>)
-                98 MAKE_FUNCTION            0
-               100 LOAD_CONST               7 ('CategoryAdminModelForm')
-               102 LOAD_NAME                1 (forms)
-               104 LOAD_ATTR               10 (ModelForm)
-               114 PRECALL                  3
-               118 CALL                     3
-               128 STORE_NAME              12 (CategoryAdminModelForm)
+    23          96 PUSH_NULL
+                98 LOAD_BUILD_CLASS
+               100 LOAD_CONST               6 (<code object CategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 23>)
+               102 MAKE_FUNCTION            0
+               104 LOAD_CONST               7 ('CategoryAdminModelForm')
+               106 LOAD_NAME                1 (forms)
+               108 LOAD_ATTR               11 (ModelForm)
+               118 PRECALL                  3
+               122 CALL                     3
+               132 STORE_NAME              13 (CategoryAdminModelForm)
    
-    25         130 PUSH_NULL
-               132 LOAD_BUILD_CLASS
-               134 LOAD_CONST               8 (<code object SubcategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 25>)
-               136 MAKE_FUNCTION            0
-               138 LOAD_CONST               9 ('SubcategoryAdminModelForm')
-               140 LOAD_NAME                1 (forms)
-               142 LOAD_ATTR               10 (ModelForm)
-               152 PRECALL                  3
-               156 CALL                     3
-               166 STORE_NAME              13 (SubcategoryAdminModelForm)
+    32         134 PUSH_NULL
+               136 LOAD_BUILD_CLASS
+               138 LOAD_CONST               8 (<code object SubcategoryAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 32>)
+               140 MAKE_FUNCTION            0
+               142 LOAD_CONST               9 ('SubcategoryAdminModelForm')
+               144 LOAD_NAME                1 (forms)
+               146 LOAD_ATTR               11 (ModelForm)
+               156 PRECALL                  3
+               160 CALL                     3
+               170 STORE_NAME              14 (SubcategoryAdminModelForm)
    
-    34         168 PUSH_NULL
-               170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              10 (<code object ThreadAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 34>)
-               174 MAKE_FUNCTION            0
-               176 LOAD_CONST              11 ('ThreadAdminModelForm')
-               178 LOAD_NAME                1 (forms)
-               180 LOAD_ATTR               10 (ModelForm)
-               190 PRECALL                  3
-               194 CALL                     3
-               204 STORE_NAME              14 (ThreadAdminModelForm)
+    41         172 PUSH_NULL
+               174 LOAD_BUILD_CLASS
+               176 LOAD_CONST              10 (<code object ThreadAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 41>)
+               178 MAKE_FUNCTION            0
+               180 LOAD_CONST              11 ('ThreadAdminModelForm')
+               182 LOAD_NAME                1 (forms)
+               184 LOAD_ATTR               11 (ModelForm)
+               194 PRECALL                  3
+               198 CALL                     3
+               208 STORE_NAME              15 (ThreadAdminModelForm)
    
-    43         206 PUSH_NULL
-               208 LOAD_BUILD_CLASS
-               210 LOAD_CONST              12 (<code object PostAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 43>)
-               212 MAKE_FUNCTION            0
-               214 LOAD_CONST              13 ('PostAdminModelForm')
-               216 LOAD_NAME                1 (forms)
-               218 LOAD_ATTR               10 (ModelForm)
-               228 PRECALL                  3
-               232 CALL                     3
-               242 STORE_NAME              15 (PostAdminModelForm)
-               244 LOAD_CONST              14 (None)
-               246 RETURN_VALUE
+    50         210 PUSH_NULL
+               212 LOAD_BUILD_CLASS
+               214 LOAD_CONST              12 (<code object PostAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 50>)
+               216 MAKE_FUNCTION            0
+               218 LOAD_CONST              13 ('PostAdminModelForm')
+               220 LOAD_NAME                1 (forms)
+               222 LOAD_ATTR               11 (ModelForm)
+               232 PRECALL                  3
+               236 CALL                     3
+               246 STORE_NAME              16 (PostAdminModelForm)
+   
+    59         248 PUSH_NULL
+               250 LOAD_BUILD_CLASS
+               252 LOAD_CONST              14 (<code object GroupStyleAdminModelForm, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 59>)
+               254 MAKE_FUNCTION            0
+               256 LOAD_CONST              15 ('GroupStyleAdminModelForm')
+               258 LOAD_NAME                1 (forms)
+               260 LOAD_ATTR               11 (ModelForm)
+               270 PRECALL                  3
+               274 CALL                     3
+               284 STORE_NAME              17 (GroupStyleAdminModelForm)
+               286 LOAD_CONST              16 (None)
+               288 RETURN_VALUE
    consts
       0
       ('forms',)
-      ('BoardProfile', 'Category', 'Post', 'Subcategory', 'Thread')
+      ('BoardProfile', 'Category', 'GroupStyle', 'Post', 'Subcategory', 'Thread')
       ('BBCodeEditorWidget',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-           7           0 RESUME                   0
+          14           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfileAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-           8          10 PUSH_NULL
+          15          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 8>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 15>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -138,77 +152,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                 8           0 RESUME                   0
+                15           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BoardProfileAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                 9          10 LOAD_NAME                3 (BoardProfile)
+                16          10 LOAD_NAME                3 (BoardProfile)
                             12 STORE_NAME               4 (model)
                
-                10          14 LOAD_CONST               1 ('__all__')
+                17          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                12          18 LOAD_CONST               2 ('signature')
+                19          18 LOAD_CONST               2 ('signature')
                             20 PUSH_NULL
                             22 LOAD_NAME                6 (BBCodeEditorWidget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                11          38 BUILD_MAP                1
+                18          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'BoardProfileAdminModelForm.Meta'
                   '__all__'
                   'signature'
                   None
                names      ('__name__', '__module__', '__qualname__', 'BoardProfile', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 8
+               firstlineno 15
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'BoardProfileAdminModelForm'
-         firstlineno 7
+         firstlineno 14
          lnotab 0x0a01
       'BoardProfileAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          16           0 RESUME                   0
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CategoryAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          17          10 PUSH_NULL
+          24          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 17>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 24>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -218,77 +232,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                17           0 RESUME                   0
+                24           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('CategoryAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                18          10 LOAD_NAME                3 (Category)
+                25          10 LOAD_NAME                3 (Category)
                             12 STORE_NAME               4 (model)
                
-                19          14 LOAD_CONST               1 ('__all__')
+                26          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                21          18 LOAD_CONST               2 ('description')
+                28          18 LOAD_CONST               2 ('description')
                             20 PUSH_NULL
                             22 LOAD_NAME                6 (BBCodeEditorWidget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                20          38 BUILD_MAP                1
+                27          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'CategoryAdminModelForm.Meta'
                   '__all__'
                   'description'
                   None
                names      ('__name__', '__module__', '__qualname__', 'Category', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 17
+               firstlineno 24
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'CategoryAdminModelForm'
-         firstlineno 16
+         firstlineno 23
          lnotab 0x0a01
       'CategoryAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          25           0 RESUME                   0
+          32           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SubcategoryAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          26          10 PUSH_NULL
+          33          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 26>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 33>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -298,77 +312,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                26           0 RESUME                   0
+                33           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('SubcategoryAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                27          10 LOAD_NAME                3 (Subcategory)
+                34          10 LOAD_NAME                3 (Subcategory)
                             12 STORE_NAME               4 (model)
                
-                28          14 LOAD_CONST               1 ('__all__')
+                35          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                30          18 LOAD_CONST               2 ('description')
+                37          18 LOAD_CONST               2 ('description')
                             20 PUSH_NULL
                             22 LOAD_NAME                6 (BBCodeEditorWidget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                29          38 BUILD_MAP                1
+                36          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'SubcategoryAdminModelForm.Meta'
                   '__all__'
                   'description'
                   None
                names      ('__name__', '__module__', '__qualname__', 'Subcategory', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 26
+               firstlineno 33
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'SubcategoryAdminModelForm'
-         firstlineno 25
+         firstlineno 32
          lnotab 0x0a01
       'SubcategoryAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          34           0 RESUME                   0
+          41           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          35          10 PUSH_NULL
+          42          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 35>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 42>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -378,77 +392,77 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                35           0 RESUME                   0
+                42           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('ThreadAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                36          10 LOAD_NAME                3 (Thread)
+                43          10 LOAD_NAME                3 (Thread)
                             12 STORE_NAME               4 (model)
                
-                37          14 LOAD_CONST               1 ('__all__')
+                44          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                39          18 LOAD_CONST               2 ('content')
+                46          18 LOAD_CONST               2 ('content')
                             20 PUSH_NULL
                             22 LOAD_NAME                6 (BBCodeEditorWidget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                38          38 BUILD_MAP                1
+                45          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'ThreadAdminModelForm.Meta'
                   '__all__'
                   'content'
                   None
                names      ('__name__', '__module__', '__qualname__', 'Thread', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 35
+               firstlineno 42
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'ThreadAdminModelForm'
-         firstlineno 34
+         firstlineno 41
          lnotab 0x0a01
       'ThreadAdminModelForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0202004700640184006402a6020000ab02000000
             00000000005a0364035300
-          43           0 RESUME                   0
+          50           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostAdminModelForm')
                        8 STORE_NAME               2 (__qualname__)
          
-          44          10 PUSH_NULL
+          51          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 44>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 51>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -458,62 +472,142 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
                   00000000000000000069015a0764035300
-                44           0 RESUME                   0
+                51           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('PostAdminModelForm.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                45          10 LOAD_NAME                3 (Post)
+                52          10 LOAD_NAME                3 (Post)
                             12 STORE_NAME               4 (model)
                
-                46          14 LOAD_CONST               1 ('__all__')
+                53          14 LOAD_CONST               1 ('__all__')
                             16 STORE_NAME               5 (fields)
                
-                48          18 LOAD_CONST               2 ('content')
+                55          18 LOAD_CONST               2 ('content')
                             20 PUSH_NULL
                             22 LOAD_NAME                6 (BBCodeEditorWidget)
                             24 PRECALL                  0
                             28 CALL                     0
                
-                47          38 BUILD_MAP                1
+                54          38 BUILD_MAP                1
                             40 STORE_NAME               7 (widgets)
                             42 LOAD_CONST               3 (None)
                             44 RETURN_VALUE
                consts
                   'PostAdminModelForm.Meta'
                   '__all__'
                   'content'
                   None
                names      ('__name__', '__module__', '__qualname__', 'Post', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
                name       'Meta'
-               firstlineno 44
+               firstlineno 51
                lnotab 0x0a010401040214ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
          name       'PostAdminModelForm'
-         firstlineno 43
+         firstlineno 50
          lnotab 0x0a01
       'PostAdminModelForm'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 4
+         flags     : 0
+         code
+            0x970065005a0164005a0202004700640184006402a6020000ab02000000
+            00000000005a0364035300
+          59           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('GroupStyleAdminModelForm')
+                       8 STORE_NAME               2 (__qualname__)
+         
+          60          10 PUSH_NULL
+                      12 LOAD_BUILD_CLASS
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py", line 60>)
+                      16 MAKE_FUNCTION            0
+                      18 LOAD_CONST               2 ('Meta')
+                      20 PRECALL                  2
+                      24 CALL                     2
+                      34 STORE_NAME               3 (Meta)
+                      36 LOAD_CONST               3 (None)
+                      38 RETURN_VALUE
+         consts
+            'GroupStyleAdminModelForm'
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 3
+               flags     : 0
+               code
+                  0x970065005a0164005a0265035a0464015a05640202006506a6000000ab
+                  00000000000000000069015a0764035300
+                60           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('GroupStyleAdminModelForm.Meta')
+                             8 STORE_NAME               2 (__qualname__)
+               
+                61          10 LOAD_NAME                3 (GroupStyle)
+                            12 STORE_NAME               4 (model)
+               
+                62          14 LOAD_CONST               1 ('__all__')
+                            16 STORE_NAME               5 (fields)
+               
+                64          18 LOAD_CONST               2 ('username_style')
+                            20 PUSH_NULL
+                            22 LOAD_NAME                6 (BBCodeEditorWidget)
+                            24 PRECALL                  0
+                            28 CALL                     0
+               
+                63          38 BUILD_MAP                1
+                            40 STORE_NAME               7 (widgets)
+                            42 LOAD_CONST               3 (None)
+                            44 RETURN_VALUE
+               consts
+                  'GroupStyleAdminModelForm.Meta'
+                  '__all__'
+                  'username_style'
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'GroupStyle', 'model', 'fields', 'BBCodeEditorWidget', 'widgets')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
+               name       'Meta'
+               firstlineno 60
+               lnotab 0x0a010401040214ff
+            'Meta'
+            None
+         names      ('__name__', '__module__', '__qualname__', 'Meta')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
+         name       'GroupStyleAdminModelForm'
+         firstlineno 59
+         lnotab 0x0a01
+      'GroupStyleAdminModelForm'
       None
-   names      ('django', 'forms', 'punkweb_bb.models', 'BoardProfile', 'Category', 'Post', 'Subcategory', 'Thread', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'ModelForm', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'PostAdminModelForm')
+   names      ('django', 'forms', 'punkweb_bb.models', 'BoardProfile', 'Category', 'GroupStyle', 'Post', 'Subcategory', 'Thread', 'punkweb_bb.widgets', 'BBCodeEditorWidget', 'ModelForm', 'BoardProfileAdminModelForm', 'CategoryAdminModelForm', 'SubcategoryAdminModelForm', 'ThreadAdminModelForm', 'PostAdminModelForm', 'GroupStyleAdminModelForm')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/admin_forms.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021c010c032609260926092609
+   lnotab 0x00ff02010c0220080c0326092609260926092609
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/guests.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/guests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,28 +1,30 @@
 magic:    0xa70d0d0a
-moddate:  0xb17e5666 (Wed May 29 01:02:41 2024 UTC)
-files sz: 6348
+moddate:  0x958d5766 (Wed May 29 20:18:29 2024 UTC)
+files sz: 6962
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       026c036d045a040100640064036c056d065a060100640064046c076d085a
       080100640064056c096d0a5a0a0100640064066c0b6d0c5a0c0100640064
       076c0d6d0e5a0e0100640064086c0f6d105a100100640064096c116d125a
-      126d135a13010002006504a6000000ab0000000000000000005a14640a84
-      005a1502004700640b8400640c65136512a6040000ab0400000000000000
-      005a1602004700640d8400640e65136512a6040000ab0400000000000000
-      005a1702004700640f8400641065136512a6040000ab0400000000000000
-      005a180200470064118400641265136512a6040000ab0400000000000000
-      005a190200470064138400641465136512a6040000ab0400000000000000
-      005a1a0200470064158400641665136512a6040000ab0400000000000000
-      005a1b64015300
+      1201006400640a6c136d145a146d155a1501006400640b6c166d175a1701
+      0002006504a6000000ab0000000000000000005a18640c84005a19020047
+      00640d8400640e65156514a6040000ab0400000000000000005a1a020047
+      00640f8400641065156514a6040000ab0400000000000000005a1b020047
+      0064118400641265156514a6040000ab0400000000000000005a1c020047
+      0064138400641465156514a6040000ab0400000000000000005a1d020047
+      0064158400641665156514a6040000ab0400000000000000005a1e020047
+      0064178400641865156514a6040000ab0400000000000000005a1f020047
+      0064198400641a65156514a6040000ab0400000000000000005a20640153
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (datetime)
                  8 STORE_NAME               0 (datetime)
    
@@ -40,175 +42,202 @@
                 28 LOAD_CONST               2 (('get_user_model',))
                 30 IMPORT_NAME              3 (django.contrib.auth)
                 32 IMPORT_FROM              4 (get_user_model)
                 34 STORE_NAME               4 (get_user_model)
                 36 POP_TOP
    
      6          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('cache',))
-                42 IMPORT_NAME              5 (django.core.cache)
-                44 IMPORT_FROM              6 (cache)
-                46 STORE_NAME               6 (cache)
+                40 LOAD_CONST               3 (('Group',))
+                42 IMPORT_NAME              5 (django.contrib.auth.models)
+                44 IMPORT_FROM              6 (Group)
+                46 STORE_NAME               6 (Group)
                 48 POP_TOP
    
      7          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('models',))
-                54 IMPORT_NAME              7 (django.db)
-                56 IMPORT_FROM              8 (models)
-                58 STORE_NAME               8 (models)
+                52 LOAD_CONST               4 (('cache',))
+                54 IMPORT_NAME              7 (django.core.cache)
+                56 IMPORT_FROM              8 (cache)
+                58 STORE_NAME               8 (cache)
                 60 POP_TOP
    
      8          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('ValidationError',))
-                66 IMPORT_NAME              9 (django.forms)
-                68 IMPORT_FROM             10 (ValidationError)
-                70 STORE_NAME              10 (ValidationError)
+                64 LOAD_CONST               5 (('models',))
+                66 IMPORT_NAME              9 (django.db)
+                68 IMPORT_FROM             10 (models)
+                70 STORE_NAME              10 (models)
                 72 POP_TOP
    
      9          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               6 (('reverse',))
-                78 IMPORT_NAME             11 (django.urls)
-                80 IMPORT_FROM             12 (reverse)
-                82 STORE_NAME              12 (reverse)
+                76 LOAD_CONST               6 (('ValidationError',))
+                78 IMPORT_NAME             11 (django.forms)
+                80 IMPORT_FROM             12 (ValidationError)
+                82 STORE_NAME              12 (ValidationError)
                 84 POP_TOP
    
     10          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('timezone',))
-                90 IMPORT_NAME             13 (django.utils)
-                92 IMPORT_FROM             14 (timezone)
-                94 STORE_NAME              14 (timezone)
+                88 LOAD_CONST               7 (('reverse',))
+                90 IMPORT_NAME             13 (django.urls)
+                92 IMPORT_FROM             14 (reverse)
+                94 STORE_NAME              14 (reverse)
                 96 POP_TOP
    
     11          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               8 (('BBCodeTextField',))
-               102 IMPORT_NAME             15 (precise_bbcode.fields)
-               104 IMPORT_FROM             16 (BBCodeTextField)
-               106 STORE_NAME              16 (BBCodeTextField)
+               100 LOAD_CONST               8 (('timezone',))
+               102 IMPORT_NAME             15 (django.utils)
+               104 IMPORT_FROM             16 (timezone)
+               106 STORE_NAME              16 (timezone)
                108 POP_TOP
    
-    13         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               9 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
-               114 IMPORT_NAME             17 (punkweb_bb.mixins)
-               116 IMPORT_FROM             18 (TimestampMixin)
-               118 STORE_NAME              18 (TimestampMixin)
-               120 IMPORT_FROM             19 (UUIDPrimaryKeyMixin)
-               122 STORE_NAME              19 (UUIDPrimaryKeyMixin)
-               124 POP_TOP
-   
-    15         126 PUSH_NULL
-               128 LOAD_NAME                4 (get_user_model)
-               130 PRECALL                  0
-               134 CALL                     0
-               144 STORE_NAME              20 (User)
-   
-    18         146 LOAD_CONST              10 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 18>)
-               148 MAKE_FUNCTION            0
-               150 STORE_NAME              21 (profile_image_upload_to)
-   
-    23         152 PUSH_NULL
-               154 LOAD_BUILD_CLASS
-               156 LOAD_CONST              11 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 23>)
-               158 MAKE_FUNCTION            0
-               160 LOAD_CONST              12 ('BoardProfile')
-               162 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
-               164 LOAD_NAME               18 (TimestampMixin)
-               166 PRECALL                  4
-               170 CALL                     4
-               180 STORE_NAME              22 (BoardProfile)
-   
-    46         182 PUSH_NULL
-               184 LOAD_BUILD_CLASS
-               186 LOAD_CONST              13 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 46>)
-               188 MAKE_FUNCTION            0
-               190 LOAD_CONST              14 ('Category')
-               192 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
-               194 LOAD_NAME               18 (TimestampMixin)
-               196 PRECALL                  4
-               200 CALL                     4
-               210 STORE_NAME              23 (Category)
-   
-    64         212 PUSH_NULL
-               214 LOAD_BUILD_CLASS
-               216 LOAD_CONST              15 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 64>)
-               218 MAKE_FUNCTION            0
-               220 LOAD_CONST              16 ('Subcategory')
-               222 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
-               224 LOAD_NAME               18 (TimestampMixin)
-               226 PRECALL                  4
-               230 CALL                     4
-               240 STORE_NAME              24 (Subcategory)
-   
-   104         242 PUSH_NULL
-               244 LOAD_BUILD_CLASS
-               246 LOAD_CONST              17 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 104>)
-               248 MAKE_FUNCTION            0
-               250 LOAD_CONST              18 ('Thread')
-               252 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
-               254 LOAD_NAME               18 (TimestampMixin)
-               256 PRECALL                  4
-               260 CALL                     4
-               270 STORE_NAME              25 (Thread)
-   
-   151         272 PUSH_NULL
-               274 LOAD_BUILD_CLASS
-               276 LOAD_CONST              19 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 151>)
-               278 MAKE_FUNCTION            0
-               280 LOAD_CONST              20 ('Post')
-               282 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
-               284 LOAD_NAME               18 (TimestampMixin)
-               286 PRECALL                  4
-               290 CALL                     4
-               300 STORE_NAME              26 (Post)
-   
-   196         302 PUSH_NULL
-               304 LOAD_BUILD_CLASS
-               306 LOAD_CONST              21 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
-               308 MAKE_FUNCTION            0
-               310 LOAD_CONST              22 ('Shout')
-               312 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
-               314 LOAD_NAME               18 (TimestampMixin)
-               316 PRECALL                  4
-               320 CALL                     4
-               330 STORE_NAME              27 (Shout)
-               332 LOAD_CONST               1 (None)
-               334 RETURN_VALUE
+    12         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               9 (('BBCodeTextField',))
+               114 IMPORT_NAME             17 (precise_bbcode.fields)
+               116 IMPORT_FROM             18 (BBCodeTextField)
+               118 STORE_NAME              18 (BBCodeTextField)
+               120 POP_TOP
+   
+    14         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST              10 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
+               126 IMPORT_NAME             19 (punkweb_bb.mixins)
+               128 IMPORT_FROM             20 (TimestampMixin)
+               130 STORE_NAME              20 (TimestampMixin)
+               132 IMPORT_FROM             21 (UUIDPrimaryKeyMixin)
+               134 STORE_NAME              21 (UUIDPrimaryKeyMixin)
+               136 POP_TOP
+   
+    15         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST              11 (('get_styled_username',))
+               142 IMPORT_NAME             22 (punkweb_bb.utils)
+               144 IMPORT_FROM             23 (get_styled_username)
+               146 STORE_NAME              23 (get_styled_username)
+               148 POP_TOP
+   
+    17         150 PUSH_NULL
+               152 LOAD_NAME                4 (get_user_model)
+               154 PRECALL                  0
+               158 CALL                     0
+               168 STORE_NAME              24 (User)
+   
+    20         170 LOAD_CONST              12 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 20>)
+               172 MAKE_FUNCTION            0
+               174 STORE_NAME              25 (profile_image_upload_to)
+   
+    25         176 PUSH_NULL
+               178 LOAD_BUILD_CLASS
+               180 LOAD_CONST              13 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 25>)
+               182 MAKE_FUNCTION            0
+               184 LOAD_CONST              14 ('BoardProfile')
+               186 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               188 LOAD_NAME               20 (TimestampMixin)
+               190 PRECALL                  4
+               194 CALL                     4
+               204 STORE_NAME              26 (BoardProfile)
+   
+    52         206 PUSH_NULL
+               208 LOAD_BUILD_CLASS
+               210 LOAD_CONST              15 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 52>)
+               212 MAKE_FUNCTION            0
+               214 LOAD_CONST              16 ('Category')
+               216 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               218 LOAD_NAME               20 (TimestampMixin)
+               220 PRECALL                  4
+               224 CALL                     4
+               234 STORE_NAME              27 (Category)
+   
+    70         236 PUSH_NULL
+               238 LOAD_BUILD_CLASS
+               240 LOAD_CONST              17 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 70>)
+               242 MAKE_FUNCTION            0
+               244 LOAD_CONST              18 ('Subcategory')
+               246 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               248 LOAD_NAME               20 (TimestampMixin)
+               250 PRECALL                  4
+               254 CALL                     4
+               264 STORE_NAME              28 (Subcategory)
+   
+   110         266 PUSH_NULL
+               268 LOAD_BUILD_CLASS
+               270 LOAD_CONST              19 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 110>)
+               272 MAKE_FUNCTION            0
+               274 LOAD_CONST              20 ('Thread')
+               276 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               278 LOAD_NAME               20 (TimestampMixin)
+               280 PRECALL                  4
+               284 CALL                     4
+               294 STORE_NAME              29 (Thread)
+   
+   157         296 PUSH_NULL
+               298 LOAD_BUILD_CLASS
+               300 LOAD_CONST              21 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 157>)
+               302 MAKE_FUNCTION            0
+               304 LOAD_CONST              22 ('Post')
+               306 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               308 LOAD_NAME               20 (TimestampMixin)
+               310 PRECALL                  4
+               314 CALL                     4
+               324 STORE_NAME              30 (Post)
+   
+   202         326 PUSH_NULL
+               328 LOAD_BUILD_CLASS
+               330 LOAD_CONST              23 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 202>)
+               332 MAKE_FUNCTION            0
+               334 LOAD_CONST              24 ('Shout')
+               336 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               338 LOAD_NAME               20 (TimestampMixin)
+               340 PRECALL                  4
+               344 CALL                     4
+               354 STORE_NAME              31 (Shout)
+   
+   216         356 PUSH_NULL
+               358 LOAD_BUILD_CLASS
+               360 LOAD_CONST              25 (<code object GroupStyle, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 216>)
+               362 MAKE_FUNCTION            0
+               364 LOAD_CONST              26 ('GroupStyle')
+               366 LOAD_NAME               21 (UUIDPrimaryKeyMixin)
+               368 LOAD_NAME               20 (TimestampMixin)
+               370 PRECALL                  4
+               374 CALL                     4
+               384 STORE_NAME              32 (GroupStyle)
+               386 LOAD_CONST               1 (None)
+               388 RETURN_VALUE
    consts
       0
       None
       ('get_user_model',)
+      ('Group',)
       ('cache',)
       ('models',)
       ('ValidationError',)
       ('reverse',)
       ('timezone',)
       ('BBCodeTextField',)
       ('TimestampMixin', 'UUIDPrimaryKeyMixin')
+      ('get_styled_username',)
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c01a6010000ab010000000000
             0000006401190000000000000000007d0264027c006a0300000000000000
             006a0400000000000000009b0064037c029b009d045300
-          18           0 RESUME                   0
+          20           0 RESUME                   0
          
-          19           2 LOAD_GLOBAL              0 (os)
+          21           2 LOAD_GLOBAL              0 (os)
                       14 LOAD_ATTR                1 (path)
                       24 LOAD_METHOD              2 (splitext)
                       46 LOAD_FAST                1 (filename)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_CONST               1 (-1)
                       64 BINARY_SUBSCR
                       74 STORE_FAST               2 (ext)
          
-          20          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
+          22          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
                       78 LOAD_FAST                0 (instance)
                       80 LOAD_ATTR                3 (user)
                       90 LOAD_ATTR                4 (username)
                      100 FORMAT_VALUE             0
                      102 LOAD_CONST               3 ('/image')
                      104 LOAD_FAST                2 (ext)
                      106 FORMAT_VALUE             0
@@ -221,212 +250,249 @@
             '/image'
          names      ('os', 'path', 'splitext', 'user', 'username')
          varnames   ('instance', 'filename', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'profile_image_upload_to'
-         firstlineno 18
+         firstlineno 20
          lnotab 0x02014a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000650964036403ac04a6030000ab03000000
             00000000005a0a0200650b640564036403ac06a6030000ab030000000000
             0000005a0c02004700640784006408a6020000ab0200000000000000005a
             0d650e64098400a6000000ab0000000000000000005a0f650e640a8400a6
-            000000ab0000000000000000005a10640b84005a11640c5300
-          23           0 RESUME                   0
+            000000ab0000000000000000005a10650e640b8400a6000000ab00000000
+            00000000005a11640c84005a12640d5300
+          25           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfile')
                        8 STORE_NAME               2 (__qualname__)
          
-          24          10 PUSH_NULL
+          26          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (OneToOneField)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('profile')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-          25          58 PUSH_NULL
+          27          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (ImageField)
                       72 LOAD_NAME                9 (profile_image_upload_to)
                       74 LOAD_CONST               3 (True)
                       76 LOAD_CONST               3 (True)
                       78 KW_NAMES                 4
                       80 PRECALL                  3
                       84 CALL                     3
                       94 STORE_NAME              10 (image)
          
-          26          96 PUSH_NULL
+          28          96 PUSH_NULL
                       98 LOAD_NAME               11 (BBCodeTextField)
                      100 LOAD_CONST               5 (1024)
                      102 LOAD_CONST               3 (True)
                      104 LOAD_CONST               3 (True)
                      106 KW_NAMES                 6
                      108 PRECALL                  3
                      112 CALL                     3
                      122 STORE_NAME              12 (signature)
          
-          28         124 PUSH_NULL
+          30         124 PUSH_NULL
                      126 LOAD_BUILD_CLASS
-                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 28>)
+                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 30>)
                      130 MAKE_FUNCTION            0
                      132 LOAD_CONST               8 ('Meta')
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_NAME              13 (Meta)
          
-          31         150 LOAD_NAME               14 (property)
+          33         150 LOAD_NAME               14 (property)
          
-          32         152 LOAD_CONST               9 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 31>)
+          34         152 LOAD_CONST               9 (<code object styled_username, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 33>)
                      154 MAKE_FUNCTION            0
          
-          31         156 PRECALL                  0
+          33         156 PRECALL                  0
                      160 CALL                     0
          
-          32         170 STORE_NAME              15 (is_online)
+          34         170 STORE_NAME              15 (styled_username)
          
-          38         172 LOAD_NAME               14 (property)
+          37         172 LOAD_NAME               14 (property)
          
-          39         174 LOAD_CONST              10 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 38>)
+          38         174 LOAD_CONST              10 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 37>)
                      176 MAKE_FUNCTION            0
          
-          38         178 PRECALL                  0
+          37         178 PRECALL                  0
                      182 CALL                     0
          
-          39         192 STORE_NAME              16 (post_count)
+          38         192 STORE_NAME              16 (is_online)
+         
+          44         194 LOAD_NAME               14 (property)
          
-          42         194 LOAD_CONST              11 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 42>)
-                     196 MAKE_FUNCTION            0
-                     198 STORE_NAME              17 (__str__)
-                     200 LOAD_CONST              12 (None)
-                     202 RETURN_VALUE
+          45         196 LOAD_CONST              11 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 44>)
+                     198 MAKE_FUNCTION            0
+         
+          44         200 PRECALL                  0
+                     204 CALL                     0
+         
+          45         214 STORE_NAME              17 (post_count)
+         
+          48         216 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 48>)
+                     218 MAKE_FUNCTION            0
+                     220 STORE_NAME              18 (__str__)
+                     222 LOAD_CONST              13 (None)
+                     224 RETURN_VALUE
          consts
             'BoardProfile'
             'profile'
             ('related_name', 'on_delete')
             True
             ('upload_to', 'blank', 'null')
             1024
             ('max_length', 'blank', 'null')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-                28           0 RESUME                   0
+                30           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BoardProfile.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                29          10 LOAD_CONST               1 (('user__username',))
+                31          10 LOAD_CONST               1 (('user__username',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'BoardProfile.Meta'
                   ('user__username',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 28
+               firstlineno 30
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c006a010000000000000000a60100
+                  00ab0100000000000000005300
+                33           0 RESUME                   0
+               
+                35           2 LOAD_GLOBAL              1 (NULL + get_styled_username)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (user)
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 RETURN_VALUE
+               consts
+                  None
+               names      ('get_styled_username', 'user')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'styled_username'
+               firstlineno 33
+               lnotab 0x0202
+            code
+               argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c006a
                   0200000000000000009b009d02a6010000ab0100000000000000007d017c
                   01722d7407000000000000000000006a040000000000000000a6000000ab
                   0000000000000000007c01740b000000000000000000006a060000000000
                   0000006402ac03a6010000ab0100000000000000007a0000006b00000000
                   00530064045300
-                31           0 RESUME                   0
+                37           0 RESUME                   0
                
-                33           2 LOAD_GLOBAL              1 (NULL + cache)
+                39           2 LOAD_GLOBAL              1 (NULL + cache)
                             14 LOAD_ATTR                1 (get)
                             24 LOAD_CONST               1 ('profile_online_')
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (id)
                             38 FORMAT_VALUE             0
                             40 BUILD_STRING             2
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               1 (last_seen)
                
-                34          58 LOAD_FAST                1 (last_seen)
+                40          58 LOAD_FAST                1 (last_seen)
                             60 POP_JUMP_FORWARD_IF_FALSE    45 (to 152)
                
-                35          62 LOAD_GLOBAL              7 (NULL + timezone)
+                41          62 LOAD_GLOBAL              7 (NULL + timezone)
                             74 LOAD_ATTR                4 (now)
                             84 PRECALL                  0
                             88 CALL                     0
                             98 LOAD_FAST                1 (last_seen)
                            100 LOAD_GLOBAL             11 (NULL + datetime)
                            112 LOAD_ATTR                6 (timedelta)
                            122 LOAD_CONST               2 (5)
                            124 KW_NAMES                 3
                            126 PRECALL                  1
                            130 CALL                     1
                            140 BINARY_OP                0 (+)
                            144 COMPARE_OP               0 (<)
                            150 RETURN_VALUE
                
-                36     >>  152 LOAD_CONST               4 (False)
+                42     >>  152 LOAD_CONST               4 (False)
                            154 RETURN_VALUE
                consts
                   None
                   'profile_online_'
                   5
                   ('minutes',)
                   False
                names      ('cache', 'get', 'id', 'timezone', 'now', 'datetime', 'timedelta')
                varnames   ('self', 'last_seen')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'is_online'
-               firstlineno 31
+               firstlineno 37
                lnotab 0x0202380104015a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   007c006a0000000000000000006a030000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab0000000000000000007a
                   0000005300
-                38           0 RESUME                   0
+                44           0 RESUME                   0
                
-                40           2 LOAD_FAST                0 (self)
+                46           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (threads)
                             24 LOAD_METHOD              2 (count)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                0 (user)
@@ -440,108 +506,110 @@
                   None
                names      ('user', 'threads', 'count', 'posts')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 38
+               firstlineno 44
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                42           0 RESUME                   0
+                48           0 RESUME                   0
                
-                43           2 LOAD_FAST                0 (self)
+                49           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (username)
                             24 RETURN_VALUE
                consts
                   None
                names      ('user', 'username')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 42
+               firstlineno 48
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'BBCodeTextField', 'signature', 'Meta', 'property', 'is_online', 'post_count', '__str__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'BBCodeTextField', 'signature', 'Meta', 'property', 'styled_username', 'is_online', 'post_count', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'BoardProfile'
-         firstlineno 23
-         lnotab 0x0a01300126011c021a03020104ff0e010206020104ff0e010203
+         firstlineno 25
+         lnotab
+            0x0a01300126011c021a03020104ff0e010203020104ff0e010206020104
+            ff0e010203
       'BoardProfile'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006401ac02a6
             010000ab0100000000000000005a05020065036a06000000000000000064
             036404ac05a6020000ab0200000000000000005a07020065036a08000000
             00000000006406ac07a6010000ab0100000000000000005a090200470064
             0884006409a6020000ab0200000000000000005a0a640a84005a0b640b84
             005a0c640c5300
-          46           0 RESUME                   0
+          52           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Category')
                        8 STORE_NAME               2 (__qualname__)
          
-          47          10 PUSH_NULL
+          53          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (255)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_NAME               5 (name)
          
-          48          44 PUSH_NULL
+          54          44 PUSH_NULL
                       46 LOAD_NAME                3 (models)
                       48 LOAD_ATTR                6 (SlugField)
                       58 LOAD_CONST               3 (1024)
                       60 LOAD_CONST               4 (True)
                       62 KW_NAMES                 5
                       64 PRECALL                  2
                       68 CALL                     2
                       78 STORE_NAME               7 (slug)
          
-          49          80 PUSH_NULL
+          55          80 PUSH_NULL
                       82 LOAD_NAME                3 (models)
                       84 LOAD_ATTR                8 (PositiveIntegerField)
                       94 LOAD_CONST               6 (0)
                       96 KW_NAMES                 7
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_NAME               9 (order)
          
-          51         114 PUSH_NULL
+          57         114 PUSH_NULL
                      116 LOAD_BUILD_CLASS
-                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 51>)
+                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 57>)
                      120 MAKE_FUNCTION            0
                      122 LOAD_CONST               9 ('Meta')
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_NAME              10 (Meta)
          
-          56         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 56>)
+          62         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 62>)
                      142 MAKE_FUNCTION            0
                      144 STORE_NAME              11 (__str__)
          
-          59         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 59>)
+          65         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 65>)
                      148 MAKE_FUNCTION            0
                      150 STORE_NAME              12 (get_absolute_url)
                      152 LOAD_CONST              12 (None)
                      154 RETURN_VALUE
          consts
             'Category'
             255
@@ -553,27 +621,27 @@
             ('default',)
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                51           0 RESUME                   0
+                57           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Category.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                52          10 LOAD_CONST               1 ('category')
+                58          10 LOAD_CONST               1 ('category')
                             12 STORE_NAME               3 (verbose_name)
                
-                53          14 LOAD_CONST               2 ('categories')
+                59          14 LOAD_CONST               2 ('categories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                54          18 LOAD_CONST               3 (('order',))
+                60          18 LOAD_CONST               3 (('order',))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Category.Meta'
                   'category'
                   'categories'
@@ -581,28 +649,28 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 51
+               firstlineno 57
                lnotab 0x0a0104010401
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-                56           0 RESUME                   0
+                62           0 RESUME                   0
                
-                57           2 LOAD_FAST                0 (self)
+                63           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (order)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 ('. ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (name)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -612,34 +680,34 @@
                   '. '
                names      ('order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 56
+               firstlineno 62
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   007d017c019b0064027c006a0100000000000000009b0064037c006a0200
                   000000000000009b009d055300
-                59           0 RESUME                   0
+                65           0 RESUME                   0
                
-                60           2 LOAD_GLOBAL              1 (NULL + reverse)
+                66           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:index')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               1 (index_url)
                
-                61          32 LOAD_FAST                1 (index_url)
+                67          32 LOAD_FAST                1 (index_url)
                             34 FORMAT_VALUE             0
                             36 LOAD_CONST               2 ('#')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                1 (slug)
                             50 FORMAT_VALUE             0
                             52 LOAD_CONST               3 ('.')
                             54 LOAD_FAST                0 (self)
@@ -654,24 +722,24 @@
                   '.'
                names      ('reverse', 'slug', 'order')
                varnames   ('self', 'index_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 59
+               firstlineno 65
                lnotab 0x02011e01
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'SlugField', 'slug', 'PositiveIntegerField', 'order', 'Meta', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Category'
-         firstlineno 46
+         firstlineno 52
          lnotab 0x0a012201240122021a050603
       'Category'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -684,128 +752,128 @@
             0000005a0d020065036a0e00000000000000006409ac0aa6010000ab0100
             000000000000005a0f020065036a100000000000000000640bac0aa60100
             00ab0100000000000000005a1102004700640c8400640da6020000ab0200
             000000000000005a12640e84005a136514640f8400a6000000ab00000000
             00000000005a15651464108400a6000000ab0000000000000000005a1665
             1464118400a6000000ab0000000000000000005a17641284005a18641384
             005a1964145300
-          64           0 RESUME                   0
+          70           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Subcategory')
                        8 STORE_NAME               2 (__qualname__)
          
-          65          10 PUSH_NULL
+          71          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-          66          24 LOAD_NAME                5 (Category)
+          72          24 LOAD_NAME                5 (Category)
                       26 LOAD_CONST               1 ('subcategories')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-          65          40 KW_NAMES                 2
+          71          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (category)
          
-          68          58 PUSH_NULL
+          74          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (CharField)
                       72 LOAD_CONST               3 (255)
                       74 KW_NAMES                 4
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_NAME               9 (name)
          
-          69          92 PUSH_NULL
+          75          92 PUSH_NULL
                       94 LOAD_NAME                3 (models)
                       96 LOAD_ATTR               10 (SlugField)
                      106 LOAD_CONST               5 (1024)
                      108 LOAD_CONST               6 (True)
                      110 KW_NAMES                 7
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_NAME              11 (slug)
          
-          70         128 PUSH_NULL
+          76         128 PUSH_NULL
                      130 LOAD_NAME               12 (BBCodeTextField)
                      132 LOAD_CONST               6 (True)
                      134 LOAD_CONST               6 (True)
                      136 KW_NAMES                 8
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              13 (description)
          
-          71         154 PUSH_NULL
+          77         154 PUSH_NULL
                      156 LOAD_NAME                3 (models)
                      158 LOAD_ATTR               14 (PositiveIntegerField)
                      168 LOAD_CONST               9 (0)
                      170 KW_NAMES                10
                      172 PRECALL                  1
                      176 CALL                     1
                      186 STORE_NAME              15 (order)
          
-          72         188 PUSH_NULL
+          78         188 PUSH_NULL
                      190 LOAD_NAME                3 (models)
                      192 LOAD_ATTR               16 (BooleanField)
                      202 LOAD_CONST              11 (False)
                      204 KW_NAMES                10
                      206 PRECALL                  1
                      210 CALL                     1
                      220 STORE_NAME              17 (staff_post_only)
          
-          74         222 PUSH_NULL
+          80         222 PUSH_NULL
                      224 LOAD_BUILD_CLASS
-                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 74>)
+                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 80>)
                      228 MAKE_FUNCTION            0
                      230 LOAD_CONST              13 ('Meta')
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_NAME              18 (Meta)
          
-          82         248 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 82>)
+          88         248 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 88>)
                      250 MAKE_FUNCTION            0
                      252 STORE_NAME              19 (can_post)
          
-          85         254 LOAD_NAME               20 (property)
+          91         254 LOAD_NAME               20 (property)
          
-          86         256 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 85>)
+          92         256 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 91>)
                      258 MAKE_FUNCTION            0
          
-          85         260 PRECALL                  0
+          91         260 PRECALL                  0
                      264 CALL                     0
          
-          86         274 STORE_NAME              21 (thread_count)
+          92         274 STORE_NAME              21 (thread_count)
          
-          89         276 LOAD_NAME               20 (property)
+          95         276 LOAD_NAME               20 (property)
          
-          90         278 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 89>)
+          96         278 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 95>)
                      280 MAKE_FUNCTION            0
          
-          89         282 PRECALL                  0
+          95         282 PRECALL                  0
                      286 CALL                     0
          
-          90         296 STORE_NAME              22 (post_count)
+          96         296 STORE_NAME              22 (post_count)
          
-          93         298 LOAD_NAME               20 (property)
+          99         298 LOAD_NAME               20 (property)
          
-          94         300 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 93>)
+         100         300 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 99>)
                      302 MAKE_FUNCTION            0
          
-          93         304 PRECALL                  0
+          99         304 PRECALL                  0
                      308 CALL                     0
          
-          94         318 STORE_NAME              23 (latest_thread)
+         100         318 STORE_NAME              23 (latest_thread)
          
-          97         320 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
+         103         320 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 103>)
                      322 MAKE_FUNCTION            0
                      324 STORE_NAME              24 (__str__)
          
-         100         326 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 100>)
+         106         326 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 106>)
                      328 MAKE_FUNCTION            0
                      330 STORE_NAME              25 (get_absolute_url)
                      332 LOAD_CONST              20 (None)
                      334 RETURN_VALUE
          consts
             'Subcategory'
             'subcategories'
@@ -821,27 +889,27 @@
             False
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                74           0 RESUME                   0
+                80           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Subcategory.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                75          10 LOAD_CONST               1 ('subcategory')
+                81          10 LOAD_CONST               1 ('subcategory')
                             12 STORE_NAME               3 (verbose_name)
                
-                76          14 LOAD_CONST               2 ('subcategories')
+                82          14 LOAD_CONST               2 ('subcategories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                77          18 LOAD_CONST               3 (('category__order', 'order'))
+                83          18 LOAD_CONST               3 (('category__order', 'order'))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Subcategory.Meta'
                   'subcategory'
                   'subcategories'
@@ -849,84 +917,84 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 74
+               firstlineno 80
                lnotab 0x0a0104010401
             'Meta'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code
                   0x97007c006a0000000000000000000c0070067c016a0100000000000000
                   005300
-                82           0 RESUME                   0
+                88           0 RESUME                   0
                
-                83           2 LOAD_FAST                0 (self)
+                89           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (staff_post_only)
                             14 UNARY_NOT
                             16 JUMP_IF_TRUE_OR_POP      6 (to 30)
                             18 LOAD_FAST                1 (user)
                             20 LOAD_ATTR                1 (is_staff)
                        >>   30 RETURN_VALUE
                consts
                   None
                names      ('staff_post_only', 'is_staff')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_post'
-               firstlineno 82
+               firstlineno 88
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-                85           0 RESUME                   0
+                91           0 RESUME                   0
                
-                87           2 LOAD_FAST                0 (self)
+                93           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('threads', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'thread_count'
-               firstlineno 85
+               firstlineno 91
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000640184007c006a0100000000000000
                   00a0020000000000000000000000000000000000000000a6000000ab0000
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000005300
-                89           0 RESUME                   0
+                95           0 RESUME                   0
                
-                91           2 LOAD_GLOBAL              1 (NULL + sum)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 91>)
+                97           2 LOAD_GLOBAL              1 (NULL + sum)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (threads)
                             30 LOAD_METHOD              2 (all)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
@@ -939,15 +1007,15 @@
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                      91           0 RESUME                   0
+                      97           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (thread)
                                   10 LOAD_FAST                1 (thread)
                                   12 LOAD_ATTR                0 (post_count)
                                   22 LIST_APPEND              2
@@ -956,37 +1024,37 @@
                      consts
                      names      ('post_count',)
                      varnames   ('.0', 'thread')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                      name       '<listcomp>'
-                     firstlineno 91
+                     firstlineno 97
                      lnotab 0x
                names      ('sum', 'threads', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 89
+               firstlineno 95
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-                93           0 RESUME                   0
+                99           0 RESUME                   0
                
-                95           2 LOAD_FAST                0 (self)
+               101           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-last_post_created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -997,27 +1065,27 @@
                   '-last_post_created_at'
                names      ('threads', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_thread'
-               firstlineno 93
+               firstlineno 99
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064027c006a0200000000000000009b009d055300
-                97           0 RESUME                   0
+               103           0 RESUME                   0
                
-                98           2 LOAD_FAST                0 (self)
+               104           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (category)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (order)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               2 ('. ')
@@ -1032,27 +1100,27 @@
                   '. '
                names      ('category', 'order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 97
+               firstlineno 103
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               100           0 RESUME                   0
+               106           0 RESUME                   0
                
-               101           2 LOAD_GLOBAL              1 (NULL + reverse)
+               107           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:subcategory')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (slug)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1063,24 +1131,24 @@
                   ('args',)
                names      ('reverse', 'slug')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 100
+               firstlineno 106
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'BBCodeTextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'can_post', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Subcategory'
-         firstlineno 64
+         firstlineno 70
          lnotab
             0x0a010e0110ff1203220124011a01220122021a080603020104ff0e0102
             03020104ff0e010203020104ff0e0102030603
       'Subcategory'
       code
          argcount  : 0
          nlocals   : 0
@@ -1097,143 +1165,143 @@
             05ac06a6010000ab0100000000000000005a10020065036a110000000000
             0000006407ac08a6010000ab0100000000000000005a12020065036a1300
             000000000000006409ac06a6010000ab0100000000000000005a14020047
             00640a8400640ba6020000ab0200000000000000005a15640c84005a1664
             0d84005a17640e84005a18640f84005a19651a64108400a6000000ab0000
             000000000000005a1b651a64118400a6000000ab0000000000000000005a
             1c641284005a1d64135300
-         104           0 RESUME                   0
+         110           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Thread')
                        8 STORE_NAME               2 (__qualname__)
          
-         105          10 PUSH_NULL
+         111          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-         106          24 LOAD_NAME                5 (Subcategory)
+         112          24 LOAD_NAME                5 (Subcategory)
                       26 LOAD_CONST               1 ('threads')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-         105          40 KW_NAMES                 2
+         111          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (subcategory)
          
-         108          58 PUSH_NULL
+         114          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                4 (ForeignKey)
                       72 LOAD_NAME                8 (User)
                       74 LOAD_CONST               1 ('threads')
                       76 LOAD_NAME                3 (models)
                       78 LOAD_ATTR                6 (CASCADE)
                       88 KW_NAMES                 2
                       90 PRECALL                  3
                       94 CALL                     3
                      104 STORE_NAME               9 (user)
          
-         109         106 PUSH_NULL
+         115         106 PUSH_NULL
                      108 LOAD_NAME                3 (models)
                      110 LOAD_ATTR               10 (CharField)
                      120 LOAD_CONST               3 (255)
                      122 KW_NAMES                 4
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_NAME              11 (title)
          
-         110         140 PUSH_NULL
+         116         140 PUSH_NULL
                      142 LOAD_NAME               12 (BBCodeTextField)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 STORE_NAME              13 (content)
          
-         111         160 PUSH_NULL
+         117         160 PUSH_NULL
                      162 LOAD_NAME                3 (models)
                      164 LOAD_ATTR               14 (BooleanField)
                      174 LOAD_CONST               5 (False)
                      176 KW_NAMES                 6
                      178 PRECALL                  1
                      182 CALL                     1
                      192 STORE_NAME              15 (is_pinned)
          
-         112         194 PUSH_NULL
+         118         194 PUSH_NULL
                      196 LOAD_NAME                3 (models)
                      198 LOAD_ATTR               14 (BooleanField)
                      208 LOAD_CONST               5 (False)
                      210 KW_NAMES                 6
                      212 PRECALL                  1
                      216 CALL                     1
                      226 STORE_NAME              16 (is_closed)
          
-         113         228 PUSH_NULL
+         119         228 PUSH_NULL
                      230 LOAD_NAME                3 (models)
                      232 LOAD_ATTR               17 (DateTimeField)
                      242 LOAD_CONST               7 (True)
                      244 KW_NAMES                 8
                      246 PRECALL                  1
                      250 CALL                     1
                      260 STORE_NAME              18 (last_post_created_at)
          
-         114         262 PUSH_NULL
+         120         262 PUSH_NULL
                      264 LOAD_NAME                3 (models)
                      266 LOAD_ATTR               19 (PositiveIntegerField)
                      276 LOAD_CONST               9 (0)
                      278 KW_NAMES                 6
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_NAME              20 (view_count)
          
-         116         296 PUSH_NULL
+         122         296 PUSH_NULL
                      298 LOAD_BUILD_CLASS
-                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 116>)
+                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 122>)
                      302 MAKE_FUNCTION            0
                      304 LOAD_CONST              11 ('Meta')
                      306 PRECALL                  2
                      310 CALL                     2
                      320 STORE_NAME              21 (Meta)
          
-         127         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 127>)
+         133         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 133>)
                      324 MAKE_FUNCTION            0
                      326 STORE_NAME              22 (__str__)
          
-         130         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 130>)
+         136         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
                      330 MAKE_FUNCTION            0
                      332 STORE_NAME              23 (can_edit)
          
-         133         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 133>)
+         139         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
                      336 MAKE_FUNCTION            0
                      338 STORE_NAME              24 (can_delete)
          
-         136         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
+         142         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 142>)
                      342 MAKE_FUNCTION            0
                      344 STORE_NAME              25 (can_post)
          
-         139         346 LOAD_NAME               26 (property)
+         145         346 LOAD_NAME               26 (property)
          
-         140         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
+         146         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 145>)
                      350 MAKE_FUNCTION            0
          
-         139         352 PRECALL                  0
+         145         352 PRECALL                  0
                      356 CALL                     0
          
-         140         366 STORE_NAME              27 (post_count)
+         146         366 STORE_NAME              27 (post_count)
          
-         143         368 LOAD_NAME               26 (property)
+         149         368 LOAD_NAME               26 (property)
          
-         144         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 143>)
+         150         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 149>)
                      372 MAKE_FUNCTION            0
          
-         143         374 PRECALL                  0
+         149         374 PRECALL                  0
                      378 CALL                     0
          
-         144         388 STORE_NAME              28 (latest_post)
+         150         388 STORE_NAME              28 (latest_post)
          
-         147         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 147>)
+         153         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 153>)
                      392 MAKE_FUNCTION            0
                      394 STORE_NAME              29 (get_absolute_url)
                      396 LOAD_CONST              19 (None)
                      398 RETURN_VALUE
          consts
             'Thread'
             'threads'
@@ -1247,75 +1315,75 @@
             0
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035300
-               116           0 RESUME                   0
+               122           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Thread.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               117          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
+               123          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
                             12 STORE_NAME               3 (ordering)
                
-               122          14 LOAD_CONST               2 ((('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
+               128          14 LOAD_CONST               2 ((('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
                             16 STORE_NAME               4 (permissions)
                             18 LOAD_CONST               3 (None)
                             20 RETURN_VALUE
                consts
                   'Thread.Meta'
                   ('subcategory', '-is_pinned', '-last_post_created_at')
                   (('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread'))
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 116
+               firstlineno 122
                lnotab 0x0a010405
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000009b005300
-               127           0 RESUME                   0
+               133           0 RESUME                   0
                
-               128           2 LOAD_FAST                0 (self)
+               134           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 FORMAT_VALUE             0
                             16 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 127
+               firstlineno 133
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               130           0 RESUME                   0
+               136           0 RESUME                   0
                
-               131           2 LOAD_FAST                1 (user)
+               137           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.change_thread')
@@ -1327,28 +1395,28 @@
                   'punkweb_bb.change_thread'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_edit'
-               firstlineno 130
+               firstlineno 136
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               133           0 RESUME                   0
+               139           0 RESUME                   0
                
-               134           2 LOAD_FAST                1 (user)
+               140           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_thread')
@@ -1360,77 +1428,77 @@
                   'punkweb_bb.delete_thread'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 133
+               firstlineno 139
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000000c005300
-               136           0 RESUME                   0
+               142           0 RESUME                   0
                
-               137           2 LOAD_FAST                0 (self)
+               143           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (is_closed)
                             14 UNARY_NOT
                             16 RETURN_VALUE
                consts
                   None
                names      ('is_closed',)
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_post'
-               firstlineno 136
+               firstlineno 142
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               139           0 RESUME                   0
+               145           0 RESUME                   0
                
-               141           2 LOAD_FAST                0 (self)
+               147           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('posts', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 139
+               firstlineno 145
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-               143           0 RESUME                   0
+               149           0 RESUME                   0
                
-               145           2 LOAD_FAST                0 (self)
+               151           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1441,27 +1509,27 @@
                   '-created_at'
                names      ('posts', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_post'
-               firstlineno 143
+               firstlineno 149
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               147           0 RESUME                   0
+               153           0 RESUME                   0
                
-               148           2 LOAD_GLOBAL              1 (NULL + reverse)
+               154           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (id)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1472,24 +1540,24 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 147
+               firstlineno 153
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'can_edit', 'can_delete', 'can_post', 'property', 'post_count', 'latest_post', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Thread'
-         firstlineno 104
+         firstlineno 110
          lnotab
             0x0a010e0110ff120330012201140122012201220122021a0b0603060306
             030603020104ff0e010203020104ff0e010203
       'Thread'
       code
          argcount  : 0
          nlocals   : 0
@@ -1503,98 +1571,98 @@
             000000000000005a0b02004700640384006404a6020000ab020000000000
             0000005a0c640584005a0d640684005a0e640784005a0f651064088400a6
             000000ab0000000000000000005a11651064098400a6000000ab00000000
             00000000005a12640a84005a1388006601640b84085a14880078015a1553
             00
                        0 MAKE_CELL                0 (__class__)
          
-         151           2 RESUME                   0
+         157           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Post')
                       10 STORE_NAME               2 (__qualname__)
          
-         152          12 PUSH_NULL
+         158          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (ForeignKey)
                       26 LOAD_NAME                5 (Thread)
                       28 LOAD_CONST               1 ('posts')
                       30 LOAD_NAME                3 (models)
                       32 LOAD_ATTR                6 (CASCADE)
                       42 KW_NAMES                 2
                       44 PRECALL                  3
                       48 CALL                     3
                       58 STORE_NAME               7 (thread)
          
-         153          60 PUSH_NULL
+         159          60 PUSH_NULL
                       62 LOAD_NAME                3 (models)
                       64 LOAD_ATTR                4 (ForeignKey)
                       74 LOAD_NAME                8 (User)
                       76 LOAD_CONST               1 ('posts')
                       78 LOAD_NAME                3 (models)
                       80 LOAD_ATTR                6 (CASCADE)
                       90 KW_NAMES                 2
                       92 PRECALL                  3
                       96 CALL                     3
                      106 STORE_NAME               9 (user)
          
-         154         108 PUSH_NULL
+         160         108 PUSH_NULL
                      110 LOAD_NAME               10 (BBCodeTextField)
                      112 PRECALL                  0
                      116 CALL                     0
                      126 STORE_NAME              11 (content)
          
-         156         128 PUSH_NULL
+         162         128 PUSH_NULL
                      130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 156>)
+                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 162>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_CONST               4 ('Meta')
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              12 (Meta)
          
-         159         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 159>)
+         165         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
                      156 MAKE_FUNCTION            0
                      158 STORE_NAME              13 (__str__)
          
-         162         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 162>)
+         168         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
                      162 MAKE_FUNCTION            0
                      164 STORE_NAME              14 (can_edit)
          
-         165         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
+         171         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 171>)
                      168 MAKE_FUNCTION            0
                      170 STORE_NAME              15 (can_delete)
          
-         168         172 LOAD_NAME               16 (property)
+         174         172 LOAD_NAME               16 (property)
          
-         169         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
+         175         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
                      176 MAKE_FUNCTION            0
          
-         168         178 PRECALL                  0
+         174         178 PRECALL                  0
                      182 CALL                     0
          
-         169         192 STORE_NAME              17 (index)
+         175         192 STORE_NAME              17 (index)
          
-         176         194 LOAD_NAME               16 (property)
+         182         194 LOAD_NAME               16 (property)
          
-         177         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 176>)
+         183         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 182>)
                      198 MAKE_FUNCTION            0
          
-         176         200 PRECALL                  0
+         182         200 PRECALL                  0
                      204 CALL                     0
          
-         177         214 STORE_NAME              18 (page_number)
+         183         214 STORE_NAME              18 (page_number)
          
-         180         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 180>)
+         186         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 186>)
                      218 MAKE_FUNCTION            0
                      220 STORE_NAME              19 (get_absolute_url)
          
-         187         222 LOAD_CLOSURE             0 (__class__)
+         193         222 LOAD_CLOSURE             0 (__class__)
                      224 BUILD_TUPLE              1
-                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 187>)
+                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 193>)
                      228 MAKE_FUNCTION            8 (closure)
                      230 STORE_NAME              20 (save)
                      232 LOAD_CLOSURE             0 (__class__)
                      234 COPY                     1
                      236 STORE_NAME              21 (__classcell__)
                      238 RETURN_VALUE
          consts
@@ -1603,48 +1671,48 @@
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               156           0 RESUME                   0
+               162           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Post.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               157          10 LOAD_CONST               1 (('created_at',))
+               163          10 LOAD_CONST               1 (('created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Post.Meta'
                   ('created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 156
+               firstlineno 162
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064017c006a0200000000000000009b009d055300
-               159           0 RESUME                   0
+               165           0 RESUME                   0
                
-               160           2 LOAD_FAST                0 (self)
+               166           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (user)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               1 (' > ')
@@ -1658,28 +1726,28 @@
                   ' > '
                names      ('thread', 'user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 159
+               firstlineno 165
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               162           0 RESUME                   0
+               168           0 RESUME                   0
                
-               163           2 LOAD_FAST                1 (user)
+               169           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.change_post')
@@ -1691,28 +1759,28 @@
                   'punkweb_bb.change_post'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_edit'
-               firstlineno 162
+               firstlineno 168
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               165           0 RESUME                   0
+               171           0 RESUME                   0
                
-               166           2 LOAD_FAST                1 (user)
+               172           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_post')
@@ -1724,41 +1792,41 @@
                   'punkweb_bb.delete_post'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 165
+               firstlineno 171
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000006401a6010000ab010000000000
                   0000007d017407000000000000000000007c01a004000000000000000000
                   000000000000000000000064026403ac04a6020000ab0200000000000000
                   00a6010000ab010000000000000000a00500000000000000000000000000
                   000000000000007c006a060000000000000000a6010000ab010000000000
                   0000007d027c0264057a0000005300
-               168           0 RESUME                   0
+               174           0 RESUME                   0
                
-               172           2 LOAD_FAST                0 (self)
+               178           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 LOAD_ATTR                1 (posts)
                             24 LOAD_METHOD              2 (order_by)
                             46 LOAD_CONST               1 ('created_at')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (qs)
                
-               173          64 LOAD_GLOBAL              7 (NULL + list)
+               179          64 LOAD_GLOBAL              7 (NULL + list)
                             76 LOAD_FAST                1 (qs)
                             78 LOAD_METHOD              4 (values_list)
                            100 LOAD_CONST               2 ('id')
                            102 LOAD_CONST               3 (True)
                            104 KW_NAMES                 4
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1767,15 +1835,15 @@
                            134 LOAD_METHOD              5 (index)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                6 (id)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 STORE_FAST               2 (index)
                
-               174         184 LOAD_FAST                2 (index)
+               180         184 LOAD_FAST                2 (index)
                            186 LOAD_CONST               5 (1)
                            188 BINARY_OP                0 (+)
                            192 RETURN_VALUE
                consts
                   None
                   'created_at'
                   'id'
@@ -1784,27 +1852,27 @@
                   1
                names      ('thread', 'posts', 'order_by', 'list', 'values_list', 'index', 'id')
                varnames   ('self', 'qs', 'index')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'index'
-               firstlineno 168
+               firstlineno 174
                lnotab 0x02043e017801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   0000000000000064017a0b0000a6010000ab0100000000000000005300
-               176           0 RESUME                   0
+               182           0 RESUME                   0
                
-               178           2 LOAD_GLOBAL              1 (NULL + math)
+               184           2 LOAD_GLOBAL              1 (NULL + math)
                             14 LOAD_ATTR                1 (ceil)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (index)
                             36 LOAD_CONST               1 (10)
                             38 BINARY_OP               11 (/)
                             42 PRECALL                  1
                             46 CALL                     1
@@ -1814,67 +1882,67 @@
                   10
                names      ('math', 'ceil', 'index')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'page_number'
-               firstlineno 176
+               firstlineno 182
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a0100000000000000006a
                   0200000000000000006701ac02a6020000ab0200000000000000007d017c
                   0164037c006a0300000000000000009b0064047c006a0200000000000000
                   009b009d047a0d00007d017c015300
-               180           0 RESUME                   0
+               186           0 RESUME                   0
                
-               181           2 LOAD_GLOBAL              1 (NULL + reverse)
+               187           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (thread)
                             28 LOAD_ATTR                2 (id)
                             38 BUILD_LIST               1
                             40 KW_NAMES                 2
                             42 PRECALL                  2
                             46 CALL                     2
                             56 STORE_FAST               1 (thread_url)
                
-               183          58 LOAD_FAST                1 (thread_url)
+               189          58 LOAD_FAST                1 (thread_url)
                             60 LOAD_CONST               3 ('?page=')
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (page_number)
                             74 FORMAT_VALUE             0
                             76 LOAD_CONST               4 ('#post-')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                2 (id)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             4
                             94 BINARY_OP               13 (+=)
                             98 STORE_FAST               1 (thread_url)
                
-               185         100 LOAD_FAST                1 (thread_url)
+               191         100 LOAD_FAST                1 (thread_url)
                            102 RETURN_VALUE
                consts
                   None
                   'punkweb_bb:thread'
                   ('args',)
                   '?page='
                   '#post-'
                names      ('reverse', 'thread', 'id', 'page_number')
                varnames   ('self', 'thread_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 180
+               firstlineno 186
                lnotab 0x020138022a02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
@@ -1885,48 +1953,48 @@
                   006a0000000000000000005f0700000000000000007c006a000000000000
                   000000a0080000000000000000000000000000000000000000a6000000ab
                   00000000000000000001000200741300000000000000000000a6000000ab
                   0000000000000000006a0800000000000000007c0169007c02a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               187           2 RESUME                   0
+               193           2 RESUME                   0
                
-               188           4 LOAD_FAST                0 (self)
+               194           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (thread)
                             16 LOAD_ATTR                1 (is_closed)
                             26 POP_JUMP_FORWARD_IF_FALSE    15 (to 58)
                
-               189          28 LOAD_GLOBAL              5 (NULL + ValidationError)
+               195          28 LOAD_GLOBAL              5 (NULL + ValidationError)
                             40 LOAD_CONST               1 ('Cannot add posts to a closed thread.')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 RAISE_VARARGS            1
                
-               190     >>   58 LOAD_FAST                0 (self)
+               196     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                3 (_state)
                             70 LOAD_ATTR                4 (adding)
                             80 POP_JUMP_FORWARD_IF_FALSE    54 (to 190)
                
-               191          82 LOAD_GLOBAL             11 (NULL + timezone)
+               197          82 LOAD_GLOBAL             11 (NULL + timezone)
                             94 LOAD_ATTR                6 (now)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                0 (thread)
                            130 STORE_ATTR               7 (last_post_created_at)
                
-               192         140 LOAD_FAST                0 (self)
+               198         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                0 (thread)
                            152 LOAD_METHOD              8 (save)
                            174 PRECALL                  0
                            178 CALL                     0
                            188 POP_TOP
                
-               193     >>  190 PUSH_NULL
+               199     >>  190 PUSH_NULL
                            192 LOAD_GLOBAL             19 (NULL + super)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 LOAD_ATTR                8 (save)
                            228 LOAD_FAST                1 (args)
                            230 BUILD_MAP                0
                            232 LOAD_FAST                2 (kwargs)
@@ -1940,23 +2008,23 @@
                   'Cannot add posts to a closed thread.'
                names      ('thread', 'is_closed', 'ValidationError', '_state', 'adding', 'timezone', 'now', 'last_post_created_at', 'save', 'super')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'save'
-               firstlineno 187
+               firstlineno 193
                lnotab 0x040118011e0118013a013201
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'can_edit', 'can_delete', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Post'
-         firstlineno 151
+         firstlineno 157
          lnotab
             0x0c013001300114021a03060306030603020104ff0e010207020104ff0e
             0102030607
       'Post'
       code
          argcount  : 0
          nlocals   : 0
@@ -1964,101 +2032,101 @@
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000a6000000ab0000000000000000005a0902
             004700640384006404a6020000ab0200000000000000005a0a640584005a
             0b640684005a0c64075300
-         196           0 RESUME                   0
+         202           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Shout')
                        8 STORE_NAME               2 (__qualname__)
          
-         197          10 PUSH_NULL
+         203          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('shouts')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-         198          58 PUSH_NULL
+         204          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (TextField)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 STORE_NAME               9 (content)
          
-         200          88 PUSH_NULL
+         206          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
-                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 200>)
+                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 206>)
                       94 MAKE_FUNCTION            0
                       96 LOAD_CONST               4 ('Meta')
                       98 PRECALL                  2
                      102 CALL                     2
                      112 STORE_NAME              10 (Meta)
          
-         203         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 203>)
+         209         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 209>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              11 (__str__)
          
-         206         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 206>)
+         212         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 212>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              12 (can_delete)
                      126 LOAD_CONST               7 (None)
                      128 RETURN_VALUE
          consts
             'Shout'
             'shouts'
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               200           0 RESUME                   0
+               206           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Shout.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               201          10 LOAD_CONST               1 (('-created_at',))
+               207          10 LOAD_CONST               1 (('-created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Shout.Meta'
                   ('-created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 200
+               firstlineno 206
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-               203           0 RESUME                   0
+               209           0 RESUME                   0
                
-               204           2 LOAD_FAST                0 (self)
+               210           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (created_at)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -2068,28 +2136,28 @@
                   ' > '
                names      ('user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 203
+               firstlineno 209
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               206           0 RESUME                   0
+               212           0 RESUME                   0
                
-               207           2 LOAD_FAST                1 (user)
+               213           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_shout')
@@ -2101,29 +2169,168 @@
                   'punkweb_bb.delete_shout'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 206
+               firstlineno 212
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'User', 'CASCADE', 'user', 'TextField', 'content', 'Meta', '__str__', 'can_delete')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Shout'
-         firstlineno 196
+         firstlineno 202
          lnotab 0x0a0130011e021a030603
       'Shout'
-   names      ('datetime', 'math', 'os', 'django.contrib.auth', 'get_user_model', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout')
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 5
+         flags     : 0
+         code
+            0x970065005a0164005a02020065036a0400000000000000006505640165
+            036a060000000000000000ac02a6030000ab0300000000000000005a0702
+            0065036a08000000000000000064036404ac05a6020000ab020000000000
+            0000005a090200650aa6000000ab0000000000000000005a0b0200470064
+            0684006407a6020000ab0200000000000000005a0c640884005a0d640953
+            00
+         216           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('GroupStyle')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         217          10 PUSH_NULL
+                      12 LOAD_NAME                3 (models)
+                      14 LOAD_ATTR                4 (OneToOneField)
+                      24 LOAD_NAME                5 (Group)
+                      26 LOAD_CONST               1 ('style')
+                      28 LOAD_NAME                3 (models)
+                      30 LOAD_ATTR                6 (CASCADE)
+                      40 KW_NAMES                 2
+                      42 PRECALL                  3
+                      46 CALL                     3
+                      56 STORE_NAME               7 (group)
+         
+         218          58 PUSH_NULL
+                      60 LOAD_NAME                3 (models)
+                      62 LOAD_ATTR                8 (PositiveIntegerField)
+         
+         219          72 LOAD_CONST               3 (0)
+         
+         220          74 LOAD_CONST               4 ('Highest priority is displayed')
+         
+         218          76 KW_NAMES                 5
+                      78 PRECALL                  2
+                      82 CALL                     2
+                      92 STORE_NAME               9 (priority)
+         
+         222          94 PUSH_NULL
+                      96 LOAD_NAME               10 (BBCodeTextField)
+                      98 PRECALL                  0
+                     102 CALL                     0
+                     112 STORE_NAME              11 (username_style)
+         
+         224         114 PUSH_NULL
+                     116 LOAD_BUILD_CLASS
+                     118 LOAD_CONST               6 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 224>)
+                     120 MAKE_FUNCTION            0
+                     122 LOAD_CONST               7 ('Meta')
+                     124 PRECALL                  2
+                     128 CALL                     2
+                     138 STORE_NAME              12 (Meta)
+         
+         227         140 LOAD_CONST               8 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 227>)
+                     142 MAKE_FUNCTION            0
+                     144 STORE_NAME              13 (__str__)
+                     146 LOAD_CONST               9 (None)
+                     148 RETURN_VALUE
+         consts
+            'GroupStyle'
+            'style'
+            ('related_name', 'on_delete')
+            0
+            'Highest priority is displayed'
+            ('default', 'help_text')
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 1
+               flags     : 0
+               code 0x970065005a0164005a0264015a0364025300
+               224           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('GroupStyle.Meta')
+                             8 STORE_NAME               2 (__qualname__)
+               
+               225          10 LOAD_CONST               1 (('-priority',))
+                            12 STORE_NAME               3 (ordering)
+                            14 LOAD_CONST               2 (None)
+                            16 RETURN_VALUE
+               consts
+                  'GroupStyle.Meta'
+                  ('-priority',)
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'ordering')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'Meta'
+               firstlineno 224
+               lnotab 0x0a01
+            'Meta'
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000009b0064017c006a0100000000000000
+                  009b009d035300
+               227           0 RESUME                   0
+               
+               228           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (group)
+                            14 FORMAT_VALUE             0
+                            16 LOAD_CONST               1 (' > ')
+                            18 LOAD_FAST                0 (self)
+                            20 LOAD_ATTR                1 (priority)
+                            30 FORMAT_VALUE             0
+                            32 BUILD_STRING             3
+                            34 RETURN_VALUE
+               consts
+                  None
+                  ' > '
+               names      ('group', 'priority')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       '__str__'
+               firstlineno 227
+               lnotab 0x0201
+            None
+         names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'Group', 'CASCADE', 'group', 'PositiveIntegerField', 'priority', 'BBCodeTextField', 'username_style', 'Meta', '__str__')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+         name       'GroupStyle'
+         firstlineno 216
+         lnotab 0x0a0130010e01020102fe120414021a03
+      'GroupStyle'
+   names      ('datetime', 'math', 'os', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'punkweb_bb.utils', 'get_styled_username', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout', 'GroupStyle')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108020c010c010c010c010c010c010c021002140306
-      051e171e121e281e2f1e2d
+      0x00ff02010801080108020c010c010c010c010c010c010c010c0210010c
+      02140306051e1b1e121e281e2f1e2d1e0e
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/admin.py` & `punkweb_bb-0.2.2/punkweb_bb/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from django.contrib import admin
 from django.utils.safestring import mark_safe
 
 from punkweb_bb.admin_forms import (
     BoardProfileAdminModelForm,
     CategoryAdminModelForm,
+    GroupStyleAdminModelForm,
     PostAdminModelForm,
     SubcategoryAdminModelForm,
     ThreadAdminModelForm,
 )
-from punkweb_bb.models import BoardProfile, Category, Post, Shout, Subcategory, Thread
+from punkweb_bb.models import (
+    BoardProfile,
+    Category,
+    GroupStyle,
+    Post,
+    Shout,
+    Subcategory,
+    Thread,
+)
 
 
 @admin.register(BoardProfile)
 class BoardProfileModelAdmin(admin.ModelAdmin):
     form = BoardProfileAdminModelForm
     list_display = ("user",)
     list_filter = (
@@ -110,7 +119,20 @@
         "created_at",
     )
     search_fields = (
         "user__username",
         "user__email",
         "content",
     )
+
+
+@admin.register(GroupStyle)
+class GroupStyleModelAdmin(admin.ModelAdmin):
+    form = GroupStyleAdminModelForm
+    list_display = (
+        "group",
+        "priority",
+    )
+    search_fields = (
+        "group__name",
+        "username_style",
+    )
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/admin_forms.py` & `punkweb_bb-0.2.2/punkweb_bb/admin_forms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from django import forms
 
-from punkweb_bb.models import BoardProfile, Category, Post, Subcategory, Thread
+from punkweb_bb.models import (
+    BoardProfile,
+    Category,
+    GroupStyle,
+    Post,
+    Subcategory,
+    Thread,
+)
 from punkweb_bb.widgets import BBCodeEditorWidget
 
 
 class BoardProfileAdminModelForm(forms.ModelForm):
     class Meta:
         model = BoardProfile
         fields = "__all__"
@@ -43,7 +50,16 @@
 class PostAdminModelForm(forms.ModelForm):
     class Meta:
         model = Post
         fields = "__all__"
         widgets = {
             "content": BBCodeEditorWidget(),
         }
+
+
+class GroupStyleAdminModelForm(forms.ModelForm):
+    class Meta:
+        model = GroupStyle
+        fields = "__all__"
+        widgets = {
+            "username_style": BBCodeEditorWidget(),
+        }
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.2.2/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/forms.py` & `punkweb_bb-0.2.2/punkweb_bb/forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/middleware.py` & `punkweb_bb-0.2.2/punkweb_bb/middleware.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.2.2/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/migrations/0003_alter_thread_options.py` & `punkweb_bb-0.2.2/punkweb_bb/migrations/0003_alter_thread_options.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/models.py` & `punkweb_bb-0.2.2/punkweb_bb/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import datetime
 import math
 import os
 
 from django.contrib.auth import get_user_model
+from django.contrib.auth.models import Group
 from django.core.cache import cache
 from django.db import models
 from django.forms import ValidationError
 from django.urls import reverse
 from django.utils import timezone
 from precise_bbcode.fields import BBCodeTextField
 
 from punkweb_bb.mixins import TimestampMixin, UUIDPrimaryKeyMixin
+from punkweb_bb.utils import get_styled_username
 
 User = get_user_model()
 
 
 def profile_image_upload_to(instance, filename):
     ext = os.path.splitext(filename)[-1]
     return f"punkweb_bb/board_profiles/{instance.user.username}/image{ext}"
@@ -25,14 +27,18 @@
     image = models.ImageField(upload_to=profile_image_upload_to, blank=True, null=True)
     signature = BBCodeTextField(max_length=1024, blank=True, null=True)
 
     class Meta:
         ordering = ("user__username",)
 
     @property
+    def styled_username(self):
+        return get_styled_username(self.user)
+
+    @property
     def is_online(self):
         last_seen = cache.get(f"profile_online_{self.id}")
         if last_seen:
             return timezone.now() < last_seen + datetime.timedelta(minutes=5)
         return False
 
     @property
@@ -201,7 +207,22 @@
         ordering = ("-created_at",)
 
     def __str__(self):
         return f"{self.user} > {self.created_at}"
 
     def can_delete(self, user):
         return user == self.user or user.has_perm("punkweb_bb.delete_shout")
+
+
+class GroupStyle(UUIDPrimaryKeyMixin, TimestampMixin):
+    group = models.OneToOneField(Group, related_name="style", on_delete=models.CASCADE)
+    priority = models.PositiveIntegerField(
+        default=0,
+        help_text="Highest priority is displayed",
+    )
+    username_style = BBCodeTextField()
+
+    class Meta:
+        ordering = ("-priority",)
+
+    def __str__(self):
+        return f"{self.group} > {self.priority}"
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/parsers.py` & `punkweb_bb-0.2.2/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/settings.py` & `punkweb_bb-0.2.2/punkweb_bb/settings.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/shoutbox.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/shoutbox.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 .thread__title .material-symbols-outlined {
   font-size: 1rem;
 }
 
 .thread__latestPost {
   align-items: center;
   display: flex;
+  justify-content: end;
   gap: 0.75rem;
 }
 
 .thread__latestPost__info {
   font-size: 0.875rem;
 }
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files 4% similar despite different names*

```diff
@@ -59,16 +59,16 @@
   display: flex;
   flex-direction: column;
   gap: 0.5rem;
   width: 100%;
 }
 
 .thread__user__group {
-  background-color: var(--primary-8);
-  border: 1px solid var(--primary-9);
+  background-color: var(--oc-gray-0);
+  border: 1px solid var(--border);
   border-radius: 0.25rem;
   color: var(--text-on-primary);
   display: flex;
   font-size: 0.875rem;
   justify-content: center;
   padding: 0.5rem;
   width: 100%;
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.2.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_create.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_update.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/category_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends 'punkweb_bb/base.html' %}
 
-{% load static %}
+{% load static bbcode_tags styled_username %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/index.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/shoutbox.css' %}" />
 {% endblock %}
 
 {% block extra_script %}
@@ -97,15 +97,15 @@
                       <div>
                         <time datetime="{{subcategory.latest_thread.latest_post.created_at|date:'c'}}">
                           {{subcategory.latest_thread.latest_post.created_at|date:'M j, Y'}} at
                           {{subcategory.latest_thread.latest_post.created_at|date:'g:i A'}}
                         </time>
                         •
                         <a href="{% url 'punkweb_bb:profile' subcategory.latest_thread.latest_post.user.id %}">
-                          {{subcategory.latest_thread.latest_post.user.username}}
+                          {{subcategory.latest_thread.latest_post.user|styled_username}}
                         </a>
                       </div>
                     </div>
                   </div>
                   {% else %}
                   <div class="subcategory__latestThread">
                     {% if subcategory.latest_thread.user.profile.image %}
@@ -121,15 +121,15 @@
                       <div>
                         <time datetime="{{subcategory.latest_thread.created_at|date:'c'}}">
                           {{subcategory.latest_thread.created_at|date:'M j, Y'}} at
                           {{subcategory.latest_thread.created_at|date:'g:i A'}}
                         </time>
                         •
                         <a href="{% url 'punkweb_bb:profile' subcategory.latest_thread.user.id %}">
-                          {{subcategory.latest_thread.user.username}}
+                          {{subcategory.latest_thread.user|styled_username}}
                         </a>
                       </div>
                     </div>
                   </div>
                   {% endif %}
                   {% else %}
                   No threads
@@ -171,15 +171,15 @@
               <div>
                 <time datetime="{{thread.created_at|date:'c'}}">
                   {{thread.created_at|date:'M j, Y'}} at
                   {{thread.created_at|date:'g:i A'}}
                 </time>
                 •
                 <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
-                  {{thread.user.username}}
+                  {{thread.user|styled_username}}
                 </a>
               </div>
             </div>
           </div>
           {% endfor %}
         </div>
       </div>
@@ -202,15 +202,15 @@
               <div class="index__statistics__value">{{users|length}}</div>
             </div>
             {% if newest_user %}
             <div class="index__statistics__row">
               <div class="index__statistics__label">Newest member:</div>
               <div class="index__statistics__value">
                 <a href="{% url 'punkweb_bb:profile' newest_user.id %}">
-                  {{newest_user.username}}
+                  {{newest_user|styled_username}}
                 </a>
               </div>
             </div>
             {% endif %}
             <div class="index__statistics__row">
               <div class="index__statistics__label">Users online:</div>
               <div class="index__statistics__value">{{total_online}} ({{members_online|length}} members, {{staff_online|length}} staff, {{guests_online}} guests)</div>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% extends 'punkweb_bb/base.html' %} {% load static %} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static bbcode_tags styled_username
+%} {% block extra_head %}
 {% endblock %} {% block extra_script %}
 {% endblock %} {% block content %}
 {% if punkweb_bb.settings.SHOUTBOX_ENABLED|default:True %} {% include
 'punkweb_bb/shoutbox/shoutbox.html' %} {% endif %} {% for category in
 categories %}
 _{{_{{_cc_aa_tt_ee_gg_oo_rr_yy_.._nn_aa_mm_ee_}}_}} {{%% iiff
 ppeerrmmss..ppuunnkkwweebb__bbbb..aadddd__ssuubbccaatteeggoorryy %%}}
@@ -18,44 +19,44 @@
                                                                                           {subcategory.latest_thread.latest_post.user.profile.image.url}}]
                                                                                           {% else%} [{% static 'punkweb_bb/img/default-profile-image.png'
                                                                                           %}]{% endif %}
                                                                                           _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
                                                                                           {{subcategory.latest_thread.latest_post.created_at|date:'M j,
 _{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}                                                                      Y'}} at {{subcategory.latest_thread.latest_post.created_at|date:
 {                                   {                           {                         'g:i A'}} â¢ _{
-{subcategory.description.rendered}} {subcategory.thread_count}} {subcategory.post_count}} _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+{subcategory.description.rendered}} {subcategory.thread_count}} {subcategory.post_count}} _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
                                                                                           {% else %}
                                                                                           {% if subcategory.latest_thread.user.profile.image %} [{
                                                                                           {subcategory.latest_thread.user.profile.image.url}}]{% else%} [
                                                                                           {% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif
                                                                                           %}
                                                                                           _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
                                                                                           {{subcategory.latest_thread.created_at|date:'M j, Y'}} at {
                                                                                           {subcategory.latest_thread.created_at|date:'g:i A'}} â¢ _{
-                                                                                          _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+                                                                                          _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
                                                                                           {% endif %} {% else %} No threads {% endif %}
 {% endfor %} {% if perms.punkweb_bb.add_category %} _a_d_d_ {% endif %}
 Recent threads
 {% for thread in recent_threads %}
 {% if thread.user.profile.image %} [{{thread.user.profile.image.url}}]{% else%}
 [{% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_}
 {{thread.created_at|date:'M j, Y'}} at {{thread.created_at|date:'g:i A'}} â¢ _{
-_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+_{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 {% endfor %}
 Statistics
 Total threads:
 {{thread_count}}
 Total posts:
 {{post_count}}
 Total members:
 {{users|length}}
 {% if newest_user %}
 Newest member:
-_{_{_n_e_w_e_s_t___u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+_{_{_n_e_w_e_s_t___u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 {% endif %}
 Users online:
 {{total_online}} ({{members_online|length}} members, {{staff_online|length}}
 staff, {{guests_online}} guests)
 {% if punkweb_bb.settings.DISCORD_WIDGET_ENABLED %} {% if
 punkweb_bb.settings.DISCORD_SERVER_ID %} {% else %}
 ****** DDiissccoorrdd WWiiddggeett EErrrroorr ******
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends "punkweb_bb/base.html" %}
-{% load static %}
+{% load static styled_username %}
 
 {% block title_prefix %}Members | {% endblock%}
 {% block og_title_prefix %}Members | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/members.css' %}" />
 {% endblock %}
@@ -29,15 +29,15 @@
         {% if user.profile.image %}
         <img class="pw-avatar sm" src="{{user.profile.image.url}}" />
         {% else %}
         <img class="pw-avatar sm" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" />
         {% endif %}
       </div>
       <div class="members__user__info">
-        <div class="members__user__username"><a href="{% url 'punkweb_bb:profile' user.id %}">{{ user.username }}</a></div>
+        <div class="members__user__username"><a href="{% url 'punkweb_bb:profile' user.id %}">{{ user|styled_username }}</a></div>
         <div class="members__user__stats">
           <div class="members__user__stat">
             Posts:
             <span class="members__user__stat__value">{{user.profile.post_count}}</span>
           </div>
           <div class="members__user__stat">
             Date Joined:
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-{% extends "punkweb_bb/base.html" %} {% load static %} {% block title_prefix
-%}Members | {% endblock%} {% block og_title_prefix %}Members | {% endblock %}
-{% block extra_head %}
+{% extends "punkweb_bb/base.html" %} {% load static styled_username %} {% block
+title_prefix %}Members | {% endblock%} {% block og_title_prefix %}Members | {%
+endblock %} {% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * Members
     * {% for user in users %}
     * {% if user.profile.image %} [{{user.profile.image.url}}]{% else %} [{%
       static 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
-      _{_{_ _u_s_e_r_._u_s_e_r_n_a_m_e_ _}_}
+      _{_{_ _u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_ _}_}
       Posts: {{user.profile.post_count}}
       Date Joined: {{user.date_joined | date:'m/d/Y'}}
     * {% endfor %}
 {% if users.has_other_pages %}
     * {% if users.has_previous %}
     * _P_r_e_v
     * {% else %}
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static %}
+{% load static styled_username %}
 
 {% block title_prefix %}{{ user.username }} | {% endblock%}
 {% block og_title_prefix %}{{ user.username }} | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/profile.css' %}">
 {% endblock %}
@@ -31,15 +31,15 @@
         {% if user.profile.image %}
         <img class="pw-avatar xl" src="{{user.profile.image.url}}" />
         {% else %}
         <img class="pw-avatar xl" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" />
         {% endif %}
       </div>
       <div class="profile__info__details">
-        <div class="profile__info__username">{{user.username}}</div>
+        <div class="profile__info__username">{{user|styled_username}}</div>
         <div class="profile__info__stats">
           <div class="profile__info__stat">
             Date Joined:
             <span class="profile__info__stat__value">{{user.date_joined | date:'m/d/Y'}}</span>
           </div>
           <div class="profile__info__stat">
             Last Login:
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-{% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix %}
-{{ user.username }} | {% endblock%} {% block og_title_prefix %}{{ user.username
-}} | {% endblock %} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static styled_username %} {% block
+title_prefix %}{{ user.username }} | {% endblock%} {% block og_title_prefix %}{
+{ user.username }} | {% endblock %} {% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _M_e_m_b_e_r_s
     * {{ user.username }}
 {% if user.profile.image %} [{{user.profile.image.url}}]{% else %} [{% static
 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
-{{user.username}}
+{{user|styled_username}}
 Date Joined: {{user.date_joined | date:'m/d/Y'}}
 Last Login: {{user.last_login | date:'m/d/Y'}}
 Posts: {{user.profile.post_count}}
 Threads
 {% if user.threads.count == 0 %}
 {{ user.username }} has not created any threads.
 {% else %}
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-{% load shoutbox_bbcode can_delete %}
+{% load shoutbox_bbcode can_delete styled_username %}
 
 {% for shout in shouts %}
 <div class="shoutbox__shout">
   <div class="shoutbox__shout__content">
     <span>{{shout.created_at|date:'g:i A'}}</span>
-    <span><a href="{% url 'punkweb_bb:profile' shout.user.id %}">{{shout.user.username}}</a>: </span>
+    <span><a href="{% url 'punkweb_bb:profile' shout.user.id %}">{{shout.user|styled_username}}</a>: </span>
     <span>{{ shout.content | safe | shoutbox_bbcode }}</span>
   </div>
   {% if shout|can_delete:request.user %}
   <div class="shoutbox__shout__actions">
     <button
       class="pw-icon-button default danger sm"
       title="Delete"
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{% load shoutbox_bbcode can_delete %} {% for shout in shouts %}
-{{shout.created_at|date:'g:i A'}} _{_{_s_h_o_u_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}: {{ shout.content |
-safe | shoutbox_bbcode }}
+{% load shoutbox_bbcode can_delete styled_username %} {% for shout in shouts %}
+{{shout.created_at|date:'g:i A'}} _{_{_s_h_o_u_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}: {
+{ shout.content | safe | shoutbox_bbcode }}
 {% if shout|can_delete:request.user %}
 delete
 {% endif %}
 {% endfor %}
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static humanize_int can_post %}
+{% load static humanize_int can_post styled_username %}
 
 {% block title_prefix %}{{subcategory.name}} | {% endblock%}
 {% block og_title_prefix %}{{subcategory.name}} | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/subcategory.css' %}" />
 {% endblock %}
@@ -66,18 +66,18 @@
   {% endif %}
 </div>
 
 <div class="pw-card fluid margin">
   <div class="pw-table-container">
     <table class="pw-table">
       <colgroup>
-        <col span="1">
-        <col span="1" width="96px">
-        <col span="1" width="96px">
-        <col span="1" width="160px">
+        <col>
+        <col width="96px">
+        <col width="96px">
+        <col width="192px">
       </colgroup>
       <thead>
         <tr>
           <th>Title</th>
           <th>Posts</th>
           <th>Views</th>
           <th></th>
@@ -94,15 +94,15 @@
               {% endif %}
               {% if thread.is_closed %}
               <span class="material-symbols-outlined" title="Closed">lock</span>
               {% endif %}
             </div>
             <div>
               <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
-                {{thread.user.username}}
+                {{thread.user|styled_username}}
               </a>
               •
               {{thread.created_at|date:'M j, Y'}}</div>
           </td>
           <td>{{thread.post_count}}</td>
           <td>{{thread.view_count | humanize_int}}</td>
           <td>
@@ -113,15 +113,15 @@
                   title="{{thread.latest_post.title}}">
                   <time datetime="{{thread.latest_post.created_at|date:'c'}}">
                     {{thread.latest_post.created_at|date:'M j, Y'}}
                   </time>
                 </a>
                 <div>
                   <a href="{% url 'punkweb_bb:profile' thread.latest_post.user.id %}">
-                    {{thread.latest_post.user.username}}
+                    {{thread.latest_post.user|styled_username}}
                   </a>
                 </div>
               </div>
               {% if thread.latest_post.user.profile.image %}
               <img class="pw-avatar xs" src="{{thread.latest_post.user.profile.image.url}}" />
               {% else %}
               <img class="pw-avatar xs" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" />
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-{% extends 'punkweb_bb/base.html' %} {% load static humanize_int can_post %} {%
-block title_prefix %}{{subcategory.name}} | {% endblock%} {% block
-og_title_prefix %}{{subcategory.name}} | {% endblock %} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static humanize_int can_post
+styled_username %} {% block title_prefix %}{{subcategory.name}} | {% endblock%}
+{% block og_title_prefix %}{{subcategory.name}} | {% endblock %} {% block
+extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{subcategory.name}}
 ************ {{{{ssuubbccaatteeggoorryy..nnaammee}}}} ************
 {% if perms.punkweb_bb.change_subcategory or
 perms.punkweb_bb.delete_subcategory %}
 {% if perms.punkweb_bb.change_subcategory %} _e_d_i_t_ {% endif %} {% if
 perms.punkweb_bb.delete_subcategory %} delete {% endif %}
 {% endif %}
 {% if subcategory|can_post:request.user %} _C_r_e_a_t_e_ _T_h_r_e_a_d {% else %} Create
 Thread {% endif %}
-TTiittllee                    PPoossttss                VViieewwss
-_{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                                           {% if thread.latest_post %}
-thread.is_pinned %} keep                                         _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
-{% endif %} {% if                                                _Y_'_}_}
-thread.is_closed %} lock                      {                  _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
-{% endif %}              {                    {thread.view_count {% if thread.latest_post.user.profile.image
-_{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_} {thread.post_count}} | humanize_int}}   %} [{
-â¢ {                                                            {thread.latest_post.user.profile.image.url}}]
-{thread.created_at|date:                                         {% else %} [{% static 'punkweb_bb/img/
-'M j, Y'}}                                                       default-profile-image.png' %}]{% endif %}
-                                                                 {% else %} No posts {% endif %}
+TTiittllee                          PPoossttss                VViieewwss
+_{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                                                 {% if thread.latest_post %}
+thread.is_pinned %} keep {%                                            _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
+endif %} {% if                                                         _Y_'_}_}
+thread.is_closed %} lock {%                         {                  _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
+endif %}                       {                    {thread.view_count {% if thread.latest_post.user.profile.image
+_{                              {thread.post_count}} | humanize_int}}   %} [{
+_{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}                                         {thread.latest_post.user.profile.image.url}}]
+â¢ {{thread.created_at|date:                                          {% else %} [{% static 'punkweb_bb/img/
+'M j, Y'}}                                                             default-profile-image.png' %}]{% endif %}
+                                                                       {% else %} No posts {% endif %}
 {% if threads.has_other_pages %}
     * {% if threads.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in threads.paginator.page_range %} {% if
       threads.number == i %}
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_create.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_update.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/subcategory_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static can_delete can_edit can_post %}
+{% load static can_delete can_edit can_post styled_username styled_group_name %}
 
 {% block title_prefix %}{{thread.title}} | {% endblock %}
 {% block og_title_prefix %}{{thread.title}} | {% endblock %}
 
 {% block extra_head %}
 <meta name="description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
 <meta property="og:description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
@@ -51,15 +51,15 @@
       <img class="pw-avatar" src="{% static 'punkweb_bb/img/default-profile-image.png' %}" alt="{{thread.user.username}}" />
       {% endif %}
       <div class="thread__user__usernameContainer">
         {% if thread.user.profile.is_online %}
         <div class="onlineIndicator"></div>
         {% endif %}
         <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
-          {{thread.user.username}}
+          {{thread.user|styled_username}}
         </a>
       </div>
       <div class="thread__user__info">
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Joined:</div>
           <div class="thread__user__info__value">
             {{thread.user.date_joined|date:"M d, Y"}}
@@ -69,15 +69,17 @@
           <div class="thread__user__info__label">Posts:</div>
           <div class="thread__user__info__value">{{thread.user.profile.post_count}}</div>
         </div>
       </div>
       {% if thread.user.groups.all|length > 0 %}
       <div class="thread__user__groups">
         {% for group in thread.user.groups.all %}
-        <div class="thread__user__group">{{group.name}}</div>
+        <div class="thread__user__group">
+          {{group|styled_group_name}}
+        </div>
         {% endfor %}
       </div>
       {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{thread.content.rendered}}
@@ -161,15 +163,15 @@
       </div>
       {% endif %}
       <div class="thread__user__usernameContainer">
         {% if post.user.profile.is_online %}
         <div class="onlineIndicator"></div>
         {% endif %}
         <a href="{% url 'punkweb_bb:profile' post.user.id %}">
-          {{post.user.username}}
+          {{post.user|styled_username}}
         </a>
       </div>
       <div class="thread__user__info">
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Joined:</div>
           <div class="thread__user__info__value">
             {{post.user.date_joined|date:"M d, Y"}}
@@ -179,15 +181,17 @@
           <div class="thread__user__info__label">Posts:</div>
           <div class="thread__user__info__value">{{post.user.profile.post_count}}</div>
         </div>
       </div>
       {% if post.user.groups.all|length > 0 %}
       <div class="thread__user__groups">
         {% for group in post.user.groups.all %}
-        <div class="thread__user__group">{{group.name}}</div>
+        <div class="thread__user__group">
+          {{group|styled_group_name}}
+        </div>
         {% endfor %}
       </div>
       {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{post.content.rendered}}
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
 {% extends 'punkweb_bb/base.html' %} {% load static can_delete can_edit
-can_post %} {% block title_prefix %}{{thread.title}} | {% endblock %} {% block
-og_title_prefix %}{{thread.title}} | {% endblock %} {% block extra_head %}
+can_post styled_username styled_group_name %} {% block title_prefix %}{
+{thread.title}} | {% endblock %} {% block og_title_prefix %}{{thread.title}} |
+{% endblock %} {% block extra_head %}
 {{post_form.media.css}} {% endblock %} {% block extra_script %} {
 {post_form.media.js}} {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{thread.title}}
 {% if posts.number == 1 %}
 ************ {{{{tthhrreeaadd..ttiittllee}}}} ************
 {{thread.created_at|date:'M d, Y'}}
 {% if thread.user.profile.image %} [{{thread.user.username}}]{% else %} [{
 {thread.user.username}}]{% endif %}
 {% if thread.user.profile.is_online %}
-{% endif %} _{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+{% endif %} _{_{_t_h_r_e_a_d_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 Joined:
 {{thread.user.date_joined|date:"M d, Y"}}
 Posts:
 {{thread.user.profile.post_count}}
 {% if thread.user.groups.all|length > 0 %}
 {% for group in thread.user.groups.all %}
-{{group.name}}
+{{group|styled_group_name}}
 {% endfor %}
 {% endif %}
 {{thread.content.rendered}}
 {% if thread|can_delete:request.user or thread|can_edit:request.user or
 perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
 {% if perms.punkweb_bb.pin_thread %} {% if thread.is_pinned %} keep_off {% else
 %} keep {% endif %} {% endif %} {% if perms.punkweb_bb.close_thread %} {% if
@@ -39,22 +40,22 @@
 _#_{_{_p_o_s_t_._i_n_d_e_x_}_}
 {% if post.user.profile.image %}
 [{{post.user.username}}]
 {% else %}
 [{{post.user.username}}]
 {% endif %}
 {% if post.user.profile.is_online %}
-{% endif %} _{_{_p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+{% endif %} _{_{_p_o_s_t_._u_s_e_r_|_s_t_y_l_e_d___u_s_e_r_n_a_m_e_}_}
 Joined:
 {{post.user.date_joined|date:"M d, Y"}}
 Posts:
 {{post.user.profile.post_count}}
 {% if post.user.groups.all|length > 0 %}
 {% for group in post.user.groups.all %}
-{{group.name}}
+{{group|styled_group_name}}
 {% endfor %}
 {% endif %}
 {{post.content.rendered}}
 {% if post|can_delete:request.user or post|can_edit:request.user %}
 {% if post|can_edit:request.user %} edit {% endif %} {% if post|can_delete:
 request.user %} delete {% endif %}
 {% endif %} {% if post.user.profile.signature.rendered %}
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.2.2/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.2.2/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/tests.py` & `punkweb_bb-0.2.2/punkweb_bb/tests.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/urls.py` & `punkweb_bb-0.2.2/punkweb_bb/urls.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/views.py` & `punkweb_bb-0.2.2/punkweb_bb/views.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb/widgets.py` & `punkweb_bb-0.2.2/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.1/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.2.2/punkweb_bb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.2.1
+Version: 0.2.2
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -31,15 +31,15 @@
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
 - [SCEditor](https://www.sceditor.com/)
 - [PrismJS](https://prismjs.com/)
 
 ## Requirements
 
-- Python 3.11+
+- Python 3.9+
 - Django 4.2+
 - django-precise-bbcode 1.2+
 - Pillow
 
 It may work with older versions of Python and Django, but it has not been tested.
 
 ## Installation
@@ -107,14 +107,15 @@
 These are the default settings for PunkwebBB, which can be overridden in your Django settings module:
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
   "FAVICON": "punkweb_bb/favicon.ico",
+  "OG_IMAGE": None, # Used for Open Graph meta tags, must be a full URL!
   "SHOUTBOX_ENABLED": True,
   "DISCORD_WIDGET_ENABLED": False,
   "DISCORD_WIDGET_THEME": "dark",
   "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
 ```
```

### Comparing `punkweb_bb-0.2.1/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.2.2/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,20 @@
 punkweb_bb/__pycache__/urls.cpython-311.pyc
 punkweb_bb/__pycache__/utils.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
 punkweb_bb/migrations/0002_thread_view_count.py
 punkweb_bb/migrations/0003_alter_thread_options.py
+punkweb_bb/migrations/0004_groupstyle.py
 punkweb_bb/migrations/__init__.py
 punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
+punkweb_bb/migrations/__pycache__/0004_groupstyle.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/static/punkweb_bb/favicon.ico
 punkweb_bb/static/punkweb_bb/css/category-form.css
 punkweb_bb/static/punkweb_bb/css/defaults.css
 punkweb_bb/static/punkweb_bb/css/index.css
 punkweb_bb/static/punkweb_bb/css/login.css
 punkweb_bb/static/punkweb_bb/css/members.css
@@ -233,14 +235,19 @@
 punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
 punkweb_bb/templatetags/__init__.py
 punkweb_bb/templatetags/can_delete.py
 punkweb_bb/templatetags/can_edit.py
 punkweb_bb/templatetags/can_post.py
 punkweb_bb/templatetags/humanize_int.py
 punkweb_bb/templatetags/shoutbox_bbcode.py
+punkweb_bb/templatetags/styled_group_name.py
+punkweb_bb/templatetags/styled_username.py
 punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
-punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/styled_group_name.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/styled_username.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/username.cpython-311.pyc
```

### Comparing `punkweb_bb-0.2.1/setup.py` & `punkweb_bb-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.2.1",
+    version="0.2.2",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
```

