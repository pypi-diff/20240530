# Comparing `tmp/django-lineup-0.3.1.tar.gz` & `tmp/django-lineup-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lineup-0.3.1.tar", last modified: Thu Dec 22 10:59:10 2022, max compression
+gzip compressed data, was "django-lineup-0.3.2.tar", last modified: Thu May 30 08:48:02 2024, max compression
```

## Comparing `django-lineup-0.3.1.tar` & `django-lineup-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      150 2022-12-22 10:51:04.000000 django-lineup-0.3.1/AUTHORS.rst
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     3237 2022-12-22 10:51:04.000000 django-lineup-0.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      533 2022-12-22 10:58:02.000000 django-lineup-0.3.1/HISTORY.rst
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     1071 2022-12-22 10:51:04.000000 django-lineup-0.3.1/LICENSE
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      174 2022-12-22 10:51:04.000000 django-lineup-0.3.1/MANIFEST.in
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     6039 2022-12-22 10:59:10.342905 django-lineup-0.3.1/PKG-INFO
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     4515 2022-12-22 10:51:04.000000 django-lineup-0.3.1/README.rst
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.338905 django-lineup-0.3.1/django_lineup.egg-info/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     6039 2022-12-22 10:59:10.000000 django-lineup-0.3.1/django_lineup.egg-info/PKG-INFO
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      836 2022-12-22 10:59:10.000000 django-lineup-0.3.1/django_lineup.egg-info/SOURCES.txt
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        1 2022-12-22 10:59:10.000000 django-lineup-0.3.1/django_lineup.egg-info/dependency_links.txt
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        1 2022-12-22 10:59:10.000000 django-lineup-0.3.1/django_lineup.egg-info/not-zip-safe
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)       12 2022-12-22 10:59:10.000000 django-lineup-0.3.1/django_lineup.egg-info/requires.txt
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        7 2022-12-22 10:59:10.000000 django-lineup-0.3.1/django_lineup.egg-info/top_level.txt
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)       22 2022-12-22 10:58:02.000000 django-lineup-0.3.1/lineup/__init__.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     2056 2022-12-22 10:57:30.000000 django-lineup-0.3.1/lineup/admin.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      191 2022-12-22 10:57:30.000000 django-lineup-0.3.1/lineup/apps.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      141 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/exceptions.py
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.338905 django-lineup-0.3.1/lineup/management/
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/management/commands/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     1024 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/management/commands/import_menu_from_json.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      175 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/managers.py
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/migrations/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     2035 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/migrations/0001_initial.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      883 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/migrations/0002_auto_20201213_0856.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      502 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/migrations/0003_menuitem_extras.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/migrations/__init__.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     4043 2022-12-22 10:57:30.000000 django-lineup-0.3.1/lineup/models.py
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.338905 django-lineup-0.3.1/lineup/static/
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/static/css/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/static/css/lineup.css
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/static/js/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/static/js/lineup.js
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.338905 django-lineup-0.3.1/lineup/templates/
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/templates/lineup/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      661 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/templates/lineup/base.html
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      327 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/templates/lineup/breadcrumbs.html
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      887 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/templates/lineup/menu.html
-drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:59:10.342905 django-lineup-0.3.1/lineup/templatetags/
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     4520 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/templatetags/lineup_tags.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)       24 2022-12-22 10:51:04.000000 django-lineup-0.3.1/lineup/views.py
--rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      283 2022-12-22 10:59:10.342905 django-lineup-0.3.1/setup.cfg
--rwxrwxr-x   0 abidibo   (1000) abidibo   (1000)     2507 2022-12-22 10:51:04.000000 django-lineup-0.3.1/setup.py
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      150 2022-12-22 10:51:04.000000 django-lineup-0.3.2/AUTHORS.rst
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     3237 2022-12-22 10:51:04.000000 django-lineup-0.3.2/CONTRIBUTING.rst
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      605 2024-05-30 08:41:17.000000 django-lineup-0.3.2/HISTORY.rst
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     1071 2022-12-22 10:51:04.000000 django-lineup-0.3.2/LICENSE
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      174 2022-12-22 10:51:04.000000 django-lineup-0.3.2/MANIFEST.in
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     6277 2024-05-30 08:48:02.909605 django-lineup-0.3.2/PKG-INFO
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     4681 2024-05-30 08:40:41.000000 django-lineup-0.3.2/README.rst
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/django_lineup.egg-info/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     6277 2024-05-30 08:48:02.000000 django-lineup-0.3.2/django_lineup.egg-info/PKG-INFO
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      907 2024-05-30 08:48:02.000000 django-lineup-0.3.2/django_lineup.egg-info/SOURCES.txt
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        1 2024-05-30 08:48:02.000000 django-lineup-0.3.2/django_lineup.egg-info/dependency_links.txt
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        1 2024-05-30 08:48:02.000000 django-lineup-0.3.2/django_lineup.egg-info/not-zip-safe
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)       12 2024-05-30 08:48:02.000000 django-lineup-0.3.2/django_lineup.egg-info/requires.txt
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        7 2024-05-30 08:48:02.000000 django-lineup-0.3.2/django_lineup.egg-info/top_level.txt
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)       22 2024-05-30 08:41:17.000000 django-lineup-0.3.2/lineup/__init__.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     2124 2024-05-30 08:40:41.000000 django-lineup-0.3.2/lineup/admin.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      191 2022-12-22 10:57:30.000000 django-lineup-0.3.2/lineup/apps.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      141 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/exceptions.py
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.905605 django-lineup-0.3.2/lineup/management/
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/management/commands/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     1024 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/management/commands/import_menu_from_json.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      175 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/managers.py
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/migrations/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     2035 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/migrations/0001_initial.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      883 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/migrations/0002_auto_20201213_0856.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      502 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/migrations/0003_menuitem_extras.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/migrations/__init__.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     4043 2022-12-22 10:57:30.000000 django-lineup-0.3.2/lineup/models.py
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.905605 django-lineup-0.3.2/lineup/static/
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/static/css/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/static/css/lineup.css
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/static/js/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)        0 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/static/js/lineup.js
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.905605 django-lineup-0.3.2/lineup/templates/
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.905605 django-lineup-0.3.2/lineup/templates/admin/
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.905605 django-lineup-0.3.2/lineup/templates/admin/lineup/
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/templates/admin/lineup/menuitem/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      515 2024-05-30 08:40:41.000000 django-lineup-0.3.2/lineup/templates/admin/lineup/menuitem/change_list.html
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/templates/lineup/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      661 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/templates/lineup/base.html
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      327 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/templates/lineup/breadcrumbs.html
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      887 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/templates/lineup/menu.html
+drwxrwxr-x   0 abidibo   (1000) abidibo   (1000)        0 2024-05-30 08:48:02.909605 django-lineup-0.3.2/lineup/templatetags/
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)     4520 2022-12-22 10:51:04.000000 django-lineup-0.3.2/lineup/templatetags/lineup_tags.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      152 2024-05-30 08:40:41.000000 django-lineup-0.3.2/lineup/urls.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      299 2024-05-30 08:40:41.000000 django-lineup-0.3.2/lineup/views.py
+-rw-rw-r--   0 abidibo   (1000) abidibo   (1000)      283 2024-05-30 08:48:02.909605 django-lineup-0.3.2/setup.cfg
+-rwxrwxr-x   0 abidibo   (1000) abidibo   (1000)     2507 2022-12-22 10:51:04.000000 django-lineup-0.3.2/setup.py
```

### Comparing `django-lineup-0.3.1/CONTRIBUTING.rst` & `django-lineup-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/HISTORY.rst` & `django-lineup-0.3.2/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+0.3.2 (2024-05-30)
+++++++++++++++++++
+
+* Adds rebuild command in admin
+
 0.3.1 (2022-12-22)
 ++++++++++++++++++
 
 * Adds Dajngo 4 support
 
 0.3.0 (2021-04-27)
 ++++++++++++++++++
```

### Comparing `django-lineup-0.3.1/LICENSE` & `django-lineup-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/PKG-INFO` & `django-lineup-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lineup
-Version: 0.3.1
+Version: 0.3.2
 Summary: Navigation system for django sites
 Home-page: https://github.com/otto-torino/django-lineup
 Author: abidibo
 Author-email: abidibo@gmail.com
 License: MIT
 Project-URL: Documentation, https://django-lineup.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/otto-torino/django-lineup
@@ -61,14 +61,22 @@
 
     INSTALLED_APPS = (
         ...
         'lineup.apps.LineupConfig',
         ...
     )
 
+Add to your main `urls.py`:
+
+.. code-block:: python
+
+    ...
+    path("lineup/", include("lineup.urls", namespace="lineup")),
+    ...
+
 Make sure the ``requests`` context processor is included (it is by default):
 
 .. code-block:: python
 
     TEMPLATES = [
       {
         'OPTIONS': {
@@ -156,14 +164,15 @@
 --------
 
 - Multiple menus supported
 - Visibility logic: login required / permissions
 - Render menu tree templatetags
 - Breadcrumbs templetetag
 - Import a menu from json management command
+- Rebuild tree button in admin
 - `Django Baton <https://github.com/otto-torino/django-baton>`_ integration to highlight different menu in the admin
 
 Running Tests
 -------------
 
 Does the code actually work?
 
@@ -225,14 +234,19 @@
 
 
 
 
 History
 -------
 
+0.3.2 (2024-05-30)
+++++++++++++++++++
+
+* Adds rebuild command in admin
+
 0.3.1 (2022-12-22)
 ++++++++++++++++++
 
 * Adds Dajngo 4 support
 
 0.3.0 (2021-04-27)
 ++++++++++++++++++
```

### Comparing `django-lineup-0.3.1/README.rst` & `django-lineup-0.3.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,22 @@
 
     INSTALLED_APPS = (
         ...
         'lineup.apps.LineupConfig',
         ...
     )
 
+Add to your main `urls.py`:
+
+.. code-block:: python
+
+    ...
+    path("lineup/", include("lineup.urls", namespace="lineup")),
+    ...
+
 Make sure the ``requests`` context processor is included (it is by default):
 
 .. code-block:: python
 
     TEMPLATES = [
       {
         'OPTIONS': {
@@ -130,14 +138,15 @@
 --------
 
 - Multiple menus supported
 - Visibility logic: login required / permissions
 - Render menu tree templatetags
 - Breadcrumbs templetetag
 - Import a menu from json management command
+- Rebuild tree button in admin
 - `Django Baton <https://github.com/otto-torino/django-baton>`_ integration to highlight different menu in the admin
 
 Running Tests
 -------------
 
 Does the code actually work?
```

### Comparing `django-lineup-0.3.1/django_lineup.egg-info/PKG-INFO` & `django-lineup-0.3.2/django_lineup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lineup
-Version: 0.3.1
+Version: 0.3.2
 Summary: Navigation system for django sites
 Home-page: https://github.com/otto-torino/django-lineup
 Author: abidibo
 Author-email: abidibo@gmail.com
 License: MIT
 Project-URL: Documentation, https://django-lineup.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/otto-torino/django-lineup
@@ -61,14 +61,22 @@
 
     INSTALLED_APPS = (
         ...
         'lineup.apps.LineupConfig',
         ...
     )
 
+Add to your main `urls.py`:
+
+.. code-block:: python
+
+    ...
+    path("lineup/", include("lineup.urls", namespace="lineup")),
+    ...
+
 Make sure the ``requests`` context processor is included (it is by default):
 
 .. code-block:: python
 
     TEMPLATES = [
       {
         'OPTIONS': {
@@ -156,14 +164,15 @@
 --------
 
 - Multiple menus supported
 - Visibility logic: login required / permissions
 - Render menu tree templatetags
 - Breadcrumbs templetetag
 - Import a menu from json management command
+- Rebuild tree button in admin
 - `Django Baton <https://github.com/otto-torino/django-baton>`_ integration to highlight different menu in the admin
 
 Running Tests
 -------------
 
 Does the code actually work?
 
@@ -225,14 +234,19 @@
 
 
 
 
 History
 -------
 
+0.3.2 (2024-05-30)
+++++++++++++++++++
+
+* Adds rebuild command in admin
+
 0.3.1 (2022-12-22)
 ++++++++++++++++++
 
 * Adds Dajngo 4 support
 
 0.3.0 (2021-04-27)
 ++++++++++++++++++
```

### Comparing `django-lineup-0.3.1/django_lineup.egg-info/SOURCES.txt` & `django-lineup-0.3.2/django_lineup.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 django_lineup.egg-info/top_level.txt
 lineup/__init__.py
 lineup/admin.py
 lineup/apps.py
 lineup/exceptions.py
 lineup/managers.py
 lineup/models.py
+lineup/urls.py
 lineup/views.py
 lineup/management/commands/import_menu_from_json.py
 lineup/migrations/0001_initial.py
 lineup/migrations/0002_auto_20201213_0856.py
 lineup/migrations/0003_menuitem_extras.py
 lineup/migrations/__init__.py
 lineup/static/css/lineup.css
 lineup/static/js/lineup.js
+lineup/templates/admin/lineup/menuitem/change_list.html
 lineup/templates/lineup/base.html
 lineup/templates/lineup/breadcrumbs.html
 lineup/templates/lineup/menu.html
 lineup/templatetags/lineup_tags.py
```

### Comparing `django-lineup-0.3.1/lineup/admin.py` & `django-lineup-0.3.2/lineup/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     extra = 1
     classes = ('collapse-entry', 'expand-first', )
     prepopulated_fields = {'slug': ('label',)}
 
 
 @admin.register(MenuItem)
 class MenuItemAdmin(MPTTModelAdmin):
+    change_list_template = "admin/lineup/menuitem/change_list.html"
     list_display = ('slug', 'label', 'parent', 'link', 'order', 'login_required', 'enabled', )
     list_filter = (('parent', RelatedDropdownFilter, ) if baton else 'parent', 'enabled', 'login_required', )
     list_editable = ('order', )
     search_fields = ('label', )
     filter_horizontal = ('permissions', )
     inlines = [MenuItemInline, ]
     prepopulated_fields = {'slug': ('label',)}
```

### Comparing `django-lineup-0.3.1/lineup/management/commands/import_menu_from_json.py` & `django-lineup-0.3.2/lineup/management/commands/import_menu_from_json.py`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/lineup/migrations/0001_initial.py` & `django-lineup-0.3.2/lineup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/lineup/migrations/0002_auto_20201213_0856.py` & `django-lineup-0.3.2/lineup/migrations/0002_auto_20201213_0856.py`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/lineup/models.py` & `django-lineup-0.3.2/lineup/models.py`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/lineup/templates/lineup/base.html` & `django-lineup-0.3.2/lineup/templates/lineup/base.html`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/lineup/templates/lineup/menu.html` & `django-lineup-0.3.2/lineup/templates/lineup/menu.html`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/lineup/templatetags/lineup_tags.py` & `django-lineup-0.3.2/lineup/templatetags/lineup_tags.py`

 * *Files identical despite different names*

### Comparing `django-lineup-0.3.1/setup.py` & `django-lineup-0.3.2/setup.py`

 * *Files identical despite different names*

