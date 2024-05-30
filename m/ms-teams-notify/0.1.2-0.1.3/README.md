# Comparing `tmp/ms_teams_notify-0.1.2.tar.gz` & `tmp/ms_teams_notify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_teams_notify-0.1.2.tar", last modified: Thu May 30 08:47:51 2024, max compression
+gzip compressed data, was "ms_teams_notify-0.1.3.tar", last modified: Thu May 30 08:55:41 2024, max compression
```

## Comparing `ms_teams_notify-0.1.2.tar` & `ms_teams_notify-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:47:51.203509 ms_teams_notify-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 08:47:51.203509 ms_teams_notify-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:47:34.000000 ms_teams_notify-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:47:51.203509 ms_teams_notify-0.1.2/ms_teams_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 08:47:51.000000 ms_teams_notify-0.1.2/ms_teams_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 08:47:51.000000 ms_teams_notify-0.1.2/ms_teams_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:47:51.000000 ms_teams_notify-0.1.2/ms_teams_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:47:51.000000 ms_teams_notify-0.1.2/ms_teams_notify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:47:51.203509 ms_teams_notify-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-30 08:47:34.000000 ms_teams_notify-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:41.748139 ms_teams_notify-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 08:55:41.748139 ms_teams_notify-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:21.000000 ms_teams_notify-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:41.748139 ms_teams_notify-0.1.3/ms_teams_notify/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 08:55:21.000000 ms_teams_notify-0.1.3/ms_teams_notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-30 08:55:21.000000 ms_teams_notify-0.1.3/ms_teams_notify/notify_to_teams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:41.748139 ms_teams_notify-0.1.3/ms_teams_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 08:55:41.000000 ms_teams_notify-0.1.3/ms_teams_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-30 08:55:41.000000 ms_teams_notify-0.1.3/ms_teams_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:55:41.000000 ms_teams_notify-0.1.3/ms_teams_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 08:55:41.000000 ms_teams_notify-0.1.3/ms_teams_notify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:55:41.748139 ms_teams_notify-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-30 08:55:21.000000 ms_teams_notify-0.1.3/setup.py
```

### Comparing `ms_teams_notify-0.1.2/setup.py` & `ms_teams_notify-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from setuptools import find_packages, setup
 
 with open('README.md', encoding="utf-8") as fp:
     distribution = setup(
         name='ms_teams_notify',
-        version='0.1.2',
+        version='0.1.3',
         description='Notify to Microsoft Teams with Adaptive Card.',
         long_description=fp.read(),
         long_description_content_type='text/markdown',
         author='rue1-suzuki',
         author_email='suzuki.ryuichi.1998@gmail.com',
         url='https://github.com/rue1-suzuki?tab=packages',
         packages=find_packages(),
```

