# Comparing `tmp/sentry_qiwei-1.0.2.tar.gz` & `tmp/sentry_qiwei-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_qiwei-1.0.2.tar", last modified: Thu May 30 09:32:16 2024, max compression
+gzip compressed data, was "sentry_qiwei-1.0.4.tar", last modified: Thu May 30 09:47:11 2024, max compression
```

## Comparing `sentry_qiwei-1.0.2.tar` & `sentry_qiwei-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.187790 sentry_qiwei-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 09:32:16.187790 sentry_qiwei-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:32:16.187790 sentry_qiwei-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.183790 sentry_qiwei-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.183790 sentry_qiwei-1.0.2/src/sentry_qiwei/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/src/sentry_qiwei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/src/sentry_qiwei/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/src/sentry_qiwei/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.183790 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:47:11.112178 sentry_qiwei-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:47:06.000000 sentry_qiwei-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 09:47:11.112178 sentry_qiwei-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-30 09:47:06.000000 sentry_qiwei-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:47:11.112178 sentry_qiwei-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-30 09:47:06.000000 sentry_qiwei-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:47:11.108178 sentry_qiwei-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:47:11.112178 sentry_qiwei-1.0.4/src/sentry_qiwei/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:47:06.000000 sentry_qiwei-1.0.4/src/sentry_qiwei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 09:47:06.000000 sentry_qiwei-1.0.4/src/sentry_qiwei/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-30 09:47:06.000000 sentry_qiwei-1.0.4/src/sentry_qiwei/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:47:11.112178 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 09:47:11.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 09:47:11.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:47:11.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 09:47:11.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:47:10.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 09:47:11.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 09:47:11.000000 sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/top_level.txt
```

### Comparing `sentry_qiwei-1.0.2/LICENSE` & `sentry_qiwei-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_qiwei-1.0.2/PKG-INFO` & `sentry_qiwei-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-qiwei
-Version: 1.0.2
+Version: 1.0.4
 Summary: sentry extension which can send error to qiwei.
 Home-page: https://github.com/snakeliwei/sentry_qiwei
 Author: snakeliwei
 Author-email: snakeliwei@gmail.com
 License: GNU
 Keywords: sentry qiwei
 Classifier: Framework :: Django
```

### Comparing `sentry_qiwei-1.0.2/README.md` & `sentry_qiwei-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sentry_qiwei-1.0.2/setup.py` & `sentry_qiwei-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import io
 from setuptools import setup, find_packages
 
 NAME = 'sentry-qiwei'
 AUTHOR = 'snakeliwei'
 EMAIL = 'snakeliwei@gmail.com'
-VERSION = '1.0.2'
+VERSION = '1.0.4'
 DESCRIPTION = 'sentry extension which can send error to qiwei.'
 URL = 'https://github.com/snakeliwei/sentry_qiwei'
 LICENSE = 'GNU'
 KEYWORDS = 'sentry qiwei'
 
 INSTALL_REQUIRES = [
     'sentry',
```

### Comparing `sentry_qiwei-1.0.2/src/sentry_qiwei/plugin.py` & `sentry_qiwei-1.0.4/src/sentry_qiwei/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sentry_qiwei
 from .forms import QiWeiOptionsForm
 from sentry.plugins.bases.notify import NotificationPlugin
 
 QI_WEI_API = 'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={key}'
 
 
-class qiweiPlugin(NotificationPlugin):
+class QiWeiPlugin(NotificationPlugin):
     author = 'snakeliwei'
     author_url = 'https://github.com/snakeliwei/sentry_qiwei'
     description = 'sentry extension which can send error to qiwei'
     resource_links = [
         ('Source', 'https://github.com/1018ji/sentry_qiwei_xz'),
         ('Bug Tracker', 'https://github.com/snakeliwei/sentry_qiwei/issues'),
         ('README', 'https://github.com/snakeliwei/sentry_qiwei/blob/main/README.md'),
```

### Comparing `sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/PKG-INFO` & `sentry_qiwei-1.0.4/src/sentry_qiwei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-qiwei
-Version: 1.0.2
+Version: 1.0.4
 Summary: sentry extension which can send error to qiwei.
 Home-page: https://github.com/snakeliwei/sentry_qiwei
 Author: snakeliwei
 Author-email: snakeliwei@gmail.com
 License: GNU
 Keywords: sentry qiwei
 Classifier: Framework :: Django
```

