# Comparing `tmp/django_lucide_icons-0.1.0.tar.gz` & `tmp/django_lucide_icons-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lucide_icons-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_lucide_icons-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_lucide_icons-0.1.0.tar` & `django_lucide_icons-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2024-05-30 14:15:08.953376 django_lucide_icons-0.1.0/LICENSE
--rw-r--r--   0        0        0     1083 2024-05-30 19:34:03.489281 django_lucide_icons-0.1.0/README.md
--rw-r--r--   0        0        0       48 2024-05-30 16:51:21.280344 django_lucide_icons-0.1.0/django_lucide_icons/__init__.py
--rw-r--r--   0        0        0      443 2024-05-30 19:40:26.306900 django_lucide_icons-0.1.0/django_lucide_icons/apps.py
--rw-r--r--   0        0        0        0 2024-05-30 15:49:07.177580 django_lucide_icons-0.1.0/django_lucide_icons/templatetags/__init__.py
--rw-r--r--   0        0        0     1347 2024-05-30 16:50:35.449349 django_lucide_icons-0.1.0/django_lucide_icons/templatetags/lucide_tags.py
--rw-r--r--   0        0        0      796 2024-05-30 19:40:06.321480 django_lucide_icons-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1511 1970-01-01 00:00:00.000000 django_lucide_icons-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-30 14:15:08.953376 django_lucide_icons-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1205 2024-05-30 19:42:39.271128 django_lucide_icons-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2024-05-30 19:42:25.322668 django_lucide_icons-0.1.1/django_lucide_icons/__init__.py
+-rw-r--r--   0        0        0      443 2024-05-30 19:40:26.306900 django_lucide_icons-0.1.1/django_lucide_icons/apps.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:49:07.177580 django_lucide_icons-0.1.1/django_lucide_icons/templatetags/__init__.py
+-rw-r--r--   0        0        0     1347 2024-05-30 16:50:35.449349 django_lucide_icons-0.1.1/django_lucide_icons/templatetags/lucide_tags.py
+-rw-r--r--   0        0        0      796 2024-05-30 19:40:06.321480 django_lucide_icons-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 django_lucide_icons-0.1.1/PKG-INFO
```

### Comparing `django_lucide_icons-0.1.0/LICENSE` & `django_lucide_icons-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lucide_icons-0.1.0/README.md` & `django_lucide_icons-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,41 @@
 
 To install the package, simply run:
 
 ```bash
 pip install django-lucide-icons
 ```
 
+Then add
+
+```python
+INSTALLED_APPS = [
+    # ...
+    "lucide_icons",
+]
+```
+
+to your Django project's settings.py file.
+
 ## Usage
 
 To use the template tag, add the following line to your Django project's settings.py file:
 
 ```python
 LUCIDE_ICONS_DIR = "/path/to/your/icons/directory"
 ```
 
 The LUCIDE_ICONS_DIR variable should be set to the directory where you want to store the Lucide icons.
 
 Then, you can use the `lucide` template tag in your Django templates to display Lucide icons. For example, to display the "home" icon, you can use the following code:
 
 ```html
-{% load lucide_tags %} {% lucide "home" %}
+{% load lucide_tags %} 
+
+{% lucide "home" %}
 ```
 
 The `lucide` template tag takes a single argument, which is the name of the Lucide icon you want to display.
 It returns the SVG code of the icon as a string.
 
 Since the plain SVG is rendered, it might make sense to wrap it in a "span" or "div" element to
 size it properly.
```

### Comparing `django_lucide_icons-0.1.0/django_lucide_icons/templatetags/lucide_tags.py` & `django_lucide_icons-0.1.1/django_lucide_icons/templatetags/lucide_tags.py`

 * *Files identical despite different names*

### Comparing `django_lucide_icons-0.1.0/pyproject.toml` & `django_lucide_icons-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_lucide_icons-0.1.0/PKG-INFO` & `django_lucide_icons-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lucide-icons
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django Lucide Icons
 Author-email: Fabian Binz <fabian.binz@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: uv ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
@@ -19,28 +19,41 @@
 
 To install the package, simply run:
 
 ```bash
 pip install django-lucide-icons
 ```
 
+Then add
+
+```python
+INSTALLED_APPS = [
+    # ...
+    "lucide_icons",
+]
+```
+
+to your Django project's settings.py file.
+
 ## Usage
 
 To use the template tag, add the following line to your Django project's settings.py file:
 
 ```python
 LUCIDE_ICONS_DIR = "/path/to/your/icons/directory"
 ```
 
 The LUCIDE_ICONS_DIR variable should be set to the directory where you want to store the Lucide icons.
 
 Then, you can use the `lucide` template tag in your Django templates to display Lucide icons. For example, to display the "home" icon, you can use the following code:
 
 ```html
-{% load lucide_tags %} {% lucide "home" %}
+{% load lucide_tags %} 
+
+{% lucide "home" %}
 ```
 
 The `lucide` template tag takes a single argument, which is the name of the Lucide icon you want to display.
 It returns the SVG code of the icon as a string.
 
 Since the plain SVG is rendered, it might make sense to wrap it in a "span" or "div" element to
 size it properly.
```

