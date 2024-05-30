# Comparing `tmp/django_simple_deploy-0.6.3.tar.gz` & `tmp/django_simple_deploy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_deploy-0.6.3.tar", last modified: Tue May 28 19:45:11 2024, max compression
+gzip compressed data, was "django_simple_deploy-0.6.4.tar", last modified: Thu May 30 16:45:51 2024, max compression
```

## Comparing `django_simple_deploy-0.6.3.tar` & `django_simple_deploy-0.6.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.302088 django_simple_deploy-0.6.3/
--rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-28 19:45:11.302009 django_simple_deploy-0.6.3/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301761 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2804 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       42 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       14 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.291033 django_simple_deploy-0.6.3/docs/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.292017 django_simple_deploy-0.6.3/docs/contributing/
--rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.3/docs/contributing/architecture_notes.md
--rw-r--r--   0 eric       (501) staff       (20)      836 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.3/docs/contributing/coding_guide.md
--rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.3/docs/contributing/development_environment.md
--rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/contributing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/contributing/own_account.md
--rw-r--r--   0 eric       (501) staff       (20)     5115 2024-05-28 06:37:29.000000 django_simple_deploy-0.6.3/docs/contributing/parking_lot.md
--rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.3/docs/contributing/test_run.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.292424 django_simple_deploy-0.6.3/docs/design_docs/
--rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/design_docs/rationale.md
--rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/design_docs/strengths_limitations.md
--rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/design_docs/use_cases.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.292687 django_simple_deploy-0.6.3/docs/general_documentation/
--rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.3/docs/general_documentation/choosing_platform.md
--rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/general_documentation/cli_reference.md
--rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/index.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.293313 django_simple_deploy-0.6.3/docs/maintaining/
--rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/maintaining/adr.md
--rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/maintaining/index.md
--rw-r--r--   0 eric       (501) staff       (20)     1859 2024-05-27 16:42:26.000000 django_simple_deploy-0.6.3/docs/maintaining/managing_releases.md
--rw-r--r--   0 eric       (501) staff       (20)     1666 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/docs/maintaining/merging_prs.md
--rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/maintaining/updating_docs.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.293836 django_simple_deploy-0.6.3/docs/quick_starts/
--rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/quick_starts/index.md
--rw-r--r--   0 eric       (501) staff       (20)     4059 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.3/docs/quick_starts/quick_start_flyio.md
--rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.3/docs/quick_starts/quick_start_heroku.md
--rw-r--r--   0 eric       (501) staff       (20)     3527 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.3/docs/quick_starts/quick_start_platformsh.md
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.294081 django_simple_deploy-0.6.3/docs/roadmap/
--rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/roadmap/index.md
--rw-r--r--   0 eric       (501) staff       (20)     6149 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.3/docs/roadmap/reaching_one_point_o.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.294597 django_simple_deploy-0.6.3/docs/testing/
--rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/e2e_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/integration_tests.md
--rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.6.3/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)     1355 2024-05-28 19:45:11.302794 django_simple_deploy-0.6.3/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.294823 django_simple_deploy-0.6.3/simple_deploy/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.3/simple_deploy/apps.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.288545 django_simple_deploy-0.6.3/simple_deploy/management/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.296220 django_simple_deploy-0.6.3/simple_deploy/management/commands/
--rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/cli.py
--rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.296512 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/
--rw-r--r--   0 eric       (501) staff       (20)    29973 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     8489 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.297183 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/
--rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile
--rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
--rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
--rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/fly.toml
--rw-r--r--   0 eric       (501) staff       (20)     1416 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.297482 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/
--rw-r--r--   0 eric       (501) staff       (20)    19163 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.298965 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1285 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.299467 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/
--rw-r--r--   0 eric       (501) staff       (20)    16563 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     7112 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301110 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/services.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.289162 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301234 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301566 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
--rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
--rw-r--r--   0 eric       (501) staff       (20)      673 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
--rw-r--r--   0 eric       (501) staff       (20)      788 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/utils.py
--rw-r--r--   0 eric       (501) staff       (20)    27314 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/simple_deploy.py
--rw-r--r--   0 eric       (501) staff       (20)    12349 2024-05-25 22:52:28.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/utils.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.804474 django_simple_deploy-0.6.4/
+-rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-30 16:45:51.804420 django_simple_deploy-0.6.4/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.804200 django_simple_deploy-0.6.4/django_simple_deploy.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-30 16:45:51.000000 django_simple_deploy-0.6.4/django_simple_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2804 2024-05-30 16:45:51.000000 django_simple_deploy-0.6.4/django_simple_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-30 16:45:51.000000 django_simple_deploy-0.6.4/django_simple_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       42 2024-05-30 16:45:51.000000 django_simple_deploy-0.6.4/django_simple_deploy.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       14 2024-05-30 16:45:51.000000 django_simple_deploy-0.6.4/django_simple_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.796077 django_simple_deploy-0.6.4/docs/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.796919 django_simple_deploy-0.6.4/docs/contributing/
+-rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.4/docs/contributing/architecture_notes.md
+-rw-r--r--   0 eric       (501) staff       (20)      836 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.4/docs/contributing/coding_guide.md
+-rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.4/docs/contributing/development_environment.md
+-rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/contributing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/contributing/own_account.md
+-rw-r--r--   0 eric       (501) staff       (20)     5344 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/docs/contributing/parking_lot.md
+-rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.4/docs/contributing/test_run.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.797322 django_simple_deploy-0.6.4/docs/design_docs/
+-rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/design_docs/rationale.md
+-rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/design_docs/strengths_limitations.md
+-rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/design_docs/use_cases.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.797567 django_simple_deploy-0.6.4/docs/general_documentation/
+-rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.4/docs/general_documentation/choosing_platform.md
+-rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/general_documentation/cli_reference.md
+-rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/index.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.798225 django_simple_deploy-0.6.4/docs/maintaining/
+-rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/maintaining/adr.md
+-rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/maintaining/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     1859 2024-05-27 16:42:26.000000 django_simple_deploy-0.6.4/docs/maintaining/managing_releases.md
+-rw-r--r--   0 eric       (501) staff       (20)     1666 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.4/docs/maintaining/merging_prs.md
+-rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/maintaining/updating_docs.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.798772 django_simple_deploy-0.6.4/docs/quick_starts/
+-rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/quick_starts/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3937 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/docs/quick_starts/quick_start_flyio.md
+-rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.4/docs/quick_starts/quick_start_heroku.md
+-rw-r--r--   0 eric       (501) staff       (20)     3359 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/docs/quick_starts/quick_start_platformsh.md
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/requirements.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.799031 django_simple_deploy-0.6.4/docs/roadmap/
+-rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/docs/roadmap/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     6143 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/docs/roadmap/reaching_one_point_o.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.799543 django_simple_deploy-0.6.4/docs/testing/
+-rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.4/docs/testing/e2e_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.4/docs/testing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.4/docs/testing/integration_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.4/docs/testing/unit_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.6.4/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1355 2024-05-30 16:45:51.805126 django_simple_deploy-0.6.4/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.799758 django_simple_deploy-0.6.4/simple_deploy/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.4/simple_deploy/apps.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.793675 django_simple_deploy-0.6.4/simple_deploy/management/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.800835 django_simple_deploy-0.6.4/simple_deploy/management/commands/
+-rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/cli.py
+-rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.801093 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/
+-rw-r--r--   0 eric       (501) staff       (20)    29285 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     7830 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.801729 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/
+-rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/dockerfile
+-rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
+-rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
+-rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/fly.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1416 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.802020 django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/
+-rw-r--r--   0 eric       (501) staff       (20)    19163 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.802272 django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1285 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.802679 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/
+-rw-r--r--   0 eric       (501) staff       (20)    16433 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     6986 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.803676 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/services.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.794360 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.803864 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/tests/unit_tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-30 16:45:51.804021 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
+-rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
+-rw-r--r--   0 eric       (501) staff       (20)     1256 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
+-rw-r--r--   0 eric       (501) staff       (20)     1010 2024-05-30 16:43:25.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)    27314 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/simple_deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)    12349 2024-05-25 22:52:28.000000 django_simple_deploy-0.6.4/simple_deploy/management/commands/utils.py
```

### Comparing `django_simple_deploy-0.6.3/LICENSE` & `django_simple_deploy-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/PKG-INFO` & `django_simple_deploy-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.3
+Version: 0.6.4
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django_simple_deploy-0.6.3/README.md` & `django_simple_deploy-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/django_simple_deploy.egg-info/PKG-INFO` & `django_simple_deploy-0.6.4/django_simple_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.3
+Version: 0.6.4
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django_simple_deploy-0.6.3/django_simple_deploy.egg-info/SOURCES.txt` & `django_simple_deploy-0.6.4/django_simple_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/contributing/architecture_notes.md` & `django_simple_deploy-0.6.4/docs/contributing/architecture_notes.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/contributing/coding_guide.md` & `django_simple_deploy-0.6.4/docs/contributing/coding_guide.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/contributing/development_environment.md` & `django_simple_deploy-0.6.4/docs/contributing/development_environment.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/contributing/index.md` & `django_simple_deploy-0.6.4/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/contributing/own_account.md` & `django_simple_deploy-0.6.4/docs/contributing/own_account.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/contributing/parking_lot.md` & `django_simple_deploy-0.6.4/docs/contributing/parking_lot.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,13 +60,16 @@
 ---
 
 - Simplify approach to checking for db. See [#297](https://github.com/ehmatthes/django-simple-deploy/issues/297).
 
 Platform.sh
 ---
 
+- Update runtime to Python 3.12.
+- The method `_validate_platform()` makes sure the user is authenticated through the CLI. I believe we can remove some checks for authentication in subsequent CLI calls, as in `_get_org_name()`.
+
 
 Heroku
 ---
 
 - If not pushing from the main branch, state that explicitly. Consider confirming that's what user wants. State the branch name explicitly in the summary message. See [#5](https://github.com/ehmatthes/django-simple-deploy/issues/5).
 - Reconsider Heroku support. People have lost confidence in Heroku in recent years, but it still keeps largely working. See [#91](https://github.com/ehmatthes/django-simple-deploy/issues/91).
```

### Comparing `django_simple_deploy-0.6.3/docs/contributing/test_run.md` & `django_simple_deploy-0.6.4/docs/contributing/test_run.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/design_docs/rationale.md` & `django_simple_deploy-0.6.4/docs/design_docs/rationale.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/design_docs/strengths_limitations.md` & `django_simple_deploy-0.6.4/docs/design_docs/strengths_limitations.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/design_docs/use_cases.md` & `django_simple_deploy-0.6.4/docs/design_docs/use_cases.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/general_documentation/choosing_platform.md` & `django_simple_deploy-0.6.4/docs/general_documentation/choosing_platform.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/general_documentation/cli_reference.md` & `django_simple_deploy-0.6.4/docs/general_documentation/cli_reference.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/index.md` & `django_simple_deploy-0.6.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/maintaining/adr.md` & `django_simple_deploy-0.6.4/docs/maintaining/adr.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/maintaining/index.md` & `django_simple_deploy-0.6.4/docs/maintaining/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/maintaining/managing_releases.md` & `django_simple_deploy-0.6.4/docs/maintaining/managing_releases.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/maintaining/merging_prs.md` & `django_simple_deploy-0.6.4/docs/maintaining/merging_prs.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/maintaining/updating_docs.md` & `django_simple_deploy-0.6.4/docs/maintaining/updating_docs.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/quick_starts/quick_start_flyio.md` & `django_simple_deploy-0.6.4/docs/quick_starts/quick_start_flyio.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     - footer
 ---
 
 # Quick Start: Deploying to Fly.io
 
 ## Overview
 
-Support for Fly.io is in a preliminary phase. `django-simple-deploy` should only be used on test projects at this point.
-
 Deployment to Fly.io can be fully automated, but the configuration-only approach is recommended. This allows you to review the changes that are made to your project before committing them and making the initial push. The fully automated approach configures your project, commits these changes, and pushes the project to Fly.io's servers.
 
 ## Prerequisites
 
 Deployment to Fly.io requires three things:
 
 - You must be using Git to track your project.
```

### Comparing `django_simple_deploy-0.6.3/docs/quick_starts/quick_start_heroku.md` & `django_simple_deploy-0.6.4/docs/quick_starts/quick_start_heroku.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/quick_starts/quick_start_platformsh.md` & `django_simple_deploy-0.6.4/docs/quick_starts/quick_start_platformsh.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     - footer
 ---
 
 # Quick Start: Deploying to Platform.sh
 
 ## Overview
 
-Support for Platform.sh is in a preliminary phase. For example, it won't work if you already have a project deployed to Platform.sh, or if you have more than one org.
-
 Deployment to Platform.sh can be fully automated, but the configuration-only approach is recommended. This allows you to review the changes that are made to your project before committing them and making the initial push. The fully automated approach configures your project, commits these changes, and pushes the project to Platform.sh' servers.
 
 ## Prerequisites
 
 Deployment to Platform.sh requires three things:
 
 - You must be using Git to track your project.
```

### Comparing `django_simple_deploy-0.6.3/docs/roadmap/reaching_one_point_o.md` & `django_simple_deploy-0.6.4/docs/roadmap/reaching_one_point_o.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 ## Overall stability of deployment process
 
 Support for a new platform starts out as a proof-of-concept, showing that deployment to that platform can be automated. Full stability means people can use `simple_deploy` on a variety of projects with predictable, stable results. It also means the deployment is configured using best practices for that platform. For example, if it's a container-based platform, we produce a Dockerfile that you can build on as your deployment grows.
 
 | Fly.io | Platform.sh | Heroku |
 | :--------------------------: | :----: | :----: |
-| :fontawesome-regular-square-check: | :fontawesome-regular-square-check: | :fontawesome-regular-square-check: |
+| :fontawesome-solid-square-check: | :fontawesome-solid-square-check: | :fontawesome-solid-square-check: |
 
 ## Other notes
 
 There are a number of other questions to answer formally, and tasks to complete, before releasing a 1.0 version:
 
 - [ ] Is the API stable enough for a 1.0 release?
 - [ ] Should we adopt a plugin-based approach?
```

### Comparing `django_simple_deploy-0.6.3/docs/testing/e2e_tests.md` & `django_simple_deploy-0.6.4/docs/testing/e2e_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/testing/index.md` & `django_simple_deploy-0.6.4/docs/testing/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/testing/integration_tests.md` & `django_simple_deploy-0.6.4/docs/testing/integration_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/docs/testing/unit_tests.md` & `django_simple_deploy-0.6.4/docs/testing/unit_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/setup.cfg` & `django_simple_deploy-0.6.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-simple-deploy
-version = 0.6.3
+version = 0.6.4
 description = A management command that auto-configures a Django project for deployment.
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Documentation = https://django-simple-deploy.readthedocs.io/en/latest/
 	GitHub = https://github.com/ehmatthes/django-simple-deploy
 	Changelog = https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/cli.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/cli.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/deploy_messages.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
     # --- Public methods ---
 
     def deploy(self, *args, **options):
         """Coordinate the overall configuration and deployment."""
         self.sd.write_output("\nConfiguring project for deployment to Fly.io...")
 
-        self._confirm_preliminary()
         self._validate_platform()
 
         self._prep_automate_all()
         self._set_env_vars()
         self._add_dockerfile()
         self._add_dockerignore()
         self._add_flytoml()
@@ -54,30 +53,14 @@
         self._add_requirements()
 
         self._conclude_automate_all()
         self._show_success_message()
 
     # --- Helper methods for deploy() ---
 
-    def _confirm_preliminary(self):
-        """Confirm acknwledgement of preliminary (pre-1.0) state of project."""
-        self.sd.write_output(self.messages.confirm_preliminary)
-
-        # Unit test check is here, so message is logged.
-        if self.sd.unit_testing:
-            return
-
-        if self.sd.get_confirmation():
-            self.sd.write_output("  Continuing with Fly.io deployment...")
-        else:
-            # Quit and invite the user to try another platform. We are happily exiting
-            # the script; there's no need to raise an error.
-            self.sd.write_output(self.messages.cancel_flyio)
-            sys.exit()
-
     def _validate_platform(self):
         """Make sure the local environment and project supports deployment to Fly.io.
 
         Make sure CLI is installed, and user is authenticated. Make sure necessary
         resources have been created and identified, and that we have the user's
         permission to use those resources.
```

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy_messages.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/deploy_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,14 @@
 # For conventions, see documentation in deploy_messages.py
 
 from textwrap import dedent
 
 from django.conf import settings
 
 
-confirm_preliminary = """
-***** Support for Fly.io is in the preliminary phase ***
-
-- Support for deploying to Fly.io is in the preliminary phase at this point.
-- You should only be using this project to deploy to Fly.io at this point if
-  you are interested in helping to develop or test the simple_deploy project.
-- You should look at the deploy_flyio.py script before running this command,
-  so you know what kinds of changes will be made to your project.
-- You should understand the Fly.io console, and be comfortable deleting resources
-  that are created during this deployment.
-- You may want to cancel this run and deploy to a different platform.
-"""
-
 confirm_automate_all = """
 The --automate-all flag means simple_deploy will:
 - Run `fly apps create` for you, to create an empty Fly.io project.
 - Run `fly postgres create`, to create a new database for your project.
 - Configure your project for deployment on Fly.io.
 - Commit all changes to your project that are necessary for deployment.
 - Push these changes to Fly.io.
```

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/fly.toml` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/fly.toml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/settings.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/fly_io/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/deploy.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy_messages.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/templates/settings.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/heroku/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,45 +37,28 @@
     # --- Public methods ---
 
     def deploy(self, *args, **options):
         """Coordinate the overall configuration and deployment."""
 
         self.sd.write_output("\nConfiguring project for deployment to Platform.sh...")
 
-        self._confirm_preliminary()
         self._validate_platform()
 
         self._prep_automate_all()
         self._modify_settings()
         self._add_requirements()
         self._generate_platform_app_yaml()
         self._make_platform_dir()
         self._generate_services_yaml()
 
         self._conclude_automate_all()
         self._show_success_message()
 
     # --- Helper methods for deploy() ---
 
-    def _confirm_preliminary(self):
-        """Confirm acknwledgement of preliminary (pre-1.0) state of project."""
-        self.sd.write_output(self.messages.confirm_preliminary)
-
-        # Unit test check is here, so message is logged.
-        if self.sd.unit_testing:
-            return
-
-        if self.sd.get_confirmation():
-            self.sd.write_output("  Continuing with platform.sh deployment...")
-        else:
-            # Quit and invite the user to try another platform. We are happily exiting
-            # the script; there's no need to raise an error.
-            self.sd.write_output(self.messages.cancel_plsh)
-            sys.exit()
-
     def _validate_platform(self):
         """Make sure the local environment and project supports deployment to
         Platform.sh.
 
         Make sure CLI is installed, and user is authenticated. Make sure necessary
         resources have been created and identified, and that we have the user's
         permission to use those resources.
@@ -379,39 +362,55 @@
             return
 
         cmd = "platform organization:list --yes --format csv"
         output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
         self.sd.log_info(output_str)
 
-        if not output_str:
-            output_str = output_obj.stderr.decode()
-            if "LoginRequiredException" in output_str:
-                raise SimpleDeployCommandError(self.sd, self.messages.login_required)
-            else:
-                error_msg = self.messages.unknown_error
-                error_msg += self.messages.cli_not_installed
-                raise SimpleDeployCommandError(self.sd, error_msg)
-
-        org_name = plsh_utils.get_org_name(output_str)
-        if not org_name:
+        org_names = plsh_utils.get_org_names(output_str)
+        if not org_names:
             raise SimpleDeployCommandError(self.sd, self.messages.org_not_found)
 
-        if self._confirm_use_org_name(org_name):
-            return org_name
+        if len(org_names) == 1:
+            # Get permission to use this org.
+            org_name = org_names[0]
+            if self._confirm_use_org(org_name):
+                return org_name
+
+        # Show all orgs, ask user to make selection.
+        prompt = "\n*** Found multiple orgs on Platform.sh. ***"
+        for index, name in enumerate(org_names):
+            prompt += f"\n  {index}: {name}"
+        prompt += "\nWhich org would you like to use? "
+
+        valid_choices = [i for i in range(len(org_names))]
+
+        # Confirm selection, because we do *not* want to deploy using the wrong org.
+        confirmed = False
+        while not confirmed:
+            selection = sd_utils.get_numbered_choice(
+                self.sd, prompt, valid_choices, self.messages.no_org_available
+            )
+            selected_org = org_names[selection]
+
+            confirm_prompt = f"You have selected {selected_org}."
+            confirm_prompt += " Is that correct?"
+            confirmed = self.sd.get_confirmation(confirm_prompt)
+
+            return selected_org
 
-    def _confirm_use_org_name(self, org_name):
-        """Confirm that it's okay to use the org name that was found.
+    def _confirm_use_org(self, org_name):
+        """Confirm that it's okay to use the org that was found.
 
         Returns:
             True: if confirmed
             SimpleDeployCommandError: if not confirmed
         """
 
-        self.stdout.write(self.messages.confirm_use_org_name(org_name))
+        self.stdout.write(self.messages.confirm_use_org(org_name))
         confirmed = self.sd.get_confirmation(skip_logging=True)
 
         if confirmed:
             self.stdout.write("  Okay, continuing with deployment.")
             return True
         else:
             # Exit, with a message that configuration is still an option.
```

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy_messages.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/deploy_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,14 @@
 # For conventions, see documentation in deploy_messages.py
 
 from textwrap import dedent
 
 from django.conf import settings
 
 
-confirm_preliminary = """
-***** Deployment to platform.sh is under active development at this point ***
-
-- If you already have a project deployed on Platform.sh, configuration will fail.
-- If you have more than one org on Platform.sh, configuration will fail.
-"""
-
 confirm_automate_all = """
 The --automate-all flag means simple_deploy will:
 - Run `platform create` for you, to create an empty Platform.sh project.
   - This will create a project in the us-3.platform.sh region. If you wish
     to use a different region, cancel this operation and use the --region flag.
   - You can see a list of all regions by running `platform help project:create`
 - Commit all changes to your project that are necessary for deployment.
@@ -72,14 +65,19 @@
 The Platform.sh CLI requires an organization name when creating a new project.
 
 Please visit the Platform.sh console and make sure you have created an organization.
 You can also do this through the CLI using the `platform organization:create` command.
 For help, run `platform help organization:create`.
 """
 
+no_org_available = """
+A Platform.sh org must be used to make a deployment. Please identify or create the org
+you'd like to use, and then try again.
+"""
+
 login_required = """
 You appear to be logged out of the Platform.sh CLI. Please run the 
 command `platform login`, and then run simple_deploy again.
 
 You may be able to override this error by passing the `--deployed-project-name`
 flag.
 """
@@ -97,22 +95,22 @@
 
 
 # --- Dynamic strings ---
 # These need to be generated in functions, to display information that's
 #   determined as the script runs.
 
 
-def confirm_use_org_name(org_name):
-    """Confirm use of this org name to create a new project."""
+def confirm_use_org(org_name):
+    """Confirm use of this org to create a new project."""
 
     msg = dedent(
         f"""
         --- The Platform.sh CLI requires an organization name when creating a new project. ---
         When using --automate-all, a project will be created on your behalf. The following
-        organization name was found: {org_name}
+        organization was found: {org_name}
 
         This organization will be used to create a new project. If this is not okay,
         enter n to cancel this operation.
     """
     )
 
     return msg
```

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/settings.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/simple_deploy.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/simple_deploy.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.3/simple_deploy/management/commands/utils.py` & `django_simple_deploy-0.6.4/simple_deploy/management/commands/utils.py`

 * *Files identical despite different names*

