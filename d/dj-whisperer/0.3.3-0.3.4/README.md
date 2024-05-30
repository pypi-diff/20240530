# Comparing `tmp/dj-whisperer-0.3.3.tar.gz` & `tmp/dj-whisperer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-whisperer-0.3.3.tar", last modified: Tue May 28 23:17:11 2024, max compression
+gzip compressed data, was "dist/dj-whisperer-0.3.4.tar", last modified: Thu May 30 07:36:40 2024, max compression
```

## Comparing `dj-whisperer-0.3.3.tar` & `dj-whisperer-0.3.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     1639 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4893 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3334 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3430 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/dj_whisperer.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4893 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/dj_whisperer.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/dj_whisperer.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/dj_whisperer.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/dj_whisperer.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/dj_whisperer.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4589 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/advanced.rst
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      806 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/tox.ini
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/whisperer/
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/client.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/codes.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/countdown.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/events.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/whisperer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0002_webhook_additional_headers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0003_auto_20200505_0853.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0004_webhook_retry_count.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0005_webhook_config.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0006_auto_20200925_1710.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0007_event_queue.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/0008_ayto_20240323_2301.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3775 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/whisperer/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/resources/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/resources/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/resources/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/services.py
--rw-rw-rw-   0 root         (0) root         (0)    10262 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:17:11.000000 dj-whisperer-0.3.3/whisperer/tests/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/test_serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)    31273 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     2112 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/tests/webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2024-05-28 23:16:45.000000 dj-whisperer-0.3.3/whisperer/validators.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4944 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/dj_whisperer.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4944 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/dj_whisperer.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/dj_whisperer.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/dj_whisperer.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/dj_whisperer.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/dj_whisperer.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4589 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/advanced.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      806 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/introduction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2404 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/whisperer/
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/countdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/whisperer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0002_webhook_additional_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0003_auto_20200505_0853.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0004_webhook_retry_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0005_webhook_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0006_auto_20200925_1710.py
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0007_event_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/0008_ayto_20240323_2301.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3775 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/whisperer/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/resources/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/resources/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/resources/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/services.py
+-rw-rw-rw-   0 root         (0) root         (0)    10262 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:36:40.000000 dj-whisperer-0.3.4/whisperer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/test_serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    31273 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     2112 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/tests/webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-05-30 07:36:17.000000 dj-whisperer-0.3.4/whisperer/validators.py
```

### Comparing `dj-whisperer-0.3.3/.gitignore` & `dj-whisperer-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/LICENSE.txt` & `dj-whisperer-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/Makefile` & `dj-whisperer-0.3.4/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 COMBINATIONS := py27-django110 py27-django111 \
                 py34-django110 py34-django111 py34-django20 \
                 py35-django110 py35-django111 py35-django20 py35-django21 py35-django22 \
                 py36-django111 py36-django20 py36-django21 py36-django22 py36-django30 py36-django31 \
                 py37-django111 py37-django20 py37-django21 py37-django22 py37-django30 py37-django31 \
                 py38-django22 py38-django30 py38-django31 py38-django32 py38-django40 py38-django41 py38-django42 \
                 py39-django32 py39-django40 py39-django41 py39-django42 \
-                py310-django40 py310-django41 py310-django42
+                py310-django40 py310-django41 py310-django42 \
+                py311-django42
 
 # ANSI color codes
 YELLOW := \033[33m
 WHITE := \033[97m
 RESET := \033[0m
 
 # Define commands
```

### Comparing `dj-whisperer-0.3.3/PKG-INFO` & `dj-whisperer-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-whisperer
-Version: 0.3.3
+Version: 0.3.4
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-whisperer
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
```

### Comparing `dj-whisperer-0.3.3/README.md` & `dj-whisperer-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/bitbucket-pipelines.yml` & `dj-whisperer-0.3.4/bitbucket-pipelines.yml`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,24 @@
           script:
             - apk add postgresql-dev gcc git python3-dev musl-dev
             - pip install tox
             - tox -e py310-django40,py310-django41,py310-django42
           services:
             - postgres
             - redis
+      - step:
+          name: py311
+          image: python:3.11-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py311-django42
+          services:
+            - postgres
+            - redis
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.7-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
```

### Comparing `dj-whisperer-0.3.3/dj_whisperer.egg-info/PKG-INFO` & `dj-whisperer-0.3.4/dj_whisperer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-whisperer
-Version: 0.3.3
+Version: 0.3.4
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-whisperer
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
```

### Comparing `dj-whisperer-0.3.3/dj_whisperer.egg-info/SOURCES.txt` & `dj-whisperer-0.3.4/dj_whisperer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/Makefile` & `dj-whisperer-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/advanced.rst` & `dj-whisperer-0.3.4/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/conf.py` & `dj-whisperer-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/index.rst` & `dj-whisperer-0.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/introduction.rst` & `dj-whisperer-0.3.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/make.bat` & `dj-whisperer-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/docs/quickstart.rst` & `dj-whisperer-0.3.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/setup.py` & `dj-whisperer-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Django",
         "Framework :: Django :: 1.10",
         "Framework :: Django :: 1.11",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
```

### Comparing `dj-whisperer-0.3.3/tox.ini` & `dj-whisperer-0.3.4/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
           {py36,py37}-{django111,django20,django21,django22,django30,django31}
           py38-{django22,django30,django31,django32,django40,django41,django42}
           py39-{django32,django40,django41,django42}
           py310-{django40,django41,django42}
+          py311-{django42}
           linting
 
 [testenv]
 deps = django110: Django>=1.10,<1.11
        django110: celery==4.1.0
        django111: Django>=1.11.7,<2.0
        django{110,111}: django-filter==1.1.0
```

### Comparing `dj-whisperer-0.3.3/whisperer/client.py` & `dj-whisperer-0.3.4/whisperer/client.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/codes.py` & `dj-whisperer-0.3.4/whisperer/codes.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/countdown.py` & `dj-whisperer-0.3.4/whisperer/countdown.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/events.py` & `dj-whisperer-0.3.4/whisperer/events.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/exceptions.py` & `dj-whisperer-0.3.4/whisperer/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0001_initial.py` & `dj-whisperer-0.3.4/whisperer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0003_auto_20200505_0853.py` & `dj-whisperer-0.3.4/whisperer/migrations/0003_auto_20200505_0853.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0004_webhook_retry_count.py` & `dj-whisperer-0.3.4/whisperer/migrations/0004_webhook_retry_count.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0005_webhook_config.py` & `dj-whisperer-0.3.4/whisperer/migrations/0005_webhook_config.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0006_auto_20200925_1710.py` & `dj-whisperer-0.3.4/whisperer/migrations/0006_auto_20200925_1710.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0007_event_queue.py` & `dj-whisperer-0.3.4/whisperer/migrations/0007_event_queue.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/migrations/0008_ayto_20240323_2301.py` & `dj-whisperer-0.3.4/whisperer/migrations/0008_ayto_20240323_2301.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/models.py` & `dj-whisperer-0.3.4/whisperer/models.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/resources/filters.py` & `dj-whisperer-0.3.4/whisperer/resources/filters.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/resources/serializers.py` & `dj-whisperer-0.3.4/whisperer/resources/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/resources/views.py` & `dj-whisperer-0.3.4/whisperer/resources/views.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/services.py` & `dj-whisperer-0.3.4/whisperer/services.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tasks.py` & `dj-whisperer-0.3.4/whisperer/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/models.py` & `dj-whisperer-0.3.4/whisperer/tests/models.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/test_serializers.py` & `dj-whisperer-0.3.4/whisperer/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/test_settings.py` & `dj-whisperer-0.3.4/whisperer/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/test_utils.py` & `dj-whisperer-0.3.4/whisperer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/test_views.py` & `dj-whisperer-0.3.4/whisperer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/tests.py` & `dj-whisperer-0.3.4/whisperer/tests/tests.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/tests/webhooks.py` & `dj-whisperer-0.3.4/whisperer/tests/webhooks.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/urls.py` & `dj-whisperer-0.3.4/whisperer/urls.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/utils.py` & `dj-whisperer-0.3.4/whisperer/utils.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.3/whisperer/validators.py` & `dj-whisperer-0.3.4/whisperer/validators.py`

 * *Files identical despite different names*

