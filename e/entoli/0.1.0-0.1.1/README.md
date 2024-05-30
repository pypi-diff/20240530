# Comparing `tmp/entoli-0.1.0.tar.gz` & `tmp/entoli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entoli-0.1.0.tar", last modified: Wed May 29 15:37:56 2024, max compression
+gzip compressed data, was "entoli-0.1.1.tar", last modified: Thu May 30 04:48:39 2024, max compression
```

## Comparing `entoli-0.1.0.tar` & `entoli-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.149585 entoli-0.1.0/
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1067 2024-05-20 14:51:24.000000 entoli-0.1.0/LICENSE
--rw-r--r--   0 chanwooahn   (501) staff       (20)      475 2024-05-29 15:26:30.000000 entoli-0.1.0/MANIFEST.in
--rw-r--r--   0 chanwooahn   (501) staff       (20)     2640 2024-05-29 15:37:56.149203 entoli-0.1.0/PKG-INFO
--rw-r--r--   0 chanwooahn   (501) staff       (20)       37 2024-05-20 14:54:00.000000 entoli-0.1.0/README.md
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.137611 entoli-0.1.0/example/
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-29 08:43:44.000000 entoli-0.1.0/example/__init__.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)      684 2024-05-29 08:54:40.000000 entoli-0.1.0/example/ask_and_sleep.py
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.138661 entoli-0.1.0/example/build/
--rw-r--r--   0 chanwooahn   (501) staff       (20)        9 2024-05-25 07:18:38.000000 entoli-0.1.0/example/build/.envrc
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.139006 entoli-0.1.0/example/build/auto_project/
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.139140 entoli-0.1.0/example/build/auto_project/auto_app_0/
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/auto_project/auto_app_0/urls.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/auto_project/urls.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)       33 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/auto_project.py
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.139385 entoli-0.1.0/example/build/django/
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.139519 entoli-0.1.0/example/build/django/contrib/
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/django/contrib/admin.py
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.139651 entoli-0.1.0/example/build/django/db/
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/django/db/models.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/django/forms.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.0/example/build/django/urls.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1252 2024-05-25 07:18:38.000000 entoli-0.1.0/example/build/flake.nix
--rw-r--r--   0 chanwooahn   (501) staff       (20)      612 2024-05-29 08:57:46.000000 entoli-0.1.0/example/fib.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)      381 2024-05-29 08:43:44.000000 entoli-0.1.0/example/greet.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     4173 2024-05-29 08:43:44.000000 entoli-0.1.0/example/nix_shell.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1497 2024-05-29 08:55:33.000000 entoli-0.1.0/example/shell.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1307 2024-05-29 15:37:52.000000 entoli-0.1.0/pyproject.toml
--rw-r--r--   0 chanwooahn   (501) staff       (20)      634 2024-05-29 15:28:30.000000 entoli-0.1.0/requirements_dev.txt
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-29 08:43:44.000000 entoli-0.1.0/ruff.toml
--rw-r--r--   0 chanwooahn   (501) staff       (20)       38 2024-05-29 15:37:56.149653 entoli-0.1.0/setup.cfg
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1229 2024-05-29 15:30:43.000000 entoli-0.1.0/setup.py
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.130999 entoli-0.1.0/src/
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.141029 entoli-0.1.0/src/entoli/
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.143401 entoli-0.1.0/src/entoli/.pytest_cache/
--rw-r--r--   0 chanwooahn   (501) staff       (20)       37 2024-05-29 08:54:08.000000 entoli-0.1.0/src/entoli/.pytest_cache/.gitignore
--rw-r--r--   0 chanwooahn   (501) staff       (20)      194 2024-05-29 08:54:08.000000 entoli-0.1.0/src/entoli/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 chanwooahn   (501) staff       (20)      295 2024-05-29 08:54:08.000000 entoli-0.1.0/src/entoli/.pytest_cache/README.md
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.131241 entoli-0.1.0/src/entoli/.pytest_cache/v/
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.144271 entoli-0.1.0/src/entoli/.pytest_cache/v/cache/
--rw-r--r--   0 chanwooahn   (501) staff       (20)       22 2024-05-29 15:21:35.000000 entoli-0.1.0/src/entoli/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1450 2024-05-29 15:22:27.000000 entoli-0.1.0/src/entoli/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 chanwooahn   (501) staff       (20)        2 2024-05-29 15:22:27.000000 entoli-0.1.0/src/entoli/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 chanwooahn   (501) staff       (20)      124 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/__init__.py
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.146164 entoli-0.1.0/src/entoli/base/
--rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/__init__.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)      454 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/control.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     2923 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/either.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1089 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/io.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     3779 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/maybe.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     4456 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/result.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     3296 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/seq.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     2314 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/base/typeclass.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)    18064 2024-05-29 08:49:57.000000 entoli-0.1.0/src/entoli/prelude.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)     4444 2024-05-29 08:46:49.000000 entoli-0.1.0/src/entoli/process.py
--rw-r--r--   0 chanwooahn   (501) staff       (20)      141 2024-05-29 08:57:51.000000 entoli-0.1.0/src/entoli/pytest.ini
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1537 2024-05-29 08:43:44.000000 entoli-0.1.0/src/entoli/system.py
-drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-29 15:37:56.146421 entoli-0.1.0/src/entoli.egg-info/
--rw-r--r--   0 chanwooahn   (501) staff       (20)     2640 2024-05-29 15:37:56.000000 entoli-0.1.0/src/entoli.egg-info/PKG-INFO
--rw-r--r--   0 chanwooahn   (501) staff       (20)     1215 2024-05-29 15:37:56.000000 entoli-0.1.0/src/entoli.egg-info/SOURCES.txt
--rw-r--r--   0 chanwooahn   (501) staff       (20)        1 2024-05-29 15:37:56.000000 entoli-0.1.0/src/entoli.egg-info/dependency_links.txt
--rw-r--r--   0 chanwooahn   (501) staff       (20)      836 2024-05-29 15:37:56.000000 entoli-0.1.0/src/entoli.egg-info/requires.txt
--rw-r--r--   0 chanwooahn   (501) staff       (20)        7 2024-05-29 15:37:56.000000 entoli-0.1.0/src/entoli.egg-info/top_level.txt
--rw-r--r--   0 chanwooahn   (501) staff       (20)      537 2024-05-29 08:43:44.000000 entoli-0.1.0/tox.ini
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.619129 entoli-0.1.1/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1067 2024-05-20 14:51:24.000000 entoli-0.1.1/LICENSE
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      475 2024-05-29 15:26:30.000000 entoli-0.1.1/MANIFEST.in
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     2211 2024-05-30 04:48:39.618754 entoli-0.1.1/PKG-INFO
+-rw-r--r--   0 chanwooahn   (501) staff       (20)       37 2024-05-20 14:54:00.000000 entoli-0.1.1/README.md
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.608022 entoli-0.1.1/example/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-29 08:43:44.000000 entoli-0.1.1/example/__init__.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      684 2024-05-29 08:54:40.000000 entoli-0.1.1/example/ask_and_sleep.py
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.608672 entoli-0.1.1/example/build/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        9 2024-05-25 07:18:38.000000 entoli-0.1.1/example/build/.envrc
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.608995 entoli-0.1.1/example/build/auto_project/
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.609129 entoli-0.1.1/example/build/auto_project/auto_app_0/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/auto_project/auto_app_0/urls.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/auto_project/urls.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)       33 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/auto_project.py
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.609406 entoli-0.1.1/example/build/django/
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.609561 entoli-0.1.1/example/build/django/contrib/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/django/contrib/admin.py
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.609686 entoli-0.1.1/example/build/django/db/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/django/db/models.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/django/forms.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-25 07:18:39.000000 entoli-0.1.1/example/build/django/urls.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1252 2024-05-25 07:18:38.000000 entoli-0.1.1/example/build/flake.nix
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      612 2024-05-29 08:57:46.000000 entoli-0.1.1/example/fib.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      381 2024-05-29 08:43:44.000000 entoli-0.1.1/example/greet.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     4173 2024-05-29 08:43:44.000000 entoli-0.1.1/example/nix_shell.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1497 2024-05-29 08:55:33.000000 entoli-0.1.1/example/shell.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1307 2024-05-29 15:37:52.000000 entoli-0.1.1/pyproject.toml
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      611 2024-05-30 04:47:08.000000 entoli-0.1.1/requirements_dev.txt
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-29 08:43:44.000000 entoli-0.1.1/ruff.toml
+-rw-r--r--   0 chanwooahn   (501) staff       (20)       38 2024-05-30 04:48:39.619376 entoli-0.1.1/setup.cfg
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      897 2024-05-30 04:47:19.000000 entoli-0.1.1/setup.py
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.604706 entoli-0.1.1/src/
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.610758 entoli-0.1.1/src/entoli/
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.612160 entoli-0.1.1/src/entoli/.pytest_cache/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)       37 2024-05-29 08:54:08.000000 entoli-0.1.1/src/entoli/.pytest_cache/.gitignore
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      194 2024-05-29 08:54:08.000000 entoli-0.1.1/src/entoli/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      295 2024-05-29 08:54:08.000000 entoli-0.1.1/src/entoli/.pytest_cache/README.md
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.604926 entoli-0.1.1/src/entoli/.pytest_cache/v/
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.613354 entoli-0.1.1/src/entoli/.pytest_cache/v/cache/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)       22 2024-05-29 15:21:35.000000 entoli-0.1.1/src/entoli/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1450 2024-05-30 04:46:57.000000 entoli-0.1.1/src/entoli/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        2 2024-05-30 04:46:57.000000 entoli-0.1.1/src/entoli/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      124 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/__init__.py
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.615623 entoli-0.1.1/src/entoli/base/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        0 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/__init__.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      454 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/control.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     2923 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/either.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1089 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/io.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     3779 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/maybe.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     4456 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/result.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     3296 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/seq.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     2314 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/base/typeclass.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)    18064 2024-05-29 08:49:57.000000 entoli-0.1.1/src/entoli/prelude.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     4444 2024-05-29 08:46:49.000000 entoli-0.1.1/src/entoli/process.py
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      141 2024-05-29 08:57:51.000000 entoli-0.1.1/src/entoli/pytest.ini
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1537 2024-05-29 08:43:44.000000 entoli-0.1.1/src/entoli/system.py
+drwxr-xr-x   0 chanwooahn   (501) staff       (20)        0 2024-05-30 04:48:39.615872 entoli-0.1.1/src/entoli.egg-info/
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     2211 2024-05-30 04:48:39.000000 entoli-0.1.1/src/entoli.egg-info/PKG-INFO
+-rw-r--r--   0 chanwooahn   (501) staff       (20)     1215 2024-05-30 04:48:39.000000 entoli-0.1.1/src/entoli.egg-info/SOURCES.txt
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        1 2024-05-30 04:48:39.000000 entoli-0.1.1/src/entoli.egg-info/dependency_links.txt
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      618 2024-05-30 04:48:39.000000 entoli-0.1.1/src/entoli.egg-info/requires.txt
+-rw-r--r--   0 chanwooahn   (501) staff       (20)        7 2024-05-30 04:48:39.000000 entoli-0.1.1/src/entoli.egg-info/top_level.txt
+-rw-r--r--   0 chanwooahn   (501) staff       (20)      537 2024-05-29 08:43:44.000000 entoli-0.1.1/tox.ini
```

### Comparing `entoli-0.1.0/LICENSE` & `entoli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/PKG-INFO` & `entoli-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 Metadata-Version: 2.1
 Name: entoli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python functional programming library
 Home-page: https://github.com/cwahn/entoli
 Author: Your Name
 Author-email: cwahn0904@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: attrs==23.2.0
-Requires-Dist: distlib==0.3.8
-Requires-Dist: filelock==3.14.0
-Requires-Dist: iniconfig==2.0.0
-Requires-Dist: more-itertools==10.2.0
-Requires-Dist: packaging==24.0
-Requires-Dist: platformdirs==4.2.2
-Requires-Dist: pluggy==0.13.1
-Requires-Dist: py==1.11.0
-Requires-Dist: toml==0.10.2
-Requires-Dist: virtualenv==20.26.2
-Requires-Dist: wheel==0.33.6
 Provides-Extra: dev
 Requires-Dist: attrs==23.2.0; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
 Requires-Dist: docutils==0.21.2; extra == "dev"
 Requires-Dist: filelock==3.14.0; extra == "dev"
@@ -35,15 +23,14 @@
 Requires-Dist: iniconfig==2.0.0; extra == "dev"
 Requires-Dist: jaraco.classes==3.4.0; extra == "dev"
 Requires-Dist: jaraco.context==5.3.0; extra == "dev"
 Requires-Dist: jaraco.functools==4.0.1; extra == "dev"
 Requires-Dist: keyring==25.2.1; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
-Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: packaging==24.0; extra == "dev"
 Requires-Dist: pkginfo==1.10.0; extra == "dev"
 Requires-Dist: platformdirs==4.2.2; extra == "dev"
 Requires-Dist: pluggy==0.13.1; extra == "dev"
 Requires-Dist: py==1.11.0; extra == "dev"
 Requires-Dist: Pygments==2.18.0; extra == "dev"
```

### Comparing `entoli-0.1.0/example/ask_and_sleep.py` & `entoli-0.1.1/example/ask_and_sleep.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/example/build/flake.nix` & `entoli-0.1.1/example/build/flake.nix`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/example/fib.py` & `entoli-0.1.1/example/fib.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/example/nix_shell.py` & `entoli-0.1.1/example/nix_shell.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/example/shell.py` & `entoli-0.1.1/example/shell.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/pyproject.toml` & `entoli-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/requirements_dev.txt` & `entoli-0.1.1/requirements_dev.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 iniconfig==2.0.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
 jaraco.functools==4.0.1
 keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
-more-itertools==10.2.0
 nh3==0.2.17
 packaging==24.0
 pkginfo==1.10.0
 platformdirs==4.2.2
 pluggy==0.13.1
 py==1.11.0
 Pygments==2.18.0
```

### Comparing `entoli-0.1.0/src/entoli/.pytest_cache/v/cache/nodeids` & `entoli-0.1.1/src/entoli/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/base/either.py` & `entoli-0.1.1/src/entoli/base/either.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/base/io.py` & `entoli-0.1.1/src/entoli/base/io.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/base/maybe.py` & `entoli-0.1.1/src/entoli/base/maybe.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/base/result.py` & `entoli-0.1.1/src/entoli/base/result.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/base/seq.py` & `entoli-0.1.1/src/entoli/base/seq.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/base/typeclass.py` & `entoli-0.1.1/src/entoli/base/typeclass.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/prelude.py` & `entoli-0.1.1/src/entoli/prelude.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/process.py` & `entoli-0.1.1/src/entoli/process.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli/system.py` & `entoli-0.1.1/src/entoli/system.py`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/src/entoli.egg-info/PKG-INFO` & `entoli-0.1.1/src/entoli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 Metadata-Version: 2.1
 Name: entoli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python functional programming library
 Home-page: https://github.com/cwahn/entoli
 Author: Your Name
 Author-email: cwahn0904@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: attrs==23.2.0
-Requires-Dist: distlib==0.3.8
-Requires-Dist: filelock==3.14.0
-Requires-Dist: iniconfig==2.0.0
-Requires-Dist: more-itertools==10.2.0
-Requires-Dist: packaging==24.0
-Requires-Dist: platformdirs==4.2.2
-Requires-Dist: pluggy==0.13.1
-Requires-Dist: py==1.11.0
-Requires-Dist: toml==0.10.2
-Requires-Dist: virtualenv==20.26.2
-Requires-Dist: wheel==0.33.6
 Provides-Extra: dev
 Requires-Dist: attrs==23.2.0; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
 Requires-Dist: docutils==0.21.2; extra == "dev"
 Requires-Dist: filelock==3.14.0; extra == "dev"
@@ -35,15 +23,14 @@
 Requires-Dist: iniconfig==2.0.0; extra == "dev"
 Requires-Dist: jaraco.classes==3.4.0; extra == "dev"
 Requires-Dist: jaraco.context==5.3.0; extra == "dev"
 Requires-Dist: jaraco.functools==4.0.1; extra == "dev"
 Requires-Dist: keyring==25.2.1; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
-Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: packaging==24.0; extra == "dev"
 Requires-Dist: pkginfo==1.10.0; extra == "dev"
 Requires-Dist: platformdirs==4.2.2; extra == "dev"
 Requires-Dist: pluggy==0.13.1; extra == "dev"
 Requires-Dist: py==1.11.0; extra == "dev"
 Requires-Dist: Pygments==2.18.0; extra == "dev"
```

### Comparing `entoli-0.1.0/src/entoli.egg-info/SOURCES.txt` & `entoli-0.1.1/src/entoli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `entoli-0.1.0/tox.ini` & `entoli-0.1.1/tox.ini`

 * *Files identical despite different names*

