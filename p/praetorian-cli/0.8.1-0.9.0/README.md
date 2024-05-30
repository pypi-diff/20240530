# Comparing `tmp/praetorian_cli-0.8.1.tar.gz` & `tmp/praetorian_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praetorian_cli-0.8.1.tar", last modified: Mon Apr 15 19:12:40 2024, max compression
+gzip compressed data, was "praetorian_cli-0.9.0.tar", last modified: Sat Apr 20 00:19:52 2024, max compression
```

## Comparing `praetorian_cli-0.8.1.tar` & `praetorian_cli-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.745303 praetorian_cli-0.8.1/
--rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-15 19:12:40.745166 praetorian_cli-0.8.1/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)     1111 2024-03-23 18:37:05.000000 praetorian_cli-0.8.1/README.md
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.722090 praetorian_cli-0.8.1/praetorian_cli/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian_cli-0.8.1/praetorian_cli/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)      674 2024-04-08 21:35:19.000000 praetorian_cli-0.8.1/praetorian_cli/cli.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.734631 praetorian_cli-0.8.1/praetorian_cli/handlers/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2833 2024-04-13 14:46:54.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/account.py
--rw-r--r--   0 privateducky   (501) staff       (20)     5145 2024-04-15 11:06:17.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/backend.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1186 2024-04-11 14:42:01.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.735740 praetorian_cli-0.8.1/praetorian_cli/sdk/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     3424 2024-04-14 13:45:08.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/chaos.py
--rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/keychain.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.744310 praetorian_cli-0.8.1/praetorian_cli/sdk/test/
--rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-08 21:35:19.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_file_upload.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2539 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_job_capabilities.py
--rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-10 11:11:30.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_link_account.py
--rw-r--r--   0 privateducky   (501) staff       (20)      757 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_manual_risk.py
--rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-08 21:35:19.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_nvd.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1848 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_seed.py
--rw-r--r--   0 privateducky   (501) staff       (20)      909 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.744859 praetorian_cli-0.8.1/praetorian_cli.egg-info/
--rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/SOURCES.txt
--rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/dependency_links.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/entry_points.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/requires.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/top_level.txt
--rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian_cli-0.8.1/pyproject.toml
--rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-15 19:12:40.746073 praetorian_cli-0.8.1/setup.cfg
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-20 00:19:52.486108 praetorian_cli-0.9.0/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1610 2024-04-20 00:19:52.485906 praetorian_cli-0.9.0/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)     1108 2024-04-18 10:40:49.000000 praetorian_cli-0.9.0/README.md
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-20 00:19:52.477408 praetorian_cli-0.9.0/praetorian_cli/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian_cli-0.9.0/praetorian_cli/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      674 2024-04-08 21:35:19.000000 praetorian_cli-0.9.0/praetorian_cli/cli.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-20 00:19:52.480459 praetorian_cli-0.9.0/praetorian_cli/handlers/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian_cli-0.9.0/praetorian_cli/handlers/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2708 2024-04-20 00:19:16.000000 praetorian_cli-0.9.0/praetorian_cli/handlers/account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     5608 2024-04-18 10:40:49.000000 praetorian_cli-0.9.0/praetorian_cli/handlers/backend.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1186 2024-04-11 14:42:01.000000 praetorian_cli-0.9.0/praetorian_cli/handlers/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-20 00:19:52.481164 praetorian_cli-0.9.0/praetorian_cli/sdk/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3837 2024-04-19 17:26:58.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/chaos.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/keychain.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-20 00:19:52.485052 praetorian_cli-0.9.0/praetorian_cli/sdk/test/
+-rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-08 21:35:19.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_file_upload.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2539 2024-04-15 14:23:33.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_job_capabilities.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-10 11:11:30.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_link_account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      757 2024-04-15 14:23:33.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_manual_risk.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-08 21:35:19.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_nvd.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1848 2024-04-15 14:23:33.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_seed.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      909 2024-04-15 14:23:33.000000 praetorian_cli-0.9.0/praetorian_cli/sdk/test/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-20 00:19:52.485649 praetorian_cli-0.9.0/praetorian_cli.egg-info/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1610 2024-04-20 00:19:52.000000 praetorian_cli-0.9.0/praetorian_cli.egg-info/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-20 00:19:52.000000 praetorian_cli-0.9.0/praetorian_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-20 00:19:52.000000 praetorian_cli-0.9.0/praetorian_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-20 00:19:52.000000 praetorian_cli-0.9.0/praetorian_cli.egg-info/entry_points.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-20 00:19:52.000000 praetorian_cli-0.9.0/praetorian_cli.egg-info/requires.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-20 00:19:52.000000 praetorian_cli-0.9.0/praetorian_cli.egg-info/top_level.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian_cli-0.9.0/pyproject.toml
+-rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-20 00:19:52.486567 praetorian_cli-0.9.0/setup.cfg
```

### Comparing `praetorian_cli-0.8.1/PKG-INFO` & `praetorian_cli-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: click>8
 Requires-Dist: boto3
 Requires-Dist: requests
 
 # Praetorian CLI
 
-The CLI is a fully-featured companion to the Chaos UI, which is hosted at research.praetorian.com.
+The CLI is a fully-featured companion to the Chaos UI, which is hosted at chaos.praetorian.com.
 
 ## Install
 
 Python 3.8+ and PIP are required.
 
 ```zsh
 pip install praetorian-cli
```

### Comparing `praetorian_cli-0.8.1/README.md` & `praetorian_cli-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Praetorian CLI
 
-The CLI is a fully-featured companion to the Chaos UI, which is hosted at research.praetorian.com.
+The CLI is a fully-featured companion to the Chaos UI, which is hosted at chaos.praetorian.com.
 
 ## Install
 
 Python 3.8+ and PIP are required.
 
 ```zsh
 pip install praetorian-cli
```

### Comparing `praetorian_cli-0.8.1/praetorian_cli/cli.py` & `praetorian_cli-0.9.0/praetorian_cli/cli.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/handlers/account.py` & `praetorian_cli-0.9.0/praetorian_cli/handlers/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,14 @@
 def my_accounts(controller):
     """ Fetch my associated accounts """
     result = controller.my(dict(key=f'#account'))
     for hit in result.get('accounts', []):
         print(f"{hit['key']}")
 
 
-@chaos.command('link-chaos')
-@click.pass_obj
-@handle_api_error
-@click.argument('username')
-@click.option('-config', '--config', default="", help="Add an optional configuration")
-def link_account(controller, username, config):
-    """ Link another Chaos account to yours """
-    result = controller.link_account(username=username, config=config)
-    print(f"{result['key']}")
-
-
 @chaos.command('unlink')
 @click.pass_obj
 @handle_api_error
 @click.argument('username')
 def unlink_account(controller, username):
     """ Unlink a Chaos account from yours """
     result = controller.unlink_account(username=username)
@@ -48,21 +37,30 @@
     controller.link_account(username="hook", config=pin)
     username = b64encode(controller.keychain.username.encode('utf8'))
     encoded_string = username.decode('utf8')
     encoded_username = encoded_string.rstrip('=')
     print(f'{controller.keychain.api}/hook/{encoded_username}/{pin}')
 
 
+@chaos.command('link-chaos')
+@click.pass_obj
+@handle_api_error
+@click.argument('username')
+def link_account(controller, username):
+    """ Link another Chaos account to yours """
+    controller.link_account(username, config={})
+
+
 @chaos.command('link-slack')
 @click.pass_obj
 @handle_api_error
 @click.argument('webhook')
 def link_slack(controller, webhook):
     """ Send all new risks to Slack """
-    controller.link_account('slack', webhook)
+    controller.link_account('slack', {'webhook': webhook})
 
 
 @chaos.command('link-jira')
 @click.pass_obj
 @handle_api_error
 @click.argument('domain')
 @click.argument('access_token')
@@ -87,8 +85,8 @@
 
 @chaos.command('link-github')
 @click.pass_obj
 @handle_api_error
 @click.argument('pat')
 def link_github(controller, pat):
     """ Allow Chaos to scan your private repos """
-    controller.link_account('github', pat)
+    controller.link_account('github', {'pat': pat})
```

### Comparing `praetorian_cli-0.8.1/praetorian_cli/handlers/backend.py` & `praetorian_cli-0.9.0/praetorian_cli/handlers/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 def my_risks(controller, seed):
     """ Fetch current risks """
     result = controller.my(dict(key=f'#risk#{seed}'))
     for hit in result.get('risks', []):
         print(f"{hit['key']}")
 
 
-@chaos.command('services')
+@chaos.command('technology')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
-def my_services(controller, seed):
-    """ Fetch recently seen services """
-    result = controller.my(dict(key=f'#service#{seed}'))
-    for hit in result.get('services', []):
+def my_technology(controller, seed):
+    """ Fetch recently seen technology """
+    result = controller.my(dict(key=f'#tech#{seed}'))
+    for hit in result.get('technology', []):
         print(f"{hit['key']}")
 
 
 @chaos.command('jobs')
 @click.pass_obj
 @handle_api_error
 @click.option('-updated', '--updated', default="", help="Fetch jobs since date")
@@ -86,47 +86,59 @@
 @chaos.command('add-seed')
 @click.pass_obj
 @handle_api_error
 @click.argument('seed')
 @click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
 @click.option('-comment', '--comment', default="", help="Add a comment")
 def add_seed(controller, seed, status, comment=""):
-    """ Add a new seed domain """
-    controller.add_asset(seed, status=status, comment=comment)
+    """ Add a new seed """
+    controller.add_seed(seed, status=status, comment=comment)
 
 
 @chaos.command('delete-seed')
 @click.pass_obj
 @handle_api_error
 @click.argument('seed')
 def delete_seed(controller, seed):
     """ Delete any seed """
-    controller.delete_asset(f'#seed#{seed}')
+    controller.delete_seed(f'#seed#{seed}')
+
+
+@chaos.command('update-seed')
+@click.pass_obj
+@handle_api_error
+@click.argument('key')
+@click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
+@click.option('-comment', '--comment', help="Add a comment")
+def update_seed(controller, key, status, comment=''):
+    """ Update any seed """
+    controller.update_seed(key, status=status, comment=comment)
 
 
 @chaos.command('update-asset')
 @click.pass_obj
 @handle_api_error
 @click.argument('key')
 @click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
 @click.option('-comment', '--comment', help="Add a comment")
 def update_asset(controller, key, status, comment=''):
-    """ Update any asset or seed """
+    """ Update any asset """
     controller.update_asset(key, status=status, comment=comment)
 
 
 @chaos.command('add-risk')
 @click.pass_obj
 @handle_api_error
 @click.argument('key')
 @click.option('-name', '--name', required=True, help="Generic risk identifier")
 @click.option('-status', '--status', type=click.Choice([s.value for s in Status]), required=False, default='TO')
-def add_risk(controller, key, name, status):
+@click.option('-comment', '--comment', help="Add a comment")
+def add_risk(controller, key, name, status, comment):
     """ Apply a risk to an asset key """
-    print(controller.add_risk(key, name, status))
+    print(controller.add_risk(key, name, status, comment))
 
 
 @chaos.command('upload')
 @click.pass_obj
 @handle_api_error
 @click.argument('name')
 def upload(controller, name):
```

### Comparing `praetorian_cli-0.8.1/praetorian_cli/handlers/utils.py` & `praetorian_cli-0.9.0/praetorian_cli/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/chaos.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/chaos.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,50 +14,59 @@
     def my(self, params: dict) -> {}:
         resp = requests.get(f"{self.keychain.api}/my", params=params, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def add_risk(self, key: str, name: str, status: str):
-        data = dict(key=key, name=name, status=status)
+    def add_risk(self, key: str, name: str, status: str, comment: str):
+        data = dict(key=key, name=name, status=status, comment=comment)
 
-        resp = requests.post(f"{self.keychain.api}/risk", json=data, headers=self.keychain.headers)
+        resp = requests.put(f"{self.keychain.api}/risk", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def add_asset(self, seed: str, status: str, comment: str = "") -> {}:
+    def add_seed(self, seed: str, status: str, comment: str = "") -> {}:
         data = {"seed": seed, "status": status, "comment": comment}
 
-        resp = requests.post(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
+        resp = requests.post(f"{self.keychain.api}/seed", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def update_asset(self, key: str, status: str, comment: str = "") -> {}:
+    def update_seed(self, key: str, status: str, comment: str = "") -> {}:
         data = {"key": key, "status": status, "comment": comment}
 
-        resp = requests.put(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
+        resp = requests.put(f"{self.keychain.api}/seed", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def delete_asset(self, key: str) -> {}:
-        resp = requests.delete(f"{self.keychain.api}/asset", json={'key': key}, headers=self.keychain.headers)
+    def delete_seed(self, key: str) -> {}:
+        resp = requests.delete(f"{self.keychain.api}/seed", json={'key': key}, headers=self.keychain.headers)
+        if not resp.ok:
+            raise Exception(f'[{resp.status_code}] Request failed')
+        return resp.json()
+
+    @verify_credentials
+    def update_asset(self, key: str, status: str, comment: str = "") -> {}:
+        data = {"key": key, "status": status, "comment": comment}
+
+        resp = requests.put(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def link_account(self, username: str, config: str):
-        resp = requests.post(f"{self.keychain.api}/account/{username}", json={'config':config}, headers=self.keychain.headers)
+    def link_account(self, username: str, config: dict):
+        resp = requests.post(f"{self.keychain.api}/account/{username}", json={'config': config}, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
     def unlink_account(self, username: str):
         resp = requests.delete(f"{self.keychain.api}/account/{username}", headers=self.keychain.headers)
```

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/keychain.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/keychain.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_file_upload.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_job_capabilities.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_job_capabilities.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_link_account.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_link_account.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_manual_risk.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_manual_risk.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_nvd.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_nvd.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_seed.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/test_seed.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli/sdk/test/utils.py` & `praetorian_cli-0.9.0/praetorian_cli/sdk/test/utils.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/praetorian_cli.egg-info/PKG-INFO` & `praetorian_cli-0.9.0/praetorian_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: click>8
 Requires-Dist: boto3
 Requires-Dist: requests
 
 # Praetorian CLI
 
-The CLI is a fully-featured companion to the Chaos UI, which is hosted at research.praetorian.com.
+The CLI is a fully-featured companion to the Chaos UI, which is hosted at chaos.praetorian.com.
 
 ## Install
 
 Python 3.8+ and PIP are required.
 
 ```zsh
 pip install praetorian-cli
```

### Comparing `praetorian_cli-0.8.1/praetorian_cli.egg-info/SOURCES.txt` & `praetorian_cli-0.9.0/praetorian_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8.1/setup.cfg` & `praetorian_cli-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = praetorian-cli
-version = 0.8.1
+version = 0.9.0
 author = Praetorian Labs
 author_email = research@praetorian.com
 description = For interacting with the Chaos API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/praetorian-inc/praetorian-cli
 classifiers =
```

