# Comparing `tmp/django-mellon-1.8.tar.gz` & `tmp/django-mellon-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mellon-1.8.tar", last modified: Sun Sep 22 12:54:39 2019, max compression
+gzip compressed data, was "dist/django-mellon-1.9.tar", last modified: Sat Oct  5 11:21:40 2019, max compression
```

## Comparing `django-mellon-1.8.tar` & `django-mellon-1.9.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/
--rwxr-xr-x   0 fred      (1000) fred      (1000)     3310 2019-09-22 12:45:43.000000 django-mellon-1.8/setup.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/sessions_backends/
--rw-r--r--   0 fred      (1000) fred      (1000)     1720 2019-06-25 13:16:27.000000 django-mellon-1.8/mellon/sessions_backends/db.py
--rw-r--r--   0 fred      (1000) fred      (1000)      883 2019-06-25 13:16:27.000000 django-mellon-1.8/mellon/sessions_backends/cached_db.py
--rw-r--r--   0 fred      (1000) fred      (1000)        0 2016-01-21 13:56:08.000000 django-mellon-1.8/mellon/sessions_backends/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)    26763 2019-09-22 08:32:29.000000 django-mellon-1.8/mellon/views.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/templates/
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/templates/mellon/
--rw-r--r--   0 fred      (1000) fred      (1000)      287 2015-01-17 11:03:19.000000 django-mellon-1.8/mellon/templates/mellon/user_not_found.html
--rw-r--r--   0 fred      (1000) fred      (1000)     1540 2019-03-25 13:00:35.000000 django-mellon-1.8/mellon/templates/mellon/authentication_failed.html
--rw-r--r--   0 fred      (1000) fred      (1000)      677 2014-12-09 12:45:33.000000 django-mellon-1.8/mellon/templates/mellon/session_dump.xml
--rw-r--r--   0 fred      (1000) fred      (1000)      259 2015-01-17 11:03:19.000000 django-mellon-1.8/mellon/templates/mellon/inactive_user.html
--rw-r--r--   0 fred      (1000) fred      (1000)     3812 2018-05-10 13:40:11.000000 django-mellon-1.8/mellon/templates/mellon/metadata.xml
--rw-r--r--   0 fred      (1000) fred      (1000)      206 2015-04-29 14:03:05.000000 django-mellon-1.8/mellon/templates/mellon/base.html
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/migrations/
--rw-r--r--   0 fred      (1000) fred      (1000)     1271 2019-09-22 07:46:58.000000 django-mellon-1.8/mellon/migrations/0001_initial.py
--rw-r--r--   0 fred      (1000) fred      (1000)        0 2014-12-09 12:45:33.000000 django-mellon-1.8/mellon/migrations/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3089 2019-09-22 07:46:47.000000 django-mellon-1.8/mellon/middleware.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2137 2019-06-25 13:16:27.000000 django-mellon-1.8/mellon/app_settings.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1865 2019-09-22 10:30:38.000000 django-mellon-1.8/mellon/backends.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/locale/
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/locale/fr/
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/locale/fr/LC_MESSAGES/
--rw-r--r--   0 fred      (1000) fred      (1000)     1681 2019-09-22 12:54:39.000000 django-mellon-1.8/mellon/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 fred      (1000) fred      (1000)     2372 2019-03-25 13:00:35.000000 django-mellon-1.8/mellon/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 fred      (1000) fred      (1000)      441 2019-07-11 21:26:07.000000 django-mellon-1.8/mellon/urls.py
--rw-r--r--   0 fred      (1000) fred      (1000)      223 2018-05-10 13:40:11.000000 django-mellon-1.8/mellon/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1530 2019-09-22 07:46:58.000000 django-mellon-1.8/mellon/models.py
--rw-r--r--   0 fred      (1000) fred      (1000)    10060 2019-09-22 07:46:58.000000 django-mellon-1.8/mellon/utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)    21137 2019-09-22 08:32:30.000000 django-mellon-1.8/mellon/adapters.py
--rw-r--r--   0 fred      (1000) fred      (1000)      117 2014-12-09 12:45:33.000000 django-mellon-1.8/COPYING
--rw-r--r--   0 fred      (1000) fred      (1000)     1106 2019-09-22 08:35:03.000000 django-mellon-1.8/tox.ini
--rw-r--r--   0 fred      (1000) fred      (1000)    10174 2019-09-22 09:09:33.000000 django-mellon-1.8/README
--rw-r--r--   0 fred      (1000) fred      (1000)        3 2019-09-22 12:54:39.000000 django-mellon-1.8/VERSION
--rw-r--r--   0 fred      (1000) fred      (1000)      242 2016-05-08 18:08:17.000000 django-mellon-1.8/MANIFEST.in
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/django_mellon.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)       47 2019-09-22 12:54:39.000000 django-mellon-1.8/django_mellon.egg-info/requires.txt
--rw-r--r--   0 fred      (1000) fred      (1000)        1 2019-09-22 12:54:39.000000 django-mellon-1.8/django_mellon.egg-info/dependency_links.txt
--rw-r--r--   0 fred      (1000) fred      (1000)        7 2019-09-22 12:54:39.000000 django-mellon-1.8/django_mellon.egg-info/top_level.txt
--rw-r--r--   0 fred      (1000) fred      (1000)    13093 2019-09-22 12:54:39.000000 django-mellon-1.8/django_mellon.egg-info/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)     1133 2019-09-22 12:54:39.000000 django-mellon-1.8/django_mellon.egg-info/SOURCES.txt
--rw-r--r--   0 fred      (1000) fred      (1000)     5034 2016-03-08 12:16:21.000000 django-mellon-1.8/Changelog
--rw-r--r--   0 fred      (1000) fred      (1000)     1342 2019-09-22 08:35:03.000000 django-mellon-1.8/testsettings.py
--rw-r--r--   0 fred      (1000) fred      (1000)    13093 2019-09-22 12:54:39.000000 django-mellon-1.8/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)       38 2019-09-22 12:54:39.000000 django-mellon-1.8/setup.cfg
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/tests/
--rw-r--r--   0 fred      (1000) fred      (1000)      990 2019-06-25 13:16:27.000000 django-mellon-1.8/tests/urls_tests.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4446 2019-07-11 21:26:07.000000 django-mellon-1.8/tests/test_utils.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2019-09-22 12:54:39.000000 django-mellon-1.8/tests/templates/
--rw-r--r--   0 fred      (1000) fred      (1000)       73 2016-03-12 15:47:48.000000 django-mellon-1.8/tests/templates/base.html
--rw-r--r--   0 fred      (1000) fred      (1000)    10187 2019-09-22 08:35:03.000000 django-mellon-1.8/tests/test_views.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2344 2019-06-25 13:16:27.000000 django-mellon-1.8/tests/conftest.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1261 2019-06-25 13:16:27.000000 django-mellon-1.8/tests/utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1296 2019-06-25 13:16:27.000000 django-mellon-1.8/tests/xml_utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4137 2019-04-07 18:37:59.000000 django-mellon-1.8/tests/metadata.xml
--rw-r--r--   0 fred      (1000) fred      (1000)    16087 2019-09-22 08:35:03.000000 django-mellon-1.8/tests/test_sso_slo.py
--rw-r--r--   0 fred      (1000) fred      (1000)    15976 2019-07-11 21:26:07.000000 django-mellon-1.8/tests/test_default_adapter.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    10174 2019-09-29 14:24:49.000000 django-mellon-1.9/README
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2636 2019-10-04 22:53:34.000000 django-mellon-1.9/mellon/middleware.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      441 2019-09-29 15:21:38.000000 django-mellon-1.9/mellon/urls.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    26654 2019-10-04 22:53:34.000000 django-mellon-1.9/mellon/views.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1865 2019-09-29 14:24:49.000000 django-mellon-1.9/mellon/backends.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/templates/
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/templates/mellon/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     3865 2019-10-04 15:45:25.000000 django-mellon-1.9/mellon/templates/mellon/metadata.xml
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      259 2019-03-02 13:18:08.000000 django-mellon-1.9/mellon/templates/mellon/inactive_user.html
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      206 2019-09-30 22:19:43.000000 django-mellon-1.9/mellon/templates/mellon/base.html
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1540 2019-03-19 22:44:27.000000 django-mellon-1.9/mellon/templates/mellon/authentication_failed.html
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      287 2019-03-02 13:18:08.000000 django-mellon-1.9/mellon/templates/mellon/user_not_found.html
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      677 2017-12-21 14:29:26.000000 django-mellon-1.9/mellon/templates/mellon/session_dump.xml
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    21137 2019-08-07 09:48:34.000000 django-mellon-1.9/mellon/adapters.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/migrations/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1271 2019-09-29 14:24:49.000000 django-mellon-1.9/mellon/migrations/0001_initial.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        0 2017-12-21 14:29:26.000000 django-mellon-1.9/mellon/migrations/__init__.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      223 2019-03-02 13:18:08.000000 django-mellon-1.9/mellon/__init__.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2145 2019-10-04 22:53:34.000000 django-mellon-1.9/mellon/app_settings.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/sessions_backends/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1720 2019-07-04 17:08:30.000000 django-mellon-1.9/mellon/sessions_backends/db.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-03-02 13:18:08.000000 django-mellon-1.9/mellon/sessions_backends/__init__.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      883 2019-07-04 17:08:30.000000 django-mellon-1.9/mellon/sessions_backends/cached_db.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1123 2019-10-04 22:53:34.000000 django-mellon-1.9/mellon/compat.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    10082 2019-10-04 22:53:34.000000 django-mellon-1.9/mellon/utils.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/locale/
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/locale/fr/
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1681 2019-10-05 11:21:40.000000 django-mellon-1.9/mellon/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2372 2019-03-19 22:44:27.000000 django-mellon-1.9/mellon/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1530 2019-09-29 14:24:49.000000 django-mellon-1.9/mellon/models.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       38 2019-10-05 11:21:40.000000 django-mellon-1.9/setup.cfg
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1464 2019-10-04 22:53:34.000000 django-mellon-1.9/testsettings.py
+-rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)     3310 2019-09-29 14:24:49.000000 django-mellon-1.9/setup.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/django_mellon.egg-info/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1150 2019-10-05 11:21:40.000000 django-mellon-1.9/django_mellon.egg-info/SOURCES.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       47 2019-10-05 11:21:40.000000 django-mellon-1.9/django_mellon.egg-info/requires.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    13093 2019-10-05 11:21:40.000000 django-mellon-1.9/django_mellon.egg-info/PKG-INFO
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        1 2019-10-05 11:21:40.000000 django-mellon-1.9/django_mellon.egg-info/dependency_links.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        7 2019-10-05 11:21:40.000000 django-mellon-1.9/django_mellon.egg-info/top_level.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1102 2019-10-04 15:45:25.000000 django-mellon-1.9/tox.ini
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      117 2017-12-21 14:29:26.000000 django-mellon-1.9/COPYING
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    13093 2019-10-05 11:21:40.000000 django-mellon-1.9/PKG-INFO
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/tests/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1296 2019-07-04 17:08:30.000000 django-mellon-1.9/tests/xml_utils.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    15976 2019-07-04 17:08:30.000000 django-mellon-1.9/tests/test_default_adapter.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4137 2019-06-07 19:42:16.000000 django-mellon-1.9/tests/metadata.xml
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2344 2019-07-04 17:08:30.000000 django-mellon-1.9/tests/conftest.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2019-10-05 11:21:40.000000 django-mellon-1.9/tests/templates/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       73 2019-03-02 13:18:08.000000 django-mellon-1.9/tests/templates/base.html
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    17286 2019-10-04 22:53:34.000000 django-mellon-1.9/tests/test_sso_slo.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     5580 2019-10-04 15:45:25.000000 django-mellon-1.9/tests/test_utils.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    10098 2019-10-04 22:53:34.000000 django-mellon-1.9/tests/test_views.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      975 2019-10-04 22:53:34.000000 django-mellon-1.9/tests/urls_tests.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1261 2019-07-04 17:08:30.000000 django-mellon-1.9/tests/utils.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    12238 2019-10-05 11:19:11.000000 django-mellon-1.9/Changelog
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        3 2019-10-05 11:21:40.000000 django-mellon-1.9/VERSION
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      242 2019-03-02 13:18:08.000000 django-mellon-1.9/MANIFEST.in
```

### Comparing `django-mellon-1.8/setup.py` & `django-mellon-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/sessions_backends/db.py` & `django-mellon-1.9/mellon/sessions_backends/db.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/sessions_backends/cached_db.py` & `django-mellon-1.9/mellon/sessions_backends/cached_db.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/views.py` & `django-mellon-1.9/mellon/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,29 @@
 import lasso
 import uuid
 from requests.exceptions import RequestException
 from xml.sax.saxutils import escape
 import xml.etree.ElementTree as ET
 
 
-import django
-if django.VERSION < (1, 11, 0):
-    from django.core.urlresolvers import reverse
-else:
-    from django.urls import reverse
 from django.views.generic import View
 from django.http import HttpResponseBadRequest, HttpResponseRedirect, HttpResponse
 from django.contrib import auth
 from django.conf import settings
 from django.views.decorators.csrf import csrf_exempt
 from django.shortcuts import render, resolve_url
 from django.utils.http import urlencode
 from django.utils import six
 from django.utils.encoding import force_text
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.db import transaction
 from django.utils.translation import ugettext as _
 
 from . import app_settings, utils
+from .compat import reverse
 
 RETRY_LOGIN_COOKIE = 'MELLON_RETRY_LOGIN'
 
 lasso.setFlag('thin-sessions')
 
 if six.PY3:
     def lasso_decode(x):
```

### Comparing `django-mellon-1.8/mellon/templates/mellon/authentication_failed.html` & `django-mellon-1.9/mellon/templates/mellon/authentication_failed.html`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/templates/mellon/session_dump.xml` & `django-mellon-1.9/mellon/templates/mellon/session_dump.xml`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/templates/mellon/metadata.xml` & `django-mellon-1.9/mellon/templates/mellon/metadata.xml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 <EntityDescriptor
  entityID="{{ entity_id }}"
  xmlns="urn:oasis:names:tc:SAML:2.0:metadata">
  <SPSSODescriptor
    AuthnRequestsSigned="true"
    WantAssertionsSigned="true"
    protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
+   {% if discovery_endpoint_url %}
     <Extensions>
       <idpdisc:DiscoveryResponse index="1"
         xmlns:idpdisc="urn:oasis:names:tc:SAML:profiles:SSO:idp-discovery-protocol"
         Binding="urn:oasis:names:tc:SAML:profiles:SSO:idp-discovery-protocol"
         Location="{{ discovery_endpoint_url }}"/>
-   </Extensions>
+      </Extensions>
+   {% endif %}
      {% for public_key in public_keys %}
        <KeyDescriptor>
            <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
                <ds:X509Data>
                    <ds:X509Certificate>{{ public_key }}</ds:X509Certificate>
                </ds:X509Data>
            </ds:KeyInfo>
```

### Comparing `django-mellon-1.8/mellon/migrations/0001_initial.py` & `django-mellon-1.9/mellon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/middleware.py` & `django-mellon-1.9/mellon/middleware.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import unicode_literals
 
 from django.utils.http import urlencode
 from django.http import HttpResponseRedirect
-from django.core.urlresolvers import reverse
 
 from . import app_settings, utils
+from .compat import reverse, MiddlewareClass, is_authenticated
 
 PASSIVE_TRIED_COOKIE = 'MELLON_PASSIVE_TRIED'
 
 
-class PassiveAuthenticationMiddleware(object):
+class PassiveAuthenticationMiddleware(MiddlewareClass):
     def process_response(self, request, response):
         # When unlogged remove the PASSIVE_TRIED cookie
         if app_settings.OPENED_SESSION_COOKIE_NAME \
            and PASSIVE_TRIED_COOKIE in request.COOKIES \
            and app_settings.OPENED_SESSION_COOKIE_NAME not in request.COOKIES:
             response.delete_cookie(PASSIVE_TRIED_COOKIE)
         return response
@@ -43,30 +43,23 @@
         # Skip mellon views
         if request.resolver_match.url_name and request.resolver_match.url_name.startswith('mellon_'):
             return
         if not any(utils.get_idps()):
             return
         if not app_settings.OPENED_SESSION_COOKIE_NAME:
             return
-        if hasattr(request, 'user') and request.user.is_authenticated():
+        if hasattr(request, 'user') and is_authenticated(request.user):
             return
         if PASSIVE_TRIED_COOKIE in request.COOKIES:
             return
-        if app_settings.OPENED_SESSION_COOKIE_NAME in request.COOKIES:
-            # get the common domain or guess
-            common_domain = app_settings.OPENED_SESSION_COOKIE_DOMAIN
-            if not common_domain:
-                host = request.get_host()
-                # accept automatic common domain selection if domain has at least three components
-                # and is not an IP address
-                if not host.count('.') > 1 or host.replace('.', '').isdigit():
-                    return
-                common_domain = request.get_host().split('.', 1)[1]
-            params = {
-                'next': request.build_absolute_uri(),
-                'passive': '',
-            }
-            url = reverse('mellon_login') + '?%s' % urlencode(params)
-            response = HttpResponseRedirect(url)
-            # prevent loops
-            response.set_cookie(PASSIVE_TRIED_COOKIE, value='1', max_age=None)
-            return response
+        if app_settings.OPENED_SESSION_COOKIE_NAME not in request.COOKIES:
+            return
+        # all is good, try passive login
+        params = {
+            'next': request.build_absolute_uri(),
+            'passive': '',
+        }
+        url = reverse('mellon_login') + '?%s' % urlencode(params)
+        response = HttpResponseRedirect(url)
+        # prevent loops
+        response.set_cookie(PASSIVE_TRIED_COOKIE, value='1', max_age=None)
+        return response
```

### Comparing `django-mellon-1.8/mellon/app_settings.py` & `django-mellon-1.9/mellon/app_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
         'GROUP_ATTRIBUTE': None,
         'CREATE_GROUP': True,
         'ERROR_URL': None,
         'ERROR_REDIRECT_AFTER_TIMEOUT': 120,
         'DEFAULT_ASSERTION_CONSUMER_BINDING': 'post',  # or artifact
         'VERIFY_SSL_CERTIFICATE': True,
         'OPENED_SESSION_COOKIE_NAME': None,
-        'OPENED_SESSION_COOKIE_DOMAIN': None,
         'ORGANIZATION': None,
         'CONTACT_PERSONS': [],
         'TRANSIENT_FEDERATION_ATTRIBUTE': None,
         'LOGIN_URL': 'mellon_login',
         'LOGOUT_URL': 'mellon_logout',
         'ARTIFACT_RESOLVE_TIMEOUT': 10.0,
         'LOGIN_HINTS': [],
         'SIGNATURE_METHOD': 'RSA-SHA256',
         'LOOKUP_BY_ATTRIBUTES': [],
         'METADATA_CACHE_TIME': 3600,
         'METADATA_HTTP_TIMEOUT': 10,
+        'METADATA_PUBLISH_DISCOVERY_RESPONSE': False,
     }
 
     @property
     def IDENTITY_PROVIDERS(self):
         from django.conf import settings
         try:
             idps = settings.MELLON_IDENTITY_PROVIDERS
```

### Comparing `django-mellon-1.8/mellon/backends.py` & `django-mellon-1.9/mellon/backends.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/locale/fr/LC_MESSAGES/django.mo` & `django-mellon-1.9/mellon/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/locale/fr/LC_MESSAGES/django.po` & `django-mellon-1.9/mellon/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/models.py` & `django-mellon-1.9/mellon/models.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/mellon/utils.py` & `django-mellon-1.9/mellon/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,50 +20,51 @@
 import importlib
 from functools import wraps
 import isodate
 from xml.parsers import expat
 
 import django
 from django.contrib import auth
-if django.VERSION < (1, 11, 0):
-    from django.core.urlresolvers import reverse
-else:
-    from django.urls import reverse
 from django.template.loader import render_to_string
 from django.utils.timezone import make_aware, now, make_naive, is_aware, get_default_timezone
 from django.conf import settings
 from django.utils.six.moves.urllib.parse import urlparse
 import lasso
 
 from . import app_settings
+from .compat import reverse
 
 
 def create_metadata(request):
     entity_id = reverse('mellon_metadata')
     login_url = reverse(app_settings.LOGIN_URL)
     logout_url = reverse(app_settings.LOGOUT_URL)
     public_keys = []
     for public_key in app_settings.PUBLIC_KEYS:
         if public_key.startswith('/'):
             # clean PEM file
             content = open(public_key).read()
             public_key = ''.join(content.splitlines()[1:-1])
         public_keys.append(public_key)
     name_id_formats = app_settings.NAME_ID_FORMATS
-    return render_to_string('mellon/metadata.xml', {
+    ctx = {
+        'request': request,
         'entity_id': request.build_absolute_uri(entity_id),
         'login_url': request.build_absolute_uri(login_url),
         'logout_url': request.build_absolute_uri(logout_url),
         'public_keys': public_keys,
         'name_id_formats': name_id_formats,
         'default_assertion_consumer_binding': app_settings.DEFAULT_ASSERTION_CONSUMER_BINDING,
         'organization': app_settings.ORGANIZATION,
         'contact_persons': app_settings.CONTACT_PERSONS,
-        'discovery_endpoint_url': request.build_absolute_uri(reverse('mellon_login')),
-    })
+    }
+    if app_settings.METADATA_PUBLISH_DISCOVERY_RESPONSE:
+        ctx['discovery_endpoint_url'] = request.build_absolute_uri(
+            reverse('mellon_login'))
+    return render_to_string('mellon/metadata.xml', ctx)
 
 
 def create_server(request):
     logger = logging.getLogger(__name__)
     root = request.build_absolute_uri('/')
     cache = getattr(settings, '_MELLON_SERVER_CACHE', {})
     if root not in cache:
```

### Comparing `django-mellon-1.8/mellon/adapters.py` & `django-mellon-1.9/mellon/adapters.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/tox.ini` & `django-mellon-1.9/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 deps =
   dj18: django>=1.8,<1.9
   dj111: django>=1.11,<1.12
   dj22: django>=2.2,<2.3
   pg: psycopg2
   mock
   httmock
-  pytest<4.1
+  pytest
   pytest-cov
   pytest-random
   pytest-mock
   pytest-django
   pytest-freezegun
   pytest-localserver
   pytz
```

### Comparing `django-mellon-1.8/README` & `django-mellon-1.9/README`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/django_mellon.egg-info/PKG-INFO` & `django-mellon-1.9/django_mellon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-mellon
-Version: 1.8
+Version: 1.9
 Summary: SAML 2.0 authentication for Django
 Home-page: http://dev.entrouvert.org/projects/django-mellon/
 Author: Entr'ouvert
 Author-email: info@entrouvert.org
 License: AGPLv3 or later
 Description: django-mellon
         =============
```

### Comparing `django-mellon-1.8/django_mellon.egg-info/SOURCES.txt` & `django-mellon-1.9/django_mellon.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 django_mellon.egg-info/dependency_links.txt
 django_mellon.egg-info/requires.txt
 django_mellon.egg-info/top_level.txt
 mellon/__init__.py
 mellon/adapters.py
 mellon/app_settings.py
 mellon/backends.py
+mellon/compat.py
 mellon/middleware.py
 mellon/models.py
 mellon/urls.py
 mellon/utils.py
 mellon/views.py
 mellon/locale/fr/LC_MESSAGES/django.mo
 mellon/locale/fr/LC_MESSAGES/django.po
```

### Comparing `django-mellon-1.8/testsettings.py` & `django-mellon-1.9/testsettings.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 INSTALLED_APPS = ('mellon', 'django.contrib.auth',
                   'django.contrib.contenttypes', 'django.contrib.sessions')
 if hasattr(global_settings, 'MIDDLEWARE_CLASSES'):
     MIDDLEWARE_CLASSES = global_settings.MIDDLEWARE_CLASSES
     MIDDLEWARE_CLASSES += (
         'django.contrib.sessions.middleware.SessionMiddleware',
         'django.contrib.auth.middleware.AuthenticationMiddleware',
+        'mellon.middleware.PassiveAuthenticationMiddleware',
     )
 else:
     MIDDLEWARE = global_settings.MIDDLEWARE
     MIDDLEWARE += (
         'django.contrib.sessions.middleware.SessionMiddleware',
         'django.contrib.auth.middleware.AuthenticationMiddleware',
+        'mellon.middleware.PassiveAuthenticationMiddleware',
     )
 
 AUTHENTICATION_BACKENDS = (
     'mellon.backends.SAMLBackend',
 )
 ROOT_URLCONF = 'urls_tests'
 TEMPLATE_DIRS = [
```

### Comparing `django-mellon-1.8/PKG-INFO` & `django-mellon-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-mellon
-Version: 1.8
+Version: 1.9
 Summary: SAML 2.0 authentication for Django
 Home-page: http://dev.entrouvert.org/projects/django-mellon/
 Author: Entr'ouvert
 Author-email: info@entrouvert.org
 License: AGPLv3 or later
 Description: django-mellon
         =============
```

### Comparing `django-mellon-1.8/tests/urls_tests.py` & `django-mellon-1.9/tests/urls_tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import django
-
 from django.conf.urls import url, include
 from django.http import HttpResponse
 
 
 def homepage(request):
     return HttpResponse('ok')
```

### Comparing `django-mellon-1.8/tests/test_utils.py` & `django-mellon-1.9/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,36 @@
     with mock.patch('mellon.utils.open', mock.mock_open(read_data='BEGIN\nyyy\nEND'), create=True):
         metadata = create_metadata(request)
     assert_xml_constraints(
         metadata.encode('utf-8'),
         ('/sm:EntityDescriptor[@entityID="http://testserver/metadata/"]', 1,
          ('/*', 1),
          ('/sm:SPSSODescriptor', 1,
+          ('/*', 6),
+          ('/sm:NameIDFormat', 1),
+          ('/sm:SingleLogoutService', 1),
+          ('/sm:AssertionConsumerService[@isDefault=\'true\'][@Binding=\'urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Artifact\']', 1),
+          ('/sm:AssertionConsumerService[@isDefault=\'true\'][@Binding=\'urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\']',
+           0),
+          ('/sm:AssertionConsumerService[@Binding=\'urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\']',
+           1),
+          ('/sm:KeyDescriptor/ds:KeyInfo/ds:X509Data', 2,
+           ('/ds:X509Certificate', 2),
+           ('/ds:X509Certificate[text()=\'xxx\']', 1),
+           ('/ds:X509Certificate[text()=\'yyy\']', 1)))),
+        namespaces=ns)
+
+    private_settings.MELLON_METADATA_PUBLISH_DISCOVERY_RESPONSE = True
+    with mock.patch('mellon.utils.open', mock.mock_open(read_data='BEGIN\nyyy\nEND'), create=True):
+        metadata = create_metadata(request)
+    assert_xml_constraints(
+        metadata.encode('utf-8'),
+        ('/sm:EntityDescriptor[@entityID="http://testserver/metadata/"]', 1,
+         ('/*', 1),
+         ('/sm:SPSSODescriptor', 1,
           ('/*', 7),
           ('/sm:Extensions', 1,
            ('/idpdisc:DiscoveryResponse', 1)),
           ('/sm:NameIDFormat', 1),
           ('/sm:SingleLogoutService', 1),
           ('/sm:AssertionConsumerService[@isDefault=\'true\'][@Binding=\'urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Artifact\']', 1),
           ('/sm:AssertionConsumerService[@isDefault=\'true\'][@Binding=\'urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\']',
```

### Comparing `django-mellon-1.8/tests/test_views.py` & `django-mellon-1.9/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,21 @@
 from django.utils.six.moves.urllib.parse import parse_qs, urlparse
 import base64
 import random
 import hashlib
 from httmock import HTTMock
 
 import django
-if django.VERSION >= (1, 11, 0):
-    from django.urls import reverse
-else:
-    from django.core.urlresolvers import reverse
 from django.utils.encoding import force_text
 from django.utils.http import urlencode
 
 from xml_utils import assert_xml_constraints
 
+from mellon.compat import reverse
+
 from utils import error_500, html_response
 
 pytestmark = pytest.mark.django_db
 
 
 def test_null_character_on_samlresponse_post(app):
     app.post(reverse('mellon_login'), params={'SAMLResponse': '\x00'}, status=400)
@@ -108,15 +106,15 @@
     with mock.patch('mellon.utils.open', mock.mock_open(read_data='BEGIN\nyyy\nEND'), create=True):
         response = client.get('/metadata/')
     assert_xml_constraints(
         response.content,
         ('/sm:EntityDescriptor[@entityID="http://testserver/metadata/"]', 1,
          ('/*', 4),
          ('/sm:SPSSODescriptor', 1,
-          ('/*', 7),
+          ('/*', 6),
           ('/sm:NameIDFormat', 1),
           ('/sm:SingleLogoutService', 1),
           ('/sm:AssertionConsumerService', None,
            ('[@isDefault="true"]', None,
             ('[@Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Artifact"]', 1),
             ('[@Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST"]', 0)),
            ('[@Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST"]', 1)),
```

### Comparing `django-mellon-1.8/tests/conftest.py` & `django-mellon-1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/tests/utils.py` & `django-mellon-1.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/tests/xml_utils.py` & `django-mellon-1.9/tests/xml_utils.py`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/tests/metadata.xml` & `django-mellon-1.9/tests/metadata.xml`

 * *Files identical despite different names*

### Comparing `django-mellon-1.8/tests/test_sso_slo.py` & `django-mellon-1.9/tests/test_sso_slo.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,24 @@
 import zlib
 import xml.etree.ElementTree as ET
 
 import lasso
 
 from pytest import fixture
 
-import django
-if django.VERSION >= (1, 11, 0):
-    from django.urls import reverse
-else:
-    from django.core.urlresolvers import reverse
 from django.utils import six
 from django.utils.six.moves.urllib import parse as urlparse
 from django.utils.encoding import force_str
 
 from mellon.utils import create_metadata
 
 from httmock import all_requests, HTTMock, response as mock_response
 
+from mellon.compat import reverse
+
 from utils import reset_caplog
 
 
 @fixture
 def idp_metadata():
     return open('tests/metadata.xml').read()
 
@@ -372,7 +369,35 @@
     for next_url in ['/manage/', '/admin/', '/manager/']:
         response = app.get(reverse('mellon_login') + '?next=%s' % next_url)
         url, body, relay_state = idp.process_authn_request_redirect(response['Location'])
         root = ET.fromstring(idp.request)
         login_hints = root.findall('.//{https://www.entrouvert.com/}login-hint')
         assert len(login_hints) == 1, 'missing login hint'
         assert login_hints[0].text == 'backoffice', 'login hint is not backoffice'
+
+
+def test_middleware_mixin_first_time(db, app, idp, caplog, settings):
+    settings.MELLON_OPENED_SESSION_COOKIE_NAME = 'IDP_SESSION'
+    assert 'MELLON_PASSIVE_TRIED' not in app.cookies
+    # webtest-lint is against unicode
+    app.set_cookie(str('IDP_SESSION'), str('1'))
+    response = app.get('/', status=302)
+    assert urlparse.urlparse(response.location).path == '/login/'
+    assert (urlparse.parse_qs(urlparse.urlparse(response.location).query, keep_blank_values=True)
+            == {'next': ['http://testserver/'], 'passive': ['']})
+
+    # simulate closing of session at IdP
+    app.cookiejar.clear('testserver.local', '/', 'IDP_SESSION')
+    assert 'IDP_SESSION' not in app.cookies
+
+    # verify MELLON_PASSIVE_TRIED is removed
+    assert 'MELLON_PASSIVE_TRIED' in app.cookies
+    response = app.get('/', status=200)
+    assert 'MELLON_PASSIVE_TRIED' not in app.cookies
+
+    # check passive authentication is tried again
+    app.set_cookie(str('IDP_SESSION'), str('1'))
+    response = app.get('/', status=302)
+    assert urlparse.urlparse(response.location).path == '/login/'
+    assert (urlparse.parse_qs(urlparse.urlparse(response.location).query, keep_blank_values=True)
+            == {'next': ['http://testserver/'], 'passive': ['']})
+    assert 'MELLON_PASSIVE_TRIED' in app.cookies
```

### Comparing `django-mellon-1.8/tests/test_default_adapter.py` & `django-mellon-1.9/tests/test_default_adapter.py`

 * *Files identical despite different names*

