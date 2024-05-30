# Comparing `tmp/django_azure_auth-1.4.0.tar.gz` & `tmp/django_azure_auth-1.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.4.0.tar", max compression
+gzip compressed data, was "django_azure_auth-1.4.1a0.tar", max compression
```

## Comparing `django_azure_auth-1.4.0.tar` & `django_azure_auth-1.4.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/LICENSE
--rw-r--r--   0        0        0     6081 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/backends.py
--rw-r--r--   0        0        0      529 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/exceptions.py
--rw-r--r--   0        0        0     6704 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/handlers.py
--rw-r--r--   0        0        0     1327 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2091 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1409 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     2019 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    13037 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-05-28 16:20:29.819346 django_azure_auth-1.4.0/azure_auth/urls.py
--rw-r--r--   0        0        0     1045 2024-05-28 16:20:29.819346 django_azure_auth-1.4.0/azure_auth/views.py
--rw-r--r--   0        0        0     1464 2024-05-28 16:20:29.819346 django_azure_auth-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 django_azure_auth-1.4.0/PKG-INFO
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

### Comparing `django_azure_auth-1.4.0/LICENSE` & `django_azure_auth-1.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/README.md` & `django_azure_auth-1.4.1a0/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/azure_auth/handlers.py` & `django_azure_auth-1.4.1a0/azure_auth/handlers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from http import HTTPStatus
 from typing import cast
 from urllib import parse
 
 import msal
 import requests
 from django.conf import settings
@@ -69,14 +70,21 @@
         accounts = self.msal_app.get_accounts()
         if accounts:  # pragma: no branch
             # Will return `None` if CCA cannot retrieve or generate new token
             token_result = self.msal_app.acquire_token_silent(
                 scopes=settings.AZURE_AUTH["SCOPES"], account=accounts[0]
             )
             self._save_cache()
+
+            # `acquire_token_silent` doesn't always return ID token/ID token claims
+            # https://github.com/AzureAD/microsoft-authentication-library-for-python/issues/139
+            if token_result and token_result.get("id_token_claims"):
+                self.request.session["id_token_claims"] = token_result[
+                    "id_token_claims"
+                ]
             return token_result
 
     def authenticate(self, token: dict) -> AbstractBaseUser:
         """
         Helper method to authenticate the user. Gets the Azure user from the
         Microsoft Graph endpoint and gets/creates the associated Django user.
 
@@ -134,14 +142,28 @@
             "post_logout_redirect_uri": settings.AZURE_AUTH.get("LOGOUT_URI"),
             "logout_hint": self.claims.get("login_hint"),
         }
         query_params = {k: v for k, v in _query_params.items() if v}
         return f"{authority}/oauth2/v2.0/logout?{parse.urlencode(query_params)}"
 
     @property
+    def user_is_authenticated(self) -> bool:
+        now = datetime.datetime.now(datetime.timezone.utc).timestamp()
+
+        # Check the ID token is still valid in the first instance
+        if now < self.claims.get("exp", 0) and self.request.user.is_authenticated:
+            return True
+
+        # Otherwise try refresh the token
+        return (
+            self.get_token_from_cache() is not None
+            and self.request.user.is_authenticated
+        )
+
+    @property
     def msal_app(self):
         if self._msal_app is None:
             self._msal_app = msal.ConfidentialClientApplication(
                 client_id=settings.AZURE_AUTH["CLIENT_ID"],
                 client_credential=settings.AZURE_AUTH["CLIENT_SECRET"],
                 authority=settings.AZURE_AUTH["AUTHORITY"],
                 token_cache=self.cache,
```

### Comparing `django_azure_auth-1.4.0/azure_auth/middleware.py` & `django_azure_auth-1.4.1a0/azure_auth/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,13 @@
             return self.get_response(request)
 
         # Added to resolve paths that can't be reversed
         for path in public_paths:
             if request.path_info.startswith(path):
                 return self.get_response(request)
 
-        if AuthHandler(request).get_token_from_cache():
-            # If the user is authenticated
-            if request.user.is_authenticated:
-                return self.get_response(request)
+        if AuthHandler(request).user_is_authenticated:
+            return self.get_response(request)
 
         # Save the intended path on the session to be redirected there upon login
         request.session["next"] = request.path
         return redirect("azure_auth:login")
```

### Comparing `django_azure_auth-1.4.0/azure_auth/tests/conftest.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/azure_auth/tests/settings.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/test_middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from http import HTTPStatus
 from unittest.mock import patch
 
 import msal
 import pytest
 from django.test import TransactionTestCase
 from django.urls import reverse
@@ -29,14 +30,52 @@
 
     def test_valid_token_authenticated_user(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
         self.client.force_login(self.user)  # type: ignore
 
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.OK
+        assert mocked_msal_app.return_value.acquire_token_silent.call_count == 1
+
+    def test_valid_id_token_claims_authenticated_user(self, mocked_msal_app):
+        self.client.force_login(self.user)  # type: ignore
+
+        # Set up valid id token claims in session
+        session = self.client.session
+        session["id_token_claims"] = {
+            "exp": datetime.datetime.now(datetime.timezone.utc).timestamp() + 10
+        }
+        session.save()
+
+        resp = self.client.get(reverse("middleware_protected"))
+        assert resp.status_code == HTTPStatus.OK
+        assert mocked_msal_app.return_value.acquire_token_silent.call_count == 0
+
+    def test_expired_id_token_claims_authenticated_user(self, mocked_msal_app):
+        # Set up mocked incoming token
+        new_token_expiry = (
+            datetime.datetime.now(datetime.timezone.utc).timestamp() + 1000
+        )
+        new_token = self.token  # type: ignore
+        new_token["id_token_claims"]["exp"] = new_token_expiry
+
+        mocked_msal_app.return_value.acquire_token_silent.return_value = new_token
+        self.client.force_login(self.user)  # type: ignore
+
+        # Set up expired id token claims in session
+        session = self.client.session
+        session["id_token_claims"] = {
+            "exp": datetime.datetime.now(datetime.timezone.utc).timestamp() - 10
+        }
+        session.save()
+
+        resp = self.client.get(reverse("middleware_protected"))
+        assert resp.status_code == HTTPStatus.OK
+        assert mocked_msal_app.return_value.acquire_token_silent.call_count == 1
+        assert self.client.session["id_token_claims"]["exp"] == new_token_expiry
 
     def test_public_view(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = None
         resp = self.client.get(reverse("public"))
         assert resp.status_code == HTTPStatus.OK
 
     def test_public_external_view(self, mocked_msal_app):
```

### Comparing `django_azure_auth-1.4.0/azure_auth/tests/test_views.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/azure_auth/tests/urls.py` & `django_azure_auth-1.4.1a0/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/azure_auth/views.py` & `django_azure_auth-1.4.1a0/azure_auth/views.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.0/pyproject.toml` & `django_azure_auth-1.4.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.4.0"
+version = "1.4.1a0"
 description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
```

### Comparing `django_azure_auth-1.4.0/PKG-INFO` & `django_azure_auth-1.4.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.4.0
+Version: 1.4.1a0
 Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
 Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
```

