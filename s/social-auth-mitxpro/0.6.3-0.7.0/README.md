# Comparing `tmp/social_auth_mitxpro-0.6.3.tar.gz` & `tmp/social_auth_mitxpro-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_auth_mitxpro-0.6.3.tar", max compression
+gzip compressed data, was "social_auth_mitxpro-0.7.0.tar", max compression
```

## Comparing `social_auth_mitxpro-0.6.3.tar` & `social_auth_mitxpro-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1530 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.6.3/LICENSE
--rw-r--r--   0        0        0     1622 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.6.3/README.md
--rw-r--r--   0        0        0     1101 2023-11-07 19:54:11.894350 social_auth_mitxpro-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-28 18:12:18.638889 social_auth_mitxpro-0.6.3/social_auth_mitxpro/__init__.py
--rw-r--r--   0        0        0     1843 2021-09-28 20:27:44.529698 social_auth_mitxpro-0.6.3/social_auth_mitxpro/backends.py
--rw-r--r--   0        0        0     2359 2021-09-28 20:27:44.529698 social_auth_mitxpro-0.6.3/social_auth_mitxpro/backends_test.py
--rw-r--r--   0        0        0      201 2021-09-28 18:12:18.638889 social_auth_mitxpro-0.6.3/social_auth_mitxpro/conftest.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 social_auth_mitxpro-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1530 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1506 2024-05-30 14:39:22.452481 social_auth_mitxpro-0.7.0/README.md
+-rw-r--r--   0        0        0     3142 2024-05-30 14:53:28.402361 social_auth_mitxpro-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 14:28:36.942581 social_auth_mitxpro-0.7.0/social_auth_mitxpro/__init__.py
+-rw-r--r--   0        0        0     1960 2024-05-30 14:39:22.522481 social_auth_mitxpro-0.7.0/social_auth_mitxpro/backends.py
+-rw-r--r--   0        0        0     2422 2024-05-30 14:39:22.522481 social_auth_mitxpro-0.7.0/social_auth_mitxpro/backends_test.py
+-rw-r--r--   0        0        0      204 2024-05-30 14:39:22.522481 social_auth_mitxpro-0.7.0/social_auth_mitxpro/conftest.py
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 social_auth_mitxpro-0.7.0/PKG-INFO
```

### Comparing `social_auth_mitxpro-0.6.3/LICENSE` & `social_auth_mitxpro-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `social_auth_mitxpro-0.6.3/README.md` & `social_auth_mitxpro-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 social-auth-mitxpro
 ---
 
 
 #### Prerequisites
 
 - [`pyenv`](https://github.com/pyenv/pyenv#installation) for managing python versions
-  - Install `python3.6` and `python2.7`
+  - Install `python3.8` and `python3.11`
 - `pip install tox tox-pyenv` for running tests and discovering python versions from `pyenv`
 - [`poetry`](https://poetry.eustace.io/docs/#installation) for building, testing, and releasing
 
 If this is your first time using `poetry`, you'll need to configure your pypi credentials via:
 - Configure pypi repository:
   - `poetry config http-basic.pypi USERNAME PASSWORD`
 - Configure testpypi repository:
   - `poetry config repositories.testpypi https://test.pypi.org/legacy`
   - `poetry config http-basic.testpypi USERNAME PASSWORD`
 
 **NOTE:** when running `poetry` commands, particularly `pylint` and `black`, you must `python3.6`
 
 #### Testing
 
-You can just run `tox` locally to test, lint, and check formatting in the supported python versions. This works by having `tox` manage the virtualenvs, which `poetry` then detects and uses. Note that some of the tools (e.g. `pylint`, `black`) only support running in `python3.6` and this is reflected in `tox.ini`.
+You can just run `tox` locally to test, lint, and check formatting in the supported python versions. This works by having `tox` manage the virtualenvs, which `poetry` then detects and uses.
 
 Run individual commands can be run interactively in a `poetry shell` session or directly via `poetry run CMD`:
 
 - `pytest` - run python tests
-- `pylint` - lint python code
-- `black .` - format python code
+- `ruff check` - lint python code
+- `ruff format` - format python code
 
 #### Building
 
 - `poetry build` - builds a pip-installable package into `dist/`
 
 #### Releasing
```

### Comparing `social_auth_mitxpro-0.6.3/social_auth_mitxpro/backends.py` & `social_auth_mitxpro-0.7.0/social_auth_mitxpro/backends.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """MIT xPro social auth backend"""
+
 from social_core.backends.oauth import BaseOAuth2
 
 
 class MITxProOAuth2(BaseOAuth2):
     """MIT xPro social auth backend"""
 
     name = "mitxpro-oauth2"
 
     ID_KEY = "username"
     REQUIRES_EMAIL_VALIDATION = False
 
-    ACCESS_TOKEN_METHOD = "POST"
+    ACCESS_TOKEN_METHOD = "POST"  # noqa: S105
 
     # at a minimum we need to be able to read the user
-    DEFAULT_SCOPE = ["user:read"]
+    DEFAULT_SCOPE = ["user:read"]  # noqa: RUF012
 
     def authorization_url(self):
-        """Provides authorization_url from settings"""
+        """Provides authorization_url from settings"""  # noqa: D401
         return self.setting("AUTHORIZATION_URL")
 
     def access_token_url(self):
-        """Provides access_token_url from settings"""
+        """Provides access_token_url from settings"""  # noqa: D401
         return self.setting("ACCESS_TOKEN_URL")
 
     def api_root(self):
-        """Returns the API root as configured"""
+        """Returns the API root as configured"""  # noqa: D401
         root = self.setting("API_ROOT")
 
         if root and root[-1] != "/":
             root = f"{root}/"
 
         return root
 
@@ -40,23 +41,23 @@
 
     def api_url(self, path):
         """
         Returns the full api url given a relative path
 
         Args:
             path (str): relative api path
-        """
+        """  # noqa: D401
         return f"{self.api_root()}{path}"
 
     def get_user_details(self, response):
         """Return user details from xPro account"""
         return {
             "username": response.get("username"),
             "email": response.get("email", ""),
             "name": response.get("name", ""),
         }
 
-    def user_data(self, access_token, *args, **kwargs):
-        """Loads user data from xpro"""
+    def user_data(self, access_token, *args, **kwargs):  # noqa: ARG002
+        """Loads user data from xpro"""  # noqa: D401
         url = self.api_url("api/users/me")
         headers = {"Authorization": f"Bearer {access_token}"}
         return self.get_json(url, headers=headers)
```

### Comparing `social_auth_mitxpro-0.6.3/social_auth_mitxpro/backends_test.py` & `social_auth_mitxpro-0.7.0/social_auth_mitxpro/backends_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Tests for our backend"""
+
 from urllib.parse import urljoin
 
 import pytest
 
 from social_auth_mitxpro.backends import MITxProOAuth2
 
-
 # pylint: disable=redefined-outer-name
 
 
-@pytest.fixture
+@pytest.fixture()
 def strategy(mocker):
     """Mock strategy"""
     return mocker.Mock()
 
 
-@pytest.fixture
+@pytest.fixture()
 def backend(strategy):
     """MITxProOAuth2 backend fixture"""
     return MITxProOAuth2(strategy)
 
 
 @pytest.mark.parametrize(
-    "response, expected",
+    "response, expected",  # noqa: PT006
     [
         (
             {"username": "abc123", "email": "user@example.com", "name": "Jane Doe"},
             {"username": "abc123", "email": "user@example.com", "name": "Jane Doe"},
         ),
         ({"username": "abc123"}, {"username": "abc123", "email": "", "name": ""}),
     ],
@@ -34,25 +34,25 @@
 def test_get_user_details(backend, response, expected):
     """Test that get_user_details produces expected results"""
     assert backend.get_user_details(response) == expected
 
 
 def test_user_data(backend, strategy, mocked_responses):
     """Tests that the backend makes a correct appropriate request"""
-    access_token = "user_token"
+    access_token = "user_token"  # noqa: S105
     api_root = "http://xpro.example.com/"
     response = {"username": "abc123", "email": "user@example.com", "name": "Jane Doe"}
 
     mocked_responses.add(
         mocked_responses.GET, urljoin(api_root, "/api/users/me"), json=response
     )
     settings = {"API_ROOT": api_root}
 
-    def _setting(name, *, backend, default=None):  # pylint: disable=unused-argument
-        """Dummy setting func"""
+    def _setting(name, *, backend, default=None):  # pylint: disable=unused-argument  # noqa: ARG001
+        """Dummy setting func"""  # noqa: D401
         return settings.get(name, default)
 
     strategy.setting.side_effect = _setting
 
     assert backend.user_data(access_token) == response
 
     request, _ = mocked_responses.calls[0]
```

### Comparing `social_auth_mitxpro-0.6.3/PKG-INFO` & `social_auth_mitxpro-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: social-auth-mitxpro
-Version: 0.6.3
+Version: 0.7.0
 Summary: python-social-auth backend for mitxpro
 Home-page: https://pypi.org/project/social-auth-mitxpro
 License: MIT
 Author: MIT Office of Open Learning
 Author-email: mitx-devops@mit.edu
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.0.0,<24.0.0)
 Requires-Dist: social-auth-core (>=4.1.0,<5.0.0)
 Project-URL: Repository, https://github.com/mitodl/social-auth-mitxpro/
 Description-Content-Type: text/markdown
 
 
 social-auth-mitxpro
 ---
 
 
 #### Prerequisites
 
 - [`pyenv`](https://github.com/pyenv/pyenv#installation) for managing python versions
-  - Install `python3.6` and `python2.7`
+  - Install `python3.8` and `python3.11`
 - `pip install tox tox-pyenv` for running tests and discovering python versions from `pyenv`
 - [`poetry`](https://poetry.eustace.io/docs/#installation) for building, testing, and releasing
 
 If this is your first time using `poetry`, you'll need to configure your pypi credentials via:
 - Configure pypi repository:
   - `poetry config http-basic.pypi USERNAME PASSWORD`
 - Configure testpypi repository:
   - `poetry config repositories.testpypi https://test.pypi.org/legacy`
   - `poetry config http-basic.testpypi USERNAME PASSWORD`
 
 **NOTE:** when running `poetry` commands, particularly `pylint` and `black`, you must `python3.6`
 
 #### Testing
 
-You can just run `tox` locally to test, lint, and check formatting in the supported python versions. This works by having `tox` manage the virtualenvs, which `poetry` then detects and uses. Note that some of the tools (e.g. `pylint`, `black`) only support running in `python3.6` and this is reflected in `tox.ini`.
+You can just run `tox` locally to test, lint, and check formatting in the supported python versions. This works by having `tox` manage the virtualenvs, which `poetry` then detects and uses.
 
 Run individual commands can be run interactively in a `poetry shell` session or directly via `poetry run CMD`:
 
 - `pytest` - run python tests
-- `pylint` - lint python code
-- `black .` - format python code
+- `ruff check` - lint python code
+- `ruff format` - format python code
 
 #### Building
 
 - `poetry build` - builds a pip-installable package into `dist/`
 
 #### Releasing
```

