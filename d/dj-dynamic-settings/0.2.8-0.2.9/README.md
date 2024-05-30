# Comparing `tmp/dj-dynamic-settings-0.2.8.tar.gz` & `tmp/dj-dynamic-settings-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-dynamic-settings-0.2.8.tar", last modified: Tue May 28 23:11:56 2024, max compression
+gzip compressed data, was "dj-dynamic-settings-0.2.9.tar", last modified: Thu May 30 07:31:54 2024, max compression
```

## Comparing `dj-dynamic-settings-0.2.8.tar` & `dj-dynamic-settings-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:11:56.728675 dj-dynamic-settings-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)     1311 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     4866 2024-05-28 23:11:56.728675 dj-dynamic-settings-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3305 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:11:56.724675 dj-dynamic-settings-0.2.8/dj_dynamic_settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/compat.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/metadata.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:11:56.724675 dj-dynamic-settings-0.2.8/dj_dynamic_settings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/serializers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:11:56.728675 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_dynamic_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_override_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4014 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings/views.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 23:11:56.724675 dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4866 2024-05-28 23:11:56.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-28 23:11:56.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 23:11:56.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 23:11:56.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-28 23:11:56.000000 dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 23:11:56.728675 dj-dynamic-settings-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2024-05-28 23:11:26.000000 dj-dynamic-settings-0.2.8/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3305 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/dj_dynamic_settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/metadata.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/dj_dynamic_settings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/serializers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_dynamic_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_override_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4014 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-30 07:31:54.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-30 07:31:54.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 07:31:54.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 07:31:54.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-30 07:31:54.000000 dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-30 07:31:54.967398 dj-dynamic-settings-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-30 07:31:29.000000 dj-dynamic-settings-0.2.9/tox.ini
```

### Comparing `dj-dynamic-settings-0.2.8/.gitignore` & `dj-dynamic-settings-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/LICENSE.txt` & `dj-dynamic-settings-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/PKG-INFO` & `dj-dynamic-settings-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.8
+Version: 0.2.9
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
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

### Comparing `dj-dynamic-settings-0.2.8/README.md` & `dj-dynamic-settings-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/bitbucket-pipelines.yml` & `dj-dynamic-settings-0.2.9/bitbucket-pipelines.yml`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,23 @@
           image: python:3.10-alpine
           script:
             - apk add postgresql-dev gcc git python3-dev musl-dev
             - pip install tox
             - tox -e py310-django40,py310-django41,py310-django42
           services:
             - postgres
+      - step:
+          name: py311
+          image: python:3.11-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py311-django42
+          services:
+            - postgres
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.8-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
```

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/app_settings.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/app_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/compat.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/compat.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/conf.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/conf.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/metadata.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/metadata.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/migrations/0001_initial.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/models.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/models.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/registry.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/registry.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/serializers.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/definitions.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_dynamic_settings.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_override_settings.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_override_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_settings.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/tests/test_views.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/utils.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/validators.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/validators.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings/views.py` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings/views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/PKG-INFO` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.8
+Version: 0.2.9
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
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

### Comparing `dj-dynamic-settings-0.2.8/dj_dynamic_settings.egg-info/SOURCES.txt` & `dj-dynamic-settings-0.2.9/dj_dynamic_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.8/setup.py` & `dj-dynamic-settings-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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

### Comparing `dj-dynamic-settings-0.2.8/tox.ini` & `dj-dynamic-settings-0.2.9/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
           {py36,py37}-{django111,django20,django21,django22,django30,django31,django32}
           py38-{django22,django30,django31,django32, django40, django41, django42}
           py39-{django32,django40,django41,django42}
           py310-{django32,django40,django41,django42}
+          py311-{django42}
           linting
 
 [testenv]
 deps = django110: Django>=1.10,<1.11
        django111: Django>=1.11.7,<2.0
        django20: Django>=2.0,<2.1
        django21: Django>=2.1,<2.2
@@ -32,11 +33,11 @@
        pytz
        mock
 commands = python runtests.py
 
 [testenv:linting]
 deps = black
        isort==5.0.4
-       Django>=2.2.8,<3.0
+       Django>=2.2.8,<5.0
        djangorestframework<3.15
 commands = black --check --quiet --exclude=migrations/ dj_dynamic_settings
            isort -c --skip=migrations dj_dynamic_settings
```

