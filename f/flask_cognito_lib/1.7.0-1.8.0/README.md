# Comparing `tmp/flask_cognito_lib-1.7.0.tar.gz` & `tmp/flask_cognito_lib-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_cognito_lib-1.7.0.tar", max compression
+gzip compressed data, was "flask_cognito_lib-1.8.0.tar", max compression
```

## Comparing `flask_cognito_lib-1.7.0.tar` & `flask_cognito_lib-1.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-15 12:34:32.090129 flask_cognito_lib-1.7.0/LICENSE
--rw-r--r--   0        0        0     9231 2024-05-15 12:34:32.090129 flask_cognito_lib-1.7.0/README.md
--rw-r--r--   0        0        0     2305 2024-05-15 12:34:58.334186 flask_cognito_lib-1.7.0/pyproject.toml
--rw-r--r--   0        0        0       82 2024-05-15 12:34:58.306186 flask_cognito_lib-1.7.0/src/flask_cognito_lib/__init__.py
--rw-r--r--   0        0        0     6668 2024-05-15 12:34:32.090129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/config.py
--rw-r--r--   0        0        0     9618 2024-05-15 12:34:32.090129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/decorators.py
--rw-r--r--   0        0        0      384 2024-05-15 12:34:32.090129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/exceptions.py
--rw-r--r--   0        0        0     7330 2024-05-15 12:34:32.090129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/plugin.py
--rw-r--r--   0        0        0      326 2024-05-15 12:34:32.094129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/services/__init__.py
--rw-r--r--   0        0        0     7013 2024-05-15 12:34:32.094129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/services/cognito_svc.py
--rw-r--r--   0        0        0     7235 2024-05-15 12:34:32.094129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/services/token_svc.py
--rw-r--r--   0        0        0     1124 2024-05-15 12:34:32.094129 flask_cognito_lib-1.7.0/src/flask_cognito_lib/utils.py
--rw-r--r--   0        0        0    10715 1970-01-01 00:00:00.000000 flask_cognito_lib-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-30 09:34:15.655383 flask_cognito_lib-1.8.0/LICENSE
+-rw-r--r--   0        0        0    10313 2024-05-30 09:34:15.655383 flask_cognito_lib-1.8.0/README.md
+-rw-r--r--   0        0        0     2305 2024-05-30 09:34:38.471551 flask_cognito_lib-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-05-30 09:34:38.447551 flask_cognito_lib-1.8.0/src/flask_cognito_lib/__init__.py
+-rw-r--r--   0        0        0     6668 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/config.py
+-rw-r--r--   0        0        0    10004 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/decorators.py
+-rw-r--r--   0        0        0      384 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/exceptions.py
+-rw-r--r--   0        0        0     7722 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/plugin.py
+-rw-r--r--   0        0        0      326 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/services/__init__.py
+-rw-r--r--   0        0        0     7013 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/services/cognito_svc.py
+-rw-r--r--   0        0        0     7235 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/services/token_svc.py
+-rw-r--r--   0        0        0     1124 2024-05-30 09:34:15.659383 flask_cognito_lib-1.8.0/src/flask_cognito_lib/utils.py
+-rw-r--r--   0        0        0    11797 1970-01-01 00:00:00.000000 flask_cognito_lib-1.8.0/PKG-INFO
```

### Comparing `flask_cognito_lib-1.7.0/LICENSE` & `flask_cognito_lib-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.7.0/README.md` & `flask_cognito_lib-1.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -154,14 +154,48 @@
     return redirect(url_for("home"))
 
 
 if __name__ == "__main__":
     app.run()
 ```
 
+## Config class override
+
+There might be some cases where you want to override the default `Config` class to add custom logic. For example, to generate the `redirect_url` and `logout_redirect` dynamically using `url_for`, you can override the `Config` class as follows:
+
+```python
+from flask import url_for
+from flask_cognito_lib.config import Config
+
+class ConfigOverride(Config):
+    """
+    ConfigOverride class to generate URLs dynamically using `url_for`
+    """
+    @property
+    def redirect_url(self) -> str:
+        """Return the Redirect URL (post-login)"""
+        return url_for(endpoint='auth.cognito', _external=True)
+
+    @property
+    def logout_redirect(self) -> str:
+        """Return the Redirect URL (post-logout)"""
+        return url_for(endpoint='auth.cognito_post_logout', _external=True)
+```
+
+Then, pass the object of `ConfigOverride` class when initializing the `CognitoAuth` plugin as follows:
+
+```python
+CognitoAuth(app, cfg=ConfigOverride())
+```
+
+Or if you are using lazy initialization:
+
+```python
+CognitoAuth().init_app(app, cfg=ConfigOverride())
+```
 
 ## Development
 
 Prequisites:
 
 * [poetry](https://python-poetry.org/)
 * [pre-commit](https://pre-commit.com/)
```

### Comparing `flask_cognito_lib-1.7.0/pyproject.toml` & `flask_cognito_lib-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask_cognito_lib"
-version = "1.7.0"
+version = "1.8.0"
 description = "A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices"
 license = "MIT"
 authors = ["mblackgeo <18327836+mblackgeo@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/mblackgeo/flask-cognito-lib"
 repository = "https://github.com/mblackgeo/flask-cognito-lib"
 keywords = ["Flask", "Extension", "OAuth", "Cognito"]
```

### Comparing `flask_cognito_lib-1.7.0/src/flask_cognito_lib/config.py` & `flask_cognito_lib-1.8.0/src/flask_cognito_lib/config.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.7.0/src/flask_cognito_lib/decorators.py` & `flask_cognito_lib-1.8.0/src/flask_cognito_lib/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 from flask_cognito_lib.utils import (
     CognitoTokenResponse,
     generate_code_challenge,
     generate_code_verifier,
     secure_random,
 )
 
-cfg = Config()
 cognito_auth: CognitoAuth = LocalProxy(
-    lambda: app.extensions[cfg.APP_EXTENSION_KEY]
+    lambda: app.extensions[Config.APP_EXTENSION_KEY]
 )  # type: ignore
 
 
 def remove_from_session(keys: Iterable[str]):
     """Remove an entry from the session"""
     with app.app_context():
         for key in keys:
@@ -39,24 +38,24 @@
     tokens: CognitoTokenResponse,
     nonce: Optional[str] = None,
 ) -> None:
     """Validate and store the access token and ID token (if present) in the session"""
     # validate the JWT and get the claims
     claims = cognito_auth.verify_access_token(
         token=tokens.access_token,
-        leeway=cfg.cognito_expiration_leeway,
+        leeway=cognito_auth.cfg.cognito_expiration_leeway,
     )
     session.update({"claims": claims})
 
     # Grab the user info from the user endpoint and store in the session
     if tokens.id_token is not None:
         user_info = cognito_auth.verify_id_token(
             token=tokens.id_token,
             nonce=nonce,
-            leeway=cfg.cognito_expiration_leeway,
+            leeway=cognito_auth.cfg.cognito_expiration_leeway,
         )
         session.update({"user_info": user_info})
 
 
 def store_token_in_cookie(
     resp: Response,
     token: Union[str, None],
@@ -73,27 +72,27 @@
 
     resp.set_cookie(
         key=cookie_name,
         value=token,
         max_age=max_age,
         httponly=True,
         secure=True,
-        samesite=cfg.cookie_samesite,
-        domain=cfg.cookie_domain,
+        samesite=cognito_auth.cfg.cookie_samesite,
+        domain=cognito_auth.cfg.cookie_domain,
     )
 
 
 def get_token_from_cookie(cookie_name: str) -> Union[str, None]:
     """Get the token from the cookie"""
     token = request.cookies.get(cookie_name)
 
     if (
         token
-        and cfg.COOKIE_NAME_REFRESH == cookie_name
-        and cfg.refresh_cookie_encrypted
+        and cognito_auth.cfg.COOKIE_NAME_REFRESH == cookie_name
+        and cognito_auth.cfg.refresh_cookie_encrypted
     ):
         # Decrypt the refresh token
         return cognito_auth.token_service.decrypt_token(token)
 
     return token
 
 
@@ -122,15 +121,15 @@
 
             session.update({"state": state})
 
             login_url = cognito_auth.cognito_service.get_sign_in_url(
                 code_challenge=session["code_challenge"],
                 state=session["state"],
                 nonce=session["nonce"],
-                scopes=cfg.cognito_scopes,
+                scopes=cognito_auth.cfg.cognito_scopes,
             )
 
         return redirect(login_url)
 
     return wrapper
 
 
@@ -170,43 +169,43 @@
             # return and set the JWT as a http only cookie
             resp = fn(*args, **kwargs)
 
             # Store the access token in a HTTP only secure cookie
             store_token_in_cookie(
                 resp=resp,
                 token=tokens.access_token,
-                cookie_name=cfg.COOKIE_NAME,
-                max_age=cfg.max_cookie_age_seconds,
+                cookie_name=cognito_auth.cfg.COOKIE_NAME,
+                max_age=cognito_auth.cfg.max_cookie_age_seconds,
             )
 
             # Grab the refresh token and store in a HTTP only secure cookie
-            if cfg.refresh_flow_enabled and tokens.refresh_token:
+            if cognito_auth.cfg.refresh_flow_enabled and tokens.refresh_token:
                 store_token_in_cookie(
                     resp=resp,
                     token=tokens.refresh_token,
-                    cookie_name=cfg.COOKIE_NAME_REFRESH,
-                    max_age=cfg.max_refresh_cookie_age_seconds,
-                    encrypt=cfg.refresh_cookie_encrypted,
+                    cookie_name=cognito_auth.cfg.COOKIE_NAME_REFRESH,
+                    max_age=cognito_auth.cfg.max_refresh_cookie_age_seconds,
+                    encrypt=cognito_auth.cfg.refresh_cookie_encrypted,
                 )
 
         return resp
 
     return wrapper
 
 
 def cognito_refresh_callback(fn):
     """A decorator that handles token refresh with Cognito"""
 
     @wraps(fn)
     def wrapper(*args, **kwargs):
         with app.app_context():
-            if not cfg.refresh_flow_enabled:
+            if not cognito_auth.cfg.refresh_flow_enabled:
                 raise CognitoError("Refresh flow is not enabled")
 
-            refresh_token = get_token_from_cookie(cfg.COOKIE_NAME_REFRESH)
+            refresh_token = get_token_from_cookie(cognito_auth.cfg.COOKIE_NAME_REFRESH)
 
             if not refresh_token:
                 raise CognitoError("No refresh token provided")
 
             # Exchange refresh token for the new access token.
             tokens = cognito_auth.exchange_refresh_token(
                 refresh_token=refresh_token,
@@ -218,39 +217,43 @@
             # Return and set the JWT as a http only cookie
             resp = fn(*args, **kwargs)
 
             # Store the access token in a HTTP only secure cookie
             store_token_in_cookie(
                 resp=resp,
                 token=tokens.access_token,
-                cookie_name=cfg.COOKIE_NAME,
-                max_age=cfg.max_cookie_age_seconds,
+                cookie_name=cognito_auth.cfg.COOKIE_NAME,
+                max_age=cognito_auth.cfg.max_cookie_age_seconds,
             )
 
         return resp
 
     return wrapper
 
 
 def cognito_logout(fn):
     """A decorator that handles logging out with Cognito"""
 
     @wraps(fn)
     def wrapper(*args, **kwargs):
         with app.app_context():
             # logout at cognito and remove the cookies
-            resp = redirect(cfg.logout_endpoint)
-            resp.delete_cookie(key=cfg.COOKIE_NAME, domain=cfg.cookie_domain)
+            resp = redirect(cognito_auth.cfg.logout_endpoint)
+            resp.delete_cookie(
+                key=cognito_auth.cfg.COOKIE_NAME, domain=cognito_auth.cfg.cookie_domain
+            )
 
             # Revoke the refresh token if it exists
-            if refresh_token := get_token_from_cookie(cfg.COOKIE_NAME_REFRESH):
+            if refresh_token := get_token_from_cookie(
+                cognito_auth.cfg.COOKIE_NAME_REFRESH
+            ):
                 cognito_auth.revoke_refresh_token(refresh_token)
                 resp.delete_cookie(
-                    key=cfg.COOKIE_NAME_REFRESH,
-                    domain=cfg.cookie_domain,
+                    key=cognito_auth.cfg.COOKIE_NAME_REFRESH,
+                    domain=cognito_auth.cfg.cookie_domain,
                 )
 
         # Cognito will redirect to the sign-out URL (if set) or else use
         # the callback URL
         return resp
 
     return wrapper
@@ -260,23 +263,23 @@
     """A decorator to protect a route with AWS Cognito"""
 
     def wrapper(fn):
         @wraps(fn)
         def decorator(*args, **kwargs):
             with app.app_context():
                 # return early if the extension is disabled
-                if cfg.disabled:
+                if cognito_auth.cfg.disabled:
                     return fn(*args, **kwargs)
 
                 # Try and validate the access token stored in the cookie
                 try:
-                    access_token = request.cookies.get(cfg.COOKIE_NAME)
+                    access_token = request.cookies.get(cognito_auth.cfg.COOKIE_NAME)
                     claims = cognito_auth.verify_access_token(
                         token=access_token,
-                        leeway=cfg.cognito_expiration_leeway,
+                        leeway=cognito_auth.cfg.cognito_expiration_leeway,
                     )
                     valid = True
 
                     # Check for required group membership
                     if groups:
                         if any_group:
                             valid = any(g in claims["cognito:groups"] for g in groups)
```

### Comparing `flask_cognito_lib-1.7.0/src/flask_cognito_lib/plugin.py` & `flask_cognito_lib-1.8.0/src/flask_cognito_lib/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,37 +12,45 @@
 
 class CognitoAuth:
     def __init__(
         self,
         app: Optional[Flask] = None,
         _token_service_factory: Callable = token_service_factory,
         _cognito_service_factory: Callable = cognito_service_factory,
+        cfg: Optional[Config] = None,
     ):
         """Instantiate the CognitoAuth manager
 
         Parameters
         ----------
         app : Optional[Flask], optional
             An optional instance of a Flask application. If doing lazy init
             use the `init_app` method instead
+        cfg : Optional[Config], optional
+            Configuration object to use. If not provided, a default Config is used.
         """
         self.token_service_factory = _token_service_factory
         self.cognito_service_factory = _cognito_service_factory
         if app is not None:
-            self.init_app(app)
+            self.init_app(app=app, cfg=cfg)
 
-    def init_app(self, app: Flask):
+    def init_app(self, app: Flask, cfg: Optional[Config] = None):
         """Register the extension with a Flask application
 
         Parameters
         ----------
         app : Flask
             Flask application
+        cfg : Optional[Config], optional
+            Configuration object to use. If not provided, a default Config is used.
         """
-        self.cfg = Config()
+        if cfg:
+            self.cfg = cfg
+        else:
+            self.cfg = Config()
         app.extensions[self.cfg.APP_EXTENSION_KEY] = self
 
     @property
     def token_service(self) -> TokenService:
         """Instantiate an instance of the TokenService within the app context
 
         Returns
```

### Comparing `flask_cognito_lib-1.7.0/src/flask_cognito_lib/services/cognito_svc.py` & `flask_cognito_lib-1.8.0/src/flask_cognito_lib/services/cognito_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.7.0/src/flask_cognito_lib/services/token_svc.py` & `flask_cognito_lib-1.8.0/src/flask_cognito_lib/services/token_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.7.0/src/flask_cognito_lib/utils.py` & `flask_cognito_lib-1.8.0/src/flask_cognito_lib/utils.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.7.0/PKG-INFO` & `flask_cognito_lib-1.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_cognito_lib
-Version: 1.7.0
+Version: 1.8.0
 Summary: A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices
 Home-page: https://github.com/mblackgeo/flask-cognito-lib
 License: MIT
 Keywords: Flask,Extension,OAuth,Cognito
 Author: mblackgeo
 Author-email: 18327836+mblackgeo@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -188,14 +188,48 @@
     return redirect(url_for("home"))
 
 
 if __name__ == "__main__":
     app.run()
 ```
 
+## Config class override
+
+There might be some cases where you want to override the default `Config` class to add custom logic. For example, to generate the `redirect_url` and `logout_redirect` dynamically using `url_for`, you can override the `Config` class as follows:
+
+```python
+from flask import url_for
+from flask_cognito_lib.config import Config
+
+class ConfigOverride(Config):
+    """
+    ConfigOverride class to generate URLs dynamically using `url_for`
+    """
+    @property
+    def redirect_url(self) -> str:
+        """Return the Redirect URL (post-login)"""
+        return url_for(endpoint='auth.cognito', _external=True)
+
+    @property
+    def logout_redirect(self) -> str:
+        """Return the Redirect URL (post-logout)"""
+        return url_for(endpoint='auth.cognito_post_logout', _external=True)
+```
+
+Then, pass the object of `ConfigOverride` class when initializing the `CognitoAuth` plugin as follows:
+
+```python
+CognitoAuth(app, cfg=ConfigOverride())
+```
+
+Or if you are using lazy initialization:
+
+```python
+CognitoAuth().init_app(app, cfg=ConfigOverride())
+```
 
 ## Development
 
 Prequisites:
 
 * [poetry](https://python-poetry.org/)
 * [pre-commit](https://pre-commit.com/)
```

