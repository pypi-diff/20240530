# Comparing `tmp/escape_captivity-0.1.0.tar.gz` & `tmp/escape_captivity-1.1.0.tar.gz`

## Comparing `escape_captivity-0.1.0.tar` & `escape_captivity-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/compiler.sh
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/__main__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/detect_captive_portal.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/dispatcher.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/__init__.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/abellio.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/base.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/db_regio_southeast.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/db_station.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/enno.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/src/escape_captivity/solver/ice.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/.gitignore
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/README.md
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 escape_captivity-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/compiler.sh
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/__init__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/__main__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/detect_captive_portal.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/dispatcher.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/cli/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/__init__.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/abellio.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/base.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/db_regio_southeast.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/db_station.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/enno.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/src/escape_captivity/solver/ice.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/.gitignore
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/README.md
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 escape_captivity-1.1.0/PKG-INFO
```

### Comparing `escape_captivity-0.1.0/.github/workflows/pypi-publish.yml` & `escape_captivity-1.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/detect_captive_portal.py` & `escape_captivity-1.1.0/src/escape_captivity/detect_captive_portal.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/dispatcher.py` & `escape_captivity-1.1.0/src/escape_captivity/dispatcher.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/cli/__init__.py` & `escape_captivity-1.1.0/src/escape_captivity/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/solver/abellio.py` & `escape_captivity-1.1.0/src/escape_captivity/solver/abellio.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/solver/base.py` & `escape_captivity-1.1.0/src/escape_captivity/solver/base.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/solver/db_regio_southeast.py` & `escape_captivity-1.1.0/src/escape_captivity/solver/db_regio_southeast.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/solver/db_station.py` & `escape_captivity-1.1.0/src/escape_captivity/solver/db_station.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 
 class DBStationSolver(BaseSolver):
     def applicable(self, portal_url: ParseResult) -> bool:
         return portal_url.netloc == "wifi.bahn.de"
 
     def solve(self, portal_url: ParseResult) -> bool:
-        r = requests.post(f"{portal_url.scheme}://{portal_url.netloc}/login",
-                          data={"oneSubscriptionForm_connect_policy_accept": "on", "login": "oneclick"},
-                          follow_redirects=False, #allow unsafe tls
-                          )
+        pre_request = requests.get(f"{portal_url.scheme}://{portal_url.netloc}")
+        if pre_request.url == 'https://wifi.bahn.de/cna/':
+            # For DB-Regio / Süwex; Maybe a new general system?
+            r = requests.post(f"{portal_url.scheme}://{portal_url.netloc}/cna/logon")
+        else:
+            r = requests.post(f"{portal_url.scheme}://{portal_url.netloc}/login",
+                              data={"oneSubscriptionForm_connect_policy_accept": "on", "login": "oneclick"},
+                              )
         if r.status_code in [302, 200]:
             return True
         return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `escape_captivity-0.1.0/src/escape_captivity/solver/enno.py` & `escape_captivity-1.1.0/src/escape_captivity/solver/enno.py`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/src/escape_captivity/solver/ice.py` & `escape_captivity-1.1.0/src/escape_captivity/solver/ice.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,14 @@
             "login.wifionice.de",
             "wifi.metronom.de", # Metronom / Icomera AB
         ]
 
     def solve(self, portal_url: ParseResult) -> bool:
         # Generate some random CSRF token
         csrf_token = ''.join(random.choices(string.ascii_letters + string.digits, k=33))
-        r = httpx.post(f"{portal_url.scheme}://{portal_url.netloc}/de/",
+        r = httpx.post(f"https://{portal_url.netloc}/de/",
                           data={"login": "true", "CSRFToken": csrf_token}, cookies=dict(csrf=csrf_token),
                           follow_redirects=False)
 
-        if r.status_code in [302, 200]:
+        if r.status_code in [302, 301, 200]:
             return True
         return False
```

### Comparing `escape_captivity-0.1.0/LICENSE.txt` & `escape_captivity-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/README.md` & `escape_captivity-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 -----
 
 **Table of Contents**
 
 - [About](#about)
 - [Installation](#installation)
+- [Usage](#usage)
 - [License](#license)
 
 ## About
 
 This is a tool designed to automate the process of solving captive portals, commonly found in public Wi-Fi networks.
 
 Currently solvers especially for multiple German railway providers are implemented.
@@ -23,10 +24,17 @@
 
 ## Installation
 
 ```console
 pip install escape-captivity
 ```
 
+# Usage
+
+Simply use any terminal to run the following command:
+```console
+escape-captivity
+```
+
 ## License
 
 `escape-captivity` is distributed under the terms of the [EUPL-1.2](https://spdx.org/licenses/EUPL-1.2.html) license.
```

### Comparing `escape_captivity-0.1.0/pyproject.toml` & `escape_captivity-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `escape_captivity-0.1.0/PKG-INFO` & `escape_captivity-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: escape-captivity
-Version: 0.1.0
+Version: 1.1.0
 Project-URL: Documentation, https://github.com/anjomro/escape-captivity#readme
 Project-URL: Issues, https://github.com/anjomro/escape-captivity/issues
 Project-URL: Source, https://github.com/anjomro/escape-captivity
 Author-email: anjomro <py@anjomro.de>
 License-Expression: EUPL-1.2
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -28,14 +28,15 @@
 
 -----
 
 **Table of Contents**
 
 - [About](#about)
 - [Installation](#installation)
+- [Usage](#usage)
 - [License](#license)
 
 ## About
 
 This is a tool designed to automate the process of solving captive portals, commonly found in public Wi-Fi networks.
 
 Currently solvers especially for multiple German railway providers are implemented.
@@ -46,10 +47,17 @@
 
 ## Installation
 
 ```console
 pip install escape-captivity
 ```
 
+# Usage
+
+Simply use any terminal to run the following command:
+```console
+escape-captivity
+```
+
 ## License
 
 `escape-captivity` is distributed under the terms of the [EUPL-1.2](https://spdx.org/licenses/EUPL-1.2.html) license.
```

