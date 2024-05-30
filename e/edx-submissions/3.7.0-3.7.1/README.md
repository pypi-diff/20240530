# Comparing `tmp/edx-submissions-3.7.0.tar.gz` & `tmp/edx_submissions-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-submissions-3.7.0.tar", last modified: Mon Apr  1 14:54:04 2024, max compression
+gzip compressed data, was "edx_submissions-3.7.1.tar", last modified: Thu May 30 01:55:16 2024, max compression
```

## Comparing `edx-submissions-3.7.0.tar` & `edx_submissions-3.7.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/edx_submissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.951906 edx-submissions-3.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    39466 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/commands/analyze_uploaded_file_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/commands/update_submissions_uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0002_auto_20151119_0913.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0002_team_submission_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0003_ensure_ascii.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0003_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0004_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18543 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/team_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.258397 edx_submissions-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 01:55:16.258397 edx_submissions-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.258397 edx_submissions-3.7.1/edx_submissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 01:55:16.000000 edx_submissions-3.7.1/edx_submissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-30 01:55:16.000000 edx_submissions-3.7.1/edx_submissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:55:16.000000 edx_submissions-3.7.1/edx_submissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 01:55:16.000000 edx_submissions-3.7.1/edx_submissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 01:55:16.000000 edx_submissions-3.7.1/edx_submissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.254397 edx_submissions-3.7.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-30 01:55:16.258397 edx_submissions-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.254397 edx_submissions-3.7.1/submissions/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39466 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.254397 edx_submissions-3.7.1/submissions/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.254397 edx_submissions-3.7.1/submissions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/management/commands/analyze_uploaded_file_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/management/commands/update_submissions_uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:16.258397 edx_submissions-3.7.1/submissions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0002_auto_20151119_0913.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0002_team_submission_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0003_ensure_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0003_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0004_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18543 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/team_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-30 01:55:09.000000 edx_submissions-3.7.1/submissions/views.py
```

### Comparing `edx-submissions-3.7.0/LICENSE.txt` & `edx_submissions-3.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/PKG-INFO` & `edx_submissions-3.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.7.0
+Version: 3.7.1
 Summary: An API for creating submissions and scores.
 Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
+Requires-Dist: Django
 Requires-Dist: django-model-utils
+Requires-Dist: djangorestframework
+Requires-Dist: edx-django-release-util
 Requires-Dist: jsonfield
-Requires-Dist: Django
 Requires-Dist: pytz
-Requires-Dist: djangorestframework
 
 An API for creating and scoring submissions for the Open edX platform
```

### Comparing `edx-submissions-3.7.0/README.rst` & `edx_submissions-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/edx_submissions.egg-info/PKG-INFO` & `edx_submissions-3.7.1/edx_submissions.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.7.0
+Version: 3.7.1
 Summary: An API for creating submissions and scores.
 Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
+Requires-Dist: Django
 Requires-Dist: django-model-utils
+Requires-Dist: djangorestframework
+Requires-Dist: edx-django-release-util
 Requires-Dist: jsonfield
-Requires-Dist: Django
 Requires-Dist: pytz
-Requires-Dist: djangorestframework
 
 An API for creating and scoring submissions for the Open edX platform
```

### Comparing `edx-submissions-3.7.0/edx_submissions.egg-info/SOURCES.txt` & `edx_submissions-3.7.1/edx_submissions.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 edx_submissions.egg-info/PKG-INFO
 edx_submissions.egg-info/SOURCES.txt
 edx_submissions.egg-info/dependency_links.txt
 edx_submissions.egg-info/requires.txt
 edx_submissions.egg-info/top_level.txt
 requirements/base.in
+requirements/constraints.txt
 requirements/docs.in
 requirements/test.in
 submissions/__init__.py
 submissions/admin.py
 submissions/api.py
 submissions/errors.py
 submissions/models.py
```

### Comparing `edx-submissions-3.7.0/submissions/admin.py` & `edx_submissions-3.7.1/submissions/admin.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/api.py` & `edx_submissions-3.7.1/submissions/api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/errors.py` & `edx_submissions-3.7.1/submissions/errors.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/management/commands/analyze_uploaded_file_sizes.py` & `edx_submissions-3.7.1/submissions/management/commands/analyze_uploaded_file_sizes.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/management/commands/update_submissions_uuids.py` & `edx_submissions-3.7.1/submissions/management/commands/update_submissions_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/migrations/0001_initial.py` & `edx_submissions-3.7.1/submissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py` & `edx_submissions-3.7.1/submissions/migrations/0001_squashed_0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/migrations/0002_auto_20151119_0913.py` & `edx_submissions-3.7.1/submissions/migrations/0002_auto_20151119_0913.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/migrations/0002_team_submission_optional.py` & `edx_submissions-3.7.1/submissions/migrations/0002_team_submission_optional.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/migrations/0005_CreateTeamModel.py` & `edx_submissions-3.7.1/submissions/migrations/0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/models.py` & `edx_submissions-3.7.1/submissions/models.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/serializers.py` & `edx_submissions-3.7.1/submissions/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/team_api.py` & `edx_submissions-3.7.1/submissions/team_api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.7.0/submissions/views.py` & `edx_submissions-3.7.1/submissions/views.py`

 * *Files identical despite different names*

