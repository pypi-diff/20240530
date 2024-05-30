# Comparing `tmp/salt_infisical-1.0.0.tar.gz` & `tmp/salt_infisical-2.0.0.tar.gz`

## Comparing `salt_infisical-1.0.0.tar` & `salt_infisical-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/src/salt_infisical/__about__.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/src/salt_infisical/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/LICENSE
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/README.md
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 salt_infisical-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/src/salt_infisical/__about__.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/src/salt_infisical/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/LICENSE
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/PKG-INFO
```

### Comparing `salt_infisical-1.0.0/src/salt_infisical/__init__.py` & `salt_infisical-2.0.0/src/salt_infisical/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # SPDX-FileCopyrightText: 2023-present Jonathan Treffler <mail@jonathan-treffler.de>
 #
 # SPDX-License-Identifier: MIT
 
 
-def get_token():
-    path = "/etc/salt/infisical.token"    
+def get_config():
+    import json
+
+    path = "/etc/salt/infisical_config.json"
     f = open(path, "r")
-    token = ""
+    config = {}
 
     try:
-        token = f.readline().strip('\n')
+        config = json.load(f)
     finally:
         f.close()
-        return token
+        return config
 
 def get_client():
-    from infisical import InfisicalClient
-    return InfisicalClient(token = get_token(), debug=True)
+    from infisical_client import ClientSettings, InfisicalClient, AuthenticationOptions, UniversalAuthMethod
+
+    config = get_config()
+
+    return InfisicalClient(
+        ClientSettings(
+            auth = AuthenticationOptions(
+                universal_auth = UniversalAuthMethod(**config)
+            )
+        )
+    )
 
 def secret_bundle_to_dict(secret_bundle):
     result = {}
     result[getattr(secret_bundle, "secret_name")] = getattr(secret_bundle, "secret_value")
     return result
 
 def secret_bundles_to_dict(secret_bundles):
```

### Comparing `salt_infisical-1.0.0/LICENSE` & `salt_infisical-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt_infisical-1.0.0/pyproject.toml` & `salt_infisical-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "infisical",
+  "infisical-python",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/salt-infisical#readme"
 Issues = "https://github.com/unknown/salt-infisical/issues"
 Source = "https://github.com/unknown/salt-infisical"
```

### Comparing `salt_infisical-1.0.0/PKG-INFO` & `salt_infisical-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: salt-infisical
-Version: 1.0.0
+Version: 2.0.0
 Project-URL: Documentation, https://github.com/unknown/salt-infisical#readme
 Project-URL: Issues, https://github.com/unknown/salt-infisical/issues
 Project-URL: Source, https://github.com/unknown/salt-infisical
 Author-email: Jonathan Treffler <mail@jonathan-treffler.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: infisical
+Requires-Dist: infisical-python
 Description-Content-Type: text/markdown
 
 # salt-infisical
 
 [![PyPI - Version](https://img.shields.io/pypi/v/salt-infisical.svg)](https://pypi.org/project/salt-infisical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/salt-infisical.svg)](https://pypi.org/project/salt-infisical)
 
@@ -31,13 +31,27 @@
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
-pip install salt-infisical
+salt-pip install salt-infisical
+echo "[your infisical token]" > /etc/salt/infisical.token
 ```
 
+## Usage
+
+Add a pillar file for every infisical folder you want to fetch:
+
+```python
+#!py
+def run():
+    from salt_infisical import fetch_infisical_secrets
+    return fetch_infisical_secrets("prod", "/some/path")
+```
+
+
+
 ## License
 
 `salt-infisical` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

