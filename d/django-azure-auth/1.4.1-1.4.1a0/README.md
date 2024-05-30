# Comparing `tmp/django_azure_auth-1.4.1.tar.gz` & `tmp/django_azure_auth-1.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.4.1.tar", max compression
+gzip compressed data, was "django_azure_auth-1.4.1a0.tar", max compression
```

## Comparing `django_azure_auth-1.4.1.tar` & `django_azure_auth-1.4.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/LICENSE
--rw-r--r--   0        0        0     6081 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/README.md
--rw-r--r--   0        0        0        0 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/backends.py
--rw-r--r--   0        0        0      435 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/exceptions.py
--rw-r--r--   0        0        0     7576 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/handlers.py
--rw-r--r--   0        0        0     1233 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2091 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1409 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     3699 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    13037 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/urls.py
--rw-r--r--   0        0        0     1045 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/azure_auth/views.py
--rw-r--r--   0        0        0     1464 2024-05-30 11:21:36.996879 django_azure_auth-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 django_azure_auth-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/LICENSE
+-rw-r--r--   0        0        0     6081 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/backends.py
+-rw-r--r--   0        0        0      435 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     7576 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1233 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2091 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1409 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     3699 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    13037 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-05-29 13:17:57.994004 django_azure_auth-1.4.1a0/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-05-29 13:17:57.994004 django_azure_auth-1.4.1a0/azure_auth/urls.py
+-rw-r--r--   0        0        0     1045 2024-05-29 13:17:57.994004 django_azure_auth-1.4.1a0/azure_auth/views.py
+-rw-r--r--   0        0        0     1466 2024-05-29 13:18:10.046038 django_azure_auth-1.4.1a0/pyproject.toml
+-rw-r--r--   0        0        0     7064 1970-01-01 00:00:00.000000 django_azure_auth-1.4.1a0/PKG-INFO
```

### Comparing `django_azure_auth-1.4.1/LICENSE` & `django_azure_auth-1.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/README.md` & `django_azure_auth-1.4.1a0/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/handlers.py` & `django_azure_auth-1.4.1a0/azure_auth/handlers.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/middleware.py` & `django_azure_auth-1.4.1a0/azure_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/tests/conftest.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/tests/settings.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/tests/test_views.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/tests/urls.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/azure_auth/views.py` & `django_azure_auth-1.4.1a0/azure_auth/views.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1/pyproject.toml` & `django_azure_auth-1.4.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.4.1"
+version = "1.4.1a0"
 description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
```

### Comparing `django_azure_auth-1.4.1/PKG-INFO` & `django_azure_auth-1.4.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.4.1
+Version: 1.4.1a0
 Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
 Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
```

