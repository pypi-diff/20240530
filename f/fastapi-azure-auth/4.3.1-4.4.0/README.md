# Comparing `tmp/fastapi_azure_auth-4.3.1.tar.gz` & `tmp/fastapi_azure_auth-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_azure_auth-4.3.1.tar", max compression
+gzip compressed data, was "fastapi_azure_auth-4.4.0.tar", max compression
```

## Comparing `fastapi_azure_auth-4.3.1.tar` & `fastapi_azure_auth-4.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-03-04 15:48:35.154560 fastapi_azure_auth-4.3.1/LICENSE
--rw-r--r--   0        0        0     6580 2024-03-04 15:48:35.154560 fastapi_azure_auth-4.3.1/README.md
--rw-r--r--   0        0        0      339 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/__init__.py
--rw-r--r--   0        0        0    20929 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/auth.py
--rw-r--r--   0        0        0      337 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/exceptions.py
--rw-r--r--   0        0        0     4451 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/openid_config.py
--rw-r--r--   0        0        0        0 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/py.typed
--rw-r--r--   0        0        0     9482 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/user.py
--rw-r--r--   0        0        0      457 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/fastapi_azure_auth/utils.py
--rw-r--r--   0        0        0     2428 2024-03-04 15:48:35.174560 fastapi_azure_auth-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     8196 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-30 15:50:10.151725 fastapi_azure_auth-4.4.0/LICENSE
+-rw-r--r--   0        0        0     6580 2024-05-30 15:50:10.151725 fastapi_azure_auth-4.4.0/README.md
+-rw-r--r--   0        0        0      339 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/__init__.py
+-rw-r--r--   0        0        0    21717 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/auth.py
+-rw-r--r--   0        0        0      337 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/exceptions.py
+-rw-r--r--   0        0        0     4468 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/openid_config.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/py.typed
+-rw-r--r--   0        0        0     9482 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/user.py
+-rw-r--r--   0        0        0      907 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/fastapi_azure_auth/utils.py
+-rw-r--r--   0        0        0     2383 2024-05-30 15:50:10.171725 fastapi_azure_auth-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8176 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.4.0/PKG-INFO
```

### Comparing `fastapi_azure_auth-4.3.1/LICENSE` & `fastapi_azure_auth-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.3.1/README.md` & `fastapi_azure_auth-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.3.1/fastapi_azure_auth/auth.py` & `fastapi_azure_auth-4.4.0/fastapi_azure_auth/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 import inspect
 import logging
-from typing import Any, Awaitable, Callable, Dict, Literal, Optional
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, Literal, Optional
 from warnings import warn
 
+import jwt
 from fastapi.exceptions import HTTPException
 from fastapi.security import OAuth2AuthorizationCodeBearer, SecurityScopes
 from fastapi.security.base import SecurityBase
-from jose import jwt
-from jose.exceptions import ExpiredSignatureError, JWTClaimsError, JWTError
+from jwt.exceptions import (
+    ExpiredSignatureError,
+    ImmatureSignatureError,
+    InvalidAudienceError,
+    InvalidIssuedAtError,
+    InvalidIssuerError,
+    InvalidTokenError,
+    MissingRequiredClaimError,
+)
 from starlette.requests import Request
 
 from fastapi_azure_auth.exceptions import InvalidAuth
 from fastapi_azure_auth.openid_config import OpenIdConfig
 from fastapi_azure_auth.user import User
-from fastapi_azure_auth.utils import is_guest
+from fastapi_azure_auth.utils import get_unverified_claims, get_unverified_header, is_guest
+
+if TYPE_CHECKING:  # pragma: no cover
+    from jwt.algorithms import AllowedPublicKeys
 
 log = logging.getLogger('fastapi_azure_auth')
 
 
 class AzureAuthorizationCodeBearerBase(SecurityBase):
     def __init__(
         self,
@@ -141,19 +152,21 @@
         self.model = self.oauth.model
 
     async def __call__(self, request: Request, security_scopes: SecurityScopes) -> Optional[User]:
         """
         Extends call to also validate the token.
         """
         try:
-            access_token = await self.oauth(request=request)
+            access_token = await self.extract_access_token(request)
             try:
+                if access_token is None:
+                    raise Exception('No access token provided')
                 # Extract header information of the token.
-                header: dict[str, str] = jwt.get_unverified_header(token=access_token) or {}
-                claims: dict[str, Any] = jwt.get_unverified_claims(token=access_token) or {}
+                header: dict[str, Any] = get_unverified_header(access_token)
+                claims: dict[str, Any] = get_unverified_claims(access_token)
             except Exception as error:
                 log.warning('Malformed token received. %s. Error: %s', access_token, error, exc_info=True)
                 raise InvalidAuth(detail='Invalid token format') from error
 
             user_is_guest: bool = is_guest(claims=claims)
             if not self.allow_guest_users and user_is_guest:
                 log.info('User denied, is a guest user', claims)
@@ -176,69 +189,87 @@
             else:
                 iss = self.openid_config.issuer
 
             # Use the `kid` from the header to find a matching signing key to use
             try:
                 if key := self.openid_config.signing_keys.get(header.get('kid', '')):
                     # We require and validate all fields in an Azure AD token
+                    required_claims = ['exp', 'aud', 'iat', 'nbf', 'sub']
+                    if self.validate_iss:
+                        required_claims.append('iss')
+
                     options = {
                         'verify_signature': True,
                         'verify_aud': True,
                         'verify_iat': True,
                         'verify_exp': True,
                         'verify_nbf': True,
                         'verify_iss': self.validate_iss,
-                        'verify_sub': True,
-                        'verify_jti': True,
-                        'verify_at_hash': True,
-                        'require_aud': True,
-                        'require_iat': True,
-                        'require_exp': True,
-                        'require_nbf': True,
-                        'require_iss': self.validate_iss,
-                        'require_sub': True,
-                        'require_jti': False,
-                        'require_at_hash': False,
-                        'leeway': self.leeway,
+                        'require': required_claims,
                     }
                     # Validate token
-                    token = jwt.decode(
-                        access_token,
-                        key=key,
-                        algorithms=['RS256'],
-                        audience=self.app_client_id if self.token_version == 2 else f'api://{self.app_client_id}',
-                        issuer=iss,
-                        options=options,
-                    )
+                    token = self.validate(access_token=access_token, iss=iss, key=key, options=options)
                     # Attach the user to the request. Can be accessed through `request.state.user`
                     user: User = User(
                         **{**token, 'claims': token, 'access_token': access_token, 'is_guest': user_is_guest}
                     )
                     request.state.user = user
                     return user
-            except JWTClaimsError as error:
+            except (
+                InvalidAudienceError,
+                InvalidIssuerError,
+                InvalidIssuedAtError,
+                ImmatureSignatureError,
+                MissingRequiredClaimError,
+            ) as error:
                 log.info('Token contains invalid claims. %s', error)
                 raise InvalidAuth(detail='Token contains invalid claims') from error
             except ExpiredSignatureError as error:
                 log.info('Token signature has expired. %s', error)
                 raise InvalidAuth(detail='Token signature has expired') from error
-            except JWTError as error:
+            except InvalidTokenError as error:
                 log.warning('Invalid token. Error: %s', error, exc_info=True)
                 raise InvalidAuth(detail='Unable to validate token') from error
             except Exception as error:
                 # Extra failsafe in case of a bug in a future version of the jwt library
                 log.exception('Unable to process jwt token. Uncaught error: %s', error)
                 raise InvalidAuth(detail='Unable to process token') from error
             log.warning('Unable to verify token. No signing keys found')
             raise InvalidAuth(detail='Unable to verify token, no signing keys found')
         except (HTTPException, InvalidAuth):
             if not self.auto_error:
                 return None
             raise
 
+    async def extract_access_token(self, request: Request) -> Optional[str]:
+        """
+        Extracts the access token from the request.
+        """
+        return await self.oauth(request=request)
+
+    def validate(
+        self, access_token: str, key: 'AllowedPublicKeys', iss: str, options: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        """
+        Validates the token using the provided key and options.
+        """
+        alg = 'RS256'
+        aud = self.app_client_id if self.token_version == 2 else f'api://{self.app_client_id}'
+        return dict(
+            jwt.decode(
+                access_token,
+                key=key,
+                algorithms=[alg],
+                audience=aud,
+                issuer=iss,
+                leeway=self.leeway,
+                options=options,
+            )
+        )
+
 
 class SingleTenantAzureAuthorizationCodeBearer(AzureAuthorizationCodeBearerBase):
     def __init__(
         self,
         app_client_id: str,
         tenant_id: str,
         auto_error: bool = True,
```

### Comparing `fastapi_azure_auth-4.3.1/fastapi_azure_auth/openid_config.py` & `fastapi_azure_auth-4.4.0/fastapi_azure_auth/openid_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 from datetime import datetime, timedelta
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
-from cryptography.hazmat.primitives.asymmetric.types import PublicKeyTypes as KeyTypes
+import jwt
 from fastapi import HTTPException, status
 from httpx import AsyncClient
-from jose import jwk
+
+if TYPE_CHECKING:  # pragma: no cover
+    from jwt.algorithms import AllowedPublicKeys
 
 log = logging.getLogger('fastapi_azure_auth')
 
 
 class OpenIdConfig:
     def __init__(
         self,
@@ -23,15 +25,15 @@
         self._config_timestamp: Optional[datetime] = None
         self.multi_tenant: bool = multi_tenant
         self.token_version: int = token_version
         self.app_id = app_id
         self.config_url = config_url
 
         self.authorization_endpoint: str
-        self.signing_keys: dict[str, KeyTypes]
+        self.signing_keys: dict[str, 'AllowedPublicKeys']
         self.token_endpoint: str
         self.issuer: str
 
     async def load_config(self) -> None:
         """
         Loads config from the Intility openid-config endpoint if it's over 24 hours old (or don't exist)
         """
@@ -94,10 +96,10 @@
         """
         Create certificates based on signing keys and store them
         """
         self.signing_keys = {}
         for key in keys:
             if key.get('use') == 'sig':  # Only care about keys that are used for signatures, not encryption
                 log.debug('Loading public key from certificate: %s', key)
-                cert_obj = jwk.construct(key, 'RS256')
+                cert_obj = jwt.PyJWK(key, 'RS256')
                 if kid := key.get('kid'):  # In case a key would not have a thumbprint we can match, we don't want it.
-                    self.signing_keys[kid] = cert_obj
+                    self.signing_keys[kid] = cert_obj.key
```

### Comparing `fastapi_azure_auth-4.3.1/fastapi_azure_auth/user.py` & `fastapi_azure_auth-4.4.0/fastapi_azure_auth/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.3.1/pyproject.toml` & `fastapi_azure_auth-4.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-azure-auth"
-version = "4.3.1"  # Remember to change in __init__.py as well
+version = "4.4.0"  # Remember to change in __init__.py as well
 description = "Easy and secure implementation of Azure AD for your FastAPI APIs"
 authors = ["Jonas Krüger Svensson <jonas.svensson@intility.no>"]
 readme = "README.md"
 homepage = "https://github.com/intility/fastapi-azure-auth"
 repository = "https://github.com/intility/fastapi-azure-auth"
 documentation = "https://github.com/intility/fastapi-azure-auth"
 keywords = [
@@ -39,16 +39,16 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = ">0.68.0"
 cryptography = ">=40.0.1"
-python-jose = {extras = ["cryptography"], version = "^3.3.0"}
 httpx = ">0.18.2"
+pyjwt = "^2.8.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.9.3"
 black = "^22.1.0"
 pytest = "^7.0.1"
 pytest-cov = "^3.0.0"
```

### Comparing `fastapi_azure_auth-4.3.1/PKG-INFO` & `fastapi_azure_auth-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-azure-auth
-Version: 4.3.1
+Version: 4.4.0
 Summary: Easy and secure implementation of Azure AD for your FastAPI APIs
 Home-page: https://github.com/intility/fastapi-azure-auth
 Keywords: ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi tenant,oauth2,oidc,security,single tenant,starlette,trio
 Author: Jonas Krüger Svensson
 Author-email: jonas.svensson@intility.no
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cryptography (>=40.0.1)
 Requires-Dist: fastapi (>0.68.0)
 Requires-Dist: httpx (>0.18.2)
-Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
+Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Project-URL: Documentation, https://github.com/intility/fastapi-azure-auth
 Project-URL: Repository, https://github.com/intility/fastapi-azure-auth
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <img margin="0 10px 0 0" src="https://avatars.githubusercontent.com/u/35199565" width="124px"/>
   <img margin="0 10px 0 0" src="https://raw.githubusercontent.com/Intility/fastapi-azure-auth/main/docs/static/img/global/fastad.png" width="124px"/><br/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.3.1 Summary: Easy and
+Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.4.0 Summary: Easy and
 secure implementation of Azure AD for your FastAPI APIs Home-page: https://
 github.com/intility/fastapi-azure-auth Keywords:
 ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi
 tenant,oauth2,oidc,security,single tenant,starlette,trio Author: Jonas KrÃ¼ger
 Svensson Author-email: jonas.svensson@intility.no Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Dist: cryptography (>=40.0.1) Requires-Dist: fastapi (>0.68.0)
-Requires-Dist: httpx (>0.18.2) Requires-Dist: python-jose[cryptography]
-(>=3.3.0,<4.0.0) Project-URL: Documentation, https://github.com/intility/
-fastapi-azure-auth Project-URL: Repository, https://github.com/intility/
-fastapi-azure-auth Description-Content-Type: text/markdown
+Requires-Dist: httpx (>0.18.2) Requires-Dist: pyjwt (>=2.8.0,<3.0.0) Project-
+URL: Documentation, https://github.com/intility/fastapi-azure-auth Project-URL:
+Repository, https://github.com/intility/fastapi-azure-auth Description-Content-
+Type: text/markdown
       ************ [[hhttttppss::////aavvaattaarrss..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//uu//3355119999556655]][[hhttttppss::////
   rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//IInnttiilliittyy//ffaassttaappii--aazzuurree--aauutthh//mmaaiinn//ddooccss//ssttaattiicc//iimmgg//
                               gglloobbaall//ffaassttaadd..ppnngg]]
                            FFaassttAAPPII--AAzzuurree--AAuutthh ************
               AAzzuurree AADD AAuutthheennttiiccaattiioonn ffoorr FFaassttAAPPII aappppss mmaaddee eeaassyy..
               _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_F_a_s_t_A_P_I_ _V_e_r_s_i_o_n_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
                    _[_C_o_d_e_c_o_v_]_[_P_r_e_-_c_o_m_m_i_t_]_[_B_l_a_c_k_]_[_m_y_p_y_]_[_i_s_o_r_t_]
```

