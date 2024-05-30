# Comparing `tmp/djangorestframework_simplejwt_mongoengine-1.2.1.tar.gz` & `tmp/djangorestframework_simplejwt_mongoengine-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework_simplejwt_mongoengine-1.2.1.tar", last modified: Wed Jan 18 02:23:14 2023, max compression
+gzip compressed data, was "djangorestframework_simplejwt_mongoengine-1.3.0.tar", last modified: Thu May 30 15:04:00 2024, max compression
```

## Comparing `djangorestframework_simplejwt_mongoengine-1.2.1.tar` & `djangorestframework_simplejwt_mongoengine-1.3.0.tar`

### file list

```diff
@@ -1,111 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.158636 djangorestframework_simplejwt_mongoengine-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-01-18 02:23:14.158636 djangorestframework_simplejwt_mongoengine-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.146636 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-01-18 02:23:14.000000 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-01-18 02:23:14.000000 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 02:23:14.000000 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 02:23:13.000000 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-18 02:23:14.000000 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-18 02:23:14.000000 djangorestframework_simplejwt_mongoengine-1.2.1/djangorestframework_simplejwt_mongoengine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.150636 djangorestframework_simplejwt_mongoengine-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/blacklist_app.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5177 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/creating_tokens_manually.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/customizing_token_claims.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/stateless_user_authentication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/docs/token_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.150636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.146636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.150636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/de_CH/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.150636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/de_CH/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/de_CH/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.150636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_CL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fa_IR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/id_ID/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.142635 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.146636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.146636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.146636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/uk_UA/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.146636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.154636 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/management/commands/flushexpiredtokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-01-18 02:23:14.158636 djangorestframework_simplejwt_mongoengine-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:23:14.158636 djangorestframework_simplejwt_mongoengine-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    21502 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_token_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13130 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-18 02:22:57.000000 djangorestframework_simplejwt_mongoengine-1.2.1/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.962225 djangorestframework_simplejwt_mongoengine-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-30 15:04:00.962225 djangorestframework_simplejwt_mongoengine-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.958225 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:03:39.000000 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/djangorestframework_simplejwt_mongoengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.942225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.934225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.934225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.934225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.934225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_CL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.946225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fa_IR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/he_IL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/he_IL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/he_IL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/id_ID/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pl_PL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.950225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ru_RU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.938225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.942225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.942225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/uk_UA/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.942225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-30 15:04:00.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.954225 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/management/commands/flushexpiredtokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-30 15:04:00.962225 djangorestframework_simplejwt_mongoengine-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:04:00.958225 djangorestframework_simplejwt_mongoengine-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_token_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-05-30 15:03:24.000000 djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_views.py
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/LICENSE` & `djangorestframework_simplejwt_mongoengine-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/PKG-INFO` & `djangorestframework_simplejwt_mongoengine-1.3.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,37 @@
-Metadata-Version: 2.1
-Name: djangorestframework_simplejwt_mongoengine
-Version: 1.2.1
-Summary: Simple JWT is a JSON Web Token authentication plugin for the Django REST Framework which to be compatible with MongoEngine.
-Home-page: https://github.com/ngocngoan/djangorestframework-simplejwt-mongoengine
-Author: Đỗ Ngọc Ngoạn (aka Ngoan Do)
-Author-email: ngocngoan060288@gmail.com
-License: GNU General Public License v3
-Keywords: djangorestframework_simplejwt_mongoengine
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.8
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-|PyPI version| |Build Status| |Docs badge| |Code Style| |Pyup| |License|
+|PyPI Version| |Python Version| |Django Version| |GitHub Actions| |Code Style| |License|
 
 ======================
 Simple JWT MongoEngine
 ======================
 
 
-.. |PyPI version| image:: https://img.shields.io/pypi/v/djangorestframework-simplejwt-mongoengine.svg
-        :target: https://pypi.python.org/pypi/djangorestframework-simplejwt-mongoengine
-
-.. |Build Status| image:: https://img.shields.io/travis/ngocngoan/djangorestframework-simplejwt-mongoengine.svg
-        :target: https://travis-ci.com/ngocngoan/djangorestframework-simplejwt-mongoengine
-
-.. |Docs badge| image:: https://readthedocs.org/projects/djangorestframework-simplejwt-mongoengine/badge/?version=latest
-        :target: https://djangorestframework-simplejwt-mongoengine.readthedocs.io/en/latest/
-        :alt: Documentation Status
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/djangorestframework-simplejwt-mongoengine
+   :target: https://github.com/ngocngoan/djangorestframework-simplejwt-mongoengine
+   :alt: PyPI - Version
+
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/djangorestframework-simplejwt-mongoengine
+   :target: https://github.com/ngocngoan/djangorestframework-simplejwt-mongoengine/blob/main/LICENSE
+   :alt: Python Version
+
+.. |Django Version| image:: https://img.shields.io/pypi/frameworkversions/django/djangorestframework-simplejwt-mongoengine
+   :target: https://github.com/django
+   :alt: Django Version
+
+.. |GitHub Actions| image:: https://img.shields.io/github/actions/workflow/status/ngocngoan/djangorestframework-simplejwt-mongoengine/test.yaml
+   :target: https://github.com/ngocngoan/djangorestframework-simplejwt-mongoengine/actions
+   :alt: GitHub Actions Workflow Status
 
 .. |Code Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/ambv/black
-
-
-.. |Pyup| image:: https://pyup.io/repos/github/ngocngoan/djangorestframework-simplejwt-mongoengine/shield.svg
-     :target: https://pyup.io/repos/github/ngocngoan/djangorestframework-simplejwt-mongoengine/
-     :alt: Updates
-
-.. |License| image:: https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg
-    :target: COPYING
-    :alt: Repository License
+   :target: https://github.com/psf/black
+   :alt: Black Format
 
+.. |License| image:: https://img.shields.io/github/license/ngocngoan/djangorestframework-simplejwt-mongoengine
+   :target: https://github.com/ngocngoan/djangorestframework-simplejwt-mongoengine/blob/main/LICENSE
+   :alt: Repository License
 
 
 Simple JWT MongoEngine is a JSON Web Token authentication plugin for the `Django REST Framework`_
 which to be compatible with `MongoEngine`_. It is re-written from `Simple JWT`_.
 
 .. _`Django REST Framework`: http://www.django-rest-framework.org
 .. _`MongoEngine`: http://mongoengine.org
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/authentication.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/authentication.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,79 @@
+from typing import Optional, Set, Tuple, TypeVar
+
 from django.utils.translation import gettext_lazy as _
 from django_mongoengine.mongo_auth.managers import get_user_document
-from rest_framework import HTTP_HEADER_ENCODING
-from rest_framework_simplejwt.authentication import JWTAuthentication as SimpleJWTAuthentication
-from rest_framework_simplejwt.exceptions import AuthenticationFailed, InvalidToken, TokenError
+from django_mongoengine.mongo_auth.models import AbstractUser
+from rest_framework import HTTP_HEADER_ENCODING, authentication
+from rest_framework.request import Request
 
+from .exceptions import AuthenticationFailed, InvalidToken, TokenError
+from .models import TokenUser
 from .settings import api_settings
+from .tokens import Token
+from .utils import get_md5_hash_password
 
 AUTH_HEADER_TYPES = api_settings.AUTH_HEADER_TYPES
 
 if not isinstance(api_settings.AUTH_HEADER_TYPES, (list, tuple)):
     AUTH_HEADER_TYPES = (AUTH_HEADER_TYPES,)
 
-AUTH_HEADER_TYPE_BYTES = {h.encode(HTTP_HEADER_ENCODING) for h in AUTH_HEADER_TYPES}
+AUTH_HEADER_TYPE_BYTES: Set[bytes] = {
+    h.encode(HTTP_HEADER_ENCODING) for h in AUTH_HEADER_TYPES
+}
+
+AuthUser = TypeVar("AuthUser", AbstractUser, TokenUser)
 
 
-class JWTAuthentication(SimpleJWTAuthentication):
+class JWTAuthentication(authentication.BaseAuthentication):
     """
     An authentication plugin that authenticates requests through a JSON web
     token provided in a request header.
     """
 
     www_authenticate_realm = "api"
     media_type = "application/json"
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.user_model = get_user_document()
 
-    def authenticate(self, request):
+    def authenticate(self, request: Request) -> Optional[Tuple[AuthUser, Token]]:
         header = self.get_header(request)
         if header is None:
             return None
 
         raw_token = self.get_raw_token(header)
         if raw_token is None:
             return None
 
         validated_token = self.get_validated_token(raw_token)
 
         return self.get_user(validated_token), validated_token
 
-    def authenticate_header(self, request):
+    def authenticate_header(self, request: Request) -> str:
         return '{} realm="{}"'.format(
             AUTH_HEADER_TYPES[0],
             self.www_authenticate_realm,
         )
 
-    def get_header(self, request):
+    def get_header(self, request: Request) -> bytes:
         """
         Extracts the header containing the JSON web token from the given
         request.
         """
         header = request.META.get(api_settings.AUTH_HEADER_NAME)
 
         if isinstance(header, str):
             # Work around django test client oddness
             header = header.encode(HTTP_HEADER_ENCODING)
 
         return header
 
-    def get_raw_token(self, header):
+    def get_raw_token(self, header: bytes) -> Optional[bytes]:
         """
         Extracts an unvalidated JSON web token from the given "Authorization"
         header value.
         """
         parts = header.split()
 
         if len(parts) == 0:
@@ -78,40 +88,40 @@
             raise AuthenticationFailed(
                 _("Authorization header must contain two space-delimited values"),
                 code="bad_authorization_header",
             )
 
         return parts[1]
 
-    def get_validated_token(self, raw_token):
+    def get_validated_token(self, raw_token: bytes) -> Token:
         """
         Validates an encoded JSON web token and returns a validated token
         wrapper object.
         """
         messages = []
         for AuthToken in api_settings.AUTH_TOKEN_CLASSES:
             try:
                 return AuthToken(raw_token)
-            except TokenError as ex:
+            except TokenError as e:
                 messages.append(
                     {
                         "token_class": AuthToken.__name__,
                         "token_type": AuthToken.token_type,
-                        "message": ex.args[0],
+                        "message": e.args[0],
                     }
                 )
 
         raise InvalidToken(
             {
                 "detail": _("Given token not valid for any token type"),
                 "messages": messages,
             }
         )
 
-    def get_user(self, validated_token):
+    def get_user(self, validated_token: Token) -> AuthUser:
         """
         Attempts to find and return a user using the given validated token.
         """
         try:
             user_id = validated_token[api_settings.USER_ID_CLAIM]
         except KeyError:
             raise InvalidToken(_("Token contained no recognizable user identification"))
@@ -120,24 +130,32 @@
             user = self.user_model.objects.get(**{api_settings.USER_ID_FIELD: user_id})
         except self.user_model.DoesNotExist:
             raise AuthenticationFailed(_("User not found"), code="user_not_found")
 
         if not user.is_active:
             raise AuthenticationFailed(_("User is inactive"), code="user_inactive")
 
+        if api_settings.CHECK_REVOKE_TOKEN:
+            if validated_token.get(
+                api_settings.REVOKE_TOKEN_CLAIM
+            ) != get_md5_hash_password(user.password):
+                raise AuthenticationFailed(
+                    _("The user's password has been changed."), code="password_changed"
+                )
+
         return user
 
 
 class JWTStatelessUserAuthentication(JWTAuthentication):
     """
     An authentication plugin that authenticates requests through a JSON web
     token provided in a request header without performing a database lookup to obtain a user instance.
     """
 
-    def get_user(self, validated_token):
+    def get_user(self, validated_token: Token) -> AuthUser:
         """
         Returns a stateless user object which is backed by the given validated
         token.
         """
         if api_settings.USER_ID_CLAIM not in validated_token:
             # The TokenUser class assumes tokens will have a recognizable user
             # identifier claim.
@@ -145,15 +163,15 @@
 
         return api_settings.TOKEN_USER_CLASS(validated_token)
 
 
 JWTTokenUserAuthentication = JWTStatelessUserAuthentication
 
 
-def default_user_authentication_rule(user):
+def default_user_authentication_rule(user: AuthUser) -> bool:
     # Prior to Django 1.10, inactive users could be authenticated with the
     # default `ModelBackend`.  As of Django 1.10, the `ModelBackend`
     # prevents inactive users from authenticating.  App designers can still
     # allow inactive users to authenticate by opting for the new
     # `AllowAllUsersModelBackend`.  However, we explicitly prevent inactive
     # users from authenticating to enforce a reasonable policy and provide
     # sensible backwards compatibility with older Django versions.
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/backends.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/backends.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 import json
+from collections.abc import Iterable
 from datetime import timedelta
-from typing import Optional, Type, Union
+from typing import Any, Dict, Optional, Type, Union
 
 import jwt
 from django.utils.translation import gettext_lazy as _
 from jwt import InvalidAlgorithmError, InvalidTokenError, algorithms
-from rest_framework_simplejwt.exceptions import TokenBackendError
-from rest_framework_simplejwt.utils import format_lazy
+
+from .exceptions import TokenBackendError
+from .tokens import Token
+from .utils import format_lazy
 
 try:
     from jwt import PyJWKClient, PyJWKClientError
 
     JWK_CLIENT_AVAILABLE = True
 except ImportError:
     JWK_CLIENT_AVAILABLE = False
 
-ALLOWED_ALGORITHMS = {"HS256", "HS384", "HS512", "RS256", "RS384", "RS512", "ES256", "ES384", "ES512"}
+ALLOWED_ALGORITHMS = {
+    "HS256",
+    "HS384",
+    "HS512",
+    "RS256",
+    "RS384",
+    "RS512",
+    "ES256",
+    "ES384",
+    "ES512",
+}
 
 
 class TokenBackend:
     def __init__(
         self,
-        algorithm,
-        signing_key=None,
-        verifying_key="",
-        audience=None,
-        issuer=None,
-        jwk_url: str = None,
-        leeway: Union[float, int, timedelta] = None,
+        algorithm: str,
+        signing_key: Optional[str] = None,
+        verifying_key: str = "",
+        audience: Union[str, Iterable, None] = None,
+        issuer: Optional[str] = None,
+        jwk_url: Optional[str] = None,
+        leeway: Union[float, int, timedelta, None] = None,
         json_encoder: Optional[Type[json.JSONEncoder]] = None,
-    ):
+    ) -> None:
         self._validate_algorithm(algorithm)
 
         self.algorithm = algorithm
         self.signing_key = signing_key
         self.verifying_key = verifying_key
         self.audience = audience
         self.issuer = issuer
@@ -42,72 +55,85 @@
             self.jwks_client = PyJWKClient(jwk_url) if jwk_url else None
         else:
             self.jwks_client = None
 
         self.leeway = leeway
         self.json_encoder = json_encoder
 
-    def _validate_algorithm(self, algorithm):
+    def _validate_algorithm(self, algorithm: str) -> None:
         """
         Ensure that the nominated algorithm is recognized, and that cryptography is installed for those
         algorithms that require it
         """
         if algorithm not in ALLOWED_ALGORITHMS:
-            raise TokenBackendError(format_lazy(_("Unrecognized algorithm type '{}'"), algorithm))
+            raise TokenBackendError(
+                format_lazy(_("Unrecognized algorithm type '{}'"), algorithm)
+            )
 
         if algorithm in algorithms.requires_cryptography and not algorithms.has_crypto:
-            raise TokenBackendError(format_lazy(_("You must have cryptography installed to use {}."), algorithm))
+            raise TokenBackendError(
+                format_lazy(
+                    _("You must have cryptography installed to use {}."), algorithm
+                )
+            )
 
     def get_leeway(self) -> timedelta:
         leeway = getattr(self, "leeway", None)
 
         if leeway is None:
             return timedelta(seconds=0)
         elif isinstance(leeway, (int, float)):
             return timedelta(seconds=self.leeway)
         elif isinstance(leeway, timedelta):
             return self.leeway
         else:
             raise TokenBackendError(
                 format_lazy(
-                    _("Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."),
+                    _(
+                        "Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+                    ),
                     type(self.leeway),
                 )
             )
 
-    def get_verifying_key(self, token):
+    def get_verifying_key(self, token: Token) -> Optional[str]:
         if self.algorithm.startswith("HS"):
             return self.signing_key
 
         if self.jwks_client:
             try:
                 return self.jwks_client.get_signing_key_from_jwt(token).key
             except PyJWKClientError as ex:
                 raise TokenBackendError(_("Token is invalid or expired")) from ex
 
         return self.verifying_key
 
-    def encode(self, payload):
+    def encode(self, payload: Dict[str, Any]) -> str:
         """
         Returns an encoded token for the given payload dictionary.
         """
         jwt_payload = payload.copy()
         if self.audience is not None:
             jwt_payload["aud"] = self.audience
         if self.issuer is not None:
             jwt_payload["iss"] = self.issuer
 
-        token = jwt.encode(jwt_payload, self.signing_key, algorithm=self.algorithm, json_encoder=self.json_encoder)
+        token = jwt.encode(
+            jwt_payload,
+            self.signing_key,
+            algorithm=self.algorithm,
+            json_encoder=self.json_encoder,
+        )
         if isinstance(token, bytes):
             # For PyJWT <= 1.7.1
             return token.decode("utf-8")
         # For PyJWT >= 2.0.0a1
         return token
 
-    def decode(self, token, verify=True):
+    def decode(self, token: Token, verify: bool = True) -> Dict[str, Any]:
         """
         Performs a validation of the given token and returns its payload
         dictionary.
 
         Raises a `TokenBackendError` if the token is malformed, if its
         signature check fails, or if its 'exp' claim indicates it has expired.
         """
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/cs/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -7,100 +7,105 @@
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
 "Last-Translator: Lukáš Rod <info@lukasrod.cz>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr "Autorizační hlavička musí obsahovat dvě hodnoty oddělené mezerou"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "Daný token není validní pro žádný typ tokenu"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr "Token neobsahoval žádnou rozpoznatelnou identifikaci uživatele"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "Uživatel nenalezen"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "Uživatel není aktivní"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Nerozpoznaný typ algoritmu '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "Token není validní nebo vypršela jeho platnost"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
 msgstr "Žádný aktivní účet s danými údaji nebyl nalezen"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr "Nastavení '{}' bylo odstraněno. Dostupná nastavení jsou v '{}'"
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "uživatel"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "vytvořený v"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "platí do"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Token Blacklist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "Nelze vytvořit token bez zadaného typu nebo životnosti"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "Token nemá žádný identifikátor"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "Token nemá žádný typ"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "Token má špatný typ"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "Token nemá žádnou hodnotu '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "Hodnota tokenu '{}' vypršela"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "Token je na černé listině"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "uživatel"
+
+#~ msgid "created at"
+#~ msgstr "vytvořený v"
+
+#~ msgid "expires at"
+#~ msgstr "platí do"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/de_CH/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,116 @@
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <rene@matraxi.ch>, 2020.
+# FIRST AUTHOR <alfonso.pola@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"Last-Translator: rene <rene@matraxi.ch>\n"
-"Language: de_CH\n"
+"Last-Translator: Alfonso Pola <alfonso.pola@gmail.com>\n"
+"Language: es_CL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
-"Der Authorizationheader muss zwei leerzeichen-getrennte Werte enthalten"
+"El header de autorización debe contener dos valores delimitados por espacio"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "Der Token ist für keinen Tokentyp gültig"
+msgstr "El token provisto no es válido para ningún tipo de token"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "Token enthält keine erkennbare Benutzeridentifikation"
+msgstr "El token no contiene identificación de usuario reconocible"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "Benutzer nicht gefunden"
+msgstr "Usuario no encontrado"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "Inaktiver Benutzer"
+msgstr "El usuario está inactivo"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "Unerkannter Algorithmustyp '{}'"
+msgstr "Tipo de algoritmo no reconocido '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "Ungültiger oder abgelaufener Token"
+msgstr "Token inválido o expirado"
+
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
 
-#: serializers.py:24
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr "Kein aktiver Account mit diesen Zugangsdaten gefunden"
+msgstr ""
+"No se encontró una cuenta de usuario activa para las credenciales provistas"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
-"Die Einstellung '{}' wurde gelöscht. Bitte beachte '{}' für verfügbare "
-"Einstellungen."
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "Benutzer"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "erstellt am"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "läuft ab am"
+"La configuración '{}' fue removida. Por favor, refiérase a '{}' para "
+"configuraciones disponibles."
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Token Blacklist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "Ein Token ohne Typ oder Lebensdauer kann nicht erstellt werden"
+msgstr "No es posible crear un token sin tipo o tiempo de vida"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "Token hat keine Id"
+msgstr "Token no tiene id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "Token hat keinen Typ"
+msgstr "Token no tiene tipo"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "Token hat den falschen Typ"
+msgstr "Token tiene tipo erróneo"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "Token hat kein '{}' Recht"
+msgstr "Token no tiene privilegio '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "Das Tokenrecht '{}' ist abgelaufen"
+msgstr "El provilegio '{}' del token está expirado"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "Token steht auf der Blacklist"
+msgstr "Token está en la blacklist"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "Usuario"
+
+#~ msgid "created at"
+#~ msgstr "creado en"
+
+#~ msgid "expires at"
+#~ msgstr "expira en"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -8,103 +8,108 @@
 "Last-Translator: zeack <zeack@protonmail.com>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
 "El encabezado 'Authorization' debe contener valores delimitados por espacios"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "El token dado no es valido para ningun tipo de token"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr "El token no contenía identificación de usuario reconocible"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "Usuario no encontrado"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "El usuario está inactivo"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Tipo de algoritmo no reconocido '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr "Debe tener criptografía instalada para usar {}."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
-msgstr "Algoritmo especificado no válido"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "El token es inválido o ha expirado"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "Algoritmo especificado no válido"
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr "La combination de credenciales no tiene una cuenta activa"
+msgstr "La combinación de credenciales no tiene una cuenta activa"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
 "La configuración '{}' fue removida. Por favor, refiérase a '{}' para "
 "consultar las disponibles."
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "usuario"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "creado en"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "expira en"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Lista negra de Tokens"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "No se puede crear un token sin tipo o de tan larga vida"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "El token no tiene id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "El token no tiene tipo"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "El token tiene un tipo incorrecto"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "El token no tiene el privilegio '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "El privilegio '{}' del token ha expirado"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "El token está en lista negra"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "usuario"
+
+#~ msgid "created at"
+#~ msgstr "creado en"
+
+#~ msgid "expires at"
+#~ msgstr "expira en"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,115 @@
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-#
-# Translators:
-# Ariel Torti <arieltorti14@gmail.com>, 2020.
-#
-#, fuzzy
+# FIRST AUTHOR <sinvalju@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"Last-Translator: Ariel Torti <arieltort14@gmail.com>\n"
-"Language: es_AR\n"
+"Last-Translator: Bruno Ducraux <bruno.drx@gmail.com>\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
-"El header de autorización debe contener dos valores delimitados por espacio"
+"Cabeçalho de autorização deve conter dois valores delimitados por espaço"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "El token dado no es válido para ningún tipo de token"
+msgstr "O token informado não é válido para qualquer tipo de token"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "El token no contiene ninguna identificación de usuario"
+msgstr "O token não continha nenhuma identificação reconhecível do usuário"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "Usuario no encontrado"
+msgstr "Usuário não encontrado"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "El usuario está inactivo"
+msgstr "Usuário está inativo"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "Tipo de algoritmo no reconocido '{}'"
+msgstr "Tipo de algoritmo '{}' não reconhecido"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr ""
+msgstr "Você deve ter criptografia instalada para usar {}."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "El token es inválido o ha expirado"
+msgstr "O token é inválido ou expirado"
+
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "Algoritmo inválido especificado"
 
-#: serializers.py:24
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr ""
-"No se encontró una cuenta de usuario activa para las credenciales dadas"
+msgstr "Usuário e/ou senha incorreto(s)"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
-"La configuración '{}' fue removida. Por favor, refiérase a '{}' para "
-"consultar las configuraciones disponibles."
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "usuario"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "creado en"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "expira en"
+"A configuração '{}' foi removida. Por favor, consulte '{}' para disponível "
+"definições."
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Lista negra de Tokens"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "No es posible crear un token sin tipo o tiempo de vida"
+msgstr "Não é possível criar token sem tipo ou tempo de vida"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "El token no tiene id"
+msgstr "Token não tem id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "El token no tiene tipo"
+msgstr "Token não tem nenhum tipo"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "El token tiene un tipo incorrecto"
+msgstr "Token tem tipo errado"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "El token no tiene el privilegio '{}'"
+msgstr "Token não tem '{}' privilégio"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "El privilegio '{}' del token ha expirado"
+msgstr "O privilégio '{}' do token expirou"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "El token está en la lista negra"
+msgstr "Token está na blacklist"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "usuário"
+
+#~ msgid "created at"
+#~ msgstr "criado em"
+
+#~ msgid "expires at"
+#~ msgstr "expira em"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/es_CL/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/tr/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,114 @@
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <alfonso.pola@gmail.com>, 2019.
+# FIRST AUTHOR <suayip.541@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"Last-Translator: Alfonso Pola <alfonso.pola@gmail.com>\n"
-"Language: es_CL\n"
+"POT-Creation-Date: 2022-01-13 23:05+0300\n"
+"Last-Translator: Şuayip Üzülmez <suayip.541@gmail.com>\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
-"El header de autorización debe contener dos valores delimitados por espacio"
+"Yetkilendirme header'i boşlukla sınırlandırılmış iki değer bulundurmak "
+"zorunda"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "El token provisto no es válido para ningún tipo de token"
+msgstr "Verilen token hiçbir token tipi için geçerli değil"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "El token no contiene identificación de usuario reconocible"
+msgstr "Token tanınabilir bir kullanıcı kimliği içermiyor"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "Usuario no encontrado"
+msgstr "Kullanıcı bulunamadı"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "El usuario está inactivo"
+msgstr "Kullanıcı etkin değil"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "Tipo de algoritmo no reconocido '{}'"
+msgstr "Tanınmayan algortima tipi '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr ""
+msgstr "{} kullanmak için cryptography yüklemeniz gerekiyor."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "Token inválido o expirado"
+msgstr "Token geçersiz veya süresi geçmiş"
+
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "Geçersiz algoritma belirtildi"
 
-#: serializers.py:24
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr ""
-"No se encontró una cuenta de usuario activa para las credenciales provistas"
+msgstr "Verilen kimlik bilgileriyle aktif bir hesap bulunamadı"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
-msgstr ""
-"La configuración '{}' fue removida. Por favor, refiérase a '{}' para "
-"configuraciones disponibles."
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "Usuario"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "creado en"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "expira en"
+msgstr "'{}' ayarı kaldırıldı. Mevcut ayarlar için '{}' adresini ziyaret edin."
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
-msgstr "Token Blacklist"
+msgstr "Token Kara Listesi"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "No es posible crear un token sin tipo o tiempo de vida"
+msgstr "Tipi veya geçerlilik süresi olmayan token oluşturulamaz"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "Token no tiene id"
+msgstr "Token'in id'si yok"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "Token no tiene tipo"
+msgstr "Token'in tipi yok"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "Token tiene tipo erróneo"
+msgstr "Token'in tipi yanlış"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "Token no tiene privilegio '{}'"
+msgstr "Token'in '{}' claim'i yok"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "El provilegio '{}' del token está expirado"
+msgstr "Token'in '{}' claim'i sona erdi"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "Token está en la blacklist"
+msgstr "Token kara listeye alınmış"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "kullanıcı"
+
+#~ msgid "created at"
+#~ msgstr "oluşturulma tarihi"
+
+#~ msgid "expires at"
+#~ msgstr "sona erme tarihi"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fa_IR/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/sv/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,113 @@
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <hirad.daneshvar@gmail.com>, 2020.
+# FIRST AUTHOR Pasindu <pasinduprabashitha@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"Last-Translator: Hirad Daneshvar <hirad.daneshvar@gmail.com>\n"
-"Language: fa_IR\n"
+"POT-Creation-Date: 2022-05-29 17:30+0100\n"
+"Last-Translator: Pasindu <pasinduprabashitha@gmail.com>\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
-msgstr "هدر اعتبارسنجی باید شامل دو مقدار جدا شده با فاصله باشد"
+msgstr "Auktoriseringshuvudet måste innehålla två mellanslagsavgränsade värden"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "توکن داده شده برای هیچ نوع توکنی معتبر نمی‌باشد"
+msgstr "Givet token är inte giltigt för någon tokentyp"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "توکن شامل هیچ شناسه قابل تشخیصی از کاربر نیست"
+msgstr "Token innehöll ingen identifiering av användaren"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "کاربر یافت نشد"
+msgstr "Användaren hittades inte"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "کاربر غیرفعال است"
+msgstr "Användaren är inaktiv"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "نوع الگوریتم ناشناخته '{}'"
+msgstr "Okänd algoritmtyp '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr ""
+msgstr "Du måste ha kryptografi installerad för att kunna använda {}."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "توکن نامعتبر است یا منقضی شده است"
+msgstr "Token är ogiltig eller har löpt ut"
+
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "Ogiltig algoritm har angetts"
 
-#: serializers.py:24
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr "هیچ اکانت فعالی برای اطلاعات داده شده یافت نشد"
+msgstr "Inget aktivt konto hittades med de angivna användaruppgifterna"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
-msgstr "تنظیمات '{}' حذف شده است. لطفا به '{}' برای تنظیمات موجود مراجعه کنید."
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "کاربر"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "زمان ایجاد"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "زمان انقضا"
+msgstr ""
+"Inställningen '{}' har tagits bort. Se '{}' för tillgängliga inställningar"
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
-msgstr "لیست سیاه توکن"
+msgstr "Token svartlist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "توکن بدون هیچ نوع و طول عمر قابل ساخت نیست"
+msgstr "Kan inte skapa token utan typ eller livslängd"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "توکن id ندارد"
+msgstr "Token har inget id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "توکن نوع ندارد"
+msgstr "Token har ingen typ"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "توکن نوع اشتباهی دارد"
+msgstr "Token har fel typ"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "توکن دارای '{}' claim نمی‌باشد"
+msgstr "Token har inget '{}'-anspråk"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "'{}' claim توکن منقضی شده"
+msgstr "Token '{}'-anspråket har löpt ut"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "توکن به لیست سیاه رفته است"
+msgstr "Token är svartlistad"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "användare"
+
+#~ msgid "created at"
+#~ msgstr "skapad vid"
+
+#~ msgid "expires at"
+#~ msgstr "går ut kl"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/fr/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -7,104 +7,109 @@
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
 "Last-Translator: Stéphane Malta e Sousa <stephane.maltaesousa@ne.ch>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
 "L'en-tête 'Authorization' doit contenir deux valeurs séparées par des espaces"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "Le type de jeton fourni n'est pas valide"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr ""
 "Le jeton ne contient aucune information permettant d'identifier l'utilisateur"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "L'utilisateur n'a pas été trouvé"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "L'utilisateur est désactivé"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Type d'algorithme non reconnu '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr "Vous devez installer cryptography afin d'utiliser {}."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
-msgstr "L'algorithme spécifié est invalide"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "Le jeton est invalide ou expiré"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "L'algorithme spécifié est invalide"
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
 msgstr "Aucun compte actif n'a été trouvé avec les identifiants fournis"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
 "Le paramètre '{}' a été supprimé. Voir '{}' pour la liste des paramètres "
 "disponibles."
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "Utilisateur"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "Créé le"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "Expire le"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Liste des jetons bannis"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "Ne peut pas créer de jeton sans type ni durée de vie"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "Le jeton n'a pas d'id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "Le jeton n'a pas de type"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "Le jeton a un type erroné"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "Le jeton n'a pas le privilège '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "Le privilège '{}' du jeton a expiré"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "Le jeton a été banni"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "Utilisateur"
+
+#~ msgid "created at"
+#~ msgstr "Créé le"
+
+#~ msgid "expires at"
+#~ msgstr "Expire le"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/id_ID/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,109 +1,119 @@
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <oon.arfiandwi@gmail.com>, 2020.
+#
+# Translators:
+# <oon.arfiandwi@gmail.com>, 2020
+# Kira <kiraware@github.com>, 2023
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"Last-Translator: oon arfiandwi <oon.arfiandwi@gmail.com>\n"
+"PO-Revision-Date: 2023-03-09 08:14+0000\n"
+"Last-Translator: Kira <kiraware@github.com>\n"
 "Language: id_ID\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr "Header otorisasi harus berisi dua nilai yang dipisahkan spasi"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "Token yang diberikan tidak valid untuk semua jenis token"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr "Token tidak mengandung identifikasi pengguna yang dapat dikenali"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "Pengguna tidak ditemukan"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "Pengguna tidak aktif"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Jenis algoritma tidak dikenal '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr "Anda harus memasang kriptografi untuk menggunakan {}."
+msgstr "Anda harus memasang cryptography untuk menggunakan {}."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
-msgstr "Algoritma yang ditentukan tidak valid"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+msgstr ""
+"Tipe '{}' tidak dikenali, 'leeway' harus bertipe int, float, atau timedelta."
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "Token tidak valid atau kedaluwarsa"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "Algoritma yang ditentukan tidak valid"
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
 msgstr "Tidak ada akun aktif yang ditemukan dengan kredensial yang diberikan"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
 "Setelan '{}' telah dihapus. Silakan merujuk ke '{}' untuk pengaturan yang "
 "tersedia."
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "pengguna"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "created at"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "kedaluwarsa pada"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Daftar Hitam Token"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "Tidak dapat membuat token tanpa tipe atau masa pakai"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "Token tidak memiliki id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "Token tidak memiliki tipe"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "Jenis token salah"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "Token tidak memiliki klaim '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "Klaim token '{}' telah kedaluwarsa"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "Token masuk daftar hitam"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "pengguna"
+
+#~ msgid "created at"
+#~ msgstr "created at"
+
+#~ msgid "expires at"
+#~ msgstr "kedaluwarsa pada"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/it_IT/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/es_AR/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,121 @@
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <95adriano@gmail.com>, 2020.
+#
+# Translators:
+# Ariel Torti <arieltorti14@gmail.com>, 2020.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"PO-Revision-Date: \n"
-"Last-Translator: Adriano Di Dio <95adriano@gmail.com>\n"
-"Language-Team: \n"
-"Language: it_IT\n"
+"Last-Translator: Ariel Torti <arieltort14@gmail.com>\n"
+"Language: es_AR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 2.0.6\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
-"L'header di autorizzazione deve contenere due valori delimitati da uno spazio"
+"El header de autorización debe contener dos valores delimitados por espacio"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "Il token dato non è valido per qualsiasi tipo di token"
+msgstr "El token dado no es válido para ningún tipo de token"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "Il token non conteneva nessuna informazione riconoscibile dell'utente"
+msgstr "El token no contiene ninguna identificación de usuario"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "Utente non trovato"
+msgstr "Usuario no encontrado"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "Utente non attivo"
+msgstr "El usuario está inactivo"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "Algoritmo di tipo '{}' non riconosciuto"
+msgstr "Tipo de algoritmo no reconocido '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr "Devi avere installato cryptography per usare '{}'."
+msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
-msgstr "L'algoritmo specificato non è valido"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "Il token non è valido o è scaduto"
+msgstr "El token es inválido o ha expirado"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr "Nessun account attivo trovato con queste credenziali"
+msgstr ""
+"No se encontró una cuenta de usuario activa para las credenciales dadas"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
-"L'impostazione '{}' è stata rimossa. Per favore utilizza '{}' per "
-"visualizzare le impostazioni valide."
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "utente"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "creato il"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "scade il"
+"La configuración '{}' fue removida. Por favor, refiérase a '{}' para "
+"consultar las configuraciones disponibles."
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
-msgstr "Blacklist dei token"
+msgstr "Lista negra de Tokens"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "Impossibile creare un token senza tipo o durata"
+msgstr "No es posible crear un token sin tipo o tiempo de vida"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "Il token non ha un id"
+msgstr "El token no tiene id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "Il token non ha un tipo"
+msgstr "El token no tiene tipo"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "Il token ha un tipo sbagliato"
+msgstr "El token tiene un tipo incorrecto"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "Il token non contiene il parametro '{}'"
+msgstr "El token no tiene el privilegio '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "Il parametro '{}' del token è scaduto"
+msgstr "El privilegio '{}' del token ha expirado"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "Il token è stato inserito nella blacklist"
+msgstr "El token está en la lista negra"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "usuario"
+
+#~ msgid "created at"
+#~ msgstr "creado en"
+
+#~ msgid "expires at"
+#~ msgstr "expira en"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -7,102 +7,107 @@
 "POT-Creation-Date: 2021-06-17 11:06+0200\n"
 "Last-Translator: rene <rene@roadbearstudios.com>\n"
 "Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
 "Authorisatie header moet twee waarden bevatten, gescheiden door een spatie"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "Het token is voor geen enkel token-type geldig"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr "Token bevat geen herkenbare gebruikersidentificatie"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "Gebruiker niet gevonden"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "Gebruiker is inactief"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Niet herkend algoritme type '{}"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "Token is niet geldig of verlopen"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
 msgstr "Geen actief account gevonden voor deze gegevens"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
 "De '{}' instelling bestaat niet meer. Zie '{}' for beschikbareinstellingen."
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "gebruiker"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "aangemaakt op"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "verloopt op"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Token Blacklist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "Kan geen token maken zonder type of levensduur"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "Token heeft geen id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "Token heeft geen type"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "Token heeft het verkeerde type"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "Token heeft geen '{}' recht"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "Token '{}' recht is verlopen"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "Token is ge-blacklist"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "gebruiker"
+
+#~ msgid "created at"
+#~ msgstr "aangemaakt op"
+
+#~ msgid "expires at"
+#~ msgstr "verloopt op"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -7,101 +7,106 @@
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
 "Last-Translator: Mateusz Slisz <mat.slisz@yahoo.com>\n"
 "Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr "Nagłówek autoryzacji musi zawierać dwie wartości rodzielone spacjami"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "Podany token jest błędny dla każdego typu tokena"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr "Token nie zawierał rozpoznawalnej identyfikacji użytkownika"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "Użytkownik nie znaleziony"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "Użytkownik jest nieaktywny"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Nierozpoznany typ algorytmu '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "Token jest niepoprawny lub wygasł"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
 msgstr "Nie znaleziono aktywnego konta dla podanych danych uwierzytelniających"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
 "Ustawienie '{}' zostało usunięte. Dostępne ustawienia znajdują sie w '{}'"
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "użytkownik"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "stworzony w"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "wygasa o"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Token Blacklist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "Nie można utworzyć tokena bez podanego typu lub żywotności"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "Token nie posiada numeru identyfikacyjnego"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "Token nie posiada typu"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "Token posiada zły typ"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "Token nie posiada upoważnienia '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "Upoważnienie tokena '{}' wygasło"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "Token znajduję się na czarnej liście"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "użytkownik"
+
+#~ msgid "created at"
+#~ msgstr "stworzony w"
+
+#~ msgid "expires at"
+#~ msgstr "wygasa o"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/pt_BR/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/de/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,115 @@
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <sinvalju@gmail.com>, 2019.
+# FIRST AUTHOR <rene@matraxi.ch>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-02-22 17:30+0100\n"
-"Last-Translator: Bruno Ducraux <bruno.drx@gmail.com>\n"
-"Language: pt_BR\n"
+"Last-Translator: rene <rene@matraxi.ch>\n"
+"Language: de_CH\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
-"Cabeçalho de autorização deve conter dois valores delimitados por espaço"
+"Der Authorizationheader muss zwei leerzeichen-getrennte Werte enthalten"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "O token informado não é válido para qualquer tipo de token"
+msgstr "Der Token ist für keinen Tokentyp gültig"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "O token não continha nenhuma identificação reconhecível do usuário"
+msgstr "Token enthält keine erkennbare Benutzeridentifikation"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "Usuário não encontrado"
+msgstr "Benutzer nicht gefunden"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "Usuário está inativo"
+msgstr "Inaktiver Benutzer"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "Tipo de algoritmo '{}' não reconhecido"
+msgstr "Unerkannter Algorithmustyp '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr "Você deve ter criptografia instalada para usar {}."
+msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
-msgstr "Algoritmo inválido especificado"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "O token é inválido ou expirado"
+msgstr "Ungültiger oder abgelaufener Token"
+
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
 
-#: serializers.py:24
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr "Usuário e/ou senha incorreto(s)"
+msgstr "Kein aktiver Account mit diesen Zugangsdaten gefunden"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
-"A configuração '{}' foi removida. Por favor, consulte '{}' para disponível "
-"definições."
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "usuário"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "criado em"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "expira em"
+"Die Einstellung '{}' wurde gelöscht. Bitte beachte '{}' für verfügbare "
+"Einstellungen."
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
-msgstr "Lista negra de Tokens"
+msgstr "Token Blacklist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "Não é possível criar token sem tipo ou tempo de vida"
+msgstr "Ein Token ohne Typ oder Lebensdauer kann nicht erstellt werden"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "Token não tem id"
+msgstr "Token hat keine Id"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "Token não tem nenhum tipo"
+msgstr "Token hat keinen Typ"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "Token tem tipo errado"
+msgstr "Token hat den falschen Typ"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "Token não tem '{}' privilégio"
+msgstr "Token hat kein '{}' Recht"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "O privilégio '{}' do token expirou"
+msgstr "Das Tokenrecht '{}' ist abgelaufen"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "Token está na blacklist"
+msgstr "Token steht auf der Blacklist"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "Benutzer"
+
+#~ msgid "created at"
+#~ msgstr "erstellt am"
+
+#~ msgid "expires at"
+#~ msgstr "läuft ab am"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -8,107 +8,112 @@
 "PO-Revision-Date: \n"
 "Last-Translator: Sergey Ozeranskiy <sozeranskiy@dreamclass.ru>\n"
 "Language-Team: \n"
 "Language: ru_RU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : 2);\n"
 "X-Generator: Poedit 2.2.1\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
 msgstr ""
 "Заголовок авторизации должен содержать два значения, разделенных пробелом"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
 msgstr "Данный токен недействителен для любого типа токена"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
 msgstr "Токен не содержит идентификатор пользователя"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
 msgstr "Пользователь не найден"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
 msgstr "Пользователь неактивен"
 
-#: backends.py:37
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
+
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
 msgstr "Нераспознанный тип алгоритма '{}'"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
 msgstr ""
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
 msgstr ""
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
 msgstr "Токен недействителен или просрочен"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr ""
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
 msgstr "Не найдено активной учетной записи с указанными данными"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
 "Параметр '{}' был удален. Пожалуйста, обратитесь к '{}' для просмотра "
 "доступных настроек."
 
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "пользователь"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "создан"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "истекает"
-
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
 msgstr "Token Blacklist"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
 msgstr "Невозможно создать токен без типа или времени жизни"
 
-#: tokens.py:98
+#: tokens.py:119
 msgid "Token has no id"
 msgstr "У токена нет идентификатора"
 
-#: tokens.py:109
+#: tokens.py:131
 msgid "Token has no type"
 msgstr "Токен не имеет типа"
 
-#: tokens.py:112
+#: tokens.py:134
 msgid "Token has wrong type"
 msgstr "Токен имеет неправильный тип"
 
-#: tokens.py:149
+#: tokens.py:193
 msgid "Token has no '{}' claim"
 msgstr "Токен не содержит '{}'"
 
-#: tokens.py:153
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
 msgstr "Токен имеет просроченное значение '{}'"
 
-#: tokens.py:192
+#: tokens.py:260
 msgid "Token is blacklisted"
 msgstr "Токен занесен в черный список"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "пользователь"
+
+#~ msgid "created at"
+#~ msgstr "создан"
+
+#~ msgid "expires at"
+#~ msgstr "истекает"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/locale/zh_Hans/LC_MESSAGES/django.po` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/locale/ro/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,117 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) 2021
-# This file is distributed under the same license as the Simple JWT package.
-# zengqiu <zengqiu@qq.com>, 2021.
-
+# This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR Daniel Cuznetov <danielcuznetov04@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: djangorestframework_simplejwt\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-06-23 13:29+0800\n"
-"PO-Revision-Date: 2021-06-23 13:29+080\n"
-"Last-Translator: zengqiu <zengqiu@qq.com>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2022-07-13 10:45+0100\n"
+"Last-Translator: Daniel Cuznetov <danielcuznetov04@gmail.com>\n"
+"Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: authentication.py:79
+#: authentication.py:89
 msgid "Authorization header must contain two space-delimited values"
-msgstr "授权头必须包含两个用空格分隔的值"
+msgstr ""
+"Header-ul(antetul) de autorizare trebuie să conțină două valori separate "
+"prin spațiu"
 
-#: authentication.py:100
+#: authentication.py:115
 msgid "Given token not valid for any token type"
-msgstr "此令牌对任何类型的令牌无效"
+msgstr "Tokenul dat nu este valid pentru niciun tip de token"
 
-#: authentication.py:111 authentication.py:133
+#: authentication.py:127 authentication.py:162
 msgid "Token contained no recognizable user identification"
-msgstr "令牌未包含用户标识符"
+msgstr "Tokenul nu conține date de identificare a utilizatorului"
 
-#: authentication.py:116
+#: authentication.py:132
 msgid "User not found"
-msgstr "未找到该用户"
+msgstr "Utilizatorul nu a fost găsit"
 
-#: authentication.py:119
+#: authentication.py:135
 msgid "User is inactive"
-msgstr "该用户已禁用"
+msgstr "Utilizatorul este inactiv"
+
+#: authentication.py:142
+msgid "The user's password has been changed."
+msgstr ""
 
-#: backends.py:37
+#: backends.py:69
 msgid "Unrecognized algorithm type '{}'"
-msgstr "未知算法类型 '{}'"
+msgstr "Tipul de algoritm '{}' nu este recunoscut"
 
-#: backends.py:40
+#: backends.py:75
 msgid "You must have cryptography installed to use {}."
-msgstr "你必须安装 cryptography 才能使用 {}。"
+msgstr "Trebuie să aveți instalată criptografia pentru a utiliza {}."
 
-#: backends.py:74
-msgid "Invalid algorithm specified"
-msgstr "指定的算法无效"
+#: backends.py:92
+msgid ""
+"Unrecognized type '{}', 'leeway' must be of type int, float or timedelta."
+msgstr ""
+"Tipul '{}' nu este recunoscut, 'leeway' trebuie să fie de tip int, float sau "
+"timedelta."
 
-#: backends.py:76 exceptions.py:38 tokens.py:44
+#: backends.py:106 backends.py:156 exceptions.py:47 tokens.py:61
 msgid "Token is invalid or expired"
-msgstr "令牌无效或已过期"
+msgstr "Token nu este valid sau a expirat"
 
-#: serializers.py:24
+#: backends.py:154
+msgid "Invalid algorithm specified"
+msgstr "Algoritm nevalid specificat"
+
+#: serializers.py:37
 msgid "No active account found with the given credentials"
-msgstr "找不到指定凭据对应的有效用户"
+msgstr "Nu a fost găsit cont activ cu aceste date de autentificare"
 
-#: settings.py:63
+#: settings.py:73
 msgid ""
 "The '{}' setting has been removed. Please refer to '{}' for available "
 "settings."
 msgstr ""
-"'{}' 配置已被移除。 请参阅 '{}' 获取可用的"
-"配置。"
-
-#: token_blacklist/admin.py:72
-msgid "jti"
-msgstr "jti"
-
-#: token_blacklist/admin.py:77
-msgid "user"
-msgstr "用户"
-
-#: token_blacklist/admin.py:82
-msgid "created at"
-msgstr "创建时间"
-
-#: token_blacklist/admin.py:87
-msgid "expires at"
-msgstr "过期时间"
+"Setarea '{}' a fost ștearsă. Referați la '{}' pentru setări disponibile."
 
 #: token_blacklist/apps.py:7
 msgid "Token Blacklist"
-msgstr "令牌黑名单"
+msgstr "Listă de token-uri blocate"
 
-#: tokens.py:30
+#: tokens.py:47
 msgid "Cannot create token with no type or lifetime"
-msgstr "无法创建没有类型或生存期的令牌"
+msgstr "Nu se poate crea token fără tip sau durată de viață"
 
-#: tokens.py:96
+#: tokens.py:119
 msgid "Token has no id"
-msgstr "令牌没有标识符"
+msgstr "Tokenul nu are id"
 
-#: tokens.py:107
+#: tokens.py:131
 msgid "Token has no type"
-msgstr "令牌没有类型"
+msgstr "Tokenul nu are tip"
 
-#: tokens.py:110
+#: tokens.py:134
 msgid "Token has wrong type"
-msgstr "令牌类型错误"
+msgstr "Tokenul are tipul greșit"
 
-#: tokens.py:147
+#: tokens.py:193
 msgid "Token has no '{}' claim"
-msgstr "令牌没有 '{}' 声明"
+msgstr "Tokenul nu are reclamația '{}'"
 
-#: tokens.py:151
+#: tokens.py:198
 msgid "Token '{}' claim has expired"
-msgstr "令牌 '{}' 声明已过期"
+msgstr "Reclamația tokenului '{}' a expirat"
 
-#: tokens.py:194
+#: tokens.py:260
 msgid "Token is blacklisted"
-msgstr "令牌已被加入黑名单"
+msgstr "Tokenul este în listă de tokenuri blocate"
+
+#~ msgid "jti"
+#~ msgstr "jti"
+
+#~ msgid "user"
+#~ msgstr "utilizator"
+
+#~ msgid "created at"
+#~ msgstr "creat la"
+
+#~ msgid "expires at"
+#~ msgstr "expiră la"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/models.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+from typing import TYPE_CHECKING, Any, List, Optional, Union
+
+from django.db.models.manager import EmptyManager
 from django.utils.functional import cached_property
-from rest_framework_simplejwt.compat import CallableFalse, CallableTrue
+from django_mongoengine.mongo_auth import models as auth_models
 
 from .settings import api_settings
 
+if TYPE_CHECKING:
+    from .tokens import Token
+
 
 class TokenUser:
     """
     A dummy user class modeled after django.contrib.auth.models.AnonymousUser.
     Used in conjunction with the `JWTStatelessUserAuthentication` backend to
     implement single sign-on functionality across services which share the same
     secret key.  `JWTStatelessUserAuthentication` will return an instance of this
@@ -14,83 +20,96 @@
     stateless user objects which are backed by validated tokens.
     """
 
     # User is always active since Simple JWT will never issue a token for an
     # inactive user
     is_active = True
 
-    def __init__(self, token):
+    _groups = EmptyManager(auth_models.Group)
+    _user_permissions = EmptyManager(auth_models.Permission)
+
+    def __init__(self, token: "Token") -> None:
         self.token = token
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"TokenUser {self.id}"
 
     @cached_property
-    def id(self):
+    def id(self) -> Union[int, str]:
         return self.token[api_settings.USER_ID_CLAIM]
 
     @cached_property
-    def pk(self):
+    def pk(self) -> Union[int, str]:
         return self.id
 
     @cached_property
-    def username(self):
+    def username(self) -> str:
         return self.token.get("username", "")
 
     @cached_property
-    def is_staff(self):
+    def is_staff(self) -> bool:
         return self.token.get("is_staff", False)
 
     @cached_property
-    def is_superuser(self):
+    def is_superuser(self) -> bool:
         return self.token.get("is_superuser", False)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, TokenUser):
+            return NotImplemented
         return self.id == other.id
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self.id)
 
-    def save(self):
+    def save(self) -> None:
         raise NotImplementedError("Token users have no DB representation")
 
-    def delete(self):
+    def delete(self) -> None:
         raise NotImplementedError("Token users have no DB representation")
 
-    def set_password(self, raw_password):
+    def set_password(self, raw_password: str) -> None:
         raise NotImplementedError("Token users have no DB representation")
 
-    def check_password(self, raw_password):
+    def check_password(self, raw_password: str) -> None:
         raise NotImplementedError("Token users have no DB representation")
 
-    def get_group_permissions(self, obj=None):
+    @property
+    def groups(self) -> auth_models.Group:
+        return self._groups
+
+    @property
+    def user_permissions(self) -> auth_models.Permission:
+        return self._user_permissions
+
+    def get_group_permissions(self, obj: Optional[object] = None) -> set:
         return set()
 
-    def get_all_permissions(self, obj=None):
+    def get_all_permissions(self, obj: Optional[object] = None) -> set:
         return set()
 
-    def has_perm(self, perm, obj=None):
+    def has_perm(self, perm: str, obj: Optional[object] = None) -> bool:
         return False
 
-    def has_perms(self, perm_list, obj=None):
+    def has_perms(self, perm_list: List[str], obj: Optional[object] = None) -> bool:
         return False
 
-    def has_module_perms(self, module):
+    def has_module_perms(self, module: str) -> bool:
         return False
 
     @property
-    def is_anonymous(self):
-        return CallableFalse
+    def is_anonymous(self) -> bool:
+        return False
 
     @property
-    def is_authenticated(self):
-        return CallableTrue
+    def is_authenticated(self) -> bool:
+        return True
 
-    def get_username(self):
+    def get_username(self) -> str:
         return self.username
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Optional[Any]:
         """This acts as a backup attribute getter for custom claims defined in Token serializers."""
         return self.token.get(attr, None)
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/token_blacklist/models.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/token_blacklist/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         # https://github.com/encode/django-rest-framework/issues/705
         abstract = (
             "rest_framework_simplejwt_mongoengine.token_blacklist"
             not in settings.INSTALLED_APPS
         )
         ordering = ("user",)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "Token for {} ({})".format(
             self.user,
             self.jti,
         )
 
 
 class BlacklistedTokenManager(QuerySetManager):
@@ -62,9 +62,9 @@
         # Also see corresponding ticket:
         # https://github.com/encode/django-rest-framework/issues/705
         abstract = (
             "rest_framework_simplejwt_mongoengine.token_blacklist"
             not in settings.INSTALLED_APPS
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Blacklisted token for {self.token.user}"
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/rest_framework_simplejwt_mongoengine/tokens.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/rest_framework_simplejwt_mongoengine/tokens.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,47 @@
-from datetime import timedelta
+from datetime import datetime, timedelta
+from typing import TYPE_CHECKING, Any, Dict, Generic, Optional, Type, TypeVar
 from uuid import uuid4
 
 from django.conf import settings
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
-from rest_framework_simplejwt.exceptions import TokenBackendError, TokenError
-from rest_framework_simplejwt.tokens import Token as SimpleJWTToken
-from rest_framework_simplejwt.utils import aware_utcnow, datetime_from_epoch, datetime_to_epoch, format_lazy
-
-from rest_framework_simplejwt_mongoengine.utils import drf_simplejwt_version
+from django_mongoengine.mongo_auth.models import AbstractUser
 
+from .exceptions import TokenBackendError, TokenError
+from .models import TokenUser
 from .settings import api_settings
 from .token_blacklist.models import BlacklistedToken, OutstandingToken
-from .utils import microseconds_to_milliseconds
+from .utils import (
+    aware_utcnow,
+    datetime_from_epoch,
+    datetime_to_epoch,
+    format_lazy,
+    get_md5_hash_password,
+    microseconds_to_milliseconds,
+)
+
+if TYPE_CHECKING:
+    from .backends import TokenBackend
+
+T = TypeVar("T", bound="Token")
+
+AuthUser = TypeVar("AuthUser", AbstractUser, TokenUser)
+
+
+class Token:
+    """
+    A class which validates and wraps an existing JWT or can be used to build a
+    new JWT.
+    """
 
+    token_type: Optional[str] = None
+    lifetime: Optional[timedelta] = None
 
-class Token(SimpleJWTToken):
-    def __init__(self, token=None, verify=True):
+    def __init__(self, token: Optional["Token"] = None, verify: bool = True) -> None:
         """
         !!!! IMPORTANT !!!! MUST raise a TokenError with a user-facing error
         message if the given token is invalid, expired, or otherwise not safe
         to use.
         """
         if self.token_type is None or self.lifetime is None:
             raise TokenError(_("Cannot create token with no type or lifetime"))
@@ -48,190 +69,201 @@
             # Set "exp" and "iat" claims with default value
             self.set_exp(from_time=self.current_time, lifetime=self.lifetime)
             self.set_iat(at_time=self.current_time)
 
             # Set "jti" claim
             self.set_jti()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return repr(self.payload)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str):
         return self.payload[key]
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: Any) -> None:
         self.payload[key] = value
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str) -> None:
         del self.payload[key]
 
-    def __contains__(self, key):
+    def __contains__(self, key: str) -> Any:
         return key in self.payload
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: Optional[Any] = None) -> Any:
         return self.payload.get(key, default)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         Signs and returns a token as a base64 encoded string.
         """
         return self.get_token_backend().encode(self.payload)
 
-    def verify(self):
+    def verify(self) -> None:
         """
         Performs additional validation steps which were not performed when this
         token was decoded.  This method is part of the "public" API to indicate
         the intention that it may be overridden in subclasses.
         """
         # According to RFC 7519, the "exp" claim is OPTIONAL
         # (https://tools.ietf.org/html/rfc7519#section-4.1.4).  As a more
         # correct behavior for authorization tokens, we require an "exp"
         # claim.  We don't want any zombie tokens walking around.
         self.check_exp()
 
         # If the defaults are not None then we should enforce the
         # requirement of these settings.As above, the spec labels
         # these as optional.
-        if api_settings.JTI_CLAIM is not None and api_settings.JTI_CLAIM not in self.payload:
+        if (
+            api_settings.JTI_CLAIM is not None
+            and api_settings.JTI_CLAIM not in self.payload
+        ):
             raise TokenError(_("Token has no id"))
 
         if api_settings.TOKEN_TYPE_CLAIM is not None:
-
             self.verify_token_type()
 
-    def verify_token_type(self):
+    def verify_token_type(self) -> None:
         """
         Ensures that the token type claim is present and has the correct value.
         """
         try:
             token_type = self.payload[api_settings.TOKEN_TYPE_CLAIM]
-        except KeyError as ex:
-            raise TokenError(_("Token has no type")) from ex
+        except KeyError:
+            raise TokenError(_("Token has no type"))
 
         if self.token_type != token_type:
             raise TokenError(_("Token has wrong type"))
 
-    def set_jti(self):
+    def set_jti(self) -> None:
         """
         Populates the configured jti claim of a token with a string where there
         is a negligible probability that the same string will be chosen at a
         later time.
 
         See here:
         https://tools.ietf.org/html/rfc7519#section-4.1.7
         """
         self.payload[api_settings.JTI_CLAIM] = uuid4().hex
 
-    def set_exp(self, claim="exp", from_time=None, lifetime=None):
+    def set_exp(
+        self,
+        claim: str = "exp",
+        from_time: Optional[datetime] = None,
+        lifetime: Optional[timedelta] = None,
+    ) -> None:
         """
         Updates the expiration time of a token.
 
         See here:
         https://tools.ietf.org/html/rfc7519#section-4.1.4
         """
         if from_time is None:
             from_time = self.current_time
 
         if lifetime is None:
             lifetime = self.lifetime
 
         self.payload[claim] = datetime_to_epoch(from_time + lifetime)
 
-    def set_iat(self, claim="iat", at_time=None):
+    def set_iat(self, claim: str = "iat", at_time: Optional[datetime] = None) -> None:
         """
         Updates the time at which the token was issued.
 
         See here:
         https://tools.ietf.org/html/rfc7519#section-4.1.6
         """
         if at_time is None:
             at_time = self.current_time
 
         self.payload[claim] = datetime_to_epoch(at_time)
 
-    def check_exp(self, claim="exp", current_time=None):
+    def check_exp(
+        self, claim: str = "exp", current_time: Optional[datetime] = None
+    ) -> None:
         """
         Checks whether a timestamp value in the given claim has passed (since
         the given datetime value in `current_time`).  Raises a TokenError with
         a user-facing error message if so.
         """
         if current_time is None:
             current_time = self.current_time
 
         try:
             claim_value = self.payload[claim]
-        except KeyError as ex:
-            raise TokenError(format_lazy(_("Token has no '{}' claim"), claim)) from ex
+        except KeyError:
+            raise TokenError(format_lazy(_("Token has no '{}' claim"), claim))
 
-        has_error = False
         claim_time = datetime_from_epoch(claim_value)
-
-        if "4.7" in drf_simplejwt_version:
-            has_error = claim_time <= current_time
-        else:
-            leeway = self.get_token_backend().get_leeway()
-            has_error = claim_time <= current_time - leeway
-
-        if has_error:
+        leeway = self.get_token_backend().get_leeway()
+        if claim_time <= current_time - leeway:
             raise TokenError(format_lazy(_("Token '{}' claim has expired"), claim))
 
     @classmethod
-    def for_user(cls, user):
+    def for_user(cls: Type[T], user: AuthUser) -> T:
         """
         Returns an authorization token for the given user that will be provided
         after authenticating the user's credentials.
         """
         user_id = getattr(user, api_settings.USER_ID_FIELD)
         if not isinstance(user_id, int):
             user_id = str(user_id)
 
         token = cls()
         token[api_settings.USER_ID_CLAIM] = user_id
 
+        if api_settings.CHECK_REVOKE_TOKEN:
+            token[api_settings.REVOKE_TOKEN_CLAIM] = get_md5_hash_password(
+                user.password
+            )
+
         return token
 
-    _token_backend = None
+    _token_backend: Optional["TokenBackend"] = None
 
     @property
-    def token_backend(self):
+    def token_backend(self) -> "TokenBackend":
         if self._token_backend is None:
-            self._token_backend = import_string("rest_framework_simplejwt_mongoengine.state.token_backend")
+            self._token_backend = import_string(
+                "rest_framework_simplejwt_mongoengine.state.token_backend"
+            )
         return self._token_backend
 
-    def get_token_backend(self):
+    def get_token_backend(self) -> "TokenBackend":
         # Backward compatibility.
         return self.token_backend
 
 
-class BlacklistMixin:
+class BlacklistMixin(Generic[T]):
     """
     If the `rest_framework_simplejwt_mongoengine.token_blacklist` app was configured to be
     used, tokens created from `BlacklistMixin` subclasses will insert
     themselves into an outstanding token list and also check for their
     membership in a token blacklist.
     """
 
+    payload: Dict[str, Any]
+
     if "rest_framework_simplejwt_mongoengine.token_blacklist" in settings.INSTALLED_APPS:
 
-        def verify(self, *args, **kwargs):
+        def verify(self, *args, **kwargs) -> None:
             self.check_blacklist()
 
-            super().verify(*args, **kwargs)
+            super().verify(*args, **kwargs)  # type: ignore
 
-        def check_blacklist(self):
+        def check_blacklist(self) -> None:
             """
             Checks if this token is present in the token blacklist.  Raises
             `TokenError` if so.
             """
             jti = self.payload[api_settings.JTI_CLAIM]
 
             if BlacklistedToken.objects.filter(token__in=OutstandingToken.objects.filter(jti=jti)).exists():
                 raise TokenError(_("Token is blacklisted"))
 
-        def blacklist(self):
+        def blacklist(self) -> BlacklistedToken:
             """
             Ensures this token is included in the outstanding token list and
             adds it to the blacklist.
             """
             jti = self.payload[api_settings.JTI_CLAIM]
             exp = self.payload["exp"]
 
@@ -248,19 +280,19 @@
                 blacklist_token = BlacklistedToken.objects.get(token=token)
             except BlacklistedToken.DoesNotExist:
                 blacklist_token = BlacklistedToken.objects.create(token=token)
 
             return blacklist_token
 
         @classmethod
-        def for_user(cls, user):
+        def for_user(cls: Type[T], user: AuthUser) -> T:
             """
             Adds this token to the outstanding token list.
             """
-            token = super().for_user(user)
+            token = super().for_user(user)  # type: ignore
 
             jti = token[api_settings.JTI_CLAIM]
             exp = token["exp"]
 
             OutstandingToken.objects.create(
                 user=user,
                 jti=jti,
@@ -268,19 +300,19 @@
                 created_at=token.current_time,
                 expires_at=datetime_from_epoch(exp),
             )
 
             return token
 
 
-class SlidingToken(BlacklistMixin, Token):
+class SlidingToken(BlacklistMixin["SlidingToken"], Token):
     token_type = "sliding"
     lifetime = api_settings.SLIDING_TOKEN_LIFETIME
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         if self.token is None:
             # Set sliding refresh expiration claim if new token
             self.set_exp(
                 api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM,
                 from_time=self.current_time,
@@ -289,15 +321,15 @@
 
 
 class AccessToken(Token):
     token_type = "access"
     lifetime = api_settings.ACCESS_TOKEN_LIFETIME
 
 
-class RefreshToken(BlacklistMixin, Token):
+class RefreshToken(BlacklistMixin["RefreshToken"], Token):
     token_type = "refresh"
     lifetime = api_settings.REFRESH_TOKEN_LIFETIME
     no_copy_claims = (
         api_settings.TOKEN_TYPE_CLAIM,
         "exp",
         # Both of these claims are included even though they may be the same.
         # It seems possible that a third party token might have a custom or
@@ -305,15 +337,15 @@
         # we wouldn't want to copy either one.
         api_settings.JTI_CLAIM,
         "jti",
     )
     access_token_class = AccessToken
 
     @property
-    def access_token(self):
+    def access_token(self) -> AccessToken:
         """
         Returns an access token created from this refresh token.  Copies all
         claims present in this refresh token to the new access token except
         those claims listed in the `no_copy_claims` attribute.
         """
         access = self.access_token_class()
 
@@ -332,14 +364,14 @@
         return access
 
 
 class UntypedToken(Token):
     token_type = "untyped"
     lifetime = timedelta(seconds=0)
 
-    def verify_token_type(self):
+    def verify_token_type(self) -> None:
         """
         Untyped tokens do not verify the "token_type" claim.  This is useful
         when performing general validation of a token's signature and other
         properties which do not relate to the token's intended use.
         """
         pass
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/setup.cfg` & `djangorestframework_simplejwt_mongoengine-1.3.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+[metadata]
+license_file = LICENSE.txt
+
 [bumpversion]
-current_version = 1.2.1
+current_version = 1.3.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/setup.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,98 @@
 #!/usr/bin/env python
-
-"""The setup script."""
-
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 requirements = [
-    "django>=3.2,<4.1",
-    "djangorestframework>=3.11",
-    "djangorestframework-simplejwt>=4.7,<5.3",
+    "django>=3.2,<4.3",
+    "djangorestframework>=3.12",
     "django-mongoengine>=0.5.4",
     "pyjwt>=1.7.1,<3",
 ]
 
-test_requirements = [
-    "pytest>=3",
-]
+extras_require = {
+    "test": [
+        "cryptography",
+        "coverage",
+        "freezegun",
+        "psutil",
+        "python-jose",
+        "pytest-cov",
+        "pytest-django",
+        "pytest-xdist",
+        "pytest",
+        "tox",
+    ],
+    "lint": [
+        "flake8",
+        "pep8",
+        "isort",
+    ],
+    "doc": [
+        "Sphinx>=7",
+        "sphinx_rtd_theme>=2.0.0",
+    ],
+    "dev": [
+        "pytest-watch",
+        "wheel",
+        "twine",
+        "ipython",
+    ],
+    "python-jose": [
+        "python-jose==3.3.0",
+    ],
+    "crypto": [
+        "cryptography>=3.3.1",
+    ],
+}
+
+extras_require["dev"] = (
+    extras_require["dev"]
+    + extras_require["test"]
+    + extras_require["lint"]
+    + extras_require["doc"]
+    + extras_require["python-jose"]
+)
+
 
 setup(
+    name="djangorestframework_simplejwt_mongoengine",
+    keywords="djangorestframework_simplejwt_mongoengine",
     author="Đỗ Ngọc Ngoạn (aka Ngoan Do)",
     author_email="ngocngoan060288@gmail.com",
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP",
     ],
     description="Simple JWT is a JSON Web Token authentication plugin for the Django REST Framework which to be compatible with MongoEngine.",  # noqa: E501
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     install_requires=requirements,
+    extras_require=extras_require,
     license="GNU General Public License v3",
     include_package_data=True,
-    keywords="djangorestframework_simplejwt_mongoengine",
-    name="djangorestframework_simplejwt_mongoengine",
+    zip_safe=False,
     packages=find_packages(
         include=[
             "rest_framework_simplejwt_mongoengine",
             "rest_framework_simplejwt_mongoengine.*",
         ]
     ),
     test_suite="tests",
-    tests_require=test_requirements,
     url="https://github.com/ngocngoan/djangorestframework-simplejwt-mongoengine",
-    version="1.2.1",
-    zip_safe=False,
+    version="1.3.0",
 )
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_authentication.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_authentication.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import timedelta
 from importlib import reload
 
 from bson.objectid import ObjectId
 from django_mongoengine.mongo_auth.managers import get_user_document
 from rest_framework.test import APIRequestFactory
-from rest_framework_simplejwt.exceptions import AuthenticationFailed, InvalidToken
 
 from rest_framework_simplejwt_mongoengine import authentication
+from rest_framework_simplejwt_mongoengine.exceptions import AuthenticationFailed, InvalidToken
 from rest_framework_simplejwt_mongoengine.models import TokenUser
 from rest_framework_simplejwt_mongoengine.settings import api_settings
 from rest_framework_simplejwt_mongoengine.tokens import AccessToken, SlidingToken
+from rest_framework_simplejwt_mongoengine.utils import get_md5_hash_password
 
 from .utils import BaseTestCase, override_api_settings
 
 User = get_user_document()
 AuthToken = api_settings.AUTH_TOKEN_CLASSES[0]
 
 
@@ -36,33 +37,27 @@
 
         # Should work for unicode headers
         request = self.factory.get(
             "/test-url/", HTTP_AUTHORIZATION=self.fake_header.decode("utf-8")
         )
         self.assertEqual(self.backend.get_header(request), self.fake_header)
 
-        # Should work with the x_access_token
-        with override_api_settings(AUTH_HEADER_NAME="HTTP_X_ACCESS_TOKEN"):
-            # Should pull correct header off request when using X_ACCESS_TOKEN
-            request = self.factory.get(
-                "/test-url/", HTTP_X_ACCESS_TOKEN=self.fake_header
-            )
-            self.assertEqual(self.backend.get_header(request), self.fake_header)
-
-            # Should work for unicode headers when using
-            request = self.factory.get(
-                "/test-url/", HTTP_X_ACCESS_TOKEN=self.fake_header.decode("utf-8")
-            )
-            self.assertEqual(self.backend.get_header(request), self.fake_header)
+    @override_api_settings(AUTH_HEADER_NAME="HTTP_X_ACCESS_TOKEN")
+    def test_get_header_x_access_token(self):
+        # Should pull correct header off request when using X_ACCESS_TOKEN
+        request = self.factory.get("/test-url/", HTTP_X_ACCESS_TOKEN=self.fake_header)
+        self.assertEqual(self.backend.get_header(request), self.fake_header)
+
+        # Should work for unicode headers when using
+        request = self.factory.get(
+            "/test-url/", HTTP_X_ACCESS_TOKEN=self.fake_header.decode("utf-8")
+        )
+        self.assertEqual(self.backend.get_header(request), self.fake_header)
 
     def test_get_raw_token(self):
-        # Should return None if header lacks correct type keyword
-        with override_api_settings(AUTH_HEADER_TYPES="JWT"):
-            reload(authentication)
-            self.assertIsNone(self.backend.get_raw_token(self.fake_header))
         reload(authentication)
 
         # Should return None if an empty AUTHORIZATION header is sent
         self.assertIsNone(self.backend.get_raw_token(b""))
 
         # Should raise error if header is malformed
         with self.assertRaises(AuthenticationFailed):
@@ -70,68 +65,76 @@
 
         with self.assertRaises(AuthenticationFailed):
             self.backend.get_raw_token(b"Bearer")
 
         # Otherwise, should return unvalidated token in header
         self.assertEqual(self.backend.get_raw_token(self.fake_header), self.fake_token)
 
+    @override_api_settings(AUTH_HEADER_TYPES="JWT")
+    def test_get_raw_token_incorrect_header_keyword(self):
+        # Should return None if header lacks correct type keyword
+        # AUTH_HEADER_TYPES is "JWT", but header is "Bearer"
+        reload(authentication)
+        self.assertIsNone(self.backend.get_raw_token(self.fake_header))
+
+    @override_api_settings(AUTH_HEADER_TYPES=("JWT", "Bearer"))
+    def test_get_raw_token_multi_header_keyword(self):
         # Should return token if header has one of many valid token types
-        with override_api_settings(AUTH_HEADER_TYPES=("JWT", "Bearer")):
-            reload(authentication)
-            self.assertEqual(
-                self.backend.get_raw_token(self.fake_header),
-                self.fake_token,
-            )
         reload(authentication)
+        self.assertEqual(
+            self.backend.get_raw_token(self.fake_header),
+            self.fake_token,
+        )
 
     def test_get_validated_token(self):
         # Should raise InvalidToken if token not valid
         token = AuthToken()
         token.set_exp(lifetime=-timedelta(days=1))
         with self.assertRaises(InvalidToken):
             self.backend.get_validated_token(str(token))
 
         # Otherwise, should return validated token
         token.set_exp()
         self.assertEqual(
             self.backend.get_validated_token(str(token)).payload, token.payload
         )
 
+    @override_api_settings(
+        AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.AccessToken",),
+    )
+    def test_get_validated_token_reject_unknown_token(self):
         # Should not accept tokens not included in AUTH_TOKEN_CLASSES
         sliding_token = SlidingToken()
-        with override_api_settings(
-            AUTH_TOKEN_CLASSES=(
-                "rest_framework_simplejwt_mongoengine.tokens.AccessToken",
-            )
-        ):
-            with self.assertRaises(InvalidToken) as e:
-                self.backend.get_validated_token(str(sliding_token))
-
-            messages = e.exception.detail["messages"]
-            self.assertEqual(1, len(messages))
-            self.assertEqual(
-                {
-                    "token_class": "AccessToken",
-                    "token_type": "access",
-                    "message": "Token has wrong type",
-                },
-                messages[0],
-            )
+        with self.assertRaises(InvalidToken) as e:
+            self.backend.get_validated_token(str(sliding_token))
 
+        messages = e.exception.detail["messages"]
+        self.assertEqual(1, len(messages))
+        self.assertEqual(
+            {
+                "token_class": "AccessToken",
+                "token_type": "access",
+                "message": "Token has wrong type",
+            },
+            messages[0],
+        )
+
+    @override_api_settings(
+        AUTH_TOKEN_CLASSES=(
+            "rest_framework_simplejwt_mongoengine.tokens.AccessToken",
+            "rest_framework_simplejwt_mongoengine.tokens.SlidingToken",
+        ),
+    )
+    def test_get_validated_token_accept_known_token(self):
         # Should accept tokens included in AUTH_TOKEN_CLASSES
         access_token = AccessToken()
         sliding_token = SlidingToken()
-        with override_api_settings(
-            AUTH_TOKEN_CLASSES=(
-                "rest_framework_simplejwt_mongoengine.tokens.AccessToken",
-                "rest_framework_simplejwt_mongoengine.tokens.SlidingToken",
-            )
-        ):
-            self.backend.get_validated_token(str(access_token))
-            self.backend.get_validated_token(str(sliding_token))
+
+        self.backend.get_validated_token(str(access_token))
+        self.backend.get_validated_token(str(sliding_token))
 
     def test_get_user(self):
         payload = {"some_other_id": "foo"}
         object_id = ObjectId()
 
         # Should raise error if no recognizable user identification
         with self.assertRaises(InvalidToken):
@@ -155,14 +158,54 @@
 
         u.is_active = True
         u.save()
 
         # Otherwise, should return correct user
         self.assertEqual(self.backend.get_user(payload).id, u.id)
 
+    @override_api_settings(
+        CHECK_REVOKE_TOKEN=True, REVOKE_TOKEN_CLAIM="revoke_token_claim"
+    )
+    def test_get_user_with_check_revoke_token(self):
+        payload = {"some_other_id": "foo"}
+        object_id = ObjectId()
+
+        # Should raise error if no recognizable user identification
+        with self.assertRaises(InvalidToken):
+            self.backend.get_user(payload)
+
+        payload[api_settings.USER_ID_CLAIM] = object_id
+
+        # Should raise exception if user not found
+        with self.assertRaises(AuthenticationFailed):
+            self.backend.get_user(payload)
+
+        u = User.create_user(username="markhamill", password="markhamill")
+        u.is_active = False
+        u.save()
+
+        payload[api_settings.USER_ID_CLAIM] = getattr(u, api_settings.USER_ID_FIELD)
+
+        # Should raise exception if user is inactive
+        with self.assertRaises(AuthenticationFailed):
+            self.backend.get_user(payload)
+
+        u.is_active = True
+        u.save()
+
+        # Should raise exception if hash password is different
+        with self.assertRaises(AuthenticationFailed):
+            self.backend.get_user(payload)
+
+        if api_settings.CHECK_REVOKE_TOKEN:
+            payload[api_settings.REVOKE_TOKEN_CLAIM] = get_md5_hash_password(u.password)
+
+        # Otherwise, should return correct user
+        self.assertEqual(self.backend.get_user(payload).id, u.id)
+
 
 class TestJWTStatelessUserAuthentication(BaseTestCase):
     def setUp(self):
         self.backend = authentication.JWTStatelessUserAuthentication()
 
     def test_get_user(self):
         payload = {"some_other_id": "foo"}
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_backends.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+import builtins
 import uuid
 from datetime import datetime, timedelta
+from importlib import reload
 from json import JSONEncoder
 from unittest import mock
 from unittest.mock import patch
 
 import jwt
 import pytest
+from django.test import TestCase
 from jwt import PyJWS
 from jwt import __version__ as jwt_version
 from jwt import algorithms
-from rest_framework_simplejwt.exceptions import TokenBackendError
-from rest_framework_simplejwt.utils import aware_utcnow, datetime_to_epoch, make_utc
 
 from rest_framework_simplejwt_mongoengine.backends import JWK_CLIENT_AVAILABLE, TokenBackend
-from rest_framework_simplejwt_mongoengine.utils import drf_simplejwt_version
-from tests.keys import ES256_PRIVATE_KEY, ES256_PUBLIC_KEY, PRIVATE_KEY, PRIVATE_KEY_2, PUBLIC_KEY, PUBLIC_KEY_2
-
-from .utils import BaseTestCase
+from rest_framework_simplejwt_mongoengine.exceptions import TokenBackendError
+from rest_framework_simplejwt_mongoengine.utils import aware_utcnow, datetime_to_epoch, make_utc
+from tests.keys import (
+    ES256_PRIVATE_KEY,
+    ES256_PUBLIC_KEY,
+    PRIVATE_KEY,
+    PRIVATE_KEY_2,
+    PUBLIC_KEY,
+    PUBLIC_KEY_2,
+)
 
 SECRET = "not_secret"
 
 AUDIENCE = "openid-client-id"
 
 ISSUER = "https://www.myoidcprovider.com"
 
@@ -34,81 +41,97 @@
 class UUIDJSONEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, uuid.UUID):
             return str(obj)
         return super().default(obj)
 
 
-class TestTokenBackend(BaseTestCase):
+class TestTokenBackend(TestCase):
     def setUp(self):
+        self.realimport = builtins.__import__
         self.hmac_token_backend = TokenBackend("HS256", SECRET)
-
-        if "4.7" not in drf_simplejwt_version:
-            self.hmac_leeway_token_backend = TokenBackend("HS256", SECRET, leeway=LEEWAY)
-
+        self.hmac_leeway_token_backend = TokenBackend("HS256", SECRET, leeway=LEEWAY)
         self.rsa_token_backend = TokenBackend("RS256", PRIVATE_KEY, PUBLIC_KEY)
-        self.aud_iss_token_backend = TokenBackend("RS256", PRIVATE_KEY, PUBLIC_KEY, AUDIENCE, ISSUER)
+        self.aud_iss_token_backend = TokenBackend(
+            "RS256", PRIVATE_KEY, PUBLIC_KEY, AUDIENCE, ISSUER
+        )
         self.payload = {"foo": "bar"}
         self.backends = (
-            (
-                self.hmac_token_backend,
-                self.rsa_token_backend,
-                TokenBackend("ES256", ES256_PRIVATE_KEY, ES256_PUBLIC_KEY),
-                TokenBackend("ES384", ES256_PRIVATE_KEY, ES256_PUBLIC_KEY),
-                TokenBackend("ES512", ES256_PRIVATE_KEY, ES256_PUBLIC_KEY),
-            )
-            if "5.1" in drf_simplejwt_version or "5.2" in drf_simplejwt_version
-            else (self.hmac_token_backend, self.rsa_token_backend)
+            self.hmac_token_backend,
+            self.rsa_token_backend,
+            TokenBackend("ES256", ES256_PRIVATE_KEY, ES256_PUBLIC_KEY),
+            TokenBackend("ES384", ES256_PRIVATE_KEY, ES256_PUBLIC_KEY),
+            TokenBackend("ES512", ES256_PRIVATE_KEY, ES256_PUBLIC_KEY),
         )
 
     def test_init(self):
         # Should reject unknown algorithms
         with self.assertRaises(TokenBackendError):
             TokenBackend("oienarst oieanrsto i", "not_secret")
 
         TokenBackend("HS256", "not_secret")
 
     @patch.object(algorithms, "has_crypto", new=False)
     def test_init_fails_for_rs_algorithms_when_crypto_not_installed(self):
-        test_algorithms = ("RS256", "RS384", "RS512")
+        for algo in ("RS256", "RS384", "RS512", "ES256"):
+            with self.assertRaisesRegex(
+                TokenBackendError,
+                f"You must have cryptography installed to use {algo}.",
+            ):
+                TokenBackend(algo, "not_secret")
 
-        if "5.1" in drf_simplejwt_version or "5.2" in drf_simplejwt_version:
-            test_algorithms += ("ES256",)
+    def test_jwk_client_not_available(self):
+        from rest_framework_simplejwt_mongoengine import backends
 
-        for algo in test_algorithms:
-            with self.assertRaisesRegex(TokenBackendError, f"You must have cryptography installed to use {algo}."):
-                TokenBackend(algo, "not_secret")
+        def myimport(name, globals=None, locals=None, fromlist=(), level=0):
+            if name == "jwt" and fromlist == ("PyJWKClient", "PyJWKClientError"):
+                raise ImportError
+            return self.realimport(name, globals, locals, fromlist, level)
+
+        builtins.__import__ = myimport
+
+        # Reload backends, mock jwk client is not available
+        reload(backends)
+
+        self.assertEqual(backends.JWK_CLIENT_AVAILABLE, False)
+        self.assertEqual(backends.TokenBackend("HS256").jwks_client, None)
+
+        builtins.__import__ = self.realimport
+
+    @patch("jwt.encode", mock.Mock(return_value=b"test"))
+    def test_token_encode_should_return_str_for_old_PyJWT(self):
+        self.assertIsInstance(TokenBackend("HS256").encode({}), str)
 
     def test_encode_hmac(self):
         # Should return a JSON web token for the given payload
         payload = {"exp": make_utc(datetime(year=2000, month=1, day=1))}
 
         hmac_token = self.hmac_token_backend.encode(payload)
 
         # Token could be one of two depending on header dict ordering
         self.assertIn(
             hmac_token,
             (
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMH0.NHpdD2X8ub4SE_MZLBedWa57FCpntGaN_r6f8kNKdUs",  # noqa: E501
-                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMH0.jvxQgXCSDToR8uKoRJcMT-LmMJJn2-NM76nfSR2FOgs",  # noqa: E501
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMH0.NHpdD2X8ub4SE_MZLBedWa57FCpntGaN_r6f8kNKdUs",
+                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMH0.jvxQgXCSDToR8uKoRJcMT-LmMJJn2-NM76nfSR2FOgs",
             ),
         )
 
     def test_encode_rsa(self):
         # Should return a JSON web token for the given payload
         payload = {"exp": make_utc(datetime(year=2000, month=1, day=1))}
 
         rsa_token = self.rsa_token_backend.encode(payload)
 
         # Token could be one of two depending on header dict ordering
         self.assertIn(
             rsa_token,
             (
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMH0.cuE6ocmdxVHXVrGufzn-_ZbXDV475TPPb5jtSacvJsnR3s3tLIm9yR7MF4vGcCAUGJn2hU_JgSOhs9sxntPPVjdwvC3-sxAwfUQ5AgUCEAF5XC7wTvGhmvufzhAgEG_DNsactCh79P8xRnc0iugtlGNyFp_YK582-ZrlfQEp-7C0L9BNG_JCS2J9DsGR7ojO2xGFkFfzezKRkrVTJMPLwpl0JAiZ0iqbQE-Tex7redCrGI388_mgh52GLsNlSIvW2gQMqCVMYndMuYx32Pd5tuToZmLUQ2PJ9RyAZ4fOMApTzoshItg4lGqtnt9CDYzypHULJZohJIPcxFVZZfHxhw",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMH0.pzHTOaVvKJMMkSqksGh-NdeEvQy8Thre3hBM3smUW5Sohtg77KnHpaUYjq30DyRmYQRmPSjEVprh1Yvic_-OeAXPW8WVsF-r4YdJuxWUpuZbIPwJ9E-cMfTZkDkOl18z1zOdlsLtsP2kXyAlptyy9QQsM7AxoqM6cyXoQ5TI0geWccgoahTy3cBtA6pmjm7H0nfeDGqpqYQBhtaFmRuIWn-_XtdN9C6NVmRCcZwyjH-rP3oEm6wtuKJEN25sVWlZm8YRQ-rj7A7SNqBB5tFK2anM_iv4rmBlIEkmr_f2s_WqMxn2EWUSNeqbqiwabR6CZUyJtKx1cPG0B2PqOTcZsg",  # noqa: E501
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMH0.cuE6ocmdxVHXVrGufzn-_ZbXDV475TPPb5jtSacvJsnR3s3tLIm9yR7MF4vGcCAUGJn2hU_JgSOhs9sxntPPVjdwvC3-sxAwfUQ5AgUCEAF5XC7wTvGhmvufzhAgEG_DNsactCh79P8xRnc0iugtlGNyFp_YK582-ZrlfQEp-7C0L9BNG_JCS2J9DsGR7ojO2xGFkFfzezKRkrVTJMPLwpl0JAiZ0iqbQE-Tex7redCrGI388_mgh52GLsNlSIvW2gQMqCVMYndMuYx32Pd5tuToZmLUQ2PJ9RyAZ4fOMApTzoshItg4lGqtnt9CDYzypHULJZohJIPcxFVZZfHxhw",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMH0.pzHTOaVvKJMMkSqksGh-NdeEvQy8Thre3hBM3smUW5Sohtg77KnHpaUYjq30DyRmYQRmPSjEVprh1Yvic_-OeAXPW8WVsF-r4YdJuxWUpuZbIPwJ9E-cMfTZkDkOl18z1zOdlsLtsP2kXyAlptyy9QQsM7AxoqM6cyXoQ5TI0geWccgoahTy3cBtA6pmjm7H0nfeDGqpqYQBhtaFmRuIWn-_XtdN9C6NVmRCcZwyjH-rP3oEm6wtuKJEN25sVWlZm8YRQ-rj7A7SNqBB5tFK2anM_iv4rmBlIEkmr_f2s_WqMxn2EWUSNeqbqiwabR6CZUyJtKx1cPG0B2PqOTcZsg",
             ),
         )
 
     def test_encode_aud_iss(self):
         # Should return a JSON web token for the given payload
         original_payload = {"exp": make_utc(datetime(year=2000, month=1, day=1))}
         payload = original_payload.copy()
@@ -118,62 +141,76 @@
         # Assert that payload has not been mutated by the encode() function
         self.assertEqual(payload, original_payload)
 
         # Token could be one of 12 depending on header dict ordering
         self.assertIn(
             rsa_token,
             (
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCIsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.kSz7KyUZgpKaeQHYSQlhsE-UFLG2zhBiJ2MFCIvhstA4lSIKj3U1fdP1OhEDg7X66EquRRIZrby6M7RncqCdsjRwKrEIaL74KgC4s5PDXa_HC6dtpi2GhXqaLz8YxfCPaNGZ_9q9rs4Z4O6WpwBLNmMQrTxNno9p0uT93Z2yKj5hGih8a9C_CSf_rKtsHW9AJShWGoKpR6qQFKVNP1GAwQOQ6IeEvZenq_LSEywnrfiWp4Y5UF7xi42wWx7_YPQtM9_Bp5sB-DbrKg_8t0zSc-OHeVDgH0TKqygGEea09W0QkmJcROkaEbxt2LxJg9OuSdXgudVytV8ewpgNtWNE4g",  # noqa: E501
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMCwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.l-sJR5VKGKNrEn5W8sfO4tEpPq4oQ-Fm5ttQyqUkF6FRJHmCfS1TZIUSXieDLHmarnb4hdIGLr5y-EAbykiqYaTn8d25oT2_zIPlCYHt0DxxeuOliGad5l3AXbWee0qPoZL7YCV8FaSdv2EjtMDOEiJBG5yTkaqZlRmSkbfqu1_y2DRErv3X5LpfEHuKoum4jv5YpoCS6wAWDaWJ9cXMPQaGc4gXg4cuSQxb_EjiQ3QYyztHhG37gOu1J-r_rudaiiIk_VZQdYNfCcirp8isS0z2dcNij_0bELp_oOaipsF7uwzc6WfNGR7xP50X1a_K6EBZzVs0eXFxvl9b3C_d8A",  # noqa: E501
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDAsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.aTwQEIxSzhI5fN4ffQMzZ6h61Ur-Gzh_gPkgOyyWvMX890Z18tC2RisEjXeL5xDGKe2XiEAVtuJa9CjXB9eJoCxNN1k05C-ph82cco-0m_TbMbs0d1MFnfC9ESr4JKynP_Klxi8bi0iZMazduT15pH4UhRkEGsnp8rOKtlt_8_8UOGBJAzG34161lM4JbZqrZDit1DvQdGxaC0lmMgosKg3NDMECfkPe3pGLJ5F_su5yhQk0xyKNCjYyE2FNlilWoDV2KkGiCWdsFOgRMAJwHZ-cdgPg8Vyh2WthBNblsbRVfDrGtfPX0VuW5B0RhBhvI5Iut34P9kkxKRFo3NaiEg",  # noqa: E501
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiZXhwIjo5NDY2ODQ4MDB9.w46s7u28LgsnmK6K_5O15q1SFkKeRgkkplFLi5idq1z7qJjXUi45qpXIyQw3W8a0k1fwa22WB_0XC1MTo22OK3Z0aGNCI2ZCBxvZGOAc1WcCUae44a9LckPHp80q0Hs03NvjsuRVLGXRwDVHrYxuGnFxQSEMbZ650-MQkfVFIXVzMOOAn5Yl4ntjigLcw8iPEqJPnDLdFUSnObZjRzK1M6mJf0-125pqcFsCJaa49rjdbTtnN-VuGnKmv9wV1GwevRQPWjx2vinETURVO9IyZCDtdaLJkvL7Z5IpToK5jrZPc1UWAR0VR8WeWfussFoHzJF86LxVxnqIeXnqOhq5SQ",  # noqa: E501
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDB9.Np_SJYye14vz0cvALvfYNqZXvXMD_gY6kIaxA458kbeu6veC_Ds45uWgjJFhTSYFAFWd3TB6M7qZbWgiO0ycION2-B9Yfgaf82WzNtPfgDhu51w1cbLnvuOSRvgX69Q6Z2i1SByewKaSDw25BaMv9Ty4DBdoCbG62qELnNKjDSQvuHlz8cRJv2I6xJBeOYgZV-YN8Zmxsles44a57Vvcj-DjVouHj5m4LperIxb9islNUQBPRTbvw1d_tR8O8ny0mQqbsWL7e2J-wfwdduVf1kVCPePkhHMM6GLhPIrSoTgMzZuRYLBJ61yphuDK98zTknNBM-Jtn5cMyBwP9JBJvA",  # noqa: E501
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.KJcWZtEluPrkRbYj2i_QmdWpZqGZt63Q8nO4QAJ4B4418ZfmgB6A54_vUmWd3Xc18DYgReLoNPlaOuRXtR7rzlMk0-ADjV0bsca5NwTNAV2F-gR9Xsr9iFlcPMNAYf4CAs85gg7deMIxlbGTAaoft__58ah2_vdd8o_nem1PdzsPC198AYtcwnIV206qpeCNR8S_ZTU46OaHwCoySVRx9E7tNG13YSCmGvBaEqgQHKH82qLXo0KivFrjGmGP0xePFG1B8HCZl-LH1euXGGCp6S48q-tmepX5GJwvzaZNBam4pfxQ0GIHa7z11e7sEN-196iDPCK8NzDcXFwHOAnyaA",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCIsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.MfhVcFN-9Rd0j11CLtxopzREKdyJH1loSpD4ibjP6Aco4-iM5C99B6gliPgOldtuevhneXV2I7NGhmZFULaYhulcLrAgKe3Gj_TK-sHvwb62e14ArugmK_FAhN7UqbX8hU9wP42LaWXqA7ps4kkJSx-sfgHqMzCKewlAZWwyZBoFgWEgoheKZ7ILkSGf0jzBZlS_1R0jFRSrlYD9rI1S4Px-HllS0t32wRCSbzkp6aVMRs46S0ePrN1mK3spsuQXtYhE2913ZC7p2KwyTGfC2FOOeJdRJknh6kI3Z7pTcsjN2jnQN3o8vPEkN3wl7MbAgAsHcUV45pvyxn4SNBmTMQ",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMCwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.3NjgS14SGFyJ6cix2XJZFPlcyeSu4LSduEMUIH0grJuCljbhalyoib5s4JnBaK4slKrQv1WHlhnKB737hX1FF7_EwQM3toCf--DBjrIuq5cYK3rzcn71JDe_op3CvClwpVyxd2vQZtQfP_tWqN6cNTuWF8ZQ0rJGug6Zb-NeE5h68YK_9tXLZC_i5anyjjAVONOc3Nd-TeIUBaLQKQXOddw0gcTcA7vg3uS0gXTEDq-_ZkF-v9bn1ua4_lgRPbuaYvrBFbXSCEdvNORPfPz4zfL3XU09q0gmnmXC9nxjUFVX4BjkP_YiCCO42sqUKY4y7STTB_IkK_04e2wntonVZA",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.b4pdohov81oqzLyCIp4y7e4VYz7LSez7bH0t1o0Zwzau1uXPYXcasT9lxxNMEEiZwHIovPLyWQ6XvF0bMWTk9vc4PyIpkLqsLBJPsuQ-wYUOD04fECmqUX_JaINqm2pPbohTcOQwl0xsE1UMIKTFBZDL1hEXGEMdW9lrPcXilhbC1ikyMpzsmVh55Q_wL2GqydssnOOcDQTqEkWoKvELJJhBcE-YuQkUp8jEVhF3VZ4jEZkzCErTlyXcfe1qXZHkWtw2QNo9s_SfLuRy_fACOo8XE9pHBoE7rqiSm-FmISgiLO1Jj3Pqq-abjN4SnAbU7PZWcV3fUoO1eYLGORmAcw",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDB9.yDGMBeee4hj8yDtEvVtIsS4tnkPjDMQADTkNh74wtb3oYPgQNqMRWKngXiwjvW2FmnsCUue2cFzLgTbpqlDq0QKcBP0i_UwBiXk9m2wLo0WRFtgw2zNHYSsowu26sFoEjKLgpPZzKrPlU4pnxqa8u3yqg8vIcSTlpX8t3uDqNqhUKP6x-w6wb25h67XDmnORiMwhaOZE_Gs9-H6uWnKdguTIlU1Tj4CjUEnZgZN7dJORiDnO_vHiAyL5yvRjhp5YK0Pq-TtCj5kWoJsjQiKc4laIcgofAKoq_b62Psns8MhxzAxwM7i0rbQZXXYB0VKMUho88uHlpbSWCZxu415lWw",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiZXhwIjo5NDY2ODQ4MDB9.BHSCjFeXS6B7KFJi1LpQMEd3ib4Bp9FY3WcB-v7dtP3Ay0SxQZz_gxIbi-tYiNCBQIlfKcfq6vELOjE1WJ5zxPDQM8uV0Pjl41hqYBu3qFv4649a-o2Cd-MaSPUSUogPxzTh2Bk4IdM3sG1Zbd_At4DR_DQwWJDuChA8duA5yG2XPkZr0YF1ZJ326O_jEowvCJiZpzOpH9QsLVPbiX49jtWTwqQGhvpKEj3ztTLFo8VHO-p8bhOGEph2F73F6-GB0XqiWk2Dm1yKAunJCMsM4qXooWfaX6gj-WFhPI9kEXNFfGmPal5i1gb17YoeinbdV2kjN42oxast2Iaa3CMldw",  # noqa: E501
-                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDAsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.s6sElpfKL8WHWfbD_Kbwiy_ip4O082V8ElZqwugvDpS-7yQ3FTvQ3WXqtVAJc-fBZe4ZsBnrXUWwZV0Nhoe6iWKjEjTPjonQWbWL_WUJmIC2HVz18AOISnqReV2rcuLSHQ2ckhsyktlE9K1Rfj-Hi6f3HzzzePEgTsL2ZdBH6GrcmJVDFKqLLrkvOHShoPp7rcwuFBr0J_S1oqYac5O0B-u0OVnxBXTwij0ThrTGMgVCp2rn6Hk0NvtF6CE49Eu4XP8Ue-APT8l5_SjqX9GcrjkJp8Gif_oyBheL-zRg_v-cU60X6qY9wVolO8WodVPSnlE02XyYhLVxvfK-w5129A",  # noqa: E501
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCIsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.kSz7KyUZgpKaeQHYSQlhsE-UFLG2zhBiJ2MFCIvhstA4lSIKj3U1fdP1OhEDg7X66EquRRIZrby6M7RncqCdsjRwKrEIaL74KgC4s5PDXa_HC6dtpi2GhXqaLz8YxfCPaNGZ_9q9rs4Z4O6WpwBLNmMQrTxNno9p0uT93Z2yKj5hGih8a9C_CSf_rKtsHW9AJShWGoKpR6qQFKVNP1GAwQOQ6IeEvZenq_LSEywnrfiWp4Y5UF7xi42wWx7_YPQtM9_Bp5sB-DbrKg_8t0zSc-OHeVDgH0TKqygGEea09W0QkmJcROkaEbxt2LxJg9OuSdXgudVytV8ewpgNtWNE4g",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMCwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.l-sJR5VKGKNrEn5W8sfO4tEpPq4oQ-Fm5ttQyqUkF6FRJHmCfS1TZIUSXieDLHmarnb4hdIGLr5y-EAbykiqYaTn8d25oT2_zIPlCYHt0DxxeuOliGad5l3AXbWee0qPoZL7YCV8FaSdv2EjtMDOEiJBG5yTkaqZlRmSkbfqu1_y2DRErv3X5LpfEHuKoum4jv5YpoCS6wAWDaWJ9cXMPQaGc4gXg4cuSQxb_EjiQ3QYyztHhG37gOu1J-r_rudaiiIk_VZQdYNfCcirp8isS0z2dcNij_0bELp_oOaipsF7uwzc6WfNGR7xP50X1a_K6EBZzVs0eXFxvl9b3C_d8A",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDAsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.aTwQEIxSzhI5fN4ffQMzZ6h61Ur-Gzh_gPkgOyyWvMX890Z18tC2RisEjXeL5xDGKe2XiEAVtuJa9CjXB9eJoCxNN1k05C-ph82cco-0m_TbMbs0d1MFnfC9ESr4JKynP_Klxi8bi0iZMazduT15pH4UhRkEGsnp8rOKtlt_8_8UOGBJAzG34161lM4JbZqrZDit1DvQdGxaC0lmMgosKg3NDMECfkPe3pGLJ5F_su5yhQk0xyKNCjYyE2FNlilWoDV2KkGiCWdsFOgRMAJwHZ-cdgPg8Vyh2WthBNblsbRVfDrGtfPX0VuW5B0RhBhvI5Iut34P9kkxKRFo3NaiEg",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiZXhwIjo5NDY2ODQ4MDB9.w46s7u28LgsnmK6K_5O15q1SFkKeRgkkplFLi5idq1z7qJjXUi45qpXIyQw3W8a0k1fwa22WB_0XC1MTo22OK3Z0aGNCI2ZCBxvZGOAc1WcCUae44a9LckPHp80q0Hs03NvjsuRVLGXRwDVHrYxuGnFxQSEMbZ650-MQkfVFIXVzMOOAn5Yl4ntjigLcw8iPEqJPnDLdFUSnObZjRzK1M6mJf0-125pqcFsCJaa49rjdbTtnN-VuGnKmv9wV1GwevRQPWjx2vinETURVO9IyZCDtdaLJkvL7Z5IpToK5jrZPc1UWAR0VR8WeWfussFoHzJF86LxVxnqIeXnqOhq5SQ",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDB9.Np_SJYye14vz0cvALvfYNqZXvXMD_gY6kIaxA458kbeu6veC_Ds45uWgjJFhTSYFAFWd3TB6M7qZbWgiO0ycION2-B9Yfgaf82WzNtPfgDhu51w1cbLnvuOSRvgX69Q6Z2i1SByewKaSDw25BaMv9Ty4DBdoCbG62qELnNKjDSQvuHlz8cRJv2I6xJBeOYgZV-YN8Zmxsles44a57Vvcj-DjVouHj5m4LperIxb9islNUQBPRTbvw1d_tR8O8ny0mQqbsWL7e2J-wfwdduVf1kVCPePkhHMM6GLhPIrSoTgMzZuRYLBJ61yphuDK98zTknNBM-Jtn5cMyBwP9JBJvA",
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.KJcWZtEluPrkRbYj2i_QmdWpZqGZt63Q8nO4QAJ4B4418ZfmgB6A54_vUmWd3Xc18DYgReLoNPlaOuRXtR7rzlMk0-ADjV0bsca5NwTNAV2F-gR9Xsr9iFlcPMNAYf4CAs85gg7deMIxlbGTAaoft__58ah2_vdd8o_nem1PdzsPC198AYtcwnIV206qpeCNR8S_ZTU46OaHwCoySVRx9E7tNG13YSCmGvBaEqgQHKH82qLXo0KivFrjGmGP0xePFG1B8HCZl-LH1euXGGCp6S48q-tmepX5GJwvzaZNBam4pfxQ0GIHa7z11e7sEN-196iDPCK8NzDcXFwHOAnyaA",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCIsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.MfhVcFN-9Rd0j11CLtxopzREKdyJH1loSpD4ibjP6Aco4-iM5C99B6gliPgOldtuevhneXV2I7NGhmZFULaYhulcLrAgKe3Gj_TK-sHvwb62e14ArugmK_FAhN7UqbX8hU9wP42LaWXqA7ps4kkJSx-sfgHqMzCKewlAZWwyZBoFgWEgoheKZ7ILkSGf0jzBZlS_1R0jFRSrlYD9rI1S4Px-HllS0t32wRCSbzkp6aVMRs46S0ePrN1mK3spsuQXtYhE2913ZC7p2KwyTGfC2FOOeJdRJknh6kI3Z7pTcsjN2jnQN3o8vPEkN3wl7MbAgAsHcUV45pvyxn4SNBmTMQ",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMCwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.3NjgS14SGFyJ6cix2XJZFPlcyeSu4LSduEMUIH0grJuCljbhalyoib5s4JnBaK4slKrQv1WHlhnKB737hX1FF7_EwQM3toCf--DBjrIuq5cYK3rzcn71JDe_op3CvClwpVyxd2vQZtQfP_tWqN6cNTuWF8ZQ0rJGug6Zb-NeE5h68YK_9tXLZC_i5anyjjAVONOc3Nd-TeIUBaLQKQXOddw0gcTcA7vg3uS0gXTEDq-_ZkF-v9bn1ua4_lgRPbuaYvrBFbXSCEdvNORPfPz4zfL3XU09q0gmnmXC9nxjUFVX4BjkP_YiCCO42sqUKY4y7STTB_IkK_04e2wntonVZA",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJleHAiOjk0NjY4NDgwMCwiYXVkIjoib3BlbmlkLWNsaWVudC1pZCJ9.b4pdohov81oqzLyCIp4y7e4VYz7LSez7bH0t1o0Zwzau1uXPYXcasT9lxxNMEEiZwHIovPLyWQ6XvF0bMWTk9vc4PyIpkLqsLBJPsuQ-wYUOD04fECmqUX_JaINqm2pPbohTcOQwl0xsE1UMIKTFBZDL1hEXGEMdW9lrPcXilhbC1ikyMpzsmVh55Q_wL2GqydssnOOcDQTqEkWoKvELJJhBcE-YuQkUp8jEVhF3VZ4jEZkzCErTlyXcfe1qXZHkWtw2QNo9s_SfLuRy_fACOo8XE9pHBoE7rqiSm-FmISgiLO1Jj3Pqq-abjN4SnAbU7PZWcV3fUoO1eYLGORmAcw",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJodHRwczovL3d3dy5teW9pZGNwcm92aWRlci5jb20iLCJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDB9.yDGMBeee4hj8yDtEvVtIsS4tnkPjDMQADTkNh74wtb3oYPgQNqMRWKngXiwjvW2FmnsCUue2cFzLgTbpqlDq0QKcBP0i_UwBiXk9m2wLo0WRFtgw2zNHYSsowu26sFoEjKLgpPZzKrPlU4pnxqa8u3yqg8vIcSTlpX8t3uDqNqhUKP6x-w6wb25h67XDmnORiMwhaOZE_Gs9-H6uWnKdguTIlU1Tj4CjUEnZgZN7dJORiDnO_vHiAyL5yvRjhp5YK0Pq-TtCj5kWoJsjQiKc4laIcgofAKoq_b62Psns8MhxzAxwM7i0rbQZXXYB0VKMUho88uHlpbSWCZxu415lWw",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiaXNzIjoiaHR0cHM6Ly93d3cubXlvaWRjcHJvdmlkZXIuY29tIiwiZXhwIjo5NDY2ODQ4MDB9.BHSCjFeXS6B7KFJi1LpQMEd3ib4Bp9FY3WcB-v7dtP3Ay0SxQZz_gxIbi-tYiNCBQIlfKcfq6vELOjE1WJ5zxPDQM8uV0Pjl41hqYBu3qFv4649a-o2Cd-MaSPUSUogPxzTh2Bk4IdM3sG1Zbd_At4DR_DQwWJDuChA8duA5yG2XPkZr0YF1ZJ326O_jEowvCJiZpzOpH9QsLVPbiX49jtWTwqQGhvpKEj3ztTLFo8VHO-p8bhOGEph2F73F6-GB0XqiWk2Dm1yKAunJCMsM4qXooWfaX6gj-WFhPI9kEXNFfGmPal5i1gb17YoeinbdV2kjN42oxast2Iaa3CMldw",
+                "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJvcGVuaWQtY2xpZW50LWlkIiwiZXhwIjo5NDY2ODQ4MDAsImlzcyI6Imh0dHBzOi8vd3d3Lm15b2lkY3Byb3ZpZGVyLmNvbSJ9.s6sElpfKL8WHWfbD_Kbwiy_ip4O082V8ElZqwugvDpS-7yQ3FTvQ3WXqtVAJc-fBZe4ZsBnrXUWwZV0Nhoe6iWKjEjTPjonQWbWL_WUJmIC2HVz18AOISnqReV2rcuLSHQ2ckhsyktlE9K1Rfj-Hi6f3HzzzePEgTsL2ZdBH6GrcmJVDFKqLLrkvOHShoPp7rcwuFBr0J_S1oqYac5O0B-u0OVnxBXTwij0ThrTGMgVCp2rn6Hk0NvtF6CE49Eu4XP8Ue-APT8l5_SjqX9GcrjkJp8Gif_oyBheL-zRg_v-cU60X6qY9wVolO8WodVPSnlE02XyYhLVxvfK-w5129A",
             ),
         )
 
     def test_decode_with_no_expiry(self):
         for backend in self.backends:
             with self.subTest("Test decode with no expiry for f{backend.algorithm}"):
-                no_exp_token = jwt.encode(self.payload, backend.signing_key, algorithm=backend.algorithm)
+                no_exp_token = jwt.encode(
+                    self.payload, backend.signing_key, algorithm=backend.algorithm
+                )
 
                 backend.decode(no_exp_token)
 
     def test_decode_with_no_expiry_no_verify(self):
         for backend in self.backends:
-            with self.subTest("Test decode with no expiry and no verify for f{backend.algorithm}"):
-                no_exp_token = jwt.encode(self.payload, backend.signing_key, algorithm=backend.algorithm)
-
-                self.assertEqual(backend.decode(no_exp_token, verify=False), self.payload)
+            with self.subTest(
+                "Test decode with no expiry and no verify for f{backend.algorithm}"
+            ):
+                no_exp_token = jwt.encode(
+                    self.payload, backend.signing_key, algorithm=backend.algorithm
+                )
+
+                self.assertEqual(
+                    backend.decode(no_exp_token, verify=False),
+                    self.payload,
+                )
 
     def test_decode_with_expiry(self):
         self.payload["exp"] = aware_utcnow() - timedelta(seconds=1)
         for backend in self.backends:
             with self.subTest("Test decode with expiry for f{backend.algorithm}"):
-
-                expired_token = jwt.encode(self.payload, backend.signing_key, algorithm=backend.algorithm)
+                expired_token = jwt.encode(
+                    self.payload, backend.signing_key, algorithm=backend.algorithm
+                )
 
                 with self.assertRaises(TokenBackendError):
                     backend.decode(expired_token)
 
     def test_decode_with_invalid_sig(self):
         self.payload["exp"] = aware_utcnow() - timedelta(seconds=1)
         for backend in self.backends:
             with self.subTest(f"Test decode with invalid sig for {backend.algorithm}"):
                 payload = self.payload.copy()
                 payload["exp"] = aware_utcnow() + timedelta(days=1)
-                token_1 = jwt.encode(payload, backend.signing_key, algorithm=backend.algorithm)
+                token_1 = jwt.encode(
+                    payload, backend.signing_key, algorithm=backend.algorithm
+                )
                 payload["foo"] = "baz"
-                token_2 = jwt.encode(payload, backend.signing_key, algorithm=backend.algorithm)
+                token_2 = jwt.encode(
+                    payload, backend.signing_key, algorithm=backend.algorithm
+                )
 
                 if IS_OLD_JWT:
                     token_1 = token_1.decode("utf-8")
                     token_2 = token_2.decode("utf-8")
 
                 token_2_payload = token_2.rsplit(".", 1)[0]
                 token_1_sig = token_1.rsplit(".", 1)[-1]
@@ -183,37 +220,45 @@
                     backend.decode(invalid_token)
 
     def test_decode_with_invalid_sig_no_verify(self):
         self.payload["exp"] = aware_utcnow() + timedelta(days=1)
         for backend in self.backends:
             with self.subTest("Test decode with invalid sig for f{backend.algorithm}"):
                 payload = self.payload.copy()
-                token_1 = jwt.encode(payload, backend.signing_key, algorithm=backend.algorithm)
+                token_1 = jwt.encode(
+                    payload, backend.signing_key, algorithm=backend.algorithm
+                )
                 payload["foo"] = "baz"
-                token_2 = jwt.encode(payload, backend.signing_key, algorithm=backend.algorithm)
+                token_2 = jwt.encode(
+                    payload, backend.signing_key, algorithm=backend.algorithm
+                )
                 if IS_OLD_JWT:
                     token_1 = token_1.decode("utf-8")
                     token_2 = token_2.decode("utf-8")
                 else:
                     # Payload copied
                     payload["exp"] = datetime_to_epoch(payload["exp"])
 
                 token_2_payload = token_2.rsplit(".", 1)[0]
                 token_1_sig = token_1.rsplit(".", 1)[-1]
                 invalid_token = token_2_payload + "." + token_1_sig
 
-                self.assertEqual(backend.decode(invalid_token, verify=False), payload)
+                self.assertEqual(
+                    backend.decode(invalid_token, verify=False),
+                    payload,
+                )
 
     def test_decode_success(self):
         self.payload["exp"] = aware_utcnow() + timedelta(days=1)
         self.payload["foo"] = "baz"
         for backend in self.backends:
             with self.subTest("Test decode success for f{backend.algorithm}"):
-
-                token = jwt.encode(self.payload, backend.signing_key, algorithm=backend.algorithm)
+                token = jwt.encode(
+                    self.payload, backend.signing_key, algorithm=backend.algorithm
+                )
                 if IS_OLD_JWT:
                     token = token.decode("utf-8")
                     payload = self.payload
                 else:
                     # Payload copied
                     payload = self.payload.copy()
                     payload["exp"] = datetime_to_epoch(self.payload["exp"])
@@ -232,120 +277,130 @@
         else:
             # Payload copied
             self.payload["exp"] = datetime_to_epoch(self.payload["exp"])
 
         self.assertEqual(self.aud_iss_token_backend.decode(token), self.payload)
 
     @pytest.mark.skipif(
-        # TODO: Uncomment 2 line below when JWK_URL url is reachable
-        # not JWK_CLIENT_AVAILABLE or "4.7" in drf_simplejwt_version,
-        # reason="PyJWT 1.7.1 doesn't have JWK client or Django simplejwt version 4.7.x doesn't have backend PyJWKClient",
-        True,
-        reason=f"URL: {JWK_URL} is not unreachable",
+        not JWK_CLIENT_AVAILABLE,
+        reason="PyJWT 1.7.1 doesn't have JWK client",
     )
     def test_decode_rsa_aud_iss_jwk_success(self):
         self.payload["exp"] = aware_utcnow() + timedelta(days=1)
         self.payload["foo"] = "baz"
         self.payload["aud"] = AUDIENCE
         self.payload["iss"] = ISSUER
 
-        token = jwt.encode(self.payload, PRIVATE_KEY_2, algorithm="RS256", headers={"kid": "230498151c214b788dd97f22b85410a5"})
+        token = jwt.encode(
+            self.payload,
+            PRIVATE_KEY_2,
+            algorithm="RS256",
+            headers={"kid": "230498151c214b788dd97f22b85410a5"},
+        )
         # Payload copied
         self.payload["exp"] = datetime_to_epoch(self.payload["exp"])
 
         mock_jwk_module = mock.MagicMock()
         with patch("rest_framework_simplejwt_mongoengine.backends.PyJWKClient") as mock_jwk_module:
             mock_jwk_client = mock.MagicMock()
             mock_signing_key = mock.MagicMock()
 
             mock_jwk_module.return_value = mock_jwk_client
             mock_jwk_client.get_signing_key_from_jwt.return_value = mock_signing_key
             type(mock_signing_key).key = mock.PropertyMock(return_value=PUBLIC_KEY_2)
 
             # Note the PRIV,PUB care is intentially the original pairing
-            jwk_token_backend = TokenBackend("RS256", PRIVATE_KEY, PUBLIC_KEY, AUDIENCE, ISSUER, JWK_URL)
+            jwk_token_backend = TokenBackend(
+                "RS256", PRIVATE_KEY, PUBLIC_KEY, AUDIENCE, ISSUER, JWK_URL
+            )
 
             self.assertEqual(jwk_token_backend.decode(token), self.payload)
 
     @pytest.mark.skipif(
         not JWK_CLIENT_AVAILABLE,
         reason="PyJWT 1.7.1 doesn't have JWK client",
     )
     def test_decode_jwk_missing_key_raises_tokenbackenderror(self):
         self.payload["exp"] = aware_utcnow() + timedelta(days=1)
         self.payload["foo"] = "baz"
         self.payload["aud"] = AUDIENCE
         self.payload["iss"] = ISSUER
 
-        token = jwt.encode(self.payload, PRIVATE_KEY_2, algorithm="RS256", headers={"kid": "230498151c214b788dd97f22b85410a5"})
+        token = jwt.encode(
+            self.payload,
+            PRIVATE_KEY_2,
+            algorithm="RS256",
+            headers={"kid": "230498151c214b788dd97f22b85410a5"},
+        )
 
         mock_jwk_module = mock.MagicMock()
         with patch("rest_framework_simplejwt_mongoengine.backends.PyJWKClient") as mock_jwk_module:
             mock_jwk_client = mock.MagicMock()
 
             mock_jwk_module.return_value = mock_jwk_client
-            mock_jwk_client.get_signing_key_from_jwt.side_effect = jwt.PyJWKClientError("Unable to find a signing key that matches")
+            mock_jwk_client.get_signing_key_from_jwt.side_effect = jwt.PyJWKClientError(
+                "Unable to find a signing key that matches"
+            )
 
             # Note the PRIV,PUB care is intentially the original pairing
-            jwk_token_backend = TokenBackend("RS256", PRIVATE_KEY, PUBLIC_KEY, AUDIENCE, ISSUER, JWK_URL)
+            jwk_token_backend = TokenBackend(
+                "RS256", PRIVATE_KEY, PUBLIC_KEY, AUDIENCE, ISSUER, JWK_URL
+            )
 
-            with self.assertRaisesRegex(TokenBackendError, "Token is invalid or expired"):
+            with self.assertRaisesRegex(
+                TokenBackendError, "Token is invalid or expired"
+            ):
                 jwk_token_backend.decode(token)
 
     def test_decode_when_algorithm_not_available(self):
         token = jwt.encode(self.payload, PRIVATE_KEY, algorithm="RS256")
         if IS_OLD_JWT:
             token = token.decode("utf-8")
 
         pyjwt_without_rsa = PyJWS()
         pyjwt_without_rsa.unregister_algorithm("RS256")
 
-        if drf_simplejwt_version not in ["4.7.0", "4.7.1", "4.7.2", "4.8.0"]:
-
-            def _decode(jwt, key, algorithms, options, audience, issuer, leeway):
-                return pyjwt_without_rsa.decode(jwt, key, algorithms, options)
+        def _decode(jwt, key, algorithms, options, audience, issuer, leeway):
+            return pyjwt_without_rsa.decode(jwt, key, algorithms, options)
 
-            with patch.object(jwt, "decode", new=_decode):
-                with self.assertRaisesRegex(TokenBackendError, "Invalid algorithm specified"):
-                    self.rsa_token_backend.decode(token)
-        else:
-            with patch.object(jwt, "decode", new=pyjwt_without_rsa.decode):
-                with self.assertRaisesRegex(TokenBackendError, "Invalid algorithm specified"):
-                    self.rsa_token_backend.decode(token)
+        with patch.object(jwt, "decode", new=_decode):
+            with self.assertRaisesRegex(
+                TokenBackendError, "Invalid algorithm specified"
+            ):
+                self.rsa_token_backend.decode(token)
 
     def test_decode_when_token_algorithm_does_not_match(self):
         token = jwt.encode(self.payload, PRIVATE_KEY, algorithm="RS256")
         if IS_OLD_JWT:
             token = token.decode("utf-8")
 
         with self.assertRaisesRegex(TokenBackendError, "Invalid algorithm specified"):
             self.hmac_token_backend.decode(token)
 
-    @pytest.mark.skipif(
-        "4.7" in drf_simplejwt_version,
-        reason="Django simplejwt version 4.7.x doesn't have LEEWAY property in token backend",
-    )
     def test_decode_leeway_hmac_fail(self):
-        self.payload["exp"] = datetime_to_epoch(aware_utcnow() - timedelta(seconds=LEEWAY * 2))
+        self.payload["exp"] = datetime_to_epoch(
+            aware_utcnow() - timedelta(seconds=LEEWAY * 2)
+        )
 
         expired_token = jwt.encode(self.payload, SECRET, algorithm="HS256")
 
         with self.assertRaises(TokenBackendError):
             self.hmac_leeway_token_backend.decode(expired_token)
 
-    @pytest.mark.skipif(
-        "4.7" in drf_simplejwt_version,
-        reason="Django simplejwt version 4.7.x doesn't have LEEWAY property in token backend",
-    )
     def test_decode_leeway_hmac_success(self):
-        self.payload["exp"] = datetime_to_epoch(aware_utcnow() - timedelta(seconds=LEEWAY / 2))
+        self.payload["exp"] = datetime_to_epoch(
+            aware_utcnow() - timedelta(seconds=LEEWAY / 2)
+        )
 
         expired_token = jwt.encode(self.payload, SECRET, algorithm="HS256")
 
-        self.assertEqual(self.hmac_leeway_token_backend.decode(expired_token), self.payload)
+        self.assertEqual(
+            self.hmac_leeway_token_backend.decode(expired_token),
+            self.payload,
+        )
 
     def test_custom_JSONEncoder(self):
         backend = TokenBackend("HS256", SECRET, json_encoder=UUIDJSONEncoder)
         unique = uuid.uuid4()
         self.payload["uuid"] = unique
         token = backend.encode(self.payload)
         decoded = backend.decode(token)
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_integration.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import timedelta
 
+from django.urls import reverse
 from django_mongoengine.mongo_auth.managers import get_user_document
-from rest_framework_simplejwt.compat import reverse
+from rest_framework.status import HTTP_200_OK, HTTP_401_UNAUTHORIZED
 
 from rest_framework_simplejwt_mongoengine.settings import api_settings
 from rest_framework_simplejwt_mongoengine.tokens import AccessToken
 
 from .utils import APIViewTestCase, override_api_settings
 
 User = get_user_document()
@@ -22,15 +23,15 @@
             username=self.username,
             password=self.password,
         )
 
     def test_no_authorization(self):
         res = self.view_get()
 
-        self.assertEqual(res.status_code, 401)
+        self.assertEqual(res.status_code, HTTP_401_UNAUTHORIZED)
         self.assertIn("credentials were not provided", res.data["detail"])
 
     def test_wrong_auth_type(self):
         res = self.client.post(
             reverse("token_obtain_sliding"),
             data={
                 User.USERNAME_FIELD: self.username,
@@ -39,17 +40,20 @@
         )
 
         token = res.data["token"]
         self.authenticate_with_token("Wrong", token)
 
         res = self.view_get()
 
-        self.assertEqual(res.status_code, 401)
+        self.assertEqual(res.status_code, HTTP_401_UNAUTHORIZED)
         self.assertIn("credentials were not provided", res.data["detail"])
 
+    @override_api_settings(
+        AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.AccessToken",),
+    )
     def test_expired_token(self):
         old_lifetime = AccessToken.lifetime
         AccessToken.lifetime = timedelta(seconds=0)
         try:
             res = self.client.post(
                 reverse("token_obtain_pair"),
                 data={
@@ -59,65 +63,67 @@
             )
         finally:
             AccessToken.lifetime = old_lifetime
 
         access = res.data["access"]
         self.authenticate_with_token(api_settings.AUTH_HEADER_TYPES[0], access)
 
-        with override_api_settings(AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.AccessToken",)):
-            res = self.view_get()
+        res = self.view_get()
 
-        self.assertEqual(res.status_code, 401)
+        self.assertEqual(res.status_code, HTTP_401_UNAUTHORIZED)
         self.assertEqual("token_not_valid", res.data["code"])
 
+    @override_api_settings(
+        AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.SlidingToken",),
+    )
     def test_user_can_get_sliding_token_and_use_it(self):
         res = self.client.post(
             reverse("token_obtain_sliding"),
             data={
                 User.USERNAME_FIELD: self.username,
                 "password": self.password,
             },
         )
 
         token = res.data["token"]
         self.authenticate_with_token(api_settings.AUTH_HEADER_TYPES[0], token)
 
-        with override_api_settings(AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.SlidingToken",)):
-            res = self.view_get()
+        res = self.view_get()
 
-        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.status_code, HTTP_200_OK)
         self.assertEqual(res.data["foo"], "bar")
 
+    @override_api_settings(
+        AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.AccessToken",),
+    )
     def test_user_can_get_access_and_refresh_tokens_and_use_them(self):
         res = self.client.post(
             reverse("token_obtain_pair"),
             data={
                 User.USERNAME_FIELD: self.username,
                 "password": self.password,
             },
         )
 
         access = res.data["access"]
         refresh = res.data["refresh"]
 
         self.authenticate_with_token(api_settings.AUTH_HEADER_TYPES[0], access)
 
-        with override_api_settings(AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.AccessToken",)):
-            res = self.view_get()
+        res = self.view_get()
 
-        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.status_code, HTTP_200_OK)
         self.assertEqual(res.data["foo"], "bar")
 
         res = self.client.post(
             reverse("token_refresh"),
             data={"refresh": refresh},
         )
 
         access = res.data["access"]
 
         self.authenticate_with_token(api_settings.AUTH_HEADER_TYPES[0], access)
 
-        with override_api_settings(AUTH_TOKEN_CLASSES=("rest_framework_simplejwt_mongoengine.tokens.AccessToken",)):
-            res = self.view_get()
+        res = self.view_get()
 
-        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.status_code, HTTP_200_OK)
         self.assertEqual(res.data["foo"], "bar")
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_models.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from importlib import reload
+from unittest.mock import patch
+
 from rest_framework_simplejwt_mongoengine.models import TokenUser
 from rest_framework_simplejwt_mongoengine.settings import api_settings
 
 from .utils import BaseTestCase
 
 AuthToken = api_settings.AUTH_TOKEN_CLASSES[0]
 
@@ -11,14 +14,26 @@
         self.token = AuthToken()
         self.token[api_settings.USER_ID_CLAIM] = 42
         self.token["username"] = "deep-thought"
         self.token["some_other_stuff"] = "arstarst"
 
         self.user = TokenUser(self.token)
 
+    def test_type_checking(self):
+        from rest_framework_simplejwt_mongoengine import models
+
+        with patch("typing.TYPE_CHECKING", True):
+            # Reload models, mock type checking
+            reload(models)
+
+            self.assertEqual(models.TYPE_CHECKING, True)
+
+        # Restore origin module without mock
+        reload(models)
+
     def test_username(self):
         self.assertEqual(self.user.username, "deep-thought")
 
     def test_is_active(self):
         self.assertTrue(self.user.is_active)
 
     def test_str(self):
@@ -56,14 +71,20 @@
         user1 = TokenUser({api_settings.USER_ID_CLAIM: 1})
         user2 = TokenUser({api_settings.USER_ID_CLAIM: 2})
         user3 = TokenUser({api_settings.USER_ID_CLAIM: 1})
 
         self.assertNotEqual(user1, user2)
         self.assertEqual(user1, user3)
 
+    def test_eq_not_implemented(self):
+        user1 = TokenUser({api_settings.USER_ID_CLAIM: 1})
+        user2 = "user2"
+
+        self.assertFalse(user1 == user2)
+
     def test_hash(self):
         self.assertEqual(hash(self.user), hash(self.user.id))
 
     def test_not_implemented(self):
         with self.assertRaises(NotImplementedError):
             self.user.save()
 
@@ -95,7 +116,10 @@
         self.assertFalse(self.user.is_anonymous)
 
     def test_is_authenticated(self):
         self.assertTrue(self.user.is_authenticated)
 
     def test_get_username(self):
         self.assertEqual(self.user.get_username(), "deep-thought")
+
+    def test_get_custom_claims_through_backup_getattr(self):
+        self.assertEqual(self.user.some_other_stuff, "arstarst")
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_serializers.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_serializers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,132 @@
 from datetime import timedelta
+from importlib import reload
 from unittest.mock import MagicMock, patch
 
+from django.conf import settings
+
 from django_mongoengine.mongo_auth.managers import get_user_document
 from rest_framework import exceptions as drf_exceptions
-from rest_framework_simplejwt.exceptions import TokenError
-from rest_framework_simplejwt.utils import aware_utcnow, datetime_from_epoch, datetime_to_epoch
 
+from rest_framework_simplejwt_mongoengine.exceptions import TokenError
 from rest_framework_simplejwt_mongoengine.serializers import (
+    TokenBlacklistSerializer,
     TokenObtainPairSerializer,
     TokenObtainSerializer,
     TokenObtainSlidingSerializer,
     TokenRefreshSerializer,
     TokenRefreshSlidingSerializer,
     TokenVerifySerializer,
 )
 from rest_framework_simplejwt_mongoengine.settings import api_settings
-from rest_framework_simplejwt_mongoengine.token_blacklist.models import BlacklistedToken, OutstandingToken
+from rest_framework_simplejwt_mongoengine.token_blacklist.models import (
+    BlacklistedToken,
+    OutstandingToken,
+)
 from rest_framework_simplejwt_mongoengine.tokens import AccessToken, RefreshToken, SlidingToken
-from rest_framework_simplejwt_mongoengine.utils import drf_simplejwt_version, microseconds_to_milliseconds
+from rest_framework_simplejwt_mongoengine.utils import (
+    aware_utcnow,
+    datetime_from_epoch,
+    datetime_to_epoch,
+    microseconds_to_milliseconds,
+)
 
 from .utils import BaseTestCase, override_api_settings
 
 User = get_user_document()
 
 
 class TestTokenObtainSerializer(BaseTestCase):
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_it_should_not_validate_if_any_fields_missing(self):
         s = TokenObtainSerializer(data={})
         self.assertFalse(s.is_valid())
         self.assertIn(s.username_field, s.errors)
         self.assertIn("password", s.errors)
 
-        s = TokenObtainSerializer(data={TokenObtainSerializer.username_field: "oieanrst"})
+        s = TokenObtainSerializer(
+            data={
+                TokenObtainSerializer.username_field: "oieanrst",
+            }
+        )
         self.assertFalse(s.is_valid())
         self.assertIn("password", s.errors)
 
-        s = TokenObtainSerializer(data={"password": "oieanrst"})
+        s = TokenObtainSerializer(
+            data={
+                "password": "oieanrst",
+            }
+        )
         self.assertFalse(s.is_valid())
         self.assertIn(s.username_field, s.errors)
 
     def test_it_should_not_validate_if_user_not_found(self):
         s = TokenObtainSerializer(
             context=MagicMock(),
-            data={TokenObtainSerializer.username_field: "missing", "password": "pass"},
+            data={
+                TokenObtainSerializer.username_field: "missing",
+                "password": "pass",
+            },
         )
 
         with self.assertRaises(drf_exceptions.AuthenticationFailed):
             s.is_valid()
 
+    def test_it_should_pass_validate_if_request_not_in_context(self):
+        s = TokenObtainSerializer(
+            context={},
+            data={
+                "username": self.username,
+                "password": self.password,
+            },
+        )
+
+        s.is_valid()
+
     def test_it_should_raise_if_user_not_active(self):
         self.user.is_active = False
         self.user.save()
 
         s = TokenObtainSerializer(
             context=MagicMock(),
-            data={TokenObtainSerializer.username_field: self.username, "password": self.password},
+            data={
+                TokenObtainSerializer.username_field: self.username,
+                "password": self.password,
+            },
         )
 
         with self.assertRaises(drf_exceptions.AuthenticationFailed):
             s.is_valid()
 
 
 class TestTokenObtainSlidingSerializer(BaseTestCase):
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_it_should_produce_a_json_web_token_when_valid(self):
         s = TokenObtainSlidingSerializer(
             context=MagicMock(),
-            data={TokenObtainSlidingSerializer.username_field: self.username, "password": self.password},
+            data={
+                TokenObtainSlidingSerializer.username_field: self.username,
+                "password": self.password,
+            },
         )
 
         self.assertTrue(s.is_valid())
         self.assertIn("token", s.validated_data)
 
         # Expecting token type claim to be correct for sliding token.  If this
         # is the case, instantiating a `SlidingToken` instance with encoded
@@ -90,20 +135,26 @@
 
 
 class TestTokenObtainPairSerializer(BaseTestCase):
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_it_should_produce_a_json_web_token_when_valid(self):
         s = TokenObtainPairSerializer(
             context=MagicMock(),
-            data={TokenObtainPairSerializer.username_field: self.username, "password": self.password},
+            data={
+                TokenObtainPairSerializer.username_field: self.username,
+                "password": self.password,
+            },
         )
 
         self.assertTrue(s.is_valid())
         self.assertIn("access", s.validated_data)
         self.assertIn("refresh", s.validated_data)
 
         # Expecting token type claim to be correct for both tokens.  If this is
@@ -139,26 +190,36 @@
         del token[api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM]
 
         s = TokenRefreshSlidingSerializer(data={"token": str(token)})
 
         with self.assertRaises(TokenError) as e:
             s.is_valid()
 
-        self.assertIn(f"has no '{api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM}' claim", e.exception.args[0])
+        self.assertIn(
+            f"has no '{api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM}' claim",
+            e.exception.args[0],
+        )
 
     def test_it_should_raise_token_error_if_token_has_refresh_period_expired(self):
         token = SlidingToken()
-        token.set_exp(api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM, lifetime=-timedelta(days=1))
+        token.set_exp(
+            api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM, lifetime=-timedelta(days=1)
+        )
 
         s = TokenRefreshSlidingSerializer(data={"token": str(token)})
 
         with self.assertRaises(TokenError) as e:
             s.is_valid()
 
-        self.assertIn(f"'{api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM}' claim has expired", e.exception.args[0])
+        self.assertIn(
+            "'{}' claim has expired".format(
+                api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM
+            ),
+            e.exception.args[0],
+        )
 
     def test_it_should_raise_token_error_if_token_has_wrong_type(self):
         token = SlidingToken()
         token[api_settings.TOKEN_TYPE_CLAIM] = "wrong_type"
 
         s = TokenRefreshSlidingSerializer(data={"token": str(token)})
 
@@ -230,85 +291,131 @@
         with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
             fake_aware_utcnow.return_value = now
             self.assertTrue(s.is_valid())
 
         access = AccessToken(s.validated_data["access"])
 
         self.assertEqual(refresh["test_claim"], access["test_claim"])
-        self.assertEqual(access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME))
+        self.assertEqual(
+            access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME)
+        )
 
+    @override_api_settings(
+        ROTATE_REFRESH_TOKENS=True,
+        BLACKLIST_AFTER_ROTATION=False,
+    )
     def test_it_should_return_refresh_token_if_tokens_should_be_rotated(self):
         refresh = RefreshToken()
 
         refresh["test_claim"] = "arst"
 
         old_jti = refresh["jti"]
         old_exp = refresh["exp"]
 
         # Serializer validates
         ser = TokenRefreshSerializer(data={"refresh": str(refresh)})
 
-        now = microseconds_to_milliseconds(aware_utcnow()) - api_settings.ACCESS_TOKEN_LIFETIME / 2
+        now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
 
-        with override_api_settings(ROTATE_REFRESH_TOKENS=True, BLACKLIST_AFTER_ROTATION=False):
-            with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
-                fake_aware_utcnow.return_value = now
-                self.assertTrue(ser.is_valid())
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
+            fake_aware_utcnow.return_value = now
+            self.assertTrue(ser.is_valid())
 
         access = AccessToken(ser.validated_data["access"])
         new_refresh = RefreshToken(ser.validated_data["refresh"])
 
         self.assertEqual(refresh["test_claim"], access["test_claim"])
         self.assertEqual(refresh["test_claim"], new_refresh["test_claim"])
 
         self.assertNotEqual(old_jti, new_refresh["jti"])
         self.assertNotEqual(old_exp, new_refresh["exp"])
 
-        self.assertEqual(access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME))
-        self.assertEqual(new_refresh["exp"], datetime_to_epoch(now + api_settings.REFRESH_TOKEN_LIFETIME))
+        self.assertEqual(
+            access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME)
+        )
+        self.assertEqual(
+            new_refresh["exp"],
+            datetime_to_epoch(now + api_settings.REFRESH_TOKEN_LIFETIME),
+        )
 
-    def test_it_should_blacklist_refresh_token_if_tokens_should_be_rotated_and_blacklisted(self):
+    @override_api_settings(
+        ROTATE_REFRESH_TOKENS=True,
+        BLACKLIST_AFTER_ROTATION=True,
+    )
+    def test_it_should_blacklist_refresh_token_if_tokens_should_be_rotated_and_blacklisted(
+        self,
+    ):
         self.assertEqual(OutstandingToken.objects.count(), 0)
         self.assertEqual(BlacklistedToken.objects.count(), 0)
 
         refresh = RefreshToken()
 
         refresh["test_claim"] = "arst"
 
         old_jti = refresh["jti"]
         old_exp = refresh["exp"]
 
         # Serializer validates
         ser = TokenRefreshSerializer(data={"refresh": str(refresh)})
 
-        now = microseconds_to_milliseconds(aware_utcnow()) - api_settings.ACCESS_TOKEN_LIFETIME / 2
+        now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
 
-        with override_api_settings(ROTATE_REFRESH_TOKENS=True, BLACKLIST_AFTER_ROTATION=True):
-            with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
-                fake_aware_utcnow.return_value = now
-                self.assertTrue(ser.is_valid())
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
+            fake_aware_utcnow.return_value = now
+            self.assertTrue(ser.is_valid())
 
         access = AccessToken(ser.validated_data["access"])
         new_refresh = RefreshToken(ser.validated_data["refresh"])
 
         self.assertEqual(refresh["test_claim"], access["test_claim"])
         self.assertEqual(refresh["test_claim"], new_refresh["test_claim"])
 
         self.assertNotEqual(old_jti, new_refresh["jti"])
         self.assertNotEqual(old_exp, new_refresh["exp"])
 
-        self.assertEqual(access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME))
-        self.assertEqual(new_refresh["exp"], datetime_to_epoch(now + api_settings.REFRESH_TOKEN_LIFETIME))
+        self.assertEqual(
+            access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME)
+        )
+        self.assertEqual(
+            new_refresh["exp"],
+            datetime_to_epoch(now + api_settings.REFRESH_TOKEN_LIFETIME),
+        )
 
         self.assertEqual(OutstandingToken.objects.count(), 1)
         self.assertEqual(BlacklistedToken.objects.count(), 1)
 
         # Assert old refresh token is blacklisted
         self.assertEqual(BlacklistedToken.objects.first().token.jti, old_jti)
 
+    @override_api_settings(
+        ROTATE_REFRESH_TOKENS=True,
+        BLACKLIST_AFTER_ROTATION=True,
+    )
+    def test_blacklist_app_not_installed_should_pass(self):
+        from rest_framework_simplejwt_mongoengine import serializers, tokens
+
+        # Remove blacklist app
+        new_apps = list(settings.INSTALLED_APPS)
+        new_apps.remove("rest_framework_simplejwt_mongoengine.token_blacklist")
+
+        with self.settings(INSTALLED_APPS=tuple(new_apps)):
+            # Reload module that blacklist app not installed
+            reload(tokens)
+            reload(serializers)
+
+            refresh = tokens.RefreshToken()
+
+            # Serializer validates
+            ser = serializers.TokenRefreshSerializer(data={"refresh": str(refresh)})
+            ser.validate({"refresh": str(refresh)})
+
+        # Restore origin module without mock
+        reload(tokens)
+        reload(serializers)
+
 
 class TestTokenVerifySerializer(BaseTestCase):
     def test_it_should_raise_token_error_if_token_invalid(self):
         token = RefreshToken()
         del token["exp"]
 
         s = TokenVerifySerializer(data={"token": str(token)})
@@ -347,81 +454,100 @@
         with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
             fake_aware_utcnow.return_value = now
             self.assertTrue(s.is_valid())
 
         self.assertEqual(len(s.validated_data), 0)
 
 
-if drf_simplejwt_version in ["5.0.0", "5.1.0", "5.2.0", "5.2.1", "5.2.2"]:
-    from rest_framework_simplejwt_mongoengine.serializers import TokenBlacklistSerializer
+class TestTokenBlacklistSerializer(BaseTestCase):
+    def test_it_should_raise_token_error_if_token_invalid(self):
+        token = RefreshToken()
+        del token["exp"]
+
+        s = TokenBlacklistSerializer(data={"refresh": str(token)})
+
+        with self.assertRaises(TokenError) as e:
+            s.is_valid()
 
-    class TestTokenBlacklistSerializer(BaseTestCase):
-        def test_it_should_raise_token_error_if_token_invalid(self):
-            token = RefreshToken()
-            del token["exp"]
+        self.assertIn("has no 'exp' claim", e.exception.args[0])
 
-            s = TokenBlacklistSerializer(data={"refresh": str(token)})
+        token.set_exp(lifetime=-timedelta(days=1))
 
-            with self.assertRaises(TokenError) as e:
-                s.is_valid()
+        s = TokenBlacklistSerializer(data={"refresh": str(token)})
 
-            self.assertIn("has no 'exp' claim", e.exception.args[0])
+        with self.assertRaises(TokenError) as e:
+            s.is_valid()
 
-            token.set_exp(lifetime=-timedelta(days=1))
+        self.assertIn("invalid or expired", e.exception.args[0])
 
-            s = TokenBlacklistSerializer(data={"refresh": str(token)})
+    def test_it_should_raise_token_error_if_token_has_wrong_type(self):
+        token = RefreshToken()
+        token[api_settings.TOKEN_TYPE_CLAIM] = "wrong_type"
 
-            with self.assertRaises(TokenError) as e:
-                s.is_valid()
+        s = TokenBlacklistSerializer(data={"refresh": str(token)})
 
-            self.assertIn("invalid or expired", e.exception.args[0])
+        with self.assertRaises(TokenError) as e:
+            s.is_valid()
 
-        def test_it_should_raise_token_error_if_token_has_wrong_type(self):
-            token = RefreshToken()
-            token[api_settings.TOKEN_TYPE_CLAIM] = "wrong_type"
+        self.assertIn("wrong type", e.exception.args[0])
 
-            s = TokenBlacklistSerializer(data={"refresh": str(token)})
+    def test_it_should_return_nothing_if_everything_ok(self):
+        refresh = RefreshToken()
+        refresh["test_claim"] = "arst"
 
-            with self.assertRaises(TokenError) as e:
-                s.is_valid()
+        # Serializer validates
+        s = TokenBlacklistSerializer(data={"refresh": str(refresh)})
 
-            self.assertIn("wrong type", e.exception.args[0])
+        now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
 
-        def test_it_should_return_nothing_if_everything_ok(self):
-            refresh = RefreshToken()
-            refresh["test_claim"] = "arst"
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
+            fake_aware_utcnow.return_value = now
+            self.assertTrue(s.is_valid())
 
-            # Serializer validates
-            s = TokenBlacklistSerializer(data={"refresh": str(refresh)})
+        self.assertDictEqual(s.validated_data, {})
 
-            now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
+    def test_it_should_blacklist_refresh_token_if_everything_ok(self):
+        self.assertEqual(OutstandingToken.objects.count(), 0)
+        self.assertEqual(BlacklistedToken.objects.count(), 0)
 
-            with patch("rest_framework_simplejwt.tokens.aware_utcnow") as fake_aware_utcnow:
-                fake_aware_utcnow.return_value = now
-                self.assertTrue(s.is_valid())
+        refresh = RefreshToken()
+
+        refresh["test_claim"] = "arst"
+
+        old_jti = refresh["jti"]
 
-            self.assertDictEqual(s.validated_data, {})
+        # Serializer validates
+        ser = TokenBlacklistSerializer(data={"refresh": str(refresh)})
 
-        def test_it_should_blacklist_refresh_token_if_everything_ok(self):
-            self.assertEqual(OutstandingToken.objects.count(), 0)
-            self.assertEqual(BlacklistedToken.objects.count(), 0)
+        now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
 
-            refresh = RefreshToken()
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
+            fake_aware_utcnow.return_value = now
+            self.assertTrue(ser.is_valid())
 
-            refresh["test_claim"] = "arst"
+        self.assertEqual(OutstandingToken.objects.count(), 1)
+        self.assertEqual(BlacklistedToken.objects.count(), 1)
 
-            old_jti = refresh["jti"]
+        # Assert old refresh token is blacklisted
+        self.assertEqual(BlacklistedToken.objects.first().token.jti, old_jti)
 
-            # Serializer validates
-            ser = TokenBlacklistSerializer(data={"refresh": str(refresh)})
+    def test_blacklist_app_not_installed_should_pass(self):
+        from rest_framework_simplejwt_mongoengine import serializers, tokens
 
-            now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
+        # Remove blacklist app
+        new_apps = list(settings.INSTALLED_APPS)
+        new_apps.remove("rest_framework_simplejwt_mongoengine.token_blacklist")
+
+        with self.settings(INSTALLED_APPS=tuple(new_apps)):
+            # Reload module that blacklist app not installed
+            reload(tokens)
+            reload(serializers)
 
-            with patch("rest_framework_simplejwt.tokens.aware_utcnow") as fake_aware_utcnow:
-                fake_aware_utcnow.return_value = now
-                self.assertTrue(ser.is_valid())
+            refresh = tokens.RefreshToken()
 
-            self.assertEqual(OutstandingToken.objects.count(), 1)
-            self.assertEqual(BlacklistedToken.objects.count(), 1)
+            # Serializer validates
+            ser = serializers.TokenBlacklistSerializer(data={"refresh": str(refresh)})
+            ser.validate({"refresh": str(refresh)})
 
-            # Assert old refresh token is blacklisted
-            self.assertEqual(BlacklistedToken.objects.first().token.jti, old_jti)
+        # Restore origin module without mock
+        reload(tokens)
+        reload(serializers)
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_token_blacklist.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_token_blacklist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,48 @@
+from importlib import reload
 from unittest.mock import patch
 
 from django.core.management import call_command
+from django.utils import timezone
 from django_mongoengine.mongo_auth.managers import get_user_document
-from rest_framework_simplejwt.exceptions import TokenError
-from rest_framework_simplejwt.utils import aware_utcnow, datetime_from_epoch
 
+from rest_framework_simplejwt_mongoengine.exceptions import TokenError
 from rest_framework_simplejwt_mongoengine.settings import api_settings
 from rest_framework_simplejwt_mongoengine.token_blacklist.models import (
     BlacklistedToken,
     OutstandingToken,
 )
-from rest_framework_simplejwt_mongoengine.tokens import (
-    AccessToken,
-    RefreshToken,
-    SlidingToken,
-)
+from rest_framework_simplejwt_mongoengine.tokens import AccessToken, RefreshToken, SlidingToken
+from rest_framework_simplejwt_mongoengine.utils import aware_utcnow, datetime_from_epoch
 
 from .utils import BaseTestCase
 
 User = get_user_document()
 
 
 class TestTokenBlacklist(BaseTestCase):
     def setUp(self):
         self.user = User.objects.create(
             username="test_user",
             password="test_password",
         )
 
+    def test_token_blacklist_old_django(self):
+        with patch("django.VERSION", (3, 1)):
+            # Import package mock blacklist old django
+            import rest_framework_simplejwt_mongoengine.token_blacklist.__init__ as blacklist
+
+            self.assertEqual(
+                blacklist.default_app_config,
+                ("rest_framework_simplejwt_mongoengine.token_blacklist.apps.TokenBlacklistConfig"),
+            )
+
+        # Restore origin module without mock
+        reload(blacklist)
+
     def test_sliding_tokens_are_added_to_outstanding_list(self):
         token = SlidingToken.for_user(self.user)
 
         qs = OutstandingToken.objects.all()
         outstanding_token = qs.first()
 
         self.assertEqual(qs.count(), 1)
@@ -110,14 +121,31 @@
         # Should add token to outstanding list if not already present
         new_token = RefreshToken()
         blacklisted_token = new_token.blacklist()
         self.assertEqual(blacklisted_token.token.jti, new_token["jti"])
 
         self.assertEqual(OutstandingToken.objects.count(), 2)
 
+    def test_outstanding_token_and_blacklisted_token_expected_str(self):
+        outstanding = OutstandingToken.objects.create(
+            user=self.user,
+            jti="abc",
+            token="xyz",
+            expires_at=timezone.now(),
+        )
+        blacklisted = BlacklistedToken.objects.create(token=outstanding)
+
+        expected_outstanding_str = "Token for {} ({})".format(
+            outstanding.user, outstanding.jti
+        )
+        expected_blacklisted_str = f"Blacklisted token for {blacklisted.token.user}"
+
+        self.assertEqual(str(outstanding), expected_outstanding_str)
+        self.assertEqual(str(blacklisted), expected_blacklisted_str)
+
 
 class TestTokenBlacklistFlushExpiredTokens(BaseTestCase):
     def setUp(self):
         self.user = User.objects.create(
             username="test_user",
             password="test_password",
         )
@@ -131,17 +159,15 @@
         # Blacklist fresh tokens
         not_expired_2.blacklist()
         not_expired_3.blacklist()
 
         # Make tokens with fake exp time that will expire soon
         fake_now = aware_utcnow() - api_settings.REFRESH_TOKEN_LIFETIME
 
-        with patch(
-            "rest_framework_simplejwt_mongoengine.tokens.aware_utcnow"
-        ) as fake_aware_utcnow:
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
             fake_aware_utcnow.return_value = fake_now
             expired_1 = RefreshToken.for_user(self.user)
             expired_2 = RefreshToken()
 
         # Blacklist expired tokens
         expired_1.blacklist()
         expired_2.blacklist()
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_tokens.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from datetime import datetime, timedelta
+from importlib import reload
 from unittest.mock import patch
 
-import pytest
 from django_mongoengine.mongo_auth.managers import get_user_document
 from jose import jwt
-from rest_framework_simplejwt.exceptions import TokenBackendError, TokenError
-from rest_framework_simplejwt.utils import aware_utcnow, datetime_to_epoch, make_utc
 
+from rest_framework_simplejwt_mongoengine.exceptions import TokenBackendError, TokenError
 from rest_framework_simplejwt_mongoengine.settings import api_settings
 from rest_framework_simplejwt_mongoengine.state import token_backend
 from rest_framework_simplejwt_mongoengine.tokens import AccessToken, RefreshToken, SlidingToken, Token, UntypedToken
-from rest_framework_simplejwt_mongoengine.utils import drf_simplejwt_version, microseconds_to_milliseconds
+from rest_framework_simplejwt_mongoengine.utils import aware_utcnow, datetime_to_epoch, make_utc, microseconds_to_milliseconds
 
 from .utils import BaseTestCase, override_api_settings
 
 User = get_user_document()
 
 
 class MyToken(Token):
@@ -22,14 +21,34 @@
     lifetime = timedelta(days=1)
 
 
 class TestToken(BaseTestCase):
     def setUp(self):
         self.token = MyToken()
 
+    @classmethod
+    def setUpTestData(cls):
+        cls.username = "test_user"
+        cls.user = User.create_user(
+            username=cls.username,
+            password="test_password",
+        )
+
+    def test_type_checking(self):
+        from rest_framework_simplejwt_mongoengine import tokens
+
+        with patch("typing.TYPE_CHECKING", True):
+            # Reload tokens, mock type checking
+            reload(tokens)
+
+            self.assertEqual(tokens.TYPE_CHECKING, True)
+
+        # Restore origin module without mock
+        reload(tokens)
+
     def test_init_no_token_type_or_lifetime(self):
         class MyTestToken(Token):
             pass
 
         with self.assertRaises(TokenError):
             MyTestToken()
 
@@ -173,16 +192,16 @@
         # Should encode the given token
         encoded_token = str(token)
 
         # Token could be one of two depending on header dict ordering
         self.assertIn(
             encoded_token,
             (
-                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMH0.VKoOnMgmETawjDZwxrQaHG0xHdo6xBodFy6FXJzTVxs",  # noqa: E501
-                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMH0.iqxxOHV63sjeqNR1GDxX3LPvMymfVB76sOIDqTbjAgk",  # noqa: E501
+                "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjk0NjY4NDgwMH0.VKoOnMgmETawjDZwxrQaHG0xHdo6xBodFy6FXJzTVxs",
+                "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjk0NjY4NDgwMH0.iqxxOHV63sjeqNR1GDxX3LPvMymfVB76sOIDqTbjAgk",
             ),
         )
 
     def test_repr(self):
         self.assertEqual(repr(self.token), repr(self.token.payload))
 
     def test_getitem(self):
@@ -216,22 +235,22 @@
         old_jti = token["jti"]
 
         token.set_jti()
 
         self.assertIn("jti", token)
         self.assertNotEqual(old_jti, token["jti"])
 
+    @override_api_settings(JTI_CLAIM=None)
     def test_optional_jti(self):
-        with override_api_settings(JTI_CLAIM=None):
-            token = MyToken()
+        token = MyToken()
         self.assertNotIn("jti", token)
 
+    @override_api_settings(TOKEN_TYPE_CLAIM=None)
     def test_optional_type_token(self):
-        with override_api_settings(TOKEN_TYPE_CLAIM=None):
-            token = MyToken()
+        token = MyToken()
         self.assertNotIn("type", token)
 
     def test_set_exp(self):
         now = make_utc(datetime(year=2000, month=1, day=1))
 
         token = MyToken()
         token.current_time = now
@@ -240,30 +259,34 @@
         # and the TOKEN_LIFETIME setting
         token.set_exp()
         self.assertEqual(token["exp"], datetime_to_epoch(now + MyToken.lifetime))
 
         # Should allow overriding of beginning time, lifetime, and claim name
         token.set_exp(claim="refresh_exp", from_time=now, lifetime=timedelta(days=1))
         self.assertIn("refresh_exp", token)
-        self.assertEqual(token["refresh_exp"], datetime_to_epoch(now + timedelta(days=1)))
+        self.assertEqual(
+            token["refresh_exp"], datetime_to_epoch(now + timedelta(days=1))
+        )
 
     def test_set_iat(self):
         now = make_utc(datetime(year=2000, month=1, day=1))
 
         token = MyToken()
         token.current_time = now
 
         # By default, should add 'iat' claim to token using `self.current_time`
         token.set_iat()
         self.assertEqual(token["iat"], datetime_to_epoch(now))
 
         # Should allow overriding of time and claim name
         token.set_iat(claim="refresh_iat", at_time=now + timedelta(days=1))
         self.assertIn("refresh_iat", token)
-        self.assertEqual(token["refresh_iat"], datetime_to_epoch(now + timedelta(days=1)))
+        self.assertEqual(
+            token["refresh_iat"], datetime_to_epoch(now + timedelta(days=1))
+        )
 
     def test_check_exp(self):
         token = MyToken()
 
         # Should raise an exception if no claim of given kind
         with self.assertRaises(TokenError):
             token.check_exp("non_existent_claim")
@@ -298,22 +321,22 @@
         token.set_exp("refresh_exp", lifetime=timedelta(days=1))
 
         # Default timestamp
         token.check_exp("refresh_exp")
 
         # Given claim and timestamp
         with self.assertRaises(TokenError):
-            token.check_exp("refresh_exp", current_time=current_time + timedelta(days=1))
-        with self.assertRaises(TokenError):
-            token.check_exp("refresh_exp", current_time=current_time + timedelta(days=2))
+            token.check_exp(
+                "refresh_exp", current_time=current_time + timedelta(days=1)
+            )
+        with self.assertRaises(TokenError):
+            token.check_exp(
+                "refresh_exp", current_time=current_time + timedelta(days=2)
+            )
 
-    @pytest.mark.skipif(
-        "4.7" in drf_simplejwt_version,
-        reason="Django simplejwt version 4.7.x doesn't have LEEWAY property in token backend",
-    )
     def test_check_token_not_expired_if_in_leeway(self):
         token = MyToken()
         token.set_exp("refresh_exp", lifetime=timedelta(days=1))
 
         datetime_in_leeway = token.current_time + timedelta(days=1)
 
         with self.assertRaises(TokenError):
@@ -330,64 +353,61 @@
 
         # integer (seconds)
         token.token_backend.leeway = 10
         token.check_exp("refresh_exp", current_time=datetime_in_leeway)
 
         token.token_backend.leeway = 0
 
-    @pytest.mark.skipif(
-        "4.7" in drf_simplejwt_version,
-        reason="Django simplejwt version 4.7.x doesn't have LEEWAY property in token backend",
-    )
     def test_check_token_if_wrong_type_leeway(self):
         token = MyToken()
         token.set_exp("refresh_exp", lifetime=timedelta(days=1))
 
         datetime_in_leeway = token.current_time + timedelta(days=1)
 
         token.token_backend.leeway = "1"
         with self.assertRaises(TokenBackendError):
             token.check_exp("refresh_exp", current_time=datetime_in_leeway)
         token.token_backend.leeway = 0
 
     def test_for_user(self):
-        username = "test_user"
-        user = User.create_user(
-            username=username,
-            password="test_password",
-        )
+        token = MyToken.for_user(self.user)
 
-        token = MyToken.for_user(user)
-
-        user_id = getattr(user, api_settings.USER_ID_FIELD)
+        user_id = getattr(self.user, api_settings.USER_ID_FIELD)
         if not isinstance(user_id, int):
             user_id = str(user_id)
 
         self.assertEqual(token[api_settings.USER_ID_CLAIM], user_id)
 
+    @override_api_settings(USER_ID_FIELD="username")
+    def test_for_user_with_username(self):
         # Test with non-int user id
-        with override_api_settings(USER_ID_FIELD="username"):
-            token = MyToken.for_user(user)
+        token = MyToken.for_user(self.user)
+        self.assertEqual(token[api_settings.USER_ID_CLAIM], self.username)
 
-        self.assertEqual(token[api_settings.USER_ID_CLAIM], username)
+    @override_api_settings(CHECK_REVOKE_TOKEN=True)
+    def test_revoke_token_claim_included_in_authorization_token(self):
+        token = MyToken.for_user(self.user)
+        self.assertIn(api_settings.REVOKE_TOKEN_CLAIM, token)
 
     def test_get_token_backend(self):
         token = MyToken()
 
         self.assertEqual(token.get_token_backend(), token_backend)
 
 
 class TestSlidingToken(BaseTestCase):
     def test_init(self):
         # Should set sliding refresh claim and token type claim
         token = SlidingToken()
 
         self.assertEqual(
             token[api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM],
-            datetime_to_epoch(token.current_time + api_settings.SLIDING_TOKEN_REFRESH_LIFETIME),
+            datetime_to_epoch(
+                token.current_time + api_settings.SLIDING_TOKEN_REFRESH_LIFETIME
+            ),
         )
         self.assertEqual(token[api_settings.TOKEN_TYPE_CLAIM], "sliding")
 
 
 class TestAccessToken(BaseTestCase):
     def test_init(self):
         # Should set token type claim
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_utils.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,87 @@
-from datetime import datetime, timedelta
-from unittest.mock import patch
+from datetime import datetime, timedelta, timezone
 
 from django.test import TestCase
-from django.utils import timezone
+from freezegun import freeze_time
 
-from rest_framework_simplejwt.utils import (
-    aware_utcnow, datetime_from_epoch, datetime_to_epoch, format_lazy,
-    make_utc,
-)
+from rest_framework_simplejwt_mongoengine.utils import aware_utcnow, datetime_from_epoch, datetime_to_epoch, format_lazy, make_utc
 
 
 class TestMakeUtc(TestCase):
     def test_it_should_return_the_correct_values(self):
         # It should make a naive datetime into an aware, utc datetime if django
         # is configured to use timezones and the datetime doesn't already have
         # a timezone
 
         # Naive datetime
         dt = datetime(year=1970, month=12, day=1)
 
         with self.settings(USE_TZ=False):
             dt = make_utc(dt)
-            self.assertTrue(timezone.is_naive(dt))
+            self.assertTrue(dt.tzinfo is None)
 
         with self.settings(USE_TZ=True):
             dt = make_utc(dt)
-            self.assertTrue(timezone.is_aware(dt))
+            self.assertTrue(dt.tzinfo is not None)
             self.assertEqual(dt.utcoffset(), timedelta(seconds=0))
 
 
 class TestAwareUtcnow(TestCase):
     def test_it_should_return_the_correct_value(self):
-        now = datetime.utcnow()
-
-        with patch('rest_framework_simplejwt.utils.datetime') as fake_datetime:
-            fake_datetime.utcnow.return_value = now
+        now = datetime.now(tz=timezone.utc).replace(tzinfo=None)
 
+        with freeze_time(now):
             # Should return aware utcnow if USE_TZ == True
             with self.settings(USE_TZ=True):
-                self.assertEqual(timezone.make_aware(now, timezone=timezone.utc), aware_utcnow())
+                self.assertEqual(now.replace(tzinfo=timezone.utc), aware_utcnow())
 
             # Should return naive utcnow if USE_TZ == False
             with self.settings(USE_TZ=False):
                 self.assertEqual(now, aware_utcnow())
 
 
 class TestDatetimeToEpoch(TestCase):
     def test_it_should_return_the_correct_values(self):
         self.assertEqual(datetime_to_epoch(datetime(year=1970, month=1, day=1)), 0)
-        self.assertEqual(datetime_to_epoch(datetime(year=1970, month=1, day=1, second=1)), 1)
-        self.assertEqual(datetime_to_epoch(datetime(year=2000, month=1, day=1)), 946684800)
+        self.assertEqual(
+            datetime_to_epoch(datetime(year=1970, month=1, day=1, second=1)), 1
+        )
+        self.assertEqual(
+            datetime_to_epoch(datetime(year=2000, month=1, day=1)), 946684800
+        )
 
 
 class TestDatetimeFromEpoch(TestCase):
     def test_it_should_return_the_correct_values(self):
         with self.settings(USE_TZ=False):
-            self.assertEqual(datetime_from_epoch(0), datetime(year=1970, month=1, day=1))
-            self.assertEqual(datetime_from_epoch(1), datetime(year=1970, month=1, day=1, second=1))
-            self.assertEqual(datetime_from_epoch(946684800), datetime(year=2000, month=1, day=1), 946684800)
+            self.assertEqual(
+                datetime_from_epoch(0), datetime(year=1970, month=1, day=1)
+            )
+            self.assertEqual(
+                datetime_from_epoch(1), datetime(year=1970, month=1, day=1, second=1)
+            )
+            self.assertEqual(
+                datetime_from_epoch(946684800),
+                datetime(year=2000, month=1, day=1),
+                946684800,
+            )
 
         with self.settings(USE_TZ=True):
-            self.assertEqual(datetime_from_epoch(0), make_utc(datetime(year=1970, month=1, day=1)))
-            self.assertEqual(datetime_from_epoch(1), make_utc(datetime(year=1970, month=1, day=1, second=1)))
-            self.assertEqual(datetime_from_epoch(946684800), make_utc(datetime(year=2000, month=1, day=1)))
+            self.assertEqual(
+                datetime_from_epoch(0), make_utc(datetime(year=1970, month=1, day=1))
+            )
+            self.assertEqual(
+                datetime_from_epoch(1),
+                make_utc(datetime(year=1970, month=1, day=1, second=1)),
+            )
+            self.assertEqual(
+                datetime_from_epoch(946684800),
+                make_utc(datetime(year=2000, month=1, day=1)),
+            )
 
 
 class TestFormatLazy(TestCase):
     def test_it_should_work(self):
-        obj = format_lazy('{} {}', 'arst', 'zxcv')
+        obj = format_lazy("{} {}", "arst", "zxcv")
 
         self.assertNotIsInstance(obj, str)
-        self.assertEqual(str(obj), 'arst zxcv')
+        self.assertEqual(str(obj), "arst zxcv")
```

### Comparing `djangorestframework_simplejwt_mongoengine-1.2.1/tests/test_views.py` & `djangorestframework_simplejwt_mongoengine-1.3.0/tests/test_views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from datetime import timedelta
-from importlib import reload
 from unittest.mock import patch
 
 from django.utils import timezone
 from django_mongoengine.mongo_auth.managers import get_user_document
 from rest_framework.test import APIRequestFactory
-from rest_framework_simplejwt.utils import aware_utcnow, datetime_from_epoch, datetime_to_epoch
 
 from rest_framework_simplejwt_mongoengine import serializers
 from rest_framework_simplejwt_mongoengine.settings import api_settings
 from rest_framework_simplejwt_mongoengine.tokens import AccessToken, RefreshToken, SlidingToken
-from rest_framework_simplejwt_mongoengine.utils import drf_simplejwt_version
+from rest_framework_simplejwt_mongoengine.utils import aware_utcnow, datetime_from_epoch, datetime_to_epoch
 from rest_framework_simplejwt_mongoengine.views import TokenViewBase
 
 from .utils import APIViewTestCase, override_api_settings
 
 User = get_user_document()
 
 
 class TestTokenObtainPairView(APIViewTestCase):
     view_name = "token_obtain_pair"
 
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_fields_missing(self):
         res = self.view_post(data={})
         self.assertEqual(res.status_code, 400)
         self.assertIn(User.USERNAME_FIELD, res.data)
         self.assertIn("password", res.data)
 
@@ -38,51 +39,84 @@
         self.assertIn("password", res.data)
 
         res = self.view_post(data={"password": self.password})
         self.assertEqual(res.status_code, 400)
         self.assertIn(User.USERNAME_FIELD, res.data)
 
     def test_credentials_wrong(self):
-        res = self.view_post(data={User.USERNAME_FIELD: self.username, "password": "test_user"})
+        res = self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": "test_user",
+            }
+        )
         self.assertEqual(res.status_code, 401)
         self.assertIn("detail", res.data)
 
     def test_user_inactive(self):
         self.user.is_active = False
         self.user.save()
 
-        res = self.view_post(data={User.USERNAME_FIELD: self.username, "password": self.password})
+        res = self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
         self.assertEqual(res.status_code, 401)
         self.assertIn("detail", res.data)
 
     def test_success(self):
-        res = self.view_post(data={User.USERNAME_FIELD: self.username, "password": self.password})
+        res = self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
         self.assertEqual(res.status_code, 200)
         self.assertIn("access", res.data)
         self.assertIn("refresh", res.data)
 
     def test_update_last_login(self):
-        with override_api_settings(UPDATE_LAST_LOGIN=True):
-            reload(serializers)
-            self.view_post(data={User.USERNAME_FIELD: self.username, "password": self.password})
-            user = User.objects.get(username=self.username)
-            self.assertIsNotNone(user.last_login)
-            self.assertGreaterEqual(timezone.now(), user.last_login)
+        self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
+
+        # verify last_login is not updated
+        user = User.objects.get(username=self.username)
+        self.assertGreaterEqual(timezone.now(), user.last_login)
 
-        reload(serializers)
+    @override_api_settings(UPDATE_LAST_LOGIN=True)
+    def test_update_last_login_updated(self):
+        # verify last_login is updated
+        self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
+        user = User.objects.get(username=self.username)
+        self.assertIsNotNone(user.last_login)
+        self.assertGreaterEqual(timezone.now(), user.last_login)
 
 
 class TestTokenRefreshView(APIViewTestCase):
     view_name = "token_refresh"
 
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_fields_missing(self):
         res = self.view_post(data={})
         self.assertEqual(res.status_code, 400)
         self.assertIn("refresh", res.data)
 
     def test_it_should_return_401_if_token_invalid(self):
@@ -112,25 +146,30 @@
             res = self.view_post(data={"refresh": str(refresh)})
 
         self.assertEqual(res.status_code, 200)
 
         access = AccessToken(res.data["access"])
 
         self.assertEqual(refresh["test_claim"], access["test_claim"])
-        self.assertEqual(access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME))
+        self.assertEqual(
+            access["exp"], datetime_to_epoch(now + api_settings.ACCESS_TOKEN_LIFETIME)
+        )
 
 
 class TestTokenObtainSlidingView(APIViewTestCase):
     view_name = "token_obtain_sliding"
 
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_fields_missing(self):
         res = self.view_post(data={})
         self.assertEqual(res.status_code, 400)
         self.assertIn(User.USERNAME_FIELD, res.data)
         self.assertIn("password", res.data)
 
@@ -139,51 +178,83 @@
         self.assertIn("password", res.data)
 
         res = self.view_post(data={"password": self.password})
         self.assertEqual(res.status_code, 400)
         self.assertIn(User.USERNAME_FIELD, res.data)
 
     def test_credentials_wrong(self):
-        res = self.view_post(data={User.USERNAME_FIELD: self.username, "password": "test_user"})
+        res = self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": "test_user",
+            }
+        )
         self.assertEqual(res.status_code, 401)
         self.assertIn("detail", res.data)
 
     def test_user_inactive(self):
         self.user.is_active = False
         self.user.save()
 
-        res = self.view_post(data={User.USERNAME_FIELD: self.username, "password": self.password})
+        res = self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
         self.assertEqual(res.status_code, 401)
         self.assertIn("detail", res.data)
 
     def test_success(self):
-        res = self.view_post(data={User.USERNAME_FIELD: self.username, "password": self.password})
+        res = self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
         self.assertEqual(res.status_code, 200)
         self.assertIn("token", res.data)
 
     def test_update_last_login(self):
-        # verify last_login is updated
-        with override_api_settings(UPDATE_LAST_LOGIN=True):
-            reload(serializers)
-            self.view_post(data={User.USERNAME_FIELD: self.username, "password": self.password})
-            user = User.objects.get(username=self.username)
-            self.assertIsNotNone(user.last_login)
-            self.assertGreaterEqual(timezone.now(), user.last_login)
+        self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
+
+        # verify last_login is not updated
+        user = User.objects.get(username=self.username)
+        self.assertGreaterEqual(timezone.now(), user.last_login)
 
-        reload(serializers)
+    @override_api_settings(UPDATE_LAST_LOGIN=True)
+    def test_update_last_login_updated(self):
+        # verify last_login is updated
+        self.view_post(
+            data={
+                User.USERNAME_FIELD: self.username,
+                "password": self.password,
+            }
+        )
+        user = User.objects.get(username=self.username)
+        self.assertIsNotNone(user.last_login)
+        self.assertGreaterEqual(timezone.now(), user.last_login)
 
 
 class TestTokenRefreshSlidingView(APIViewTestCase):
     view_name = "token_refresh_sliding"
 
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_fields_missing(self):
         res = self.view_post(data={})
         self.assertEqual(res.status_code, 400)
         self.assertIn("token", res.data)
 
     def test_it_should_return_401_if_token_invalid(self):
@@ -206,26 +277,31 @@
 
         res = self.view_post(data={"token": str(token)})
         self.assertEqual(res.status_code, 401)
         self.assertEqual(res.data["code"], "token_not_valid")
 
     def test_it_should_return_401_if_token_has_refresh_period_expired(self):
         token = SlidingToken()
-        token.set_exp(api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM, lifetime=-timedelta(seconds=1))
+        token.set_exp(
+            api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM, lifetime=-timedelta(seconds=1)
+        )
 
         res = self.view_post(data={"token": str(token)})
         self.assertEqual(res.status_code, 401)
         self.assertEqual(res.data["code"], "token_not_valid")
 
     def test_it_should_update_token_exp_claim_if_everything_ok(self):
         now = aware_utcnow()
 
         token = SlidingToken()
         exp = now + api_settings.SLIDING_TOKEN_LIFETIME - timedelta(seconds=1)
-        token.set_exp(from_time=now, lifetime=api_settings.SLIDING_TOKEN_LIFETIME - timedelta(seconds=1))
+        token.set_exp(
+            from_time=now,
+            lifetime=api_settings.SLIDING_TOKEN_LIFETIME - timedelta(seconds=1),
+        )
 
         # View returns 200
         res = self.view_post(data={"token": str(token)})
         self.assertEqual(res.status_code, 200)
 
         # Expiration claim has moved into future
         new_token = SlidingToken(res.data["token"])
@@ -237,15 +313,18 @@
 class TestTokenVerifyView(APIViewTestCase):
     view_name = "token_verify"
 
     def setUp(self):
         self.username = "test_user"
         self.password = "test_password"
 
-        self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
     def test_fields_missing(self):
         res = self.view_post(data={})
         self.assertEqual(res.status_code, 400)
         self.assertIn("token", res.data)
 
     def test_it_should_return_401_if_token_invalid(self):
@@ -274,85 +353,99 @@
         token[api_settings.TOKEN_TYPE_CLAIM] = "fake_type"
 
         res = self.view_post(data={"token": str(token)})
         self.assertEqual(res.status_code, 200)
         self.assertEqual(len(res.data), 0)
 
 
-if drf_simplejwt_version in ["5.0.0", "5.1.0", "5.2.0", "5.2.1", "5.2.2"]:
+class TestTokenBlacklistView(APIViewTestCase):
+    view_name = "token_blacklist"
 
-    class TestTokenBlacklistView(APIViewTestCase):
-        view_name = "token_blacklist"
-
-        def setUp(self):
-            self.username = "test_user"
-            self.password = "test_password"
+    def setUp(self):
+        self.username = "test_user"
+        self.password = "test_password"
 
-            self.user = User.create_user(username=self.username, password=self.password)
+        self.user = User.create_user(
+            username=self.username,
+            password=self.password,
+        )
 
-        def test_fields_missing(self):
-            res = self.view_post(data={})
-            self.assertEqual(res.status_code, 400)
-            self.assertIn("refresh", res.data)
+    def test_fields_missing(self):
+        res = self.view_post(data={})
+        self.assertEqual(res.status_code, 400)
+        self.assertIn("refresh", res.data)
 
-        def test_it_should_return_401_if_token_invalid(self):
-            token = RefreshToken()
-            del token["exp"]
+    def test_it_should_return_401_if_token_invalid(self):
+        token = RefreshToken()
+        del token["exp"]
 
-            res = self.view_post(data={"refresh": str(token)})
-            self.assertEqual(res.status_code, 401)
-            self.assertEqual(res.data["code"], "token_not_valid")
+        res = self.view_post(data={"refresh": str(token)})
+        self.assertEqual(res.status_code, 401)
+        self.assertEqual(res.data["code"], "token_not_valid")
 
-            token.set_exp(lifetime=-timedelta(seconds=1))
+        token.set_exp(lifetime=-timedelta(seconds=1))
 
-            res = self.view_post(data={"refresh": str(token)})
-            self.assertEqual(res.status_code, 401)
-            self.assertEqual(res.data["code"], "token_not_valid")
+        res = self.view_post(data={"refresh": str(token)})
+        self.assertEqual(res.status_code, 401)
+        self.assertEqual(res.data["code"], "token_not_valid")
 
-        def test_it_should_return_if_everything_ok(self):
-            refresh = RefreshToken()
-            refresh["test_claim"] = "arst"
+    def test_it_should_return_if_everything_ok(self):
+        refresh = RefreshToken()
+        refresh["test_claim"] = "arst"
 
-            # View returns 200
-            now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
+        # View returns 200
+        now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
 
-            with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
-                fake_aware_utcnow.return_value = now
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
+            fake_aware_utcnow.return_value = now
 
-                res = self.view_post(data={"refresh": str(refresh)})
+            res = self.view_post(data={"refresh": str(refresh)})
 
-            self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.status_code, 200)
 
-            self.assertDictEqual(res.data, {})
+        self.assertDictEqual(res.data, {})
 
-        def test_it_should_return_401_if_token_is_blacklisted(self):
-            refresh = RefreshToken()
-            refresh["test_claim"] = "arst"
+    def test_it_should_return_401_if_token_is_blacklisted(self):
+        refresh = RefreshToken()
+        refresh["test_claim"] = "arst"
 
-            # View returns 200
-            now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
+        # View returns 200
+        now = aware_utcnow() - api_settings.ACCESS_TOKEN_LIFETIME / 2
 
-            with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
-                fake_aware_utcnow.return_value = now
+        with patch("rest_framework_simplejwt_mongoengine.tokens.aware_utcnow") as fake_aware_utcnow:
+            fake_aware_utcnow.return_value = now
 
-                res = self.view_post(data={"refresh": str(refresh)})
+            res = self.view_post(data={"refresh": str(refresh)})
 
-            self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.status_code, 200)
 
-            self.view_name = "token_refresh"
-            res = self.view_post(data={"refresh": str(refresh)})
-            # make sure other tests are not affected
-            del self.view_name
+        self.view_name = "token_refresh"
+        res = self.view_post(data={"refresh": str(refresh)})
+        # make sure other tests are not affected
+        del self.view_name
 
-            self.assertEqual(res.status_code, 401)
+        self.assertEqual(res.status_code, 401)
 
 
 class TestCustomTokenView(APIViewTestCase):
     def test_custom_view_class(self):
         class CustomTokenView(TokenViewBase):
             serializer_class = serializers.TokenObtainPairSerializer
 
         factory = APIRequestFactory()
         view = CustomTokenView.as_view()
         request = factory.post("/", {}, format="json")
         res = view(request)
         self.assertEqual(res.status_code, 400)
+
+
+class TestTokenViewBase(APIViewTestCase):
+    def test_serializer_class_not_set_in_settings_and_class_attribute_or_wrong_path(
+        self,
+    ):
+        view = TokenViewBase()
+        msg = "Could not import serializer '%s'" % view._serializer_class
+
+        with self.assertRaises(ImportError) as e:
+            view.get_serializer_class()
+
+            self.assertEqual(e.exception.msg, msg)
```

