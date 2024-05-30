# Comparing `tmp/django_simple_history-3.6.0.tar.gz` & `tmp/django_simple_history-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_history-3.6.0.tar", last modified: Sun May 26 23:26:53 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django_simple_history-3.6.0.tar` & `django_simple_history-3.7.0.tar`

### file list

```diff
@@ -1,192 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.289086 django_simple_history-3.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.289086 django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.289086 django_simple_history-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/django_simple_history.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/doc-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.293086 django_simple_history-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.293086 django_simple_history-3.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/common_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19603 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/historical_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/history_diffing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/multiple_dbs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/querying_history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/quick_start.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.293086 django_simple_history-3.6.0/docs/screens/
--rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/10_revert_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)    19753 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/1_poll_history.png
--rw-r--r--   0 runner    (1001) docker     (127)    17844 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/2_revert.png
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/3_poll_reverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    21966 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/4_history_after_poll_reverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/5_history_list_display.png
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/user_tracking.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/coverage.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/tox.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     5529 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/clean_duplicate_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/clean_old_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/populate_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    44885 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/registry_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.305086 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.285086 django_simple_history-3.6.0/simple_history/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.305086 django_simple_history-3.6.0/simple_history/templates/simple_history/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/object_history.html
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/submit_line.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.305086 django_simple_history-3.6.0/simple_history/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/getattributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/simple_history_admin_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/simple_history_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/custom_user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/custom_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/custom_user/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/custom_user/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/external/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/generated_file_checks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/generated_file_checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/generated_file_checks/check_translations.py
--rw-r--r--   0 runner    (1001) docker     (127)    26580 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/other_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/simple_history/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    23446 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)   107885 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_template_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (127)    23823 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/tox.ini
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.codeclimate.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.coveragerc
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.editorconfig
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.yamllint
+-rw-r--r--   0        0        0    20586 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/CHANGES.rst
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/Makefile
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/README.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/codecov.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/doc-requirements.txt
+-rwxr-xr-x   0        0        0     5363 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/runtests.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/tox.ini
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.github/release.yml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/Makefile
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/admin.rst
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/common_issues.rst
+-rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/conf.py
+-rw-r--r--   0        0        0    19603 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/historical_model.rst
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/history_diffing.rst
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/index.rst
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/make.bat
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/multiple_dbs.rst
+-rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/querying_history.rst
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/quick_start.rst
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/signals.rst
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/user_tracking.rst
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/utils.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/_static/.keep
+-rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/screens/10_revert_disabled.png
+-rw-r--r--   0        0        0    19753 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/screens/1_poll_history.png
+-rw-r--r--   0        0        0    17844 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/screens/2_revert.png
+-rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/screens/3_poll_reverted.png
+-rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/screens/4_history_after_poll_reverted.png
+-rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/docs/screens/5_history_list_display.png
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/coverage.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/docs.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/lint.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/mysql.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/postgres.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/test.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/requirements/tox.txt
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/__init__.py
+-rw-r--r--   0        0        0    15067 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/admin.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/exceptions.py
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/manager.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/middleware.py
+-rw-r--r--   0        0        0    44885 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/models.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/signals.py
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/template_utils.py
+-rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/utils.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/ur/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/ur/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/management/commands/__init__.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/management/commands/clean_duplicate_history.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/management/commands/clean_old_history.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/management/commands/populate_history.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/models.py
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/__init__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/models.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templates/simple_history/object_history.html
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templates/simple_history/object_history_form.html
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templates/simple_history/object_history_list.html
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templates/simple_history/submit_line.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templatetags/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templatetags/getattributes.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templatetags/simple_history_admin_list.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/templatetags/simple_history_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/__init__.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/admin.py
+-rw-r--r--   0        0        0    26580 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/models.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/other_admin.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/urls.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/custom_user/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/custom_user/admin.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/custom_user/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/external/__init__.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/external/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/generated_file_checks/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/generated_file_checks/check_translations.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/__init__.py
+-rw-r--r--   0        0        0    44614 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_admin.py
+-rw-r--r--   0        0        0    23446 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_commands.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_deprecation.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_index.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_manager.py
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_middleware.py
+-rw-r--r--   0        0        0   107885 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_models.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_signals.py
+-rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_template_utils.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_templatetags.py
+-rw-r--r--   0        0        0    23823 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/test_utils.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/simple_history/tests/tests/utils.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/.gitignore
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 django_simple_history-3.7.0/PKG-INFO
```

### Comparing `django_simple_history-3.6.0/.codeclimate.yml` & `django_simple_history-3.7.0/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `django_simple_history-3.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `django_simple_history-3.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/.github/workflows/release.yml` & `django_simple_history-3.7.0/.github/workflows/release.yml`

 * *Files 23% similar despite different names*

```diff
@@ -20,22 +20,21 @@
         uses: actions/setup-python@v5
         with:
           python-version: 3.x
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U setuptools twine wheel
+          python -m pip install -U build twine
 
       - name: Build package
         run: |
-          python setup.py --version
-          python setup.py sdist --format=gztar bdist_wheel
+          python -m build
           twine check dist/*
 
       - name: Upload packages to Jazzband
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: jazzband
           password: ${{ secrets.JAZZBAND_RELEASE_KEY }}
-          repository_url: https://jazzband.co/projects/django-simple-history/upload
+          repository-url: https://jazzband.co/projects/django-simple-history/upload
```

### Comparing `django_simple_history-3.6.0/.github/workflows/test.yml` & `django_simple_history-3.7.0/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,27 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12', '3.13-dev']
-        django-version: ['3.2', '4.2', '5.0', 'main']
+        django-version: ['4.2', '5.0', 'main']
 
         exclude:
           # Exclude py3.8 and py3.9 for Django main and 5.0
           - python-version: '3.8'
             django-version: '5.0'
           - python-version: '3.9'
             django-version: '5.0'
           - python-version: '3.8'
             django-version: 'main'
           - python-version: '3.9'
             django-version: 'main'
 
-          # Exclude py3.11, py3.12 and py3.13 for Django 3.2
-          - python-version: '3.11'
-            django-version: '3.2'
-          - python-version: '3.12'
-            django-version: '3.2'
-          - python-version: '3.13-dev'
-            django-version: '3.2'
-
     services:
 
       postgres:
         image: postgres:latest
         env:
           POSTGRES_USER: postgres
           POSTGRES_PASSWORD: postgres
@@ -69,15 +61,15 @@
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
           cache-dependency-path: |
-            setup.py
+            pyproject.toml
             tox.ini
             requirements/*.txt
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements/tox.txt
```

### Comparing `django_simple_history-3.6.0/.pre-commit-config.yaml` & `django_simple_history-3.7.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -31,17 +31,27 @@
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
+      - id: check-toml
       - id: debug-statements
       - id: detect-private-key
 
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: 2.1.3
+    hooks:
+      - id: pyproject-fmt
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.18
+    hooks:
+      - id: validate-pyproject
+
   - repo: https://github.com/adrienverge/yamllint
     rev: v1.35.1
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `django_simple_history-3.6.0/.readthedocs.yaml` & `django_simple_history-3.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/AUTHORS.rst` & `django_simple_history-3.7.0/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 - Miguel Vargas
 - Mike Spainhower
 - Muneeb Shahid (`muneeb706 <https://github.com/muneeb706>`_)
 - Nathan Villagaray-Carski (`ncvc <https://github.com/ncvc>`_)
 - Nianpeng Li
 - Nick Träger
 - Noel James (`NoelJames <https://github.com/NoelJames>`_)
+- Ofek Lev (`ofek <https://github.com/ofek>`_)
 - Phillip Marshall
 - Prakash Venkatraman (`dopatraman <https://github.com/dopatraman>`_)
 - Rajesh Pappula
 - Ray Logel
 - Raynald de Lahondes
 - Renaud Perrin (`leminaw <https://github.com/leminaw>`_)
 - Roberto Aguilar
```

### Comparing `django_simple_history-3.6.0/CHANGES.rst` & `django_simple_history-3.7.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 Changes
 =======
 
 Unreleased
 ----------
 
 
+3.7.0 (2024-05-29)
+------------------
+
+- Dropped support for Django 3.2, which reached end-of-life on 2024-04-01 (gh-1344)
+- Removed the temporary requirement on ``asgiref>=3.6`` added in 3.5.0,
+  now that the minimum required Django version is 4.2 (gh-1344)
+- Migrated package building from using the deprecated ``setup.py`` to using
+  ``pyproject.toml`` (with Hatchling as build backend);
+  ``setup.py`` has consequently been removed (gh-1348)
+- Added ``django>=4.2`` as an installation dependency, to mirror the minimum version
+  tested in our CI (gh-1349)
+
 3.6.0 (2024-05-26)
 ------------------
 
 - Support custom History ``Manager`` and ``QuerySet`` classes (gh-1280)
 - Renamed the (previously internal) admin template
   ``simple_history/_object_history_list.html`` to
   ``simple_history/object_history_list.html``, and added the field
```

### Comparing `django_simple_history-3.6.0/CODE_OF_CONDUCT.md` & `django_simple_history-3.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/CONTRIBUTING.rst` & `django_simple_history-3.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/LICENSE.txt` & `django_simple_history-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/Makefile` & `django_simple_history-3.7.0/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 all: init docs clean test
 
 clean: clean-build clean-pyc
 	rm -fr htmlcov/
 
 clean-build:
-	rm -fr build/
 	rm -fr dist/
-	rm -fr *.egg-info
 
 clean-pyc:
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 
 init:
@@ -23,17 +21,16 @@
 
 docs: documentation
 
 documentation:
 	tox -e docs
 
 dist: clean
-	pip install -U wheel
-	python setup.py sdist
-	python setup.py bdist_wheel
+	pip install -U build
+	python -m build
 	for file in dist/* ; do gpg --detach-sign -a "$$file" ; done
 	ls -l dist
 
 test-release: dist
 	pip install -U twine
 	gpg --detach-sign -a dist/*
 	twine upload -r pypitest dist/*
```

### Comparing `django_simple_history-3.6.0/PKG-INFO` & `django_simple_history-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,113 +1,117 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.2
 Name: django-simple-history
-Version: 3.6.0
+Version: 3.7.0
 Summary: Store model history and view/revert changes from admin site.
-Home-page: https://github.com/jazzband/django-simple-history
-Author: Corey Bertram
-Author-email: corey@qr7.com
-Maintainer: Trey Hunner
-Project-URL: Documentation, https://django-simple-history.readthedocs.io/
 Project-URL: Changelog, https://github.com/jazzband/django-simple-history/blob/master/CHANGES.rst
+Project-URL: Documentation, https://django-simple-history.readthedocs.io/en/stable/
+Project-URL: Homepage, https://github.com/jazzband/django-simple-history
 Project-URL: Source, https://github.com/jazzband/django-simple-history
 Project-URL: Tracker, https://github.com/jazzband/django-simple-history/issues
+Author-email: Corey Bertram <corey@qr7.com>
+Maintainer: Trey Hunner
+License-File: AUTHORS.rst
+License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
 Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
+Requires-Dist: django>=4.2
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-Requires-Dist: asgiref>=3.6
 
-django-simple-history
-=====================
+|jazzband| |build-status| |docs| |coverage| |maintainability| |code-style| |downloads|
 
-.. image:: https://github.com/jazzband/django-simple-history/actions/workflows/test.yml/badge.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/django-simple-history.svg
+   :target: https://pypi.org/project/django-simple-history/
+   :alt: PyPI Version
+
+.. |jazzband| image:: https://jazzband.co/static/img/badge.svg
+   :target: https://jazzband.co/
+   :alt: Jazzband
+
+.. |build-status| image:: https://github.com/jazzband/django-simple-history/actions/workflows/test.yml/badge.svg
    :target: https://github.com/jazzband/django-simple-history/actions/workflows/test.yml
    :alt: Build Status
 
-.. image:: https://readthedocs.org/projects/django-simple-history/badge/?version=latest
+.. |docs| image:: https://readthedocs.org/projects/django-simple-history/badge/?version=latest
    :target: https://django-simple-history.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://img.shields.io/codecov/c/github/jazzband/django-simple-history/master.svg
+.. |coverage| image:: https://img.shields.io/codecov/c/github/jazzband/django-simple-history/master.svg
    :target: https://app.codecov.io/github/jazzband/django-simple-history?branch=master
    :alt: Test Coverage
 
-.. image:: https://img.shields.io/pypi/v/django-simple-history.svg
-   :target: https://pypi.org/project/django-simple-history/
-   :alt: PyPI Version
-
-.. image:: https://api.codeclimate.com/v1/badges/66cfd94e2db991f2d28a/maintainability
+.. |maintainability| image:: https://api.codeclimate.com/v1/badges/66cfd94e2db991f2d28a/maintainability
    :target: https://codeclimate.com/github/jazzband/django-simple-history/maintainability
    :alt: Maintainability
 
-.. image:: https://static.pepy.tech/badge/django-simple-history
-   :target: https://pepy.tech/project/django-simple-history
-   :alt: Downloads
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |code-style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code Style
 
-.. image:: https://jazzband.co/static/img/badge.svg
-   :target: https://jazzband.co/
-   :alt: Jazzband
+.. |downloads| image:: https://static.pepy.tech/badge/django-simple-history
+   :target: https://pepy.tech/project/django-simple-history
+   :alt: Downloads
 
 
-django-simple-history stores Django model state on every create/update/delete.
+``django-simple-history`` stores Django model state on every create/update/delete.
 
 This app supports the following combinations of Django and Python:
 
 ==========  ========================
   Django      Python
 ==========  ========================
-3.2         3.8, 3.9, 3.10
 4.2         3.8, 3.9, 3.10, 3.11, 3.12, 3.13-dev
 5.0         3.10, 3.11, 3.12, 3.13-dev
 main        3.10, 3.11, 3.12, 3.13-dev
 ==========  ========================
 
 Getting Help
 ------------
 
-Documentation is available at https://django-simple-history.readthedocs.io/
+Documentation is available at https://django-simple-history.readthedocs.io/en/stable/
 
-Pull requests are welcome.  Read the `CONTRIBUTING`_ file for tips on
+Pull requests are welcome. Read the `CONTRIBUTING`_ file for tips on
 submitting a pull request.
 
 .. _CONTRIBUTING: https://github.com/jazzband/django-simple-history/blob/master/CONTRIBUTING.rst
 
 License
 -------
 
 This project is licensed under the
 `BSD 3-Clause license <https://choosealicense.com/licenses/bsd-3-clause/>`_.
 
-Changes
-=======
+====
+
+Changelog
+=========
 
-Unreleased
-----------
+3.7.0 (2024-05-29)
+------------------
 
+- Dropped support for Django 3.2, which reached end-of-life on 2024-04-01 (gh-1344)
+- Removed the temporary requirement on ``asgiref>=3.6`` added in 3.5.0,
+  now that the minimum required Django version is 4.2 (gh-1344)
+- Migrated package building from using the deprecated ``setup.py`` to using
+  ``pyproject.toml`` (with Hatchling as build backend);
+  ``setup.py`` has consequently been removed (gh-1348)
+- Added ``django>=4.2`` as an installation dependency, to mirror the minimum version
+  tested in our CI (gh-1349)
 
 3.6.0 (2024-05-26)
 ------------------
 
 - Support custom History ``Manager`` and ``QuerySet`` classes (gh-1280)
 - Renamed the (previously internal) admin template
   ``simple_history/_object_history_list.html`` to
```

### Comparing `django_simple_history-3.6.0/PULL_REQUEST_TEMPLATE.md` & `django_simple_history-3.7.0/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/README.rst` & `django_simple_history-3.7.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -34,31 +34,43 @@
    :alt: Jazzband
 
 
 django-simple-history stores Django model state on every create/update/delete.
 
 This app supports the following combinations of Django and Python:
 
-==========  ========================
+==========  =======================
   Django      Python
-==========  ========================
-3.2         3.8, 3.9, 3.10
+==========  =======================
 4.2         3.8, 3.9, 3.10, 3.11, 3.12, 3.13-dev
 5.0         3.10, 3.11, 3.12, 3.13-dev
 main        3.10, 3.11, 3.12, 3.13-dev
-==========  ========================
+==========  =======================
 
-Getting Help
-------------
+Contribute
+----------
 
-Documentation is available at https://django-simple-history.readthedocs.io/
+- Issue Tracker: https://github.com/jazzband/django-simple-history/issues
+- Source Code: https://github.com/jazzband/django-simple-history
 
-Pull requests are welcome.  Read the `CONTRIBUTING`_ file for tips on
-submitting a pull request.
+Pull requests are welcome.
 
-.. _CONTRIBUTING: https://github.com/jazzband/django-simple-history/blob/master/CONTRIBUTING.rst
 
-License
--------
+Documentation
+-------------
 
-This project is licensed under the
-`BSD 3-Clause license <https://choosealicense.com/licenses/bsd-3-clause/>`_.
+.. toctree::
+   :maxdepth: 2
+
+   quick_start
+   querying_history
+   admin
+   historical_model
+   user_tracking
+   signals
+   history_diffing
+   multiple_dbs
+   utils
+   common_issues
+
+
+.. include:: ../CHANGES.rst
```

### Comparing `django_simple_history-3.6.0/docs/Makefile` & `django_simple_history-3.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/admin.rst` & `django_simple_history-3.7.0/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/common_issues.rst` & `django_simple_history-3.7.0/docs/common_issues.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/conf.py` & `django_simple_history-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/historical_model.rst` & `django_simple_history-3.7.0/docs/historical_model.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/history_diffing.rst` & `django_simple_history-3.7.0/docs/history_diffing.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/make.bat` & `django_simple_history-3.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/multiple_dbs.rst` & `django_simple_history-3.7.0/docs/multiple_dbs.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/querying_history.rst` & `django_simple_history-3.7.0/docs/querying_history.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/quick_start.rst` & `django_simple_history-3.7.0/docs/quick_start.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/screens/10_revert_disabled.png` & `django_simple_history-3.7.0/docs/screens/10_revert_disabled.png`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/screens/1_poll_history.png` & `django_simple_history-3.7.0/docs/screens/1_poll_history.png`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/screens/2_revert.png` & `django_simple_history-3.7.0/docs/screens/2_revert.png`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/screens/3_poll_reverted.png` & `django_simple_history-3.7.0/docs/screens/3_poll_reverted.png`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/screens/4_history_after_poll_reverted.png` & `django_simple_history-3.7.0/docs/screens/4_history_after_poll_reverted.png`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/screens/5_history_list_display.png` & `django_simple_history-3.7.0/docs/screens/5_history_list_display.png`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/signals.rst` & `django_simple_history-3.7.0/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/user_tracking.rst` & `django_simple_history-3.7.0/docs/user_tracking.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/docs/utils.rst` & `django_simple_history-3.7.0/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/runtests.py` & `django_simple_history-3.7.0/runtests.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,35 +131,31 @@
                     "django.template.context_processors.request",
                     "django.contrib.auth.context_processors.auth",
                     "django.contrib.messages.context_processors.messages",
                 ]
             },
         }
     ],
+    STORAGES={
+        "default": {
+            # Speeds up tests and prevents locally storing files created through them
+            "BACKEND": "django.core.files.storage.InMemoryStorage",
+        },
+    },
     DEFAULT_AUTO_FIELD="django.db.models.AutoField",
     USE_TZ=False,
 )
 MIDDLEWARE = [
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
 ]
 
 DEFAULT_SETTINGS["MIDDLEWARE"] = MIDDLEWARE
 
-# DEV: Merge these settings into DEFAULT_SETTINGS when the minimum required
-#      Django version is 4.2 or higher
-if django.VERSION >= (4, 2):
-    DEFAULT_SETTINGS["STORAGES"] = {
-        "default": {
-            # Speeds up tests and prevents locally storing files created through them
-            "BACKEND": "django.core.files.storage.InMemoryStorage",
-        },
-    }
-
 
 def get_default_settings(*, database_name=DEFAULT_DATABASE_NAME):
     return {
         **DEFAULT_SETTINGS,
         "DATABASES": DATABASE_NAME_TO_DATABASE_SETTINGS[database_name],
     }
```

### Comparing `django_simple_history-3.6.0/simple_history/__init__.py` & `django_simple_history-3.7.0/simple_history/__init__.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/admin.py` & `django_simple_history-3.7.0/simple_history/admin.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/ur/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/ur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_simple_history-3.7.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po` & `django_simple_history-3.7.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/management/commands/clean_duplicate_history.py` & `django_simple_history-3.7.0/simple_history/management/commands/clean_duplicate_history.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/management/commands/clean_old_history.py` & `django_simple_history-3.7.0/simple_history/management/commands/clean_old_history.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/management/commands/populate_history.py` & `django_simple_history-3.7.0/simple_history/management/commands/populate_history.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/manager.py` & `django_simple_history-3.7.0/simple_history/manager.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/middleware.py` & `django_simple_history-3.7.0/simple_history/middleware.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/models.py` & `django_simple_history-3.7.0/simple_history/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/models.py` & `django_simple_history-3.7.0/simple_history/registry_tests/migration_test_app/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/registry_tests/tests.py` & `django_simple_history-3.7.0/simple_history/registry_tests/tests.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/signals.py` & `django_simple_history-3.7.0/simple_history/signals.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/template_utils.py` & `django_simple_history-3.7.0/simple_history/template_utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/templates/simple_history/object_history.html` & `django_simple_history-3.7.0/simple_history/templates/simple_history/object_history.html`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_form.html` & `django_simple_history-3.7.0/simple_history/templates/simple_history/object_history_form.html`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_list.html` & `django_simple_history-3.7.0/simple_history/templates/simple_history/object_history_list.html`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/admin.py` & `django_simple_history-3.7.0/simple_history/tests/admin.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/external/models.py` & `django_simple_history-3.7.0/simple_history/tests/external/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/generated_file_checks/check_translations.py` & `django_simple_history-3.7.0/simple_history/tests/generated_file_checks/check_translations.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/models.py` & `django_simple_history-3.7.0/simple_history/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_admin.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timedelta
 from unittest.mock import ANY, patch
 
+import django
 from django.contrib.admin import AdminSite
 from django.contrib.admin.utils import quote
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Permission
 from django.contrib.messages.storage.fallback import FallbackStorage
 from django.test import TestCase
 from django.test.client import RequestFactory
@@ -617,14 +618,15 @@
 
         with patch("simple_history.admin.render") as mock_render:
             admin.history_form_view(request, poll.id, history.pk)
 
         context = {
             **admin_site.each_context(request),
             # Verify this is set for original object
+            "log_entries": ANY,
             "original": poll,
             "change_history": False,
             "title": "Revert %s" % force_str(poll),
             "adminform": ANY,
             "object_id": poll.id,
             "is_popup": False,
             "media": ANY,
@@ -646,17 +648,17 @@
             "form_url": "",
             "opts": ANY,
             "content_type_id": ANY,
             "save_as": admin.save_as,
             "save_on_top": admin.save_on_top,
             "root_path": getattr(admin_site, "root_path", None),
         }
-        # This key didn't exist prior to Django 4.2
-        if "log_entries" in context:
-            context["log_entries"] = ANY
+        # DEV: Remove this when support for Django 4.2 has been dropped
+        if django.VERSION < (5, 0):
+            del context["log_entries"]
 
         mock_render.assert_called_once_with(
             request, admin.object_history_form_template, context
         )
 
     def test_history_form_view_getting_history(self):
         request = RequestFactory().post("/")
@@ -676,14 +678,15 @@
         with patch("simple_history.admin.render") as mock_render:
             with patch("simple_history.admin.SIMPLE_HISTORY_EDIT", True):
                 admin.history_form_view(request, poll.id, history.pk)
 
         context = {
             **admin_site.each_context(request),
             # Verify this is set for history object not poll object
+            "log_entries": ANY,
             "original": history.instance,
             "change_history": True,
             "title": "Revert %s" % force_str(history.instance),
             "adminform": ANY,
             "object_id": poll.id,
             "is_popup": False,
             "media": ANY,
@@ -705,17 +708,17 @@
             "form_url": "",
             "opts": ANY,
             "content_type_id": ANY,
             "save_as": admin.save_as,
             "save_on_top": admin.save_on_top,
             "root_path": getattr(admin_site, "root_path", None),
         }
-        # This key didn't exist prior to Django 4.2
-        if "log_entries" in context:
-            context["log_entries"] = ANY
+        # DEV: Remove this when support for Django 4.2 has been dropped
+        if django.VERSION < (5, 0):
+            del context["log_entries"]
 
         mock_render.assert_called_once_with(
             request, admin.object_history_form_template, context
         )
 
     def test_history_form_view_getting_history_with_setting_off(self):
         request = RequestFactory().post("/")
@@ -735,14 +738,15 @@
         with patch("simple_history.admin.render") as mock_render:
             with patch("simple_history.admin.SIMPLE_HISTORY_EDIT", False):
                 admin.history_form_view(request, poll.id, history.pk)
 
         context = {
             **admin_site.each_context(request),
             # Verify this is set for history object not poll object
+            "log_entries": ANY,
             "original": poll,
             "change_history": False,
             "title": "Revert %s" % force_str(poll),
             "adminform": ANY,
             "object_id": poll.id,
             "is_popup": False,
             "media": ANY,
@@ -764,17 +768,17 @@
             "form_url": "",
             "opts": ANY,
             "content_type_id": ANY,
             "save_as": admin.save_as,
             "save_on_top": admin.save_on_top,
             "root_path": getattr(admin_site, "root_path", None),
         }
-        # This key didn't exist prior to Django 4.2
-        if "log_entries" in context:
-            context["log_entries"] = ANY
+        # DEV: Remove this when support for Django 4.2 has been dropped
+        if django.VERSION < (5, 0):
+            del context["log_entries"]
 
         mock_render.assert_called_once_with(
             request, admin.object_history_form_template, context
         )
 
     def test_history_form_view_getting_history_abstract_external(self):
         request = RequestFactory().post("/")
@@ -794,14 +798,15 @@
         with patch("simple_history.admin.render") as mock_render:
             with patch("simple_history.admin.SIMPLE_HISTORY_EDIT", True):
                 admin.history_form_view(request, obj.id, history.pk)
 
         context = {
             **admin_site.each_context(request),
             # Verify this is set for history object
+            "log_entries": ANY,
             "original": history.instance,
             "change_history": True,
             "title": "Revert %s" % force_str(history.instance),
             "adminform": ANY,
             "object_id": obj.id,
             "is_popup": False,
             "media": ANY,
@@ -825,17 +830,17 @@
             "form_url": "",
             "opts": ANY,
             "content_type_id": ANY,
             "save_as": admin.save_as,
             "save_on_top": admin.save_on_top,
             "root_path": getattr(admin_site, "root_path", None),
         }
-        # This key didn't exist prior to Django 4.2
-        if "log_entries" in context:
-            context["log_entries"] = ANY
+        # DEV: Remove this when support for Django 4.2 has been dropped
+        if django.VERSION < (5, 0):
+            del context["log_entries"]
 
         mock_render.assert_called_once_with(
             request, admin.object_history_form_template, context
         )
 
     def test_history_form_view_accepts_additional_context(self):
         request = RequestFactory().post("/")
@@ -858,14 +863,15 @@
                 history.pk,
                 extra_context={"anything_else": "will be merged into context"},
             )
 
         context = {
             **admin_site.each_context(request),
             # Verify this is set for original object
+            "log_entries": ANY,
             "anything_else": "will be merged into context",
             "original": poll,
             "change_history": False,
             "title": "Revert %s" % force_str(poll),
             "adminform": ANY,
             "object_id": poll.id,
             "is_popup": False,
@@ -888,17 +894,17 @@
             "form_url": "",
             "opts": ANY,
             "content_type_id": ANY,
             "save_as": admin.save_as,
             "save_on_top": admin.save_on_top,
             "root_path": getattr(admin_site, "root_path", None),
         }
-        # This key didn't exist prior to Django 4.2
-        if "log_entries" in context:
-            context["log_entries"] = ANY
+        # DEV: Remove this when support for Django 4.2 has been dropped
+        if django.VERSION < (5, 0):
+            del context["log_entries"]
 
         mock_render.assert_called_once_with(
             request, admin.object_history_form_template, context
         )
 
     def assert_history_view_response_contains(
         self, user=None, *, title_prefix: PermissionAction, choose_date: bool
```

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_commands.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_deprecation.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_index.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_manager.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime, timedelta
 from operator import attrgetter
 
-import django
 from django.contrib.auth import get_user_model
 from django.db import IntegrityError
 from django.test import TestCase, override_settings, skipUnlessDBFeature
 
 from simple_history.manager import SIMPLE_HISTORY_REVERSE_ATTR_NAME
 
 from ..models import Choice, Document, Poll, RankedDocument
@@ -195,21 +194,14 @@
         self.data = [
             Poll(id=1, question="Question 1", pub_date=datetime.now()),
             Poll(id=2, question="Question 2", pub_date=datetime.now()),
             Poll(id=3, question="Question 3", pub_date=datetime.now()),
             Poll(id=4, question="Question 4", pub_date=datetime.now()),
         ]
 
-    # DEV: Remove this method when the minimum required Django version is 4.2
-    def assertQuerySetEqual(self, *args, **kwargs):
-        if django.VERSION < (4, 2):
-            return self.assertQuerysetEqual(*args, **kwargs)
-        else:
-            return super().assertQuerySetEqual(*args, **kwargs)
-
     def test_simple_bulk_history_create(self):
         created = Poll.history.bulk_history_create(self.data)
         self.assertEqual(len(created), 4)
         self.assertQuerySetEqual(
             Poll.history.order_by("question"),
             ["Question 1", "Question 2", "Question 3", "Question 4"],
             attrgetter("question"),
@@ -330,21 +322,14 @@
         self.data = [
             Poll(id=1, question="Question 1", pub_date=datetime.now()),
             Poll(id=2, question="Question 2", pub_date=datetime.now()),
             Poll(id=3, question="Question 3", pub_date=datetime.now()),
             Poll(id=4, question="Question 4", pub_date=datetime.now()),
         ]
 
-    # DEV: Remove this method when the minimum required Django version is 4.2
-    def assertQuerySetEqual(self, *args, **kwargs):
-        if django.VERSION < (4, 2):
-            return self.assertQuerysetEqual(*args, **kwargs)
-        else:
-            return super().assertQuerySetEqual(*args, **kwargs)
-
     def test_simple_bulk_history_create(self):
         created = Poll.history.bulk_history_create(self.data, update=True)
         self.assertEqual(len(created), 4)
         self.assertQuerySetEqual(
             Poll.history.order_by("question"),
             ["Question 1", "Question 2", "Question 3", "Question 4"],
             attrgetter("question"),
```

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_middleware.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_models.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_signals.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_template_utils.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_template_utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/test_utils.py` & `django_simple_history-3.7.0/simple_history/tests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/tests/utils.py` & `django_simple_history-3.7.0/simple_history/tests/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/urls.py` & `django_simple_history-3.7.0/simple_history/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/tests/view.py` & `django_simple_history-3.7.0/simple_history/tests/view.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/simple_history/utils.py` & `django_simple_history-3.7.0/simple_history/utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_history-3.6.0/tox.ini` & `django_simple_history-3.7.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tox]
 envlist =
-    py{38,39,310}-dj32-{sqlite3,postgres,mysql,mariadb},
     py{38,39,310,311,312}-dj42-{sqlite3,postgres,mysql,mariadb},
     py{310,311,312}-dj50-{sqlite3,postgres,mysql,mariadb},
     py{310,311,312}-djmain-{sqlite3,postgres,mysql,mariadb},
     # DEV: Add `313` to the Python versions above (so that postgres is tested with 3.13)
-    #      when `psycopg2-binary` supports 3.13
+    #      when `psycopg` provides binaries for 3.13
     py313-dj{42,50,main}-{sqlite3,mysql,mariadb},
     docs,
     lint
 
 [gh-actions]
 python =
     3.8: py38
@@ -17,29 +16,27 @@
     3.10: py310
     3.11: py311, docs, lint
     3.12: py312
     3.13: py313
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32
     4.2: dj42
     5.0: dj50
     main: djmain
 
 [flake8]
 ignore = N802,F401,W503
 max-complexity = 10
 max-line-length = 88
 exclude = __init__.py,simple_history/registry_tests/migration_test_app/migrations/*
 
 [testenv]
 deps =
     -rrequirements/test.txt
-    dj32: Django>=3.2,<3.3
     dj42: Django>=4.2,<4.3
     dj50: Django>=5.0,<5.1
     djmain: https://github.com/django/django/tarball/main
     postgres: -rrequirements/postgres.txt
     mysql: -rrequirements/mysql.txt
     mariadb: -rrequirements/mysql.txt
 
@@ -49,16 +46,16 @@
     mysql: coverage run -a runtests.py --database=mysql {posargs}
     mariadb: coverage run -a runtests.py --database=mariadb {posargs}
     coverage report
 
 [testenv:format]
 deps = -rrequirements/lint.txt
 commands =
-    isort docs simple_history runtests.py setup.py
-    black docs simple_history runtests.py setup.py
+    isort docs simple_history runtests.py
+    black docs simple_history runtests.py
     flake8 simple_history
 
 [testenv:lint]
 deps = pre-commit
 commands =
     pre-commit run --all-files
```

