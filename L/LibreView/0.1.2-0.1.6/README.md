# Comparing `tmp/LibreView-0.1.2.tar.gz` & `tmp/LibreView-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibreView-0.1.2.tar", last modified: Thu Feb 22 08:02:41 2024, max compression
+gzip compressed data, was "LibreView-0.1.6.tar", last modified: Thu May 30 11:26:23 2024, max compression
```

## Comparing `LibreView-0.1.2.tar` & `LibreView-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 08:02:41.025163 LibreView-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-02-22 08:02:41.008648 LibreView-0.1.2/LibreView/
--rw-rw-rw-   0        0        0      497 2024-02-22 08:01:25.000000 LibreView-0.1.2/LibreView/LibreView.py
--rw-rw-rw-   0        0        0       42 2024-02-22 07:02:46.000000 LibreView-0.1.2/LibreView/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 08:02:41.017656 LibreView-0.1.2/LibreView/models/
--rw-rw-rw-   0        0        0      553 2024-02-22 07:19:36.000000 LibreView-0.1.2/LibreView/models/Connection.py
--rw-rw-rw-   0        0        0      226 2024-02-21 11:09:16.000000 LibreView-0.1.2/LibreView/models/Device.py
--rw-rw-rw-   0        0        0      996 2024-02-22 07:19:36.000000 LibreView-0.1.2/LibreView/models/GlucoseMeasurement.py
--rw-rw-rw-   0        0        0      315 2024-02-21 13:10:14.000000 LibreView-0.1.2/LibreView/models/Practice.py
--rw-rw-rw-   0        0        0      216 2024-02-21 13:10:14.000000 LibreView-0.1.2/LibreView/models/Sensor.py
--rw-rw-rw-   0        0        0      606 2024-02-22 07:06:22.000000 LibreView-0.1.2/LibreView/models/User.py
--rw-rw-rw-   0        0        0      296 2024-02-22 07:06:42.000000 LibreView-0.1.2/LibreView/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 08:02:41.018653 LibreView-0.1.2/LibreView/utils/
--rw-rw-rw-   0        0        0     2738 2024-02-22 07:59:32.000000 LibreView-0.1.2/LibreView/utils/API.py
--rw-rw-rw-   0        0        0       36 2024-02-22 07:02:55.000000 LibreView-0.1.2/LibreView/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 08:02:41.023657 LibreView-0.1.2/LibreView.egg-info/
--rw-rw-rw-   0        0        0      514 2024-02-22 08:02:40.000000 LibreView-0.1.2/LibreView.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-02-22 08:02:40.000000 LibreView-0.1.2/LibreView.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 08:02:40.000000 LibreView-0.1.2/LibreView.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 08:02:40.000000 LibreView-0.1.2/LibreView.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-02-22 08:02:40.000000 LibreView-0.1.2/LibreView.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      514 2024-02-22 08:02:41.023657 LibreView-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-22 08:02:41.022653 LibreView-0.1.2/Tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 08:46:03.000000 LibreView-0.1.2/Tests/__init__.py
--rw-rw-rw-   0        0        0     3796 2024-02-22 07:26:50.000000 LibreView-0.1.2/Tests/test_api.py
--rw-rw-rw-   0        0        0     1903 2024-02-22 08:02:21.000000 LibreView-0.1.2/Tests/test_client.py
--rw-rw-rw-   0        0        0       42 2024-02-22 08:02:41.025163 LibreView-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-02-22 08:02:40.000000 LibreView-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:26:23.294335 LibreView-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:26:23.278561 LibreView-0.1.6/LibreView/
+-rw-rw-rw-   0        0        0      497 2024-02-22 08:01:25.000000 LibreView-0.1.6/LibreView/LibreView.py
+-rw-rw-rw-   0        0        0       42 2024-02-22 07:02:46.000000 LibreView-0.1.6/LibreView/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:26:23.287331 LibreView-0.1.6/LibreView/models/
+-rw-rw-rw-   0        0        0      553 2024-02-22 07:19:36.000000 LibreView-0.1.6/LibreView/models/Connection.py
+-rw-rw-rw-   0        0        0      226 2024-02-21 11:09:16.000000 LibreView-0.1.6/LibreView/models/Device.py
+-rw-rw-rw-   0        0        0      996 2024-02-22 07:19:36.000000 LibreView-0.1.6/LibreView/models/GlucoseMeasurement.py
+-rw-rw-rw-   0        0        0      315 2024-02-21 13:10:14.000000 LibreView-0.1.6/LibreView/models/Practice.py
+-rw-rw-rw-   0        0        0      216 2024-02-21 13:10:14.000000 LibreView-0.1.6/LibreView/models/Sensor.py
+-rw-rw-rw-   0        0        0      606 2024-02-22 07:06:22.000000 LibreView-0.1.6/LibreView/models/User.py
+-rw-rw-rw-   0        0        0      296 2024-02-22 07:06:42.000000 LibreView-0.1.6/LibreView/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:26:23.288329 LibreView-0.1.6/LibreView/utils/
+-rw-rw-rw-   0        0        0     3238 2024-05-30 11:22:43.000000 LibreView-0.1.6/LibreView/utils/API.py
+-rw-rw-rw-   0        0        0       36 2024-02-22 07:02:55.000000 LibreView-0.1.6/LibreView/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:26:23.293331 LibreView-0.1.6/LibreView.egg-info/
+-rw-rw-rw-   0        0        0      514 2024-05-30 11:26:23.000000 LibreView-0.1.6/LibreView.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-30 11:26:23.000000 LibreView-0.1.6/LibreView.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 11:26:23.000000 LibreView-0.1.6/LibreView.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:26:23.000000 LibreView-0.1.6/LibreView.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 11:26:23.000000 LibreView-0.1.6/LibreView.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      514 2024-05-30 11:26:23.293331 LibreView-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 11:26:23.292331 LibreView-0.1.6/Tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 08:46:03.000000 LibreView-0.1.6/Tests/__init__.py
+-rw-rw-rw-   0        0        0     3796 2024-05-30 11:23:21.000000 LibreView-0.1.6/Tests/test_api.py
+-rw-rw-rw-   0        0        0     1903 2024-02-22 08:02:21.000000 LibreView-0.1.6/Tests/test_client.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:26:23.294335 LibreView-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-30 11:26:22.000000 LibreView-0.1.6/setup.py
```

### Comparing `LibreView-0.1.2/LibreView/models/Connection.py` & `LibreView-0.1.6/LibreView/models/Connection.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.2/LibreView/models/GlucoseMeasurement.py` & `LibreView-0.1.6/LibreView/models/GlucoseMeasurement.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.2/LibreView/models/User.py` & `LibreView-0.1.6/LibreView/models/User.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.2/LibreView/utils/API.py` & `LibreView-0.1.6/LibreView/utils/API.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import Optional
 import requests
 from LibreView.models import User, Connection
 
 
 def reauth_on_fail(func):
     def wrapper(*args):
         try:
@@ -14,38 +14,44 @@
                 return func(*args)
             raise e
 
     return wrapper
 
 
 class API:
-    username: str
-    password: str
-    base_url = "https://api.libreview.io"
-    client = requests.session()
-    product = "llu.android"
-    version = "4.7"
-
-    def __init__(self, username: str, password: str):
+    def __init__(self, username: str, password: str, region: Optional[str] = None):
+        self.base_url = "https://api.libreview.io"
+        if region:
+            self.base_url = f"https://api-{region}.libreview.io"
+        self.client = requests.session()
+        self.product = "llu.android"
+        self.version = "4.7"
         self.username = username
         self.password = password
         self.client.headers["product"] = self.product
         self.client.headers["version"] = self.version
+        self.authenticate()
 
     def authenticate(self):
         r = self.client.post(
             f"{self.base_url}/llu/auth/login",
             json={
                 "email": self.username,
                 "password": self.password,
             },
+            verify=False
         )
         r.raise_for_status()
         content = r.json()
 
+        if content and content.get("status") == 0 and content["data"].get("redirect", False):
+            region = content["data"]["region"]
+            self.base_url = f"https://api-{region}.libreview.io"
+            return self.authenticate()
+
         # status 0 == login successfull
         if content and content.get("status") == 0:
             self.set_token(content["data"]["authTicket"]["token"])
             return
 
         # status 4 == missing term accepts
         if content and content.get("status") == 4:
@@ -63,29 +69,32 @@
 
     def accept_terms(self, token):
         r = self.client.post(
             f"{self.base_url}/llu/auth/login",
             headers={
                 "Authorization": f"Bearer {token}",
             },
+            verify=False
         )
         r.raise_for_status()
         content = r.json()
         if content and content.get("status") == 0:
             self.set_token(content["data"]["authTicket"]["token"])
             return
 
     @reauth_on_fail
     def get_user(self) -> User:
         r = self.client.get(
             f"{self.base_url}/user",
+            verify=False
         )
         r.raise_for_status()
         return User.from_dict(r.json()["data"]["user"])
 
     @reauth_on_fail
-    def get_connections(self) -> List[Connection]:
+    def get_connections(self) -> list[Connection]:
         r = self.client.get(
             f"{self.base_url}/llu/connections",
+            verify=False
         )
         r.raise_for_status()
         return Connection.from_list(r.json()["data"])
```

### Comparing `LibreView-0.1.2/LibreView.egg-info/PKG-INFO` & `LibreView-0.1.6/LibreView.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibreView
-Version: 0.1.2
+Version: 0.1.6
 Summary: API interface for LibreView / LibreLinkUp glucose readings
 Home-page: https://github.com/PTST/LibreView_Py
 Author: PTST
 Author-email: patrick@steffensen.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LibreView-0.1.2/LibreView.egg-info/SOURCES.txt` & `LibreView-0.1.6/LibreView.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.2/PKG-INFO` & `LibreView-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibreView
-Version: 0.1.2
+Version: 0.1.6
 Summary: API interface for LibreView / LibreLinkUp glucose readings
 Home-page: https://github.com/PTST/LibreView_Py
 Author: PTST
 Author-email: patrick@steffensen.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LibreView-0.1.2/Tests/test_api.py` & `LibreView-0.1.6/Tests/test_api.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.2/Tests/test_client.py` & `LibreView-0.1.6/Tests/test_client.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.2/setup.py` & `LibreView-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LibreView",
-    version="0.1.2",
+    version="0.1.6",
     author="PTST",
     author_email="patrick@steffensen.io",
     description="API interface for LibreView / LibreLinkUp glucose readings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PTST/LibreView_Py",
     packages=setuptools.find_packages(),
```

