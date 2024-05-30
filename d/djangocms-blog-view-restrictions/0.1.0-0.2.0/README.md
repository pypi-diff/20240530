# Comparing `tmp/djangocms_blog_view_restrictions-0.1.0.tar.gz` & `tmp/djangocms_blog_view_restrictions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_blog_view_restrictions-0.1.0.tar", last modified: Thu Apr 18 17:05:25 2024, max compression
+gzip compressed data, was "djangocms_blog_view_restrictions-0.2.0.tar", last modified: Thu May 30 14:21:52 2024, max compression
```

## Comparing `djangocms_blog_view_restrictions-0.1.0.tar` & `djangocms_blog_view_restrictions-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.608088 djangocms_blog_view_restrictions-0.1.0/
--rw-r--r--   0 kapt       (501) kapt        (20)       44 2024-04-18 16:26:27.000000 djangocms_blog_view_restrictions-0.1.0/AUTHORS.md
--rw-r--r--   0 kapt       (501) kapt        (20)     1280 2024-04-18 16:27:10.000000 djangocms_blog_view_restrictions-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_view_restrictions-0.1.0/LICENSE
--rw-r--r--   0 kapt       (501) kapt        (20)      181 2024-04-18 16:29:29.000000 djangocms_blog_view_restrictions-0.1.0/MANIFEST.in
--rw-r--r--   0 kapt       (501) kapt        (20)     2127 2024-04-18 17:05:25.608088 djangocms_blog_view_restrictions-0.1.0/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     1319 2024-04-18 16:55:43.000000 djangocms_blog_view_restrictions-0.1.0/README.md
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.593088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-18 12:20:57.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)      525 2024-04-18 16:56:09.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/admin.py
--rw-r--r--   0 kapt       (501) kapt        (20)      136 2024-04-18 16:44:10.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/apps.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.581088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.582088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/fr/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.600088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501) kapt        (20)      918 2024-04-18 16:53:57.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501) kapt        (20)     1602 2024-04-18 16:53:54.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.603088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/migrations/
--rw-r--r--   0 kapt       (501) kapt        (20)     2042 2024-04-18 16:33:26.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-18 14:41:10.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/migrations/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1260 2024-04-18 16:56:09.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/models.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.605088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/templatetags/
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-18 14:22:52.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/templatetags/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)      598 2024-04-18 16:56:09.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/templatetags/blog_view_restrictions_tags.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 17:05:25.607088 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/
--rw-r--r--   0 kapt       (501) kapt        (20)     2127 2024-04-18 17:05:25.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)      906 2024-04-18 17:05:25.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-04-18 17:05:25.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-04-18 17:05:25.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/requires.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       33 2024-04-18 17:05:25.000000 djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501) kapt        (20)      811 2024-04-18 17:05:25.609088 djangocms_blog_view_restrictions-0.1.0/setup.cfg
--rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_view_restrictions-0.1.0/setup.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.547059 djangocms_blog_view_restrictions-0.2.0/
+-rw-r--r--   0 kapt       (501) kapt        (20)       44 2024-04-18 16:26:27.000000 djangocms_blog_view_restrictions-0.2.0/AUTHORS.md
+-rw-r--r--   0 kapt       (501) kapt        (20)     1280 2024-04-18 16:27:10.000000 djangocms_blog_view_restrictions-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_view_restrictions-0.2.0/LICENSE
+-rw-r--r--   0 kapt       (501) kapt        (20)      181 2024-04-18 16:29:29.000000 djangocms_blog_view_restrictions-0.2.0/MANIFEST.in
+-rw-r--r--   0 kapt       (501) kapt        (20)     2122 2024-05-30 14:21:52.547059 djangocms_blog_view_restrictions-0.2.0/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     1314 2024-04-18 17:06:07.000000 djangocms_blog_view_restrictions-0.2.0/README.md
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.518059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-18 12:20:57.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      525 2024-04-18 16:56:09.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/admin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      136 2024-04-18 16:44:10.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/apps.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.487059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.488059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/fr/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.537059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501) kapt        (20)      918 2024-04-18 16:53:57.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501) kapt        (20)     1602 2024-04-18 16:53:54.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.543059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/migrations/
+-rw-r--r--   0 kapt       (501) kapt        (20)     2042 2024-04-18 16:33:26.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-18 14:41:10.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/migrations/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1260 2024-04-18 16:56:09.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/models.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.543059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/templatetags/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-18 14:22:52.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/templatetags/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      706 2024-05-30 12:41:32.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/templatetags/blog_view_restrictions_tags.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-05-30 14:21:52.543059 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/
+-rw-r--r--   0 kapt       (501) kapt        (20)     2122 2024-05-30 14:21:52.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)      906 2024-05-30 14:21:52.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-05-30 14:21:52.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-05-30 14:21:52.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       33 2024-05-30 14:21:52.000000 djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)      811 2024-05-30 14:21:52.548059 djangocms_blog_view_restrictions-0.2.0/setup.cfg
+-rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_view_restrictions-0.2.0/setup.py
```

### Comparing `djangocms_blog_view_restrictions-0.1.0/CONTRIBUTING.md` & `djangocms_blog_view_restrictions-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/LICENSE` & `djangocms_blog_view_restrictions-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/PKG-INFO` & `djangocms_blog_view_restrictions-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-view-restrictions
-Version: 0.1.0
+Version: 0.2.0
 Summary: Control who can view your djangocms-blog posts
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-view-restrictions
 Author: Adrien Delhorme
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
@@ -28,16 +28,15 @@
 * Install the package
     ```bash
     python3 -m pip install djangocms-blog-view-restrictions
     ```
 
 * Add it in your `INSTALLED_APPS`:
     ```python
-
-        "djangocms_blog_view_restrictions",
+    "djangocms_blog_view_restrictions",
     ```
 
 * Run the migration:
     ```sh
     python3 manage.py migrate djangocms_blog_view_restrictions
     ```
```

### Comparing `djangocms_blog_view_restrictions-0.1.0/README.md` & `djangocms_blog_view_restrictions-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 * Install the package
     ```bash
     python3 -m pip install djangocms-blog-view-restrictions
     ```
 
 * Add it in your `INSTALLED_APPS`:
     ```python
-
-        "djangocms_blog_view_restrictions",
+    "djangocms_blog_view_restrictions",
     ```
 
 * Run the migration:
     ```sh
     python3 manage.py migrate djangocms_blog_view_restrictions
     ```
```

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/admin.py` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.mo` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.po` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/migrations/0001_initial.py` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/models.py` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions/templatetags/blog_view_restrictions_tags.py` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions/templatetags/blog_view_restrictions_tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 
 register = template.Library()
 
 
 @register.filter()
 def can_view_post(user, post):
-    if not isinstance(post, Post) or isinstance(user, AnonymousUser):
+    if post and isinstance(post, Post) and post.view_restrictions_extensions.exists():
+        if isinstance(user, AnonymousUser):
+            return False
+
+        is_user_granted = post.view_restrictions_extensions.filter(user=user).exists()
+        is_group_granted = post.view_restrictions_extensions.filter(
+            group__in=user.groups.all()
+        ).exists()
+        if is_user_granted or is_group_granted or user.is_superuser:
+            return True
         return False
-
-    is_user_granted = post.view_restrictions_extensions.filter(user=user).exists()
-    is_group_granted = post.view_restrictions_extensions.filter(
-        group__in=user.groups.all()
-    ).exists()
-    if is_user_granted or is_group_granted or user.is_superuser:
-        return True
-
-    return False
+    return True
```

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/PKG-INFO` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-view-restrictions
-Version: 0.1.0
+Version: 0.2.0
 Summary: Control who can view your djangocms-blog posts
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-view-restrictions
 Author: Adrien Delhorme
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
@@ -28,16 +28,15 @@
 * Install the package
     ```bash
     python3 -m pip install djangocms-blog-view-restrictions
     ```
 
 * Add it in your `INSTALLED_APPS`:
     ```python
-
-        "djangocms_blog_view_restrictions",
+    "djangocms_blog_view_restrictions",
     ```
 
 * Run the migration:
     ```sh
     python3 manage.py migrate djangocms_blog_view_restrictions
     ```
```

### Comparing `djangocms_blog_view_restrictions-0.1.0/djangocms_blog_view_restrictions.egg-info/SOURCES.txt` & `djangocms_blog_view_restrictions-0.2.0/djangocms_blog_view_restrictions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms_blog_view_restrictions-0.1.0/setup.cfg` & `djangocms_blog_view_restrictions-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-view-restrictions
-version = 0.1.0
+version = 0.2.0
 description = Control who can view your djangocms-blog posts
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-view-restrictions
 author = Adrien Delhorme
 author_email = dev@kapt.mobi
 classifiers =
```

