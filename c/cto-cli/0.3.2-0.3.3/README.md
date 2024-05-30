# Comparing `tmp/cto_cli-0.3.2.tar.gz` & `tmp/cto_cli-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cto_cli-0.3.2.tar", max compression
+gzip compressed data, was "cto_cli-0.3.3.tar", max compression
```

## Comparing `cto_cli-0.3.2.tar` & `cto_cli-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-05-29 14:25:25.239571 cto_cli-0.3.2/LICENSE
--rw-r--r--   0        0        0      233 2024-05-29 14:25:25.239571 cto_cli-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-05-29 14:25:25.239571 cto_cli-0.3.2/cto_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:25:25.239571 cto_cli-0.3.2/cto_cli/ecs/api/__init__.py
--rw-r--r--   0        0        0     8800 2024-05-29 14:25:25.239571 cto_cli-0.3.2/cto_cli/ecs/api/connector.py
--rw-r--r--   0        0        0        0 2024-05-29 14:25:25.239571 cto_cli-0.3.2/cto_cli/ecs/commands/__init__.py
--rw-r--r--   0        0        0     4043 2024-05-29 14:25:25.239571 cto_cli-0.3.2/cto_cli/ecs/commands/config.py
--rw-r--r--   0        0        0     2110 2024-05-29 14:25:25.239571 cto_cli-0.3.2/cto_cli/ecs/commands/users.py
--rw-r--r--   0        0        0        0 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/local/__init__.py
--rw-r--r--   0        0        0      451 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/local/commands.py
--rw-r--r--   0        0        0     7333 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/local/files.py
--rw-r--r--   0        0        0     7384 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/local/operations.py
--rw-r--r--   0        0        0     3266 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/local/settings.py
--rw-r--r--   0        0        0     1832 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/local/validators.py
--rw-r--r--   0        0        0     3837 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/ecs/main.py
--rw-r--r--   0        0        0      652 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/main.py
--rw-r--r--   0        0        0      213 2024-05-29 14:25:25.243571 cto_cli-0.3.2/cto_cli/utils/errors.py
--rw-r--r--   0        0        0     1580 2024-05-29 14:25:26.115575 cto_cli-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 15:00:54.924536 cto_cli-0.3.3/LICENSE
+-rw-r--r--   0        0        0      233 2024-05-30 15:00:54.928536 cto_cli-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/api/__init__.py
+-rw-r--r--   0        0        0     9505 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/api/connector.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/commands/__init__.py
+-rw-r--r--   0        0        0     4043 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/commands/config.py
+-rw-r--r--   0        0        0     2110 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/commands/users.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/local/__init__.py
+-rw-r--r--   0        0        0      451 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/local/commands.py
+-rw-r--r--   0        0        0     7333 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/local/files.py
+-rw-r--r--   0        0        0     7384 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/local/operations.py
+-rw-r--r--   0        0        0     3266 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/local/settings.py
+-rw-r--r--   0        0        0     1832 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/local/validators.py
+-rw-r--r--   0        0        0     3944 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/ecs/main.py
+-rw-r--r--   0        0        0      652 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/main.py
+-rw-r--r--   0        0        0      213 2024-05-30 15:00:54.928536 cto_cli-0.3.3/cto_cli/utils/errors.py
+-rw-r--r--   0        0        0     1599 2024-05-30 15:00:55.872543 cto_cli-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 cto_cli-0.3.3/PKG-INFO
```

### Comparing `cto_cli-0.3.2/LICENSE` & `cto_cli-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/api/connector.py` & `cto_cli-0.3.3/cto_cli/ecs/api/connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,37 @@
 from pathlib import Path
 from typing import Any
 
 import requests
 from requests import HTTPError, ConnectionError, Timeout
 from rich import print, print_json
 from rich.syntax import Syntax
-
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, RetryCallState
 from cto_cli.ecs.local.settings import load_ecs_settings, SettingsNotFound
 from cto_cli.utils.errors import print_error
 
 
+class ServerError(Exception):
+    pass
+
+
 class ApiTokenError(Exception):
     pass
 
 
 class ApiConnectionError(Exception):
     pass
 
 
+def server_retry_callback(retry_state: RetryCallState):
+    del retry_state
+
+    print_error('Internal server error', exit=True)
+
+
 class APIConnector:
     def __init__(self, load_settings: bool = True, url: str | None = None, headers: dict | None = None):
         self._headers = headers
         self._url = url
 
         if load_settings:
             self._set_api_details()
@@ -65,46 +75,62 @@
         }
         self._url = settings.url
 
     @staticmethod
     def _print_response(response: requests.Response) -> None:
         if response.headers['content-type'] == 'application/json':
             response_json = response.json()
+
+            if 'status' in response_json and len(response_json) == 1:
+                print(f'[green]{response_json["status"]}[/green]')
+                return
+
             print_json(data=response_json)
         elif response.headers['content-type'] == 'application/yaml':
             print(Syntax(response.text, 'yaml'))
         else:
             print(Syntax(response.text, 'text'))
 
+    @retry(
+        stop=stop_after_attempt(3),
+        retry=retry_if_exception_type(ServerError),
+        retry_error_callback=server_retry_callback,
+    )
     def _make_request(
         self,
         method: str,
         url: str,
         headers: dict | None = None,
         json: dict | None = None,
         params: dict | None = None,
         files: dict | None = None,
         **kwargs,
     ):
         if not headers:
             headers = {}
 
         try:
-            return requests.request(
+            response = requests.request(
                 method,
                 url=f'{self._url}/{url}',
                 headers={**self._headers, **headers},
                 json=json,
                 files=files,
                 params=params,
                 **kwargs,
             )
         except requests.exceptions.RequestException:
             print_error('Cannot connect to ECS API', exit=True)
 
+        else:
+            if response.status_code >= 500:
+                raise ServerError
+
+            return response
+
     # USERS
     def create_user(
         self,
         username: str,
         given_name: str,
         family_name: str,
         email: str,
```

### Comparing `cto_cli-0.3.2/cto_cli/ecs/commands/config.py` & `cto_cli-0.3.3/cto_cli/ecs/commands/config.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/commands/users.py` & `cto_cli-0.3.3/cto_cli/ecs/commands/users.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/local/files.py` & `cto_cli-0.3.3/cto_cli/ecs/local/files.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/local/operations.py` & `cto_cli-0.3.3/cto_cli/ecs/local/operations.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/local/settings.py` & `cto_cli-0.3.3/cto_cli/ecs/local/settings.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/local/validators.py` & `cto_cli-0.3.3/cto_cli/ecs/local/validators.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/cto_cli/ecs/main.py` & `cto_cli-0.3.3/cto_cli/ecs/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,8 +97,12 @@
         reinit = typer.confirm('Do you want to re-init it?', abort=True)
 
     if reinit is True or current_settings is None:
         check_working_dir_is_empty()
         store_and_validate_settings()
         check_versions_compatibility()
         create_repo_dir()
-        print('[green]Your credentials were saved, run [b]cto ecs config pull[/b] to start[/green]')
+        config.pull_remote_repo(APIConnector())
+        print(
+            '[green]Your credentials were saved and config has been downloaded, [b]cd repo[/b] to work with it['
+            '/green]'
+        )
```

### Comparing `cto_cli-0.3.2/cto_cli/main.py` & `cto_cli-0.3.3/cto_cli/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.2/pyproject.toml` & `cto_cli-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "cto-cli"
-version = "0.3.2"
+version = "0.3.3"
 description = "The CTO cli"
 authors = ["CTO <support@cloudtechnologyoffice.com>"]
 readme = "README.md"
 homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest"
 repository = "https://github.com/Cloud-Technology-Office/cto-cli"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = "0.9.0"
 rich = "13.6.0"
 requests = "2.31.0"
 PyYAML = "6.0.1"
+tenacity = "8.2.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "8.0.0"
 pytest-mock = "3.12.0"
 responses = "0.25.0"
 
 [build-system]
```

### Comparing `cto_cli-0.3.2/PKG-INFO` & `cto_cli-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cto-cli
-Version: 0.3.2
+Version: 0.3.3
 Summary: The CTO cli
 Home-page: https://doc.cloudtechnologyoffice.com/ecs/latest
 License: Apache-2.0
 Author: CTO
 Author-email: support@cloudtechnologyoffice.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.6.0)
+Requires-Dist: tenacity (==8.2.3)
 Requires-Dist: typer (==0.9.0)
 Project-URL: Repository, https://github.com/Cloud-Technology-Office/cto-cli
 Description-Content-Type: text/markdown
 
 # CTO cli
 
 CLI for ECS by CTO.
```

