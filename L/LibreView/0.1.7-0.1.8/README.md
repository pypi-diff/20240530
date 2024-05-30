# Comparing `tmp/LibreView-0.1.7.tar.gz` & `tmp/LibreView-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibreView-0.1.7.tar", last modified: Thu May 30 11:41:03 2024, max compression
+gzip compressed data, was "LibreView-0.1.8.tar", last modified: Thu May 30 11:42:23 2024, max compression
```

## Comparing `LibreView-0.1.7.tar` & `LibreView-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 11:41:03.110075 LibreView-0.1.7/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:41:03.094186 LibreView-0.1.7/LibreView/
--rw-rw-rw-   0        0        0      544 2024-05-30 11:40:58.000000 LibreView-0.1.7/LibreView/LibreView.py
--rw-rw-rw-   0        0        0       42 2024-02-22 07:02:46.000000 LibreView-0.1.7/LibreView/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:41:03.102883 LibreView-0.1.7/LibreView/models/
--rw-rw-rw-   0        0        0      553 2024-02-22 07:19:36.000000 LibreView-0.1.7/LibreView/models/Connection.py
--rw-rw-rw-   0        0        0      226 2024-02-21 11:09:16.000000 LibreView-0.1.7/LibreView/models/Device.py
--rw-rw-rw-   0        0        0      996 2024-02-22 07:19:36.000000 LibreView-0.1.7/LibreView/models/GlucoseMeasurement.py
--rw-rw-rw-   0        0        0      315 2024-02-21 13:10:14.000000 LibreView-0.1.7/LibreView/models/Practice.py
--rw-rw-rw-   0        0        0      216 2024-02-21 13:10:14.000000 LibreView-0.1.7/LibreView/models/Sensor.py
--rw-rw-rw-   0        0        0      606 2024-02-22 07:06:22.000000 LibreView-0.1.7/LibreView/models/User.py
--rw-rw-rw-   0        0        0      296 2024-02-22 07:06:42.000000 LibreView-0.1.7/LibreView/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:41:03.103883 LibreView-0.1.7/LibreView/utils/
--rw-rw-rw-   0        0        0     3238 2024-05-30 11:22:43.000000 LibreView-0.1.7/LibreView/utils/API.py
--rw-rw-rw-   0        0        0       36 2024-02-22 07:02:55.000000 LibreView-0.1.7/LibreView/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:41:03.108075 LibreView-0.1.7/LibreView.egg-info/
--rw-rw-rw-   0        0        0      514 2024-05-30 11:41:03.000000 LibreView-0.1.7/LibreView.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-30 11:41:03.000000 LibreView-0.1.7/LibreView.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 11:41:03.000000 LibreView-0.1.7/LibreView.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 11:41:03.000000 LibreView-0.1.7/LibreView.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-30 11:41:03.000000 LibreView-0.1.7/LibreView.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      514 2024-05-30 11:41:03.109074 LibreView-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 11:41:03.108075 LibreView-0.1.7/Tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 08:46:03.000000 LibreView-0.1.7/Tests/__init__.py
--rw-rw-rw-   0        0        0     3796 2024-05-30 11:23:21.000000 LibreView-0.1.7/Tests/test_api.py
--rw-rw-rw-   0        0        0     1903 2024-02-22 08:02:21.000000 LibreView-0.1.7/Tests/test_client.py
--rw-rw-rw-   0        0        0       42 2024-05-30 11:41:03.110075 LibreView-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-30 11:41:02.000000 LibreView-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:42:23.186830 LibreView-0.1.8/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:42:23.171380 LibreView-0.1.8/LibreView/
+-rw-rw-rw-   0        0        0      544 2024-05-30 11:40:58.000000 LibreView-0.1.8/LibreView/LibreView.py
+-rw-rw-rw-   0        0        0       42 2024-02-22 07:02:46.000000 LibreView-0.1.8/LibreView/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:42:23.178833 LibreView-0.1.8/LibreView/models/
+-rw-rw-rw-   0        0        0      553 2024-02-22 07:19:36.000000 LibreView-0.1.8/LibreView/models/Connection.py
+-rw-rw-rw-   0        0        0      226 2024-02-21 11:09:16.000000 LibreView-0.1.8/LibreView/models/Device.py
+-rw-rw-rw-   0        0        0      996 2024-02-22 07:19:36.000000 LibreView-0.1.8/LibreView/models/GlucoseMeasurement.py
+-rw-rw-rw-   0        0        0      315 2024-02-21 13:10:14.000000 LibreView-0.1.8/LibreView/models/Practice.py
+-rw-rw-rw-   0        0        0      216 2024-02-21 13:10:14.000000 LibreView-0.1.8/LibreView/models/Sensor.py
+-rw-rw-rw-   0        0        0      606 2024-02-22 07:06:22.000000 LibreView-0.1.8/LibreView/models/User.py
+-rw-rw-rw-   0        0        0      296 2024-02-22 07:06:42.000000 LibreView-0.1.8/LibreView/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:42:23.180834 LibreView-0.1.8/LibreView/utils/
+-rw-rw-rw-   0        0        0     3134 2024-05-30 11:42:18.000000 LibreView-0.1.8/LibreView/utils/API.py
+-rw-rw-rw-   0        0        0       36 2024-02-22 07:02:55.000000 LibreView-0.1.8/LibreView/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:42:23.184833 LibreView-0.1.8/LibreView.egg-info/
+-rw-rw-rw-   0        0        0      514 2024-05-30 11:42:23.000000 LibreView-0.1.8/LibreView.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-30 11:42:23.000000 LibreView-0.1.8/LibreView.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 11:42:23.000000 LibreView-0.1.8/LibreView.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:42:23.000000 LibreView-0.1.8/LibreView.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 11:42:23.000000 LibreView-0.1.8/LibreView.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      514 2024-05-30 11:42:23.185835 LibreView-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 11:42:23.183834 LibreView-0.1.8/Tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 08:46:03.000000 LibreView-0.1.8/Tests/__init__.py
+-rw-rw-rw-   0        0        0     3796 2024-05-30 11:23:21.000000 LibreView-0.1.8/Tests/test_api.py
+-rw-rw-rw-   0        0        0     1903 2024-02-22 08:02:21.000000 LibreView-0.1.8/Tests/test_client.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:42:23.186830 LibreView-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-30 11:42:22.000000 LibreView-0.1.8/setup.py
```

### Comparing `LibreView-0.1.7/LibreView/LibreView.py` & `LibreView-0.1.8/LibreView/LibreView.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/LibreView/models/Connection.py` & `LibreView-0.1.8/LibreView/models/Connection.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/LibreView/models/GlucoseMeasurement.py` & `LibreView-0.1.8/LibreView/models/GlucoseMeasurement.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/LibreView/models/User.py` & `LibreView-0.1.8/LibreView/models/User.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/LibreView/utils/API.py` & `LibreView-0.1.8/LibreView/utils/API.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     def authenticate(self):
         r = self.client.post(
             f"{self.base_url}/llu/auth/login",
             json={
                 "email": self.username,
                 "password": self.password,
             },
-            verify=False
         )
         r.raise_for_status()
         content = r.json()
 
         if content and content.get("status") == 0 and content["data"].get("redirect", False):
             region = content["data"]["region"]
             self.base_url = f"https://api-{region}.libreview.io"
@@ -69,32 +68,29 @@
 
     def accept_terms(self, token):
         r = self.client.post(
             f"{self.base_url}/llu/auth/login",
             headers={
                 "Authorization": f"Bearer {token}",
             },
-            verify=False
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
-            verify=False
         )
         r.raise_for_status()
         return User.from_dict(r.json()["data"]["user"])
 
     @reauth_on_fail
     def get_connections(self) -> list[Connection]:
         r = self.client.get(
             f"{self.base_url}/llu/connections",
-            verify=False
         )
         r.raise_for_status()
         return Connection.from_list(r.json()["data"])
```

### Comparing `LibreView-0.1.7/LibreView.egg-info/PKG-INFO` & `LibreView-0.1.8/LibreView.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibreView
-Version: 0.1.7
+Version: 0.1.8
 Summary: API interface for LibreView / LibreLinkUp glucose readings
 Home-page: https://github.com/PTST/LibreView_Py
 Author: PTST
 Author-email: patrick@steffensen.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LibreView-0.1.7/LibreView.egg-info/SOURCES.txt` & `LibreView-0.1.8/LibreView.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/PKG-INFO` & `LibreView-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibreView
-Version: 0.1.7
+Version: 0.1.8
 Summary: API interface for LibreView / LibreLinkUp glucose readings
 Home-page: https://github.com/PTST/LibreView_Py
 Author: PTST
 Author-email: patrick@steffensen.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LibreView-0.1.7/Tests/test_api.py` & `LibreView-0.1.8/Tests/test_api.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/Tests/test_client.py` & `LibreView-0.1.8/Tests/test_client.py`

 * *Files identical despite different names*

### Comparing `LibreView-0.1.7/setup.py` & `LibreView-0.1.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LibreView",
-    version="0.1.7",
+    version="0.1.8",
     author="PTST",
     author_email="patrick@steffensen.io",
     description="API interface for LibreView / LibreLinkUp glucose readings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PTST/LibreView_Py",
     packages=setuptools.find_packages(),
```

