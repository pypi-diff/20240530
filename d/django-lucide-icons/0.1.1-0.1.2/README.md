# Comparing `tmp/django_lucide_icons-0.1.1.tar.gz` & `tmp/django_lucide_icons-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lucide_icons-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_lucide_icons-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_lucide_icons-0.1.1.tar` & `django_lucide_icons-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-05-30 14:15:08.953376 django_lucide_icons-0.1.1/LICENSE
--rw-r--r--   0        0        0     1205 2024-05-30 19:42:39.271128 django_lucide_icons-0.1.1/README.md
--rw-r--r--   0        0        0       48 2024-05-30 19:42:25.322668 django_lucide_icons-0.1.1/django_lucide_icons/__init__.py
--rw-r--r--   0        0        0      443 2024-05-30 19:40:26.306900 django_lucide_icons-0.1.1/django_lucide_icons/apps.py
--rw-r--r--   0        0        0        0 2024-05-30 15:49:07.177580 django_lucide_icons-0.1.1/django_lucide_icons/templatetags/__init__.py
--rw-r--r--   0        0        0     1347 2024-05-30 16:50:35.449349 django_lucide_icons-0.1.1/django_lucide_icons/templatetags/lucide_tags.py
--rw-r--r--   0        0        0      796 2024-05-30 19:40:06.321480 django_lucide_icons-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 django_lucide_icons-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-30 19:45:37.809502 django_lucide_icons-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1078 2024-05-30 14:15:08.953376 django_lucide_icons-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1205 2024-05-30 19:42:39.271128 django_lucide_icons-0.1.2/README.md
+-rw-r--r--   0        0        0       49 2024-05-30 19:50:04.118765 django_lucide_icons-0.1.2/django_lucide_icons/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-30 19:49:28.035881 django_lucide_icons-0.1.2/django_lucide_icons/apps.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:49:07.177580 django_lucide_icons-0.1.2/django_lucide_icons/templatetags/__init__.py
+-rw-r--r--   0        0        0     1195 2024-05-30 19:49:49.001547 django_lucide_icons-0.1.2/django_lucide_icons/templatetags/lucide_tags.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:20:51.794225 django_lucide_icons-0.1.2/example/__init__.py
+-rw-r--r--   0        0        0      391 2024-05-30 14:20:51.798225 django_lucide_icons-0.1.2/example/asgi.py
+-rw-r--r--   0        0        0     3224 2024-05-30 14:20:51.798225 django_lucide_icons-0.1.2/example/settings.py
+-rw-r--r--   0        0        0      763 2024-05-30 14:20:51.798225 django_lucide_icons-0.1.2/example/urls.py
+-rw-r--r--   0        0        0      391 2024-05-30 14:20:51.794225 django_lucide_icons-0.1.2/example/wsgi.py
+-rwxr-xr-x   0        0        0      663 2024-05-30 14:20:51.794225 django_lucide_icons-0.1.2/manage.py
+-rw-r--r--   0        0        0      796 2024-05-30 19:40:06.321480 django_lucide_icons-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 django_lucide_icons-0.1.2/PKG-INFO
```

### Comparing `django_lucide_icons-0.1.1/LICENSE` & `django_lucide_icons-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lucide_icons-0.1.1/README.md` & `django_lucide_icons-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_lucide_icons-0.1.1/django_lucide_icons/templatetags/lucide_tags.py` & `django_lucide_icons-0.1.2/django_lucide_icons/templatetags/lucide_tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import os
 import os.path
 import urllib.request
-from glob import glob
 
 from django import template
 from django.conf import settings
 from django.utils.safestring import mark_safe
 
-register = template.Library()
+from ..apps import cache
 
-cache = {}
-for file in glob(os.path.join(settings.LUCIDE_ICONS_DIR, "*.svg")):
-    cache[file.split("/")[-1].split(".")[0]] = mark_safe(open(file).read())
+register = template.Library()
 
 
 @register.simple_tag
 def lucide(name):
     if name in cache:
         return cache[name]
```

### Comparing `django_lucide_icons-0.1.1/pyproject.toml` & `django_lucide_icons-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_lucide_icons-0.1.1/PKG-INFO` & `django_lucide_icons-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lucide-icons
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Lucide Icons
 Author-email: Fabian Binz <fabian.binz@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: uv ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
```

