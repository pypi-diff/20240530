# Comparing `tmp/django-project-base-0.75.32.tar.gz` & `tmp/django-project-base-0.75.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-base-0.75.32.tar", last modified: Tue May 28 14:10:11 2024, max compression
+gzip compressed data, was "django-project-base-0.75.33.tar", last modified: Thu May 30 14:50:29 2024, max compression
```

## Comparing `django-project-base-0.75.32.tar` & `django-project-base-0.75.33.tar`

### file list

```diff
@@ -1,228 +1,231 @@
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.745048 django-project-base-0.75.32/
--rw-r--r--   0 jure      (1000) jure      (1000)      116 2024-05-28 06:15:49.000000 django-project-base-0.75.32/MANIFEST.in
--rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-28 14:10:11.741048 django-project-base-0.75.32/PKG-INFO
--rw-r--r--   0 jure      (1000) jure      (1000)     1006 2024-05-28 06:15:49.000000 django-project-base-0.75.32/README.md
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base/
--rw-r--r--   0 jure      (1000) jure      (1000)      309 2024-05-28 14:09:55.000000 django-project-base-0.75.32/django_project_base/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/
--rw-r--r--   0 jure      (1000) jure      (1000)      168 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      420 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/apps.py
--rw-r--r--   0 jure      (1000) jure      (1000)      182 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/constants.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/management/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/management/commands/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1834 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/management/commands/allauth_to_social_core.py
--rw-r--r--   0 jure      (1000) jure      (1000)      664 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/management/commands/delete_users.py
--rw-r--r--   0 jure      (1000) jure      (1000)     3602 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/middleware.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.75.32/django_project_base/account/rest/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)    13904 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/account.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5208 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/impersonate.py
--rw-r--r--   0 jure      (1000) jure      (1000)     6815 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/invite.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5766 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/login.py
--rw-r--r--   0 jure      (1000) jure      (1000)    28708 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/profile.py
--rw-r--r--   0 jure      (1000) jure      (1000)     6048 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/profile_merge.py
--rw-r--r--   0 jure      (1000) jure      (1000)    11582 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/project_profiles.py
--rw-r--r--   0 jure      (1000) jure      (1000)     6639 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/project_profiles_utils.py
--rw-r--r--   0 jure      (1000) jure      (1000)     6529 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/reset_password.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2360 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/router.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/service/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5836 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/merge_users_service.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1392 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/register_user_service.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2504 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/reset_password_email_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/settings.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/social_auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/social_auth/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1581 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/social_auth/providers.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2244 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/social_auth/settings.py
--rw-r--r--   0 jure      (1000) jure      (1000)      226 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/urls.py
--rw-r--r--   0 jure      (1000) jure      (1000)      355 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/auth/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)       77 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/admin.py
--rw-r--r--   0 jure      (1000) jure      (1000)      160 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/auth/migrations/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/migrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      738 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/models.py
--rw-r--r--   0 jure      (1000) jure      (1000)       74 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/tests.py
--rw-r--r--   0 jure      (1000) jure      (1000)       77 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/views.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/aws/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/aws/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1769 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/aws/ses.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/base/
--rw-r--r--   0 jure      (1000) jure      (1000)       48 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1815 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/auth_backends.py
--rw-r--r--   0 jure      (1000) jure      (1000)     9026 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/event.py
--rw-r--r--   0 jure      (1000) jure      (1000)      304 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/exceptions.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2793 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/fields.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1731 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/middleware.py
--rw-r--r--   0 jure      (1000) jure      (1000)    12932 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/models.py
--rw-r--r--   0 jure      (1000) jure      (1000)     3901 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/permissions.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1991 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/queryset_with_cache.py
--rw-r--r--   0 jure      (1000) jure      (1000)      494 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/signals.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/caching/
--rw-r--r--   0 jure      (1000) jure      (1000)      980 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/caching/cache_queue/
--rw-r--r--   0 jure      (1000) jure      (1000)     2378 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/cache_queue/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2084 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/cache_queue/cache_queue_other.py
--rw-r--r--   0 jure      (1000) jure      (1000)      959 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/cache_queue/cache_queue_redis.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/celery/
--rw-r--r--   0 jure      (1000) jure      (1000)       85 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      187 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/celery/background_tasks/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/background_tasks/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1743 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/background_tasks/base_task.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1721 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/background_tasks/notification_tasks.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2533 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/celery.py
--rw-r--r--   0 jure      (1000) jure      (1000)      327 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/settings.py
--rw-r--r--   0 jure      (1000) jure      (1000)      447 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/constants.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1336 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/country_holidays.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/licensing/
--rw-r--r--   0 jure      (1000) jure      (1000)       98 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      190 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/apps.py
--rw-r--r--   0 jure      (1000) jure      (1000)     4439 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/logic.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/licensing/migrations/
--rw-r--r--   0 jure      (1000) jure      (1000)     1767 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/0001_initial.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2065 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
--rw-r--r--   0 jure      (1000) jure      (1000)      550 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      940 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/models.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/licensing/rest/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/rest/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      944 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/rest/rest.py
--rw-r--r--   0 jure      (1000) jure      (1000)      243 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/rest/router.py
--rw-r--r--   0 jure      (1000) jure      (1000)      175 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/urls.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.425044 django-project-base-0.75.32/django_project_base/locale/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.425044 django-project-base-0.75.32/django_project_base/locale/en/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/
--rw-r--r--   0 jure      (1000) jure      (1000)      380 2024-02-27 08:45:40.000000 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 jure      (1000) jure      (1000)    14046 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 jure      (1000) jure      (1000)     4562 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.425044 django-project-base-0.75.32/django_project_base/locale/sl/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/
--rw-r--r--   0 jure      (1000) jure      (1000)     6828 2024-02-27 08:45:40.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 jure      (1000) jure      (1000)    16384 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.po
--rw-r--r--   0 jure      (1000) jure      (1000)     3731 2024-02-27 08:45:40.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 jure      (1000) jure      (1000)     6150 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/management/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/management/commands/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/commands/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1791 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/commands/confirm_setting.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1621 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/commands/list_pending_settings.py
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/models.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/
--rw-r--r--   0 jure      (1000) jure      (1000)      162 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.75.32/django_project_base/notifications/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/base/channels/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)    11421 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/channel.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     4694 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_ses.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2832 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2676 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2980 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/provider_integration.py
--rw-r--r--   0 jure      (1000) jure      (1000)    10301 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/t2.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2012 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/mail_channel.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1321 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/sms_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/websocket_channel.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1613 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/duplicate_notification_mixin.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1411 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/enums.py
--rw-r--r--   0 jure      (1000) jure      (1000)    12558 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/notification.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1581 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/phone_number_parser.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1407 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/queable_notification_mixin.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5636 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/send_notification_service.py
--rw-r--r--   0 jure      (1000) jure      (1000)       59 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/constants.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5829 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/email_notification.py
--rw-r--r--   0 jure      (1000) jure      (1000)      975 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/maintenance_notification.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/management/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/management/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/management/commands/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/management/commands/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      900 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/management/commands/resend_notification.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/migrations/
--rw-r--r--   0 jure      (1000) jure      (1000)     6404 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0001_initial.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1086 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
--rw-r--r--   0 jure      (1000) jure      (1000)      413 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
--rw-r--r--   0 jure      (1000) jure      (1000)      393 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
--rw-r--r--   0 jure      (1000) jure      (1000)      412 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2533 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1501 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1458 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1056 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
--rw-r--r--   0 jure      (1000) jure      (1000)      448 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1410 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
--rw-r--r--   0 jure      (1000) jure      (1000)      412 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0010_djangoprojectbasenotification_extra_data.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     9789 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/models.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1201 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/notification_queryset.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/rest/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     3136 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/delivery_report.py
--rw-r--r--   0 jure      (1000) jure      (1000)     9090 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/maintenance_notification.py
--rw-r--r--   0 jure      (1000) jure      (1000)    23543 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/notification.py
--rw-r--r--   0 jure      (1000) jure      (1000)      934 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/router.py
--rw-r--r--   0 jure      (1000) jure      (1000)      943 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/settings.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/templates/
--rw-r--r--   0 jure      (1000) jure      (1000)      368 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/templates/account_created.html
--rw-r--r--   0 jure      (1000) jure      (1000)     4339 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/templates/notification.html
--rw-r--r--   0 jure      (1000) jure      (1000)     2614 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/templates/notification_login.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/tests/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/tests/api/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2427 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_create_mail.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2196 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_list_mail.py
--rw-r--r--   0 jure      (1000) jure      (1000)      864 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_remainig_license.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1485 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_retrieve_mail.py
--rw-r--r--   0 jure      (1000) jure      (1000)     3332 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/notifications_transaction_test_case.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/tests/unit/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/unit/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     2941 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_mail_sent.py
--rw-r--r--   0 jure      (1000) jure      (1000)      543 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
--rw-r--r--   0 jure      (1000) jure      (1000)      177 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/utils.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/permissions/
--rw-r--r--   0 jure      (1000) jure      (1000)     1082 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/permissions/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/profiling/
--rw-r--r--   0 jure      (1000) jure      (1000)       89 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/profiling/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     9135 2024-05-28 14:09:12.000000 django-project-base-0.75.32/django_project_base/profiling/middleware.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1040 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/profiling/performance_base_command.py
--rw-r--r--   0 jure      (1000) jure      (1000)     3754 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/profiling/views.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.75.32/django_project_base/rest/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)    18501 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/rest/project.py
--rw-r--r--   0 jure      (1000) jure      (1000)     4000 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/rest/project_role.py
--rw-r--r--   0 jure      (1000) jure      (1000)     4094 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/router.py
--rw-r--r--   0 jure      (1000) jure      (1000)      705 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/serialization.py
--rw-r--r--   0 jure      (1000) jure      (1000)     4017 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/settings.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1677 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/settings_parser.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base/static/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/static/browser-update/
--rw-r--r--   0 jure      (1000) jure      (1000)      421 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/static/browser-update/browser-update.js
--rw-r--r--   0 jure      (1000) jure      (1000)     9484 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/static/browser-update/update.min.js
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base/templates/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.741048 django-project-base-0.75.32/django_project_base/templates/app-debug/
--rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/templates/app-debug/main.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.741048 django-project-base-0.75.32/django_project_base/templates/email/
--rw-r--r--   0 jure      (1000) jure      (1000)      169 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/templates/email/base.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.741048 django-project-base-0.75.32/django_project_base/templatetags/
--rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/templatetags/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)      200 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/templatetags/dpb_tags.py
--rw-r--r--   0 jure      (1000) jure      (1000)      907 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/urls.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5824 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/utils.py
--rw-r--r--   0 jure      (1000) jure      (1000)      913 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/views.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base.egg-info/
--rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/PKG-INFO
--rw-r--r--   0 jure      (1000) jure      (1000)     9270 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/SOURCES.txt
--rw-r--r--   0 jure      (1000) jure      (1000)        1 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/dependency_links.txt
--rw-r--r--   0 jure      (1000) jure      (1000)      308 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/requires.txt
--rw-r--r--   0 jure      (1000) jure      (1000)       20 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/top_level.txt
--rw-r--r--   0 jure      (1000) jure      (1000)     1305 2024-05-28 06:15:49.000000 django-project-base-0.75.32/pyproject.toml
--rw-r--r--   0 jure      (1000) jure      (1000)      311 2024-05-28 13:56:03.000000 django-project-base-0.75.32/requirements.txt
--rw-r--r--   0 jure      (1000) jure      (1000)       38 2024-05-28 14:10:11.745048 django-project-base-0.75.32/setup.cfg
--rwxr-xr-x   0 jure      (1000) jure      (1000)     3354 2024-05-28 06:15:49.000000 django-project-base-0.75.32/setup.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.256242 django-project-base-0.75.33/
+-rw-r--r--   0 jure      (1000) jure      (1000)      116 2024-05-28 06:15:49.000000 django-project-base-0.75.33/MANIFEST.in
+-rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-30 14:50:29.256242 django-project-base-0.75.33/PKG-INFO
+-rw-r--r--   0 jure      (1000) jure      (1000)     1006 2024-05-28 06:15:49.000000 django-project-base-0.75.33/README.md
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.040239 django-project-base-0.75.33/django_project_base/
+-rw-r--r--   0 jure      (1000) jure      (1000)      309 2024-05-30 14:49:53.000000 django-project-base-0.75.33/django_project_base/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.044240 django-project-base-0.75.33/django_project_base/account/
+-rw-r--r--   0 jure      (1000) jure      (1000)      168 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      420 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/apps.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      182 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/constants.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.044240 django-project-base-0.75.33/django_project_base/account/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.33/django_project_base/account/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.044240 django-project-base-0.75.33/django_project_base/account/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.33/django_project_base/account/management/commands/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1834 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/management/commands/allauth_to_social_core.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      664 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/management/commands/delete_users.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3602 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/middleware.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.048240 django-project-base-0.75.33/django_project_base/account/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.75.33/django_project_base/account/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    13904 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/account.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5208 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/impersonate.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6815 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/invite.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5766 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/login.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    28708 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/profile.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6048 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/profile_merge.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    11582 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/project_profiles.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6639 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/project_profiles_utils.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6529 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/rest/reset_password.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2360 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/router.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.048240 django-project-base-0.75.33/django_project_base/account/service/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/service/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5836 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/service/merge_users_service.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1392 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/service/register_user_service.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2504 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/service/reset_password_email_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.75.33/django_project_base/account/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.048240 django-project-base-0.75.33/django_project_base/account/social_auth/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.33/django_project_base/account/social_auth/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1581 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/social_auth/providers.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2244 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/social_auth/settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      226 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/account/urls.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      355 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.048240 django-project-base-0.75.33/django_project_base/auth/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       77 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/admin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      160 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.048240 django-project-base-0.75.33/django_project_base/auth/migrations/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      738 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/models.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       74 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/tests.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       77 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/auth/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.048240 django-project-base-0.75.33/django_project_base/aws/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/aws/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1769 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/aws/ses.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.052240 django-project-base-0.75.33/django_project_base/base/
+-rw-r--r--   0 jure      (1000) jure      (1000)       48 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1815 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/auth_backends.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9026 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/event.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      304 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/exceptions.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2793 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/fields.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1731 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/middleware.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    12932 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/models.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3901 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/permissions.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1991 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/queryset_with_cache.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      494 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/base/signals.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.052240 django-project-base-0.75.33/django_project_base/caching/
+-rw-r--r--   0 jure      (1000) jure      (1000)      980 2024-05-28 13:56:15.000000 django-project-base-0.75.33/django_project_base/caching/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.052240 django-project-base-0.75.33/django_project_base/caching/cache_queue/
+-rw-r--r--   0 jure      (1000) jure      (1000)     2378 2024-05-28 13:56:15.000000 django-project-base-0.75.33/django_project_base/caching/cache_queue/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2084 2024-05-28 13:56:15.000000 django-project-base-0.75.33/django_project_base/caching/cache_queue/cache_queue_other.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      959 2024-05-28 13:56:15.000000 django-project-base-0.75.33/django_project_base/caching/cache_queue/cache_queue_redis.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.052240 django-project-base-0.75.33/django_project_base/celery/
+-rw-r--r--   0 jure      (1000) jure      (1000)       85 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      187 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.052240 django-project-base-0.75.33/django_project_base/celery/background_tasks/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/background_tasks/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1743 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/background_tasks/base_task.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1721 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/background_tasks/notification_tasks.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2533 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/celery.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      327 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/celery/settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      447 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/constants.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1336 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/country_holidays.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.056240 django-project-base-0.75.33/django_project_base/licensing/
+-rw-r--r--   0 jure      (1000) jure      (1000)       98 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      190 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/apps.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4439 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/logic.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.056240 django-project-base-0.75.33/django_project_base/licensing/migrations/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1767 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/migrations/0001_initial.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2065 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      550 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      940 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/models.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.056240 django-project-base-0.75.33/django_project_base/licensing/rest/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      944 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/rest/rest.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      243 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/rest/router.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      175 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/licensing/urls.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.036239 django-project-base-0.75.33/django_project_base/locale/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.036239 django-project-base-0.75.33/django_project_base/locale/en/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.056240 django-project-base-0.75.33/django_project_base/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jure      (1000) jure      (1000)      380 2024-02-27 08:45:40.000000 django-project-base-0.75.33/django_project_base/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jure      (1000) jure      (1000)    14046 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 jure      (1000) jure      (1000)     4562 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.036239 django-project-base-0.75.33/django_project_base/locale/sl/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.060240 django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 jure      (1000) jure      (1000)     6828 2024-02-27 08:45:40.000000 django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jure      (1000) jure      (1000)    16384 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0 jure      (1000) jure      (1000)     3731 2024-02-27 08:45:40.000000 django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 jure      (1000) jure      (1000)     6150 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.060240 django-project-base-0.75.33/django_project_base/management/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.060240 django-project-base-0.75.33/django_project_base/management/commands/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/management/commands/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1791 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/management/commands/confirm_setting.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1621 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/management/commands/list_pending_settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/models.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.064240 django-project-base-0.75.33/django_project_base/notifications/
+-rw-r--r--   0 jure      (1000) jure      (1000)      162 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.75.33/django_project_base/notifications/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.064240 django-project-base-0.75.33/django_project_base/notifications/base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/notifications/base/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.064240 django-project-base-0.75.33/django_project_base/notifications/base/channels/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    11421 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/channel.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.068240 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4694 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/aws_ses.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2832 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2676 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2980 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/provider_integration.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    10301 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/t2.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2012 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/mail_channel.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1321 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/sms_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/notifications/base/channels/websocket_channel.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1613 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/duplicate_notification_mixin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1411 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/enums.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    12558 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1581 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/phone_number_parser.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1407 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/queable_notification_mixin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5636 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/base/send_notification_service.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       59 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/constants.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5829 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/email_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      975 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/maintenance_notification.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.068240 django-project-base-0.75.33/django_project_base/notifications/management/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.068240 django-project-base-0.75.33/django_project_base/notifications/management/commands/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/management/commands/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      900 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/management/commands/resend_notification.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.068240 django-project-base-0.75.33/django_project_base/notifications/migrations/
+-rw-r--r--   0 jure      (1000) jure      (1000)     6404 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0001_initial.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1086 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      413 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      393 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      412 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2533 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1501 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1458 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1056 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      448 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1410 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      412 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/0010_djangoprojectbasenotification_extra_data.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/notifications/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9789 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/models.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1201 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/notification_queryset.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.068240 django-project-base-0.75.33/django_project_base/notifications/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/notifications/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3136 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/rest/delivery_report.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9090 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/rest/maintenance_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    23543 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/rest/notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      934 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/rest/router.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      943 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/notifications/templates/
+-rw-r--r--   0 jure      (1000) jure      (1000)      368 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/templates/account_created.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     4339 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/templates/notification.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     2614 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/templates/notification_login.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/notifications/tests/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/notifications/tests/api/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/api/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2427 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/api/test_create_mail.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2196 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/api/test_list_mail.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      864 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/api/test_remainig_license.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1485 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/api/test_retrieve_mail.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3332 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/notifications_transaction_test_case.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/notifications/tests/unit/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/unit/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2941 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/unit/test_is_mail_sent.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      543 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      177 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/notifications/utils.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/permissions/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1082 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/permissions/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/profiling/
+-rw-r--r--   0 jure      (1000) jure      (1000)       89 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/profiling/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9135 2024-05-28 14:09:12.000000 django-project-base-0.75.33/django_project_base/profiling/middleware.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1040 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/profiling/performance_base_command.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3754 2024-05-28 13:56:15.000000 django-project-base-0.75.33/django_project_base/profiling/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/query_tracker/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-22 04:42:55.000000 django-project-base-0.75.33/django_project_base/query_tracker/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4924 2024-05-30 14:47:10.000000 django-project-base-0.75.33/django_project_base/query_tracker/base.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.072240 django-project-base-0.75.33/django_project_base/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.75.33/django_project_base/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    18501 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/rest/project.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4000 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/rest/project_role.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4094 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/router.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      705 2024-05-28 13:56:15.000000 django-project-base-0.75.33/django_project_base/serialization.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4017 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1677 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/settings_parser.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.036239 django-project-base-0.75.33/django_project_base/static/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.252242 django-project-base-0.75.33/django_project_base/static/browser-update/
+-rw-r--r--   0 jure      (1000) jure      (1000)      421 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/static/browser-update/browser-update.js
+-rw-r--r--   0 jure      (1000) jure      (1000)     9484 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/static/browser-update/update.min.js
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.040239 django-project-base-0.75.33/django_project_base/templates/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.256242 django-project-base-0.75.33/django_project_base/templates/app-debug/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.75.33/django_project_base/templates/app-debug/main.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.256242 django-project-base-0.75.33/django_project_base/templates/email/
+-rw-r--r--   0 jure      (1000) jure      (1000)      169 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/templates/email/base.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.256242 django-project-base-0.75.33/django_project_base/templatetags/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/templatetags/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      200 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/templatetags/dpb_tags.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      907 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/urls.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5824 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/utils.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      913 2024-05-28 06:15:49.000000 django-project-base-0.75.33/django_project_base/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-30 14:50:29.044240 django-project-base-0.75.33/django_project_base.egg-info/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-30 14:50:28.000000 django-project-base-0.75.33/django_project_base.egg-info/PKG-INFO
+-rw-r--r--   0 jure      (1000) jure      (1000)     9358 2024-05-30 14:50:29.000000 django-project-base-0.75.33/django_project_base.egg-info/SOURCES.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)        1 2024-05-30 14:50:28.000000 django-project-base-0.75.33/django_project_base.egg-info/dependency_links.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)      308 2024-05-30 14:50:28.000000 django-project-base-0.75.33/django_project_base.egg-info/requires.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       20 2024-05-30 14:50:28.000000 django-project-base-0.75.33/django_project_base.egg-info/top_level.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)     1305 2024-05-28 06:15:49.000000 django-project-base-0.75.33/pyproject.toml
+-rw-r--r--   0 jure      (1000) jure      (1000)      311 2024-05-28 13:56:03.000000 django-project-base-0.75.33/requirements.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       38 2024-05-30 14:50:29.256242 django-project-base-0.75.33/setup.cfg
+-rwxr-xr-x   0 jure      (1000) jure      (1000)     3354 2024-05-28 06:15:49.000000 django-project-base-0.75.33/setup.py
```

### Comparing `django-project-base-0.75.32/PKG-INFO` & `django-project-base-0.75.33/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.75.32
+Version: 0.75.33
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-project-base-0.75.32/README.md` & `django-project-base-0.75.33/README.md`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/management/commands/allauth_to_social_core.py` & `django-project-base-0.75.33/django_project_base/account/management/commands/allauth_to_social_core.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/management/commands/delete_users.py` & `django-project-base-0.75.33/django_project_base/account/management/commands/delete_users.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/middleware.py` & `django-project-base-0.75.33/django_project_base/account/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/account.py` & `django-project-base-0.75.33/django_project_base/account/rest/account.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/impersonate.py` & `django-project-base-0.75.33/django_project_base/account/rest/impersonate.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/invite.py` & `django-project-base-0.75.33/django_project_base/account/rest/invite.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/login.py` & `django-project-base-0.75.33/django_project_base/account/rest/login.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/profile.py` & `django-project-base-0.75.33/django_project_base/account/rest/profile.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/profile_merge.py` & `django-project-base-0.75.33/django_project_base/account/rest/profile_merge.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/project_profiles.py` & `django-project-base-0.75.33/django_project_base/account/rest/project_profiles.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/project_profiles_utils.py` & `django-project-base-0.75.33/django_project_base/account/rest/project_profiles_utils.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/rest/reset_password.py` & `django-project-base-0.75.33/django_project_base/account/rest/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/router.py` & `django-project-base-0.75.33/django_project_base/account/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/service/merge_users_service.py` & `django-project-base-0.75.33/django_project_base/account/service/merge_users_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/service/register_user_service.py` & `django-project-base-0.75.33/django_project_base/account/service/register_user_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/service/reset_password_email_service.py` & `django-project-base-0.75.33/django_project_base/account/service/reset_password_email_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/social_auth/providers.py` & `django-project-base-0.75.33/django_project_base/account/social_auth/providers.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/account/social_auth/settings.py` & `django-project-base-0.75.33/django_project_base/account/social_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/auth/models.py` & `django-project-base-0.75.33/django_project_base/auth/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/aws/ses.py` & `django-project-base-0.75.33/django_project_base/aws/ses.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/auth_backends.py` & `django-project-base-0.75.33/django_project_base/base/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/event.py` & `django-project-base-0.75.33/django_project_base/base/event.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/fields.py` & `django-project-base-0.75.33/django_project_base/base/fields.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/middleware.py` & `django-project-base-0.75.33/django_project_base/base/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/models.py` & `django-project-base-0.75.33/django_project_base/base/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/permissions.py` & `django-project-base-0.75.33/django_project_base/base/permissions.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/base/queryset_with_cache.py` & `django-project-base-0.75.33/django_project_base/base/queryset_with_cache.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/caching/__init__.py` & `django-project-base-0.75.33/django_project_base/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/caching/cache_queue/__init__.py` & `django-project-base-0.75.33/django_project_base/caching/cache_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/caching/cache_queue/cache_queue_other.py` & `django-project-base-0.75.33/django_project_base/caching/cache_queue/cache_queue_other.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/caching/cache_queue/cache_queue_redis.py` & `django-project-base-0.75.33/django_project_base/caching/cache_queue/cache_queue_redis.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/celery/background_tasks/base_task.py` & `django-project-base-0.75.33/django_project_base/celery/background_tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/celery/background_tasks/notification_tasks.py` & `django-project-base-0.75.33/django_project_base/celery/background_tasks/notification_tasks.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/celery/celery.py` & `django-project-base-0.75.33/django_project_base/celery/celery.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/country_holidays.py` & `django-project-base-0.75.33/django_project_base/country_holidays.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/licensing/logic.py` & `django-project-base-0.75.33/django_project_base/licensing/logic.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/licensing/migrations/0001_initial.py` & `django-project-base-0.75.33/django_project_base/licensing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py` & `django-project-base-0.75.33/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/licensing/migrations/0005_auto_20230901_0613.py` & `django-project-base-0.75.33/django_project_base/licensing/migrations/0005_auto_20230901_0613.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/licensing/models.py` & `django-project-base-0.75.33/django_project_base/licensing/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/licensing/rest/rest.py` & `django-project-base-0.75.33/django_project_base/licensing/rest/rest.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/django.po` & `django-project-base-0.75.33/django_project_base/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/djangojs.po` & `django-project-base-0.75.33/django_project_base/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.mo` & `django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.po` & `django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo` & `django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.po` & `django-project-base-0.75.33/django_project_base/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/management/commands/confirm_setting.py` & `django-project-base-0.75.33/django_project_base/management/commands/confirm_setting.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/management/commands/list_pending_settings.py` & `django-project-base-0.75.33/django_project_base/management/commands/list_pending_settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/channel.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_ses.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/aws_ses.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/nexmo_sms.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/nexmo_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/provider_integration.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/provider_integration.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/t2.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/integrations/t2.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/mail_channel.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/mail_channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/channels/sms_channel.py` & `django-project-base-0.75.33/django_project_base/notifications/base/channels/sms_channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/duplicate_notification_mixin.py` & `django-project-base-0.75.33/django_project_base/notifications/base/duplicate_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/enums.py` & `django-project-base-0.75.33/django_project_base/notifications/base/enums.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/notification.py` & `django-project-base-0.75.33/django_project_base/notifications/base/notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/phone_number_parser.py` & `django-project-base-0.75.33/django_project_base/notifications/base/phone_number_parser.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/queable_notification_mixin.py` & `django-project-base-0.75.33/django_project_base/notifications/base/queable_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/base/send_notification_service.py` & `django-project-base-0.75.33/django_project_base/notifications/base/send_notification_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/email_notification.py` & `django-project-base-0.75.33/django_project_base/notifications/email_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/maintenance_notification.py` & `django-project-base-0.75.33/django_project_base/notifications/maintenance_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/management/commands/resend_notification.py` & `django-project-base-0.75.33/django_project_base/notifications/management/commands/resend_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0001_initial.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0005_merge_20230906_1213.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0005_merge_20230906_1213.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0007_auto_20231026_0555.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0007_auto_20231026_0555.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/migrations/0009_auto_20231108_0658.py` & `django-project-base-0.75.33/django_project_base/notifications/migrations/0009_auto_20231108_0658.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/models.py` & `django-project-base-0.75.33/django_project_base/notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/notification_queryset.py` & `django-project-base-0.75.33/django_project_base/notifications/notification_queryset.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/rest/delivery_report.py` & `django-project-base-0.75.33/django_project_base/notifications/rest/delivery_report.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/rest/maintenance_notification.py` & `django-project-base-0.75.33/django_project_base/notifications/rest/maintenance_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/rest/notification.py` & `django-project-base-0.75.33/django_project_base/notifications/rest/notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/rest/router.py` & `django-project-base-0.75.33/django_project_base/notifications/rest/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/settings.py` & `django-project-base-0.75.33/django_project_base/notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/templates/notification.html` & `django-project-base-0.75.33/django_project_base/notifications/templates/notification.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/templates/notification_login.html` & `django-project-base-0.75.33/django_project_base/notifications/templates/notification_login.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_create_mail.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/api/test_create_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_list_mail.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/api/test_list_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_remainig_license.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/api/test_remainig_license.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_retrieve_mail.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/api/test_retrieve_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/notifications_transaction_test_case.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/notifications_transaction_test_case.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_mail_sent.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/unit/test_is_mail_sent.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py` & `django-project-base-0.75.33/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/permissions/__init__.py` & `django-project-base-0.75.33/django_project_base/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/profiling/middleware.py` & `django-project-base-0.75.33/django_project_base/profiling/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/profiling/performance_base_command.py` & `django-project-base-0.75.33/django_project_base/profiling/performance_base_command.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/profiling/views.py` & `django-project-base-0.75.33/django_project_base/profiling/views.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/rest/project.py` & `django-project-base-0.75.33/django_project_base/rest/project.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/rest/project_role.py` & `django-project-base-0.75.33/django_project_base/rest/project_role.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/router.py` & `django-project-base-0.75.33/django_project_base/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/serialization.py` & `django-project-base-0.75.33/django_project_base/serialization.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/settings.py` & `django-project-base-0.75.33/django_project_base/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/settings_parser.py` & `django-project-base-0.75.33/django_project_base/settings_parser.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/static/browser-update/update.min.js` & `django-project-base-0.75.33/django_project_base/static/browser-update/update.min.js`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/templates/app-debug/main.html` & `django-project-base-0.75.33/django_project_base/templates/app-debug/main.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/urls.py` & `django-project-base-0.75.33/django_project_base/urls.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/utils.py` & `django-project-base-0.75.33/django_project_base/utils.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base/views.py` & `django-project-base-0.75.33/django_project_base/views.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/django_project_base.egg-info/PKG-INFO` & `django-project-base-0.75.33/django_project_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.75.32
+Version: 0.75.33
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-project-base-0.75.32/django_project_base.egg-info/SOURCES.txt` & `django-project-base-0.75.33/django_project_base.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,16 @@
 django_project_base/notifications/tests/unit/test_is_mail_sent.py
 django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
 django_project_base/permissions/__init__.py
 django_project_base/profiling/__init__.py
 django_project_base/profiling/middleware.py
 django_project_base/profiling/performance_base_command.py
 django_project_base/profiling/views.py
+django_project_base/query_tracker/__init__.py
+django_project_base/query_tracker/base.py
 django_project_base/rest/__init__.py
 django_project_base/rest/project.py
 django_project_base/rest/project_role.py
 django_project_base/static/browser-update/browser-update.js
 django_project_base/static/browser-update/update.min.js
 django_project_base/templates/app-debug/main.html
 django_project_base/templates/email/base.html
```

### Comparing `django-project-base-0.75.32/pyproject.toml` & `django-project-base-0.75.33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.32/setup.py` & `django-project-base-0.75.33/setup.py`

 * *Files identical despite different names*

