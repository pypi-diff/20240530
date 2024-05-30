# Comparing `tmp/bk_resource-0.4.7.tar.gz` & `tmp/bk_resource-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk_resource-0.4.7.tar", last modified: Mon Nov  6 12:02:29 2023, max compression
+gzip compressed data, was "dist/bk_resource-0.4.8.tar", last modified: Tue Jan  2 11:18:48 2024, max compression
```

## Comparing `bk_resource-0.4.7.tar` & `bk_resource-0.4.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/
--rw-r--r--   0 root         (0) root         (0)      141 2023-11-06 12:02:11.000000 bk_resource-0.4.7/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource.egg-info/
--rw-r--r--   0 root         (0) root         (0)      164 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      233 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      859 2023-11-06 12:02:11.000000 bk_resource-0.4.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      233 2023-11-06 12:02:29.000000 bk_resource-0.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-06 12:02:29.000000 bk_resource-0.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2023-11-06 12:02:11.000000 bk_resource-0.4.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/
--rw-r--r--   0 root         (0) root         (0)     2690 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/utils/
--rw-r--r--   0 root         (0) root         (0)    10609 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/cache.py
--rw-r--r--   0 root         (0) root         (0)    10967 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/time_tools.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/text.py
--rw-r--r--   0 root         (0) root         (0)     3317 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/request_log.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/request.py
--rw-r--r--   0 root         (0) root         (0)    13205 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/common_utils.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/local.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/generators.py
--rw-r--r--   0 root         (0) root         (0)     5104 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/factory.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/inspectors.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5017 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/utils/thread_backend.py
--rw-r--r--   0 root         (0) root         (0)     4064 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/tasks.py
--rw-r--r--   0 root         (0) root         (0)    14062 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/base.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/settings.py
--rw-r--r--   0 root         (0) root         (0)    11699 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/viewsets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     2943 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 root         (0) root         (0)     4322 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/locale/zh_CN/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3022 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 root         (0) root         (0)     4398 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 root         (0) root         (0)     2058 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/apps.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/routers.py
--rw-r--r--   0 root         (0) root         (0)     3883 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/management/
--rw-r--r--   0 root         (0) root         (0)     4859 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/finder.py
--rw-r--r--   0 root         (0) root         (0)     4974 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/stub_file_generator.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10304 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/management/commands/
--rw-r--r--   0 root         (0) root         (0)      891 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/commands/generate_resource_stub_file.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/management/commands/start_resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/conf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/conf/app_template/
--rw-r--r--   0 root         (0) root         (0)       60 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/admin.py-tpl
--rw-r--r--   0 root         (0) root         (0)       54 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/models.py-tpl
--rw-r--r--   0 root         (0) root         (0)       24 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/__init__.py-tpl
--rw-r--r--   0 root         (0) root         (0)      173 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/views.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/conf/app_template/migrations/
--rw-r--r--   0 root         (0) root         (0)       24 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/migrations/__init__.py-tpl
--rw-r--r--   0 root         (0) root         (0)       64 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/serializers.py-tpl
--rw-r--r--   0 root         (0) root         (0)      152 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/resources.py-tpl
--rw-r--r--   0 root         (0) root         (0)      196 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/apps.py-tpl
--rw-r--r--   0 root         (0) root         (0)      189 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/app_template/urls.py-tpl
--rw-r--r--   0 root         (0) root         (0)      891 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8166 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 12:02:29.000000 bk_resource-0.4.7/bk_resource/contrib/
--rw-r--r--   0 root         (0) root         (0)     2969 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/contrib/cache.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/contrib/model.py
--rw-r--r--   0 root         (0) root         (0)     1121 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8658 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/contrib/api.py
--rw-r--r--   0 root         (0) root         (0)     6007 2023-11-06 12:02:11.000000 bk_resource-0.4.7/bk_resource/contrib/bk_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/locale/zh_CN/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 root         (0) root         (0)     4398 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 root         (0) root         (0)     4322 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/utils/
+-rw-r--r--   0 root         (0) root         (0)      950 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/inspectors.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5104 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/factory.py
+-rw-r--r--   0 root         (0) root         (0)    13205 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/common_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/request_log.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/text.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/generators.py
+-rw-r--r--   0 root         (0) root         (0)     5017 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/thread_backend.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/request.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/local.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/time_tools.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/utils/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/routers.py
+-rw-r--r--   0 root         (0) root         (0)    14062 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/management/
+-rw-r--r--   0 root         (0) root         (0)     4859 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/finder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/commands/generate_resource_stub_file.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/commands/start_resource.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/stub_file_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    10304 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/management/root.py
+-rw-r--r--   0 root         (0) root         (0)     4064 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3883 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/conf/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/conf/app_template/
+-rw-r--r--   0 root         (0) root         (0)       24 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      189 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/urls.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       60 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/admin.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/conf/app_template/migrations/
+-rw-r--r--   0 root         (0) root         (0)       24 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/migrations/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       64 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/serializers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      152 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/resources.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       54 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/models.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      173 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/views.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      196 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/conf/app_template/apps.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/serializers.py
+-rw-r--r--   0 root         (0) root         (0)     8166 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/tools.py
+-rw-r--r--   0 root         (0) root         (0)    11699 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/viewsets.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource/contrib/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6304 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/contrib/bk_api.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/contrib/model.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/contrib/api.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2024-01-02 11:18:32.000000 bk_resource-0.4.8/bk_resource/contrib/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-01-02 11:18:32.000000 bk_resource-0.4.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)      233 2024-01-02 11:18:48.000000 bk_resource-0.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-02 11:18:48.000000 bk_resource-0.4.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2024-01-02 11:18:32.000000 bk_resource-0.4.8/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       12 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-02 11:18:48.000000 bk_resource-0.4.8/bk_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-01-02 11:18:32.000000 bk_resource-0.4.8/MANIFEST.in
```

### Comparing `bk_resource-0.4.7/bk_resource.egg-info/SOURCES.txt` & `bk_resource-0.4.8/bk_resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/LICENSE.txt` & `bk_resource-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/setup.py` & `bk_resource-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 to the current version of the project delivered to anyone in the future.
 """
 
 from setuptools import setup
 
 setup(
     name="bk_resource",
-    version="0.4.7",
+    version="0.4.8",
     author="blueking",
     url="https://bk.tencent.com",
     author_email="blueking@tencent.com",
     description="Bk Resource",
     packages=[
         "bk_resource",
         "bk_resource.conf",
```

### Comparing `bk_resource-0.4.7/bk_resource/serializers.py` & `bk_resource-0.4.8/bk_resource/serializers.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/cache.py` & `bk_resource-0.4.8/bk_resource/utils/cache.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/time_tools.py` & `bk_resource-0.4.8/bk_resource/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/text.py` & `bk_resource-0.4.8/bk_resource/utils/text.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/request_log.py` & `bk_resource-0.4.8/bk_resource/utils/request_log.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/request.py` & `bk_resource-0.4.8/bk_resource/utils/request.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/common_utils.py` & `bk_resource-0.4.8/bk_resource/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/local.py` & `bk_resource-0.4.8/bk_resource/utils/local.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/logger.py` & `bk_resource-0.4.8/bk_resource/utils/logger.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/generators.py` & `bk_resource-0.4.8/bk_resource/utils/generators.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/factory.py` & `bk_resource-0.4.8/bk_resource/utils/factory.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/inspectors.py` & `bk_resource-0.4.8/bk_resource/utils/inspectors.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/__init__.py` & `bk_resource-0.4.8/bk_resource/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/utils/thread_backend.py` & `bk_resource-0.4.8/bk_resource/utils/thread_backend.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/tasks.py` & `bk_resource-0.4.8/bk_resource/tasks.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/base.py` & `bk_resource-0.4.8/bk_resource/base.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/settings.py` & `bk_resource-0.4.8/bk_resource/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         REQUEST_LOG_HANDLER="bk_resource.utils.request_log.RequestLogHandler",
         REQUEST_LOG_SPLIT_LENGTH=0,
         REQUEST_VERIFY=True,
         PLATFORM_AUTH_ENABLED=False,
         PLATFORM_AUTH_ACCESS_TOKEN=None,
         PLATFORM_AUTH_ACCESS_USERNAME=None,
         REQUEST_BKAPI_COOKIE_FIELDS=["blueking_language", "django_language"],
+        REQUEST_LANGUGAE_HEADER_KEY="blueking-language",
         RESOURCE_BULK_REQUEST_PROCESSES=None,
     )
 
     LAZY_IMPORT_SETTINGS = (
         "DEFAULT_ERROR_RESPONSE_SERIALIZER",
         "DEFAULT_PAGINATOR_RESPONSE_BUILDER",
         "DEFAULT_STANDARD_RESPONSE_BUILDER",
```

### Comparing `bk_resource-0.4.7/bk_resource/viewsets.py` & `bk_resource-0.4.8/bk_resource/viewsets.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/locale/en/LC_MESSAGES/django.mo` & `bk_resource-0.4.8/bk_resource/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/locale/en/LC_MESSAGES/django.po` & `bk_resource-0.4.8/bk_resource/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo` & `bk_resource-0.4.8/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/locale/zh_CN/LC_MESSAGES/django.po` & `bk_resource-0.4.8/bk_resource/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/__init__.py` & `bk_resource-0.4.8/bk_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/apps.py` & `bk_resource-0.4.8/bk_resource/apps.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/routers.py` & `bk_resource-0.4.8/bk_resource/routers.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/exceptions.py` & `bk_resource-0.4.8/bk_resource/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/finder.py` & `bk_resource-0.4.8/bk_resource/management/finder.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/stub_file_generator.py` & `bk_resource-0.4.8/bk_resource/management/stub_file_generator.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/__init__.py` & `bk_resource-0.4.8/bk_resource/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/exceptions.py` & `bk_resource-0.4.8/bk_resource/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/root.py` & `bk_resource-0.4.8/bk_resource/management/root.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/commands/__init__.py` & `bk_resource-0.4.8/bk_resource/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/commands/generate_resource_stub_file.py` & `bk_resource-0.4.8/bk_resource/management/commands/generate_resource_stub_file.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/management/commands/start_resource.py` & `bk_resource-0.4.8/bk_resource/management/commands/start_resource.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/conf/__init__.py` & `bk_resource-0.4.8/bk_resource/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/tools.py` & `bk_resource-0.4.8/bk_resource/tools.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/contrib/cache.py` & `bk_resource-0.4.8/bk_resource/contrib/cache.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/contrib/model.py` & `bk_resource-0.4.8/bk_resource/contrib/model.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/contrib/__init__.py` & `bk_resource-0.4.8/bk_resource/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/contrib/api.py` & `bk_resource-0.4.8/bk_resource/contrib/api.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.7/bk_resource/contrib/bk_api.py` & `bk_resource-0.4.8/bk_resource/contrib/bk_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,26 +126,30 @@
         """
         构造Header
         """
 
         from blueapps.utils.request_provider import get_local_request
 
         # 初始化
-        headers = {}
+        headers = {bk_resource_settings.REQUEST_LANGUGAE_HEADER_KEY: settings.LANGUAGE_CODE}
 
         # 透传 Cookie
         request = get_local_request()
         if request is not None:
             headers["cookie"] = "; ".join(
                 [
                     f"{key}={val}"
                     for key, val in request.COOKIES.items()
                     if key in bk_resource_settings.REQUEST_BKAPI_COOKIE_FIELDS
                 ]
             )
+            # 根据用户的Cookie指定语言
+            headers[bk_resource_settings.REQUEST_LANGUGAE_HEADER_KEY] = request.COOKIES.get(
+                settings.LANGUAGE_COOKIE_NAME, settings.LANGUAGE_CODE
+            )
 
         # 鉴权参数
         if self.bkapi_header_authorization:
             params = {
                 "_request": validated_request_data.pop("_request", None),
                 "_is_backend": validated_request_data.pop("_is_backend", False),
             }
```

