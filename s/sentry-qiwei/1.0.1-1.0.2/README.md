# Comparing `tmp/sentry_qiwei-1.0.1.tar.gz` & `tmp/sentry_qiwei-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_qiwei-1.0.1.tar", last modified: Thu May 30 09:03:12 2024, max compression
+gzip compressed data, was "sentry_qiwei-1.0.2.tar", last modified: Thu May 30 09:32:16 2024, max compression
```

## Comparing `sentry_qiwei-1.0.1.tar` & `sentry_qiwei-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 well       (501) staff       (20)        0 2024-05-30 09:03:12.437450 sentry_qiwei-1.0.1/
--rw-rw-r--   0 well       (501) staff       (20)    35149 2020-06-30 13:31:52.000000 sentry_qiwei-1.0.1/LICENSE
--rw-r--r--   0 well       (501) staff       (20)     1266 2024-05-30 09:03:12.437196 sentry_qiwei-1.0.1/PKG-INFO
--rw-r--r--   0 well       (501) staff       (20)      574 2024-05-30 08:32:56.000000 sentry_qiwei-1.0.1/README.md
--rw-r--r--   0 well       (501) staff       (20)       38 2024-05-30 09:03:12.437496 sentry_qiwei-1.0.1/setup.cfg
--rw-r--r--   0 well       (501) staff       (20)     1724 2024-05-30 08:32:56.000000 sentry_qiwei-1.0.1/setup.py
-drwxr-xr-x   0 well       (501) staff       (20)        0 2024-05-30 09:03:12.433909 sentry_qiwei-1.0.1/src/
-drwxr-xr-x   0 well       (501) staff       (20)        0 2024-05-30 09:03:12.435454 sentry_qiwei-1.0.1/src/sentry_qiwei/
--rw-r--r--   0 well       (501) staff       (20)      232 2024-05-30 08:32:56.000000 sentry_qiwei-1.0.1/src/sentry_qiwei/__init__.py
--rw-r--r--   0 well       (501) staff       (20)      206 2024-05-30 08:32:56.000000 sentry_qiwei-1.0.1/src/sentry_qiwei/forms.py
--rw-r--r--   0 well       (501) staff       (20)     2476 2024-05-30 08:32:56.000000 sentry_qiwei-1.0.1/src/sentry_qiwei/plugin.py
-drwxr-xr-x   0 well       (501) staff       (20)        0 2024-05-30 09:03:12.436939 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/
--rw-r--r--   0 well       (501) staff       (20)     1266 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/PKG-INFO
--rw-r--r--   0 well       (501) staff       (20)      389 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/SOURCES.txt
--rw-r--r--   0 well       (501) staff       (20)        1 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/dependency_links.txt
--rw-r--r--   0 well       (501) staff       (20)       67 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/entry_points.txt
--rw-r--r--   0 well       (501) staff       (20)        1 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/not-zip-safe
--rw-r--r--   0 well       (501) staff       (20)       23 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/requires.txt
--rw-r--r--   0 well       (501) staff       (20)       13 2024-05-30 09:03:12.000000 sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.187790 sentry_qiwei-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 09:32:16.187790 sentry_qiwei-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:32:16.187790 sentry_qiwei-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.183790 sentry_qiwei-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.183790 sentry_qiwei-1.0.2/src/sentry_qiwei/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/src/sentry_qiwei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/src/sentry_qiwei/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-30 09:32:11.000000 sentry_qiwei-1.0.2/src/sentry_qiwei/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:32:16.183790 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 09:32:16.000000 sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/top_level.txt
```

### Comparing `sentry_qiwei-1.0.1/LICENSE` & `sentry_qiwei-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_qiwei-1.0.1/PKG-INFO` & `sentry_qiwei-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-qiwei
-Version: 1.0.1
+Version: 1.0.2
 Summary: sentry extension which can send error to qiwei.
 Home-page: https://github.com/snakeliwei/sentry_qiwei
 Author: snakeliwei
 Author-email: snakeliwei@gmail.com
 License: GNU
 Keywords: sentry qiwei
 Classifier: Framework :: Django
```

### Comparing `sentry_qiwei-1.0.1/README.md` & `sentry_qiwei-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sentry_qiwei-1.0.1/setup.py` & `sentry_qiwei-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import io
 from setuptools import setup, find_packages
 
 NAME = 'sentry-qiwei'
 AUTHOR = 'snakeliwei'
 EMAIL = 'snakeliwei@gmail.com'
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'sentry extension which can send error to qiwei.'
 URL = 'https://github.com/snakeliwei/sentry_qiwei'
 LICENSE = 'GNU'
 KEYWORDS = 'sentry qiwei'
 
 INSTALL_REQUIRES = [
     'sentry',
@@ -54,15 +54,15 @@
     packages=find_packages('src'),
 
     tests_require=INSTALL_REQUIRES,
     install_requires=INSTALL_REQUIRES,
 
     entry_points={
         'sentry.plugins': [
-            'sentry_qiwei = sentry_qiwei.plugin:DingTalkPlugin'
+            'sentry_qiwei = sentry_qiwei.plugin:QiWeiPlugin'
         ]
     },
 
     classifiers=[
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `sentry_qiwei-1.0.1/src/sentry_qiwei/plugin.py` & `sentry_qiwei-1.0.2/src/sentry_qiwei/plugin.py`

 * *Files identical despite different names*

### Comparing `sentry_qiwei-1.0.1/src/sentry_qiwei.egg-info/PKG-INFO` & `sentry_qiwei-1.0.2/src/sentry_qiwei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-qiwei
-Version: 1.0.1
+Version: 1.0.2
 Summary: sentry extension which can send error to qiwei.
 Home-page: https://github.com/snakeliwei/sentry_qiwei
 Author: snakeliwei
 Author-email: snakeliwei@gmail.com
 License: GNU
 Keywords: sentry qiwei
 Classifier: Framework :: Django
```

