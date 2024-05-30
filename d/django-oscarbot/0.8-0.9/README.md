# Comparing `tmp/django-oscarbot-0.8.tar.gz` & `tmp/django-oscarbot-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscarbot-0.8.tar", last modified: Sun Jan 14 14:01:05 2024, max compression
+gzip compressed data, was "django-oscarbot-0.9.tar", last modified: Sun Jan 14 20:35:29 2024, max compression
```

## Comparing `django-oscarbot-0.8.tar` & `django-oscarbot-0.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.210961 django-oscarbot-0.8/
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1082 2023-10-10 16:03:53.000000 django-oscarbot-0.8/LICENSE
--rw-r--r--   0 olegmaslov   (501) staff       (20)       79 2023-12-17 12:33:49.000000 django-oscarbot-0.8/MANIFEST.in
--rw-r--r--   0 olegmaslov   (501) staff       (20)     4469 2024-01-14 14:01:05.210851 django-oscarbot-0.8/PKG-INFO
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1981 2024-01-11 17:56:48.000000 django-oscarbot-0.8/README.md
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.188673 django-oscarbot-0.8/api/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-08-16 18:24:01.000000 django-oscarbot-0.8/api/__init__.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      138 2023-09-28 08:38:39.000000 django-oscarbot-0.8/api/apps.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      142 2023-10-09 15:19:14.000000 django-oscarbot-0.8/api/urls.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.192659 django-oscarbot-0.8/config/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-09 15:29:27.000000 django-oscarbot-0.8/config/__init__.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      389 2023-10-09 15:29:27.000000 django-oscarbot-0.8/config/asgi.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     3549 2024-01-14 08:03:39.000000 django-oscarbot-0.8/config/settings.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      809 2023-10-09 15:48:41.000000 django-oscarbot-0.8/config/urls.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      389 2023-10-09 15:29:27.000000 django-oscarbot-0.8/config/wsgi.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.210325 django-oscarbot-0.8/django_oscarbot.egg-info/
--rw-r--r--   0 olegmaslov   (501) staff       (20)     4469 2024-01-14 14:01:05.000000 django-oscarbot-0.8/django_oscarbot.egg-info/PKG-INFO
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2661 2024-01-14 14:01:05.000000 django-oscarbot-0.8/django_oscarbot.egg-info/SOURCES.txt
--rw-r--r--   0 olegmaslov   (501) staff       (20)        1 2024-01-14 14:01:05.000000 django-oscarbot-0.8/django_oscarbot.egg-info/dependency_links.txt
--rw-r--r--   0 olegmaslov   (501) staff       (20)       55 2024-01-14 14:01:05.000000 django-oscarbot-0.8/django_oscarbot.egg-info/requires.txt
--rw-r--r--   0 olegmaslov   (501) staff       (20)       28 2024-01-14 14:01:05.000000 django-oscarbot-0.8/django_oscarbot.egg-info/top_level.txt
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.195895 django-oscarbot-0.8/example/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-12-17 12:22:29.000000 django-oscarbot-0.8/example/__init__.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      160 2024-01-14 12:54:04.000000 django-oscarbot-0.8/example/actions.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)       63 2023-12-17 12:22:29.000000 django-oscarbot-0.8/example/admin.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      146 2023-12-17 12:22:29.000000 django-oscarbot-0.8/example/apps.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.196204 django-oscarbot-0.8/example/migrations/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-12-17 12:22:29.000000 django-oscarbot-0.8/example/migrations/__init__.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)       57 2023-12-17 12:22:29.000000 django-oscarbot-0.8/example/models.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      167 2024-01-14 12:19:05.000000 django-oscarbot-0.8/example/router.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)       60 2023-12-17 12:22:29.000000 django-oscarbot-0.8/example/tests.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      383 2024-01-14 12:49:06.000000 django-oscarbot-0.8/example/text_processor.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      647 2024-01-14 13:36:42.000000 django-oscarbot-0.8/example/views.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.200154 django-oscarbot-0.8/oscarbot/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-09 15:13:55.000000 django-oscarbot-0.8/oscarbot/__init__.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.205207 django-oscarbot-0.8/oscarbot/__pycache__/
--rw-r--r--   0 olegmaslov   (501) staff       (20)      166 2023-10-09 15:40:27.000000 django-oscarbot-0.8/oscarbot/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2578 2024-01-14 12:53:51.000000 django-oscarbot-0.8/oscarbot/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      659 2023-10-09 18:46:32.000000 django-oscarbot-0.8/oscarbot/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      541 2023-10-09 15:40:27.000000 django-oscarbot-0.8/oscarbot/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     6596 2023-10-16 18:15:27.000000 django-oscarbot-0.8/oscarbot/__pycache__/bot.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     5158 2024-01-14 14:00:41.000000 django-oscarbot-0.8/oscarbot/__pycache__/handler.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2525 2024-01-12 06:07:38.000000 django-oscarbot-0.8/oscarbot/__pycache__/menu.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     3658 2024-01-14 14:00:41.000000 django-oscarbot-0.8/oscarbot/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1835 2024-01-11 17:50:36.000000 django-oscarbot-0.8/oscarbot/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     4499 2024-01-11 17:42:31.000000 django-oscarbot-0.8/oscarbot/__pycache__/router.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      807 2023-10-09 18:45:11.000000 django-oscarbot-0.8/oscarbot/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2508 2023-10-16 17:59:39.000000 django-oscarbot-0.8/oscarbot/__pycache__/shortcut.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     3502 2023-10-09 20:04:40.000000 django-oscarbot-0.8/oscarbot/__pycache__/structures.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2787 2023-12-17 12:29:12.000000 django-oscarbot-0.8/oscarbot/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1814 2024-01-14 13:27:06.000000 django-oscarbot-0.8/oscarbot/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1335 2024-01-14 12:53:49.000000 django-oscarbot-0.8/oscarbot/action.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      207 2023-10-09 18:46:31.000000 django-oscarbot-0.8/oscarbot/admin.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      148 2023-10-09 15:13:55.000000 django-oscarbot-0.8/oscarbot/apps.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     4676 2023-10-16 18:14:50.000000 django-oscarbot-0.8/oscarbot/bot.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      146 2023-12-14 14:39:50.000000 django-oscarbot-0.8/oscarbot/exceptions.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2821 2024-01-14 13:36:31.000000 django-oscarbot-0.8/oscarbot/handler.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.205559 django-oscarbot-0.8/oscarbot/management/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-10 10:59:20.000000 django-oscarbot-0.8/oscarbot/management/__init__.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.205671 django-oscarbot-0.8/oscarbot/management/__pycache__/
--rw-r--r--   0 olegmaslov   (501) staff       (20)      177 2023-10-10 11:04:58.000000 django-oscarbot-0.8/oscarbot/management/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.206000 django-oscarbot-0.8/oscarbot/management/commands/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-10 10:59:25.000000 django-oscarbot-0.8/oscarbot/management/commands/__init__.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.206414 django-oscarbot-0.8/oscarbot/management/commands/__pycache__/
--rw-r--r--   0 olegmaslov   (501) staff       (20)      186 2023-10-10 11:04:58.000000 django-oscarbot-0.8/oscarbot/management/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2186 2023-10-10 15:36:26.000000 django-oscarbot-0.8/oscarbot/management/commands/__pycache__/runbot.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1110 2023-10-10 15:36:26.000000 django-oscarbot-0.8/oscarbot/management/commands/runbot.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1606 2024-01-12 06:07:33.000000 django-oscarbot-0.8/oscarbot/menu.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.208154 django-oscarbot-0.8/oscarbot/migrations/
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1002 2023-10-09 15:41:32.000000 django-oscarbot-0.8/oscarbot/migrations/0001_initial.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1340 2023-10-09 18:53:33.000000 django-oscarbot-0.8/oscarbot/migrations/0002_message_user.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      467 2023-10-10 10:39:45.000000 django-oscarbot-0.8/oscarbot/migrations/0003_user_last_message_id.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      414 2023-10-10 14:29:01.000000 django-oscarbot-0.8/oscarbot/migrations/0004_user_want_action.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      461 2024-01-14 13:00:41.000000 django-oscarbot-0.8/oscarbot/migrations/0005_constructor.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      395 2024-01-14 14:00:41.000000 django-oscarbot-0.8/oscarbot/migrations/0006_user_state_information.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-09 15:13:55.000000 django-oscarbot-0.8/oscarbot/migrations/__init__.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.209724 django-oscarbot-0.8/oscarbot/migrations/__pycache__/
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1432 2023-10-09 15:41:39.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1798 2023-10-09 18:53:37.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/0002_message_user.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      915 2023-10-10 10:39:48.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/0003_user_last_message_id.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      843 2023-10-10 14:29:05.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/0004_user_want_action.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      872 2024-01-14 14:00:41.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/0005_constructor.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      825 2024-01-14 14:00:44.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/0006_user_state_information.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)      177 2023-10-09 15:41:32.000000 django-oscarbot-0.8/oscarbot/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1701 2024-01-14 14:00:35.000000 django-oscarbot-0.8/oscarbot/models.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1085 2024-01-11 17:50:29.000000 django-oscarbot-0.8/oscarbot/response.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)       23 2023-08-16 18:24:01.000000 django-oscarbot-0.8/oscarbot/result.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     2092 2024-01-11 17:39:37.000000 django-oscarbot-0.8/oscarbot/router.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      320 2023-10-09 18:45:00.000000 django-oscarbot-0.8/oscarbot/services.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1370 2023-12-17 12:25:15.000000 django-oscarbot-0.8/oscarbot/shortcut.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1536 2023-10-09 20:04:39.000000 django-oscarbot-0.8/oscarbot/structures.py
-drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 14:01:05.210157 django-oscarbot-0.8/oscarbot/tests/
--rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2024-01-11 17:39:55.000000 django-oscarbot-0.8/oscarbot/tests/__init__.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1883 2023-12-17 12:28:40.000000 django-oscarbot-0.8/oscarbot/tests.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)      882 2024-01-14 13:27:05.000000 django-oscarbot-0.8/oscarbot/views.py
--rw-r--r--   0 olegmaslov   (501) staff       (20)     1253 2024-01-14 14:00:49.000000 django-oscarbot-0.8/pyproject.toml
--rw-r--r--   0 olegmaslov   (501) staff       (20)      896 2024-01-14 14:01:05.211213 django-oscarbot-0.8/setup.cfg
--rw-r--r--   0 olegmaslov   (501) staff       (20)       38 2023-10-11 20:03:04.000000 django-oscarbot-0.8/setup.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.960147 django-oscarbot-0.9/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1082 2023-10-10 16:03:53.000000 django-oscarbot-0.9/LICENSE
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       79 2023-12-17 12:33:49.000000 django-oscarbot-0.9/MANIFEST.in
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     4469 2024-01-14 20:35:29.959982 django-oscarbot-0.9/PKG-INFO
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1981 2024-01-11 17:56:48.000000 django-oscarbot-0.9/README.md
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.927985 django-oscarbot-0.9/api/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-08-16 18:24:01.000000 django-oscarbot-0.9/api/__init__.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      138 2023-09-28 08:38:39.000000 django-oscarbot-0.9/api/apps.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      142 2023-10-09 15:19:14.000000 django-oscarbot-0.9/api/urls.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.929866 django-oscarbot-0.9/config/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-09 15:29:27.000000 django-oscarbot-0.9/config/__init__.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      389 2023-10-09 15:29:27.000000 django-oscarbot-0.9/config/asgi.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     3549 2024-01-14 08:03:39.000000 django-oscarbot-0.9/config/settings.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      809 2023-10-09 15:48:41.000000 django-oscarbot-0.9/config/urls.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      389 2023-10-09 15:29:27.000000 django-oscarbot-0.9/config/wsgi.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.955462 django-oscarbot-0.9/django_oscarbot.egg-info/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     4469 2024-01-14 20:35:29.000000 django-oscarbot-0.9/django_oscarbot.egg-info/PKG-INFO
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2661 2024-01-14 20:35:29.000000 django-oscarbot-0.9/django_oscarbot.egg-info/SOURCES.txt
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        1 2024-01-14 20:35:29.000000 django-oscarbot-0.9/django_oscarbot.egg-info/dependency_links.txt
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       55 2024-01-14 20:35:29.000000 django-oscarbot-0.9/django_oscarbot.egg-info/requires.txt
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       28 2024-01-14 20:35:29.000000 django-oscarbot-0.9/django_oscarbot.egg-info/top_level.txt
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.933908 django-oscarbot-0.9/example/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-12-17 12:22:29.000000 django-oscarbot-0.9/example/__init__.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      160 2024-01-14 12:54:04.000000 django-oscarbot-0.9/example/actions.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       63 2023-12-17 12:22:29.000000 django-oscarbot-0.9/example/admin.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      146 2023-12-17 12:22:29.000000 django-oscarbot-0.9/example/apps.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.934237 django-oscarbot-0.9/example/migrations/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-12-17 12:22:29.000000 django-oscarbot-0.9/example/migrations/__init__.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       57 2023-12-17 12:22:29.000000 django-oscarbot-0.9/example/models.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      167 2024-01-14 12:19:05.000000 django-oscarbot-0.9/example/router.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       60 2023-12-17 12:22:29.000000 django-oscarbot-0.9/example/tests.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      383 2024-01-14 12:49:06.000000 django-oscarbot-0.9/example/text_processor.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      647 2024-01-14 13:36:42.000000 django-oscarbot-0.9/example/views.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.940056 django-oscarbot-0.9/oscarbot/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-09 15:13:55.000000 django-oscarbot-0.9/oscarbot/__init__.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.947858 django-oscarbot-0.9/oscarbot/__pycache__/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      166 2023-10-09 15:40:27.000000 django-oscarbot-0.9/oscarbot/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2578 2024-01-14 12:53:51.000000 django-oscarbot-0.9/oscarbot/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      659 2023-10-09 18:46:32.000000 django-oscarbot-0.9/oscarbot/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      541 2023-10-09 15:40:27.000000 django-oscarbot-0.9/oscarbot/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     6596 2023-10-16 18:15:27.000000 django-oscarbot-0.9/oscarbot/__pycache__/bot.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     5158 2024-01-14 14:00:41.000000 django-oscarbot-0.9/oscarbot/__pycache__/handler.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2525 2024-01-12 06:07:38.000000 django-oscarbot-0.9/oscarbot/__pycache__/menu.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     3658 2024-01-14 14:00:41.000000 django-oscarbot-0.9/oscarbot/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1835 2024-01-11 17:50:36.000000 django-oscarbot-0.9/oscarbot/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     4499 2024-01-11 17:42:31.000000 django-oscarbot-0.9/oscarbot/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      807 2023-10-09 18:45:11.000000 django-oscarbot-0.9/oscarbot/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2508 2023-10-16 17:59:39.000000 django-oscarbot-0.9/oscarbot/__pycache__/shortcut.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     3502 2023-10-09 20:04:40.000000 django-oscarbot-0.9/oscarbot/__pycache__/structures.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2787 2023-12-17 12:29:12.000000 django-oscarbot-0.9/oscarbot/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1814 2024-01-14 13:27:06.000000 django-oscarbot-0.9/oscarbot/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1335 2024-01-14 12:53:49.000000 django-oscarbot-0.9/oscarbot/action.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      207 2023-10-09 18:46:31.000000 django-oscarbot-0.9/oscarbot/admin.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      148 2023-10-09 15:13:55.000000 django-oscarbot-0.9/oscarbot/apps.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     4676 2023-10-16 18:14:50.000000 django-oscarbot-0.9/oscarbot/bot.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      146 2023-12-14 14:39:50.000000 django-oscarbot-0.9/oscarbot/exceptions.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2821 2024-01-14 13:36:31.000000 django-oscarbot-0.9/oscarbot/handler.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.948150 django-oscarbot-0.9/oscarbot/management/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-10 10:59:20.000000 django-oscarbot-0.9/oscarbot/management/__init__.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.948297 django-oscarbot-0.9/oscarbot/management/__pycache__/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      177 2023-10-10 11:04:58.000000 django-oscarbot-0.9/oscarbot/management/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.948691 django-oscarbot-0.9/oscarbot/management/commands/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-10 10:59:25.000000 django-oscarbot-0.9/oscarbot/management/commands/__init__.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.949197 django-oscarbot-0.9/oscarbot/management/commands/__pycache__/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      186 2023-10-10 11:04:58.000000 django-oscarbot-0.9/oscarbot/management/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2186 2023-10-10 15:36:26.000000 django-oscarbot-0.9/oscarbot/management/commands/__pycache__/runbot.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1110 2023-10-10 15:36:26.000000 django-oscarbot-0.9/oscarbot/management/commands/runbot.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1606 2024-01-12 06:07:33.000000 django-oscarbot-0.9/oscarbot/menu.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.951161 django-oscarbot-0.9/oscarbot/migrations/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1002 2023-10-09 15:41:32.000000 django-oscarbot-0.9/oscarbot/migrations/0001_initial.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1340 2023-10-09 18:53:33.000000 django-oscarbot-0.9/oscarbot/migrations/0002_message_user.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      467 2023-10-10 10:39:45.000000 django-oscarbot-0.9/oscarbot/migrations/0003_user_last_message_id.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      414 2023-10-10 14:29:01.000000 django-oscarbot-0.9/oscarbot/migrations/0004_user_want_action.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      461 2024-01-14 13:00:41.000000 django-oscarbot-0.9/oscarbot/migrations/0005_constructor.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      395 2024-01-14 14:00:41.000000 django-oscarbot-0.9/oscarbot/migrations/0006_user_state_information.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2023-10-09 15:13:55.000000 django-oscarbot-0.9/oscarbot/migrations/__init__.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.953284 django-oscarbot-0.9/oscarbot/migrations/__pycache__/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1432 2023-10-09 15:41:39.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1798 2023-10-09 18:53:37.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/0002_message_user.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      915 2023-10-10 10:39:48.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/0003_user_last_message_id.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      843 2023-10-10 14:29:05.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/0004_user_want_action.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      872 2024-01-14 14:00:41.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/0005_constructor.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      825 2024-01-14 14:00:44.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/0006_user_state_information.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      177 2023-10-09 15:41:32.000000 django-oscarbot-0.9/oscarbot/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1701 2024-01-14 14:00:35.000000 django-oscarbot-0.9/oscarbot/models.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1085 2024-01-11 17:50:29.000000 django-oscarbot-0.9/oscarbot/response.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       23 2023-08-16 18:24:01.000000 django-oscarbot-0.9/oscarbot/result.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     2092 2024-01-11 17:39:37.000000 django-oscarbot-0.9/oscarbot/router.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      320 2023-10-09 18:45:00.000000 django-oscarbot-0.9/oscarbot/services.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1370 2023-12-17 12:25:15.000000 django-oscarbot-0.9/oscarbot/shortcut.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1536 2023-10-09 20:04:39.000000 django-oscarbot-0.9/oscarbot/structures.py
+drwxr-xr-x   0 olegmaslov   (501) staff       (20)        0 2024-01-14 20:35:29.953567 django-oscarbot-0.9/oscarbot/tests/
+-rw-r--r--   0 olegmaslov   (501) staff       (20)        0 2024-01-11 17:39:55.000000 django-oscarbot-0.9/oscarbot/tests/__init__.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1883 2023-12-17 12:28:40.000000 django-oscarbot-0.9/oscarbot/tests.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      912 2024-01-14 20:34:57.000000 django-oscarbot-0.9/oscarbot/views.py
+-rw-r--r--   0 olegmaslov   (501) staff       (20)     1253 2024-01-14 20:35:05.000000 django-oscarbot-0.9/pyproject.toml
+-rw-r--r--   0 olegmaslov   (501) staff       (20)      896 2024-01-14 20:35:29.964497 django-oscarbot-0.9/setup.cfg
+-rw-r--r--   0 olegmaslov   (501) staff       (20)       38 2023-10-11 20:03:04.000000 django-oscarbot-0.9/setup.py
```

### Comparing `django-oscarbot-0.8/LICENSE` & `django-oscarbot-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/PKG-INFO` & `django-oscarbot-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscarbot
-Version: 0.8
+Version: 0.9
 Summary: Django app for create Telegram bot
 Home-page: https://oscarbot.site/
 Author: Oleg Maslov
 Author-email: Oleg Maslov <info@oscar-studio.com>
 License: Copyright (c) 2023 Oleg Maslov (https://oscar-studio.com/)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-oscarbot-0.8/README.md` & `django-oscarbot-0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/config/settings.py` & `django-oscarbot-0.9/config/settings.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/config/urls.py` & `django-oscarbot-0.9/config/urls.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/django_oscarbot.egg-info/PKG-INFO` & `django-oscarbot-0.9/django_oscarbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscarbot
-Version: 0.8
+Version: 0.9
 Summary: Django app for create Telegram bot
 Home-page: https://oscarbot.site/
 Author: Oleg Maslov
 Author-email: Oleg Maslov <info@oscar-studio.com>
 License: Copyright (c) 2023 Oleg Maslov (https://oscar-studio.com/)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-oscarbot-0.8/django_oscarbot.egg-info/SOURCES.txt` & `django-oscarbot-0.9/django_oscarbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/example/views.py` & `django-oscarbot-0.9/example/views.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/action.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/admin.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/apps.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/bot.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/bot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/handler.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/menu.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/models.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/response.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/response.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/router.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/services.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/shortcut.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/shortcut.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/structures.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/structures.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/tests.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/tests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/__pycache__/views.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/__pycache__/views.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/action.py` & `django-oscarbot-0.9/oscarbot/action.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/bot.py` & `django-oscarbot-0.9/oscarbot/bot.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/handler.py` & `django-oscarbot-0.9/oscarbot/handler.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/management/commands/__pycache__/runbot.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/management/commands/__pycache__/runbot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/management/commands/runbot.py` & `django-oscarbot-0.9/oscarbot/management/commands/runbot.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/menu.py` & `django-oscarbot-0.9/oscarbot/menu.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/0001_initial.py` & `django-oscarbot-0.9/oscarbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/0002_message_user.py` & `django-oscarbot-0.9/oscarbot/migrations/0002_message_user.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/__pycache__/0002_message_user.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/migrations/__pycache__/0002_message_user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/__pycache__/0003_user_last_message_id.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/migrations/__pycache__/0003_user_last_message_id.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/__pycache__/0004_user_want_action.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/migrations/__pycache__/0004_user_want_action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/__pycache__/0005_constructor.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/migrations/__pycache__/0005_constructor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/migrations/__pycache__/0006_user_state_information.cpython-311.pyc` & `django-oscarbot-0.9/oscarbot/migrations/__pycache__/0006_user_state_information.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/models.py` & `django-oscarbot-0.9/oscarbot/models.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/response.py` & `django-oscarbot-0.9/oscarbot/response.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/router.py` & `django-oscarbot-0.9/oscarbot/router.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/shortcut.py` & `django-oscarbot-0.9/oscarbot/shortcut.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/structures.py` & `django-oscarbot-0.9/oscarbot/structures.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/tests.py` & `django-oscarbot-0.9/oscarbot/tests.py`

 * *Files identical despite different names*

### Comparing `django-oscarbot-0.8/oscarbot/views.py` & `django-oscarbot-0.9/oscarbot/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 @csrf_exempt
 def bot_view(request, token):
     if request.method == 'POST':
         body = request.body.decode('utf-8')
         body = body.replace('\n', '')
         content = json.loads(body)
-        handle_content(token, content)
+        print(content)
+        return handle_content(token, content)
 
 
 def handle_content(token, content):
     bot_model = get_bot_model()
     current_bot = bot_model.objects.filter(token=token).first()
     if current_bot:
         handler = BaseHandler(current_bot, content)
```

### Comparing `django-oscarbot-0.8/pyproject.toml` & `django-oscarbot-0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-oscarbot"
-version = "0.8"
+version = "0.9"
 description = "Django app for create Telegram bot"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 keywords = ["django", "telegram"]
 authors = [
```

### Comparing `django-oscarbot-0.8/setup.cfg` & `django-oscarbot-0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-oscarbot
-version = 0.8
+version = 0.9
 description = Django app for create Telegram bot.
 long_description = file: README.rst
 url = https://oscarbot.site/
 author = Oleg Maslov
 author_email = info@oscar-studio.com
 license = BSD-3-Clause
 classifiers =
```

