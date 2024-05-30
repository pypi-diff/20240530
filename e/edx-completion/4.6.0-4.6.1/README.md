# Comparing `tmp/edx_completion-4.6.0.tar.gz` & `tmp/edx_completion-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_completion-4.6.0.tar", last modified: Tue Apr 16 15:41:10 2024, max compression
+gzip compressed data, was "edx_completion-4.6.1.tar", last modified: Thu May 30 02:00:48 2024, max compression
```

## Comparing `edx_completion-4.6.0.tar` & `edx_completion-4.6.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-16 15:41:05.000000 edx_completion-4.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-16 15:41:05.000000 edx_completion-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 15:41:05.000000 edx_completion-4.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-16 15:41:10.539149 edx_completion-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-16 15:41:05.000000 edx_completion-4.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.535149 edx_completion-4.6.0/completion/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.535149 edx_completion-4.6.0/completion/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/0002_auto_20180125_1510.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/0003_learning_context.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/settings/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/completion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-16 15:41:05.000000 edx_completion-4.6.0/completion/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/edx_completion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 15:41:10.000000 edx_completion-4.6.0/edx_completion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:41:10.539149 edx_completion-4.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-16 15:41:05.000000 edx_completion-4.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 15:41:05.000000 edx_completion-4.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 15:41:05.000000 edx_completion-4.6.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 15:41:10.543149 edx_completion-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-16 15:41:05.000000 edx_completion-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.768524 edx_completion-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-05-30 02:00:43.000000 edx_completion-4.6.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-30 02:00:43.000000 edx_completion-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 02:00:43.000000 edx_completion-4.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-05-30 02:00:48.768524 edx_completion-4.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-30 02:00:43.000000 edx_completion-4.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.764524 edx_completion-4.6.1/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.764524 edx_completion-4.6.1/completion/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.764524 edx_completion-4.6.1/completion/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.764524 edx_completion-4.6.1/completion/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.764524 edx_completion-4.6.1/completion/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.768524 edx_completion-4.6.1/completion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/migrations/0002_auto_20180125_1510.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/migrations/0003_learning_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.768524 edx_completion-4.6.1/completion/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/settings/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.768524 edx_completion-4.6.1/completion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-30 02:00:43.000000 edx_completion-4.6.1/completion/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.768524 edx_completion-4.6.1/edx_completion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 02:00:48.000000 edx_completion-4.6.1/edx_completion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:48.768524 edx_completion-4.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-30 02:00:43.000000 edx_completion-4.6.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-30 02:00:43.000000 edx_completion-4.6.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-30 02:00:43.000000 edx_completion-4.6.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-30 02:00:48.768524 edx_completion-4.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-30 02:00:43.000000 edx_completion-4.6.1/setup.py
```

### Comparing `edx_completion-4.6.0/CHANGELOG.rst` & `edx_completion-4.6.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/LICENSE` & `edx_completion-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/PKG-INFO` & `edx_completion-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.6.0
+Version: 4.6.1
 Summary: A library for tracking completion of blocks by learners in edX courses.
 Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock>=1.2.2
 Requires-Dist: django-model-utils
 Requires-Dist: djangorestframework
 Requires-Dist: edx-drf-extensions>=1.11.0
-Requires-Dist: edx-opaque-keys
+Requires-Dist: edx-opaque-keys[django]
 Requires-Dist: edx-toggles>=1.2.0
 Requires-Dist: event-tracking
 Requires-Dist: pytz
 Requires-Dist: setuptools
 
 completion
 ##########
```

### Comparing `edx_completion-4.6.0/README.rst` & `edx_completion-4.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/api/permissions.py` & `edx_completion-4.6.1/completion/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/api/tests/test_permissions.py` & `edx_completion-4.6.1/completion/api/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/api/v1/urls.py` & `edx_completion-4.6.1/completion/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/api/v1/views.py` & `edx_completion-4.6.1/completion/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/apps.py` & `edx_completion-4.6.1/completion/apps.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/handlers.py` & `edx_completion-4.6.1/completion/handlers.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/migrations/0001_initial.py` & `edx_completion-4.6.1/completion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/migrations/0003_learning_context.py` & `edx_completion-4.6.1/completion/migrations/0003_learning_context.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/models.py` & `edx_completion-4.6.1/completion/models.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/services.py` & `edx_completion-4.6.1/completion/services.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/settings/common.py` & `edx_completion-4.6.1/completion/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/test_utils.py` & `edx_completion-4.6.1/completion/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/tests/test_models.py` & `edx_completion-4.6.1/completion/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/tests/test_services.py` & `edx_completion-4.6.1/completion/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/tests/test_utilities.py` & `edx_completion-4.6.1/completion/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/utilities.py` & `edx_completion-4.6.1/completion/utilities.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/completion/waffle.py` & `edx_completion-4.6.1/completion/waffle.py`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/edx_completion.egg-info/PKG-INFO` & `edx_completion-4.6.1/edx_completion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.6.0
+Version: 4.6.1
 Summary: A library for tracking completion of blocks by learners in edX courses.
 Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock>=1.2.2
 Requires-Dist: django-model-utils
 Requires-Dist: djangorestframework
 Requires-Dist: edx-drf-extensions>=1.11.0
-Requires-Dist: edx-opaque-keys
+Requires-Dist: edx-opaque-keys[django]
 Requires-Dist: edx-toggles>=1.2.0
 Requires-Dist: event-tracking
 Requires-Dist: pytz
 Requires-Dist: setuptools
 
 completion
 ##########
```

### Comparing `edx_completion-4.6.0/edx_completion.egg-info/SOURCES.txt` & `edx_completion-4.6.1/edx_completion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/requirements/constraints.txt` & `edx_completion-4.6.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/requirements/test.in` & `edx_completion-4.6.1/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx_completion-4.6.0/setup.py` & `edx_completion-4.6.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,46 +41,75 @@
 
     Requirements will include any constraints from files specified
     with -c in the requirements files.
     Returns a list of requirement strings.
     """
     # UPDATED VIA SEMGREP - if you need to remove/modify this method remove this line and add a comment specifying why.
 
+    # e.g. {"django": "Django", "confluent-kafka": "confluent_kafka[avro]"}
+    by_canonical_name = {}
+
+    def check_name_consistent(package):
+        """
+        Raise exception if package is named different ways.
+
+        This ensures that packages are named consistently so we can match
+        constraints to packages. It also ensures that if we require a package
+        with extras we don't constrain it without mentioning the extras (since
+        that too would interfere with matching constraints.)
+        """
+        canonical = package.lower().replace('_', '-').split('[')[0]
+        seen_spelling = by_canonical_name.get(canonical)
+        if seen_spelling is None:
+            by_canonical_name[canonical] = package
+        elif seen_spelling != package:
+            raise Exception(
+                f'Encountered both "{seen_spelling}" and "{package}" in requirements '
+                'and constraints files; please use just one or the other.'
+            )
+
     requirements = {}
     constraint_files = set()
 
-    # groups "my-package-name<=x.y.z,..." into ("my-package-name", "<=x.y.z,...")
-    requirement_line_regex = re.compile(r"([a-zA-Z0-9-_.]+)([<>=][^#\s]+)?")
+    # groups "pkg<=x.y.z,..." into ("pkg", "<=x.y.z,...")
+    re_package_name_base_chars = r"a-zA-Z0-9\-_."  # chars allowed in base package name
+    # Two groups: name[maybe,extras], and optionally a constraint
+    requirement_line_regex = re.compile(
+        r"([%s]+(?:\[[%s,\s]+\])?)([<>=][^#\s]+)?"
+        % (re_package_name_base_chars, re_package_name_base_chars)
+    )
 
     def add_version_constraint_or_raise(current_line, current_requirements, add_if_not_present):
         regex_match = requirement_line_regex.match(current_line)
         if regex_match:
             package = regex_match.group(1)
             version_constraints = regex_match.group(2)
+            check_name_consistent(package)
             existing_version_constraints = current_requirements.get(package, None)
-            # it's fine to add constraints to an unconstrained package, but raise an error if there are already
-            # constraints in place
+            # It's fine to add constraints to an unconstrained package,
+            # but raise an error if there are already constraints in place.
             if existing_version_constraints and existing_version_constraints != version_constraints:
                 raise BaseException(f'Multiple constraint definitions found for {package}:'
                                     f' "{existing_version_constraints}" and "{version_constraints}".'
                                     f'Combine constraints into one location with {package}'
                                     f'{existing_version_constraints},{version_constraints}.')
             if add_if_not_present or package in current_requirements:
                 current_requirements[package] = version_constraints
 
-    # process .in files and store the path to any constraint files that are pulled in
+    # Read requirements from .in files and store the path to any
+    # constraint files that are pulled in.
     for path in requirements_paths:
         with open(path) as reqs:
             for line in reqs:
                 if is_requirement(line):
                     add_version_constraint_or_raise(line, requirements, True)
                 if line and line.startswith('-c') and not line.startswith('-c http'):
                     constraint_files.add(os.path.dirname(path) + '/' + line.split('#')[0].replace('-c', '').strip())
 
-    # process constraint files and add any new constraints found to existing requirements
+    # process constraint files: add constraints to existing requirements
     for constraint_file in constraint_files:
         with open(constraint_file) as reader:
             for line in reader:
                 if is_requirement(line):
                     add_version_constraint_or_raise(line, requirements, False)
 
     # process back into list of pkg><=constraints strings
```

