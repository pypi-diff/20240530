# Comparing `tmp/moira-python-client-4.2.0.tar.gz` & `tmp/moira_python_client-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moira-python-client-4.2.0.tar", last modified: Thu Feb 29 13:58:33 2024, max compression
+gzip compressed data, was "moira_python_client-4.2.1.tar", last modified: Thu May 30 08:25:00 2024, max compression
```

## Comparing `moira-python-client-4.2.0.tar` & `moira_python_client-4.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:58:33.122007 moira-python-client-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-29 13:58:33.122007 moira-python-client-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:58:33.118006 moira-python-client-4.2.0/moira_client/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:58:33.122007 moira-python-client-4.2.0/moira_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/moira_client/moira.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:58:33.122007 moira-python-client-4.2.0/moira_python_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-29 13:58:33.000000 moira-python-client-4.2.0/moira_python_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-29 13:58:33.000000 moira-python-client-4.2.0/moira_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 13:58:33.000000 moira-python-client-4.2.0/moira_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-29 13:58:33.000000 moira-python-client-4.2.0/moira_python_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-29 13:58:33.000000 moira-python-client-4.2.0/moira_python_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-29 13:58:33.122007 moira-python-client-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:58:33.122007 moira-python-client-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-02-29 13:58:25.000000 moira-python-client-4.2.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:25:00.405376 moira_python_client-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-30 08:25:00.405376 moira_python_client-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:25:00.401376 moira_python_client-4.2.1/moira_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:25:00.401376 moira_python_client-4.2.1/moira_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/moira_client/moira.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:25:00.405376 moira_python_client-4.2.1/moira_python_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-30 08:25:00.000000 moira_python_client-4.2.1/moira_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 08:25:00.000000 moira_python_client-4.2.1/moira_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:25:00.000000 moira_python_client-4.2.1/moira_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 08:25:00.000000 moira_python_client-4.2.1/moira_python_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 08:25:00.000000 moira_python_client-4.2.1/moira_python_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 08:25:00.405376 moira_python_client-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:25:00.405376 moira_python_client-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-30 08:24:56.000000 moira_python_client-4.2.1/tests/test_client.py
```

### Comparing `moira-python-client-4.2.0/CHANGELOG.md` & `moira_python_client-4.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 4.2.1
+
+Add support for name field in contacts
+
 # 4.2.0
 
 Add support for multiple clusters in trigger creation
 
 Now you can use `cluster_id` field in api to set non-default cluster for remote triggers. List of available clusters can be seen in api at `https://your-moira-url/api/config`
 
 # 4.1.0
```

### Comparing `moira-python-client-4.2.0/LICENSE` & `moira_python_client-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/PKG-INFO` & `moira_python_client-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moira-python-client
-Version: 4.2.0
+Version: 4.2.1
 Summary: Client for Moira - Alerting system based on Graphite data
 Home-page: https://github.com/moira-alert/python-moira-client
 Author: Alexander Lukyanchenko
 Author-email: al.lukyanchenko@gmail.com
 Keywords: moira monitoring client metrics alerting
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moira-python-client-4.2.0/README.md` & `moira_python_client-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/client.py` & `moira_python_client-4.2.1/moira_client/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,22 @@
     def __init__(self, content):
         """
 
         :param content: bytes response content
         """
         self.content = content
 
+class MoiraApiError(Exception):
+    def __init__(self, body):
+        """
+
+        :param body: response body
+        """
+        self.body = body
+
 
 class Client:
     def __init__(self, api_url, auth_custom=None, auth_user=None, auth_pass=None, login=None):
         """
 
         :param api_url: str Moira API URL
         :param auth_custom: dict auth custom headers
@@ -60,15 +68,20 @@
         :param kwargs: additional parameters for request
         :return: dict response
 
         :raises: HTTPError
         :raises: InvalidJSONError
         """
         r = requests.get(self._path_join(path), headers=self.headers, auth=self.auth, **kwargs)
-        r.raise_for_status()
+        
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise MoiraApiError(r.content)
+
         try:
             return r.json()
         except ValueError:
             raise InvalidJSONError(r.content)
 
     def delete(self, path='', **kwargs):
         """
@@ -77,15 +90,20 @@
         :param kwargs: additional parameters for request
         :return: dict response
 
         :raises: HTTPError
         :raises: InvalidJSONError
         """
         r = requests.delete(self._path_join(path), headers=self.headers, auth=self.auth, **kwargs)
-        r.raise_for_status()
+        
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise MoiraApiError(r.content)
+
         try:
             return r.json()
         except ValueError:
             raise InvalidJSONError(r.content)
 
     def put(self, path='', **kwargs):
         """
@@ -94,15 +112,20 @@
         :param kwargs: additional parameters for request
         :return: dict response
 
         :raises: HTTPError
         :raises: InvalidJSONError
         """
         r = requests.put(self._path_join(path), headers=self.headers, auth=self.auth, **kwargs)
-        r.raise_for_status()
+
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise MoiraApiError(r.content)
+
         try:
             return r.json()
         except ValueError:
             raise InvalidJSONError(r.content)
 
     def post(self, path='', **kwargs):
         """
@@ -111,15 +134,20 @@
         :param kwargs: additional parameters for request
         :return: dict response
 
         :raises: HTTPError
         :raises: InvalidJSONError
         """
         r = requests.post(self._path_join(path), headers=self.headers, auth=self.auth, **kwargs)
-        r.raise_for_status()
+        
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise MoiraApiError(r.content)
+
         try:
             return r.json()
         except ValueError:
             raise InvalidJSONError(r.content)
 
     def _path_join(self, *args):
         path = self.api_url
```

### Comparing `moira-python-client-4.2.0/moira_client/models/config.py` & `moira_python_client-4.2.1/moira_client/models/config.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/contact.py` & `moira_python_client-4.2.1/moira_client/models/contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,41 +17,50 @@
         :param value: str contact value
         :param contact_type: str contact type (one of CONTACT_* constants)
         :param kwargs: additional parameters
         """
         self.type = type
         self.value = value
         self.user = kwargs.get('user', None)
+        self.name = kwargs.get('name', None)
         self._id = kwargs.get('id', None)
 
 
 class ContactManager:
     def __init__(self, client):
         self._client = client
 
-    def add(self, value, contact_type):
+    def add(self, value, contact_type, name=None):
         """
         Add new contact
 
         :param value: str contact value
         :param contact_type: str contact type (one of CONTACT_* constants)
+        :param name: str contact name
         :return: Contact
 
         :raises: ResponseStructureError
         """
-        data = {
-            'value': value,
-            'type': contact_type
-        }
 
         contacts = self.fetch_by_current_user()
         for contact in contacts:
             if contact.value == value and contact.type == contact_type:
+                if name and contact.name != name:
+                    contact.name = name
+                    self.update(contact)
+                    return contact
                 return contact
 
+        data = {
+            'value': value,
+            'type': contact_type
+        }
+        if name:
+            data['name'] = name
+
         result = self._client.put(self._full_path(), json=data)
         if 'id' not in result:
             raise ResponseStructureError('No id in response', result)
 
         return Contact(id=result['id'], **data)
 
     def fetch_all(self):
@@ -131,14 +140,16 @@
         :param contact: Contact
         :return: True if ok, False otherwise
         """
         data = {
             'type': contact.type,
             'value': contact.value,
         }
+        if contact.name:
+            data['name'] = contact.name
 
         try:
             self._client.put(self._full_path(contact.id), json=data)
             return True
         except InvalidJSONError:
             return False
```

### Comparing `moira-python-client-4.2.0/moira_client/models/event.py` & `moira_python_client-4.2.1/moira_client/models/event.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/health.py` & `moira_python_client-4.2.1/moira_client/models/health.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/notification.py` & `moira_python_client-4.2.1/moira_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/pattern.py` & `moira_python_client-4.2.1/moira_client/models/pattern.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/subscription.py` & `moira_python_client-4.2.1/moira_client/models/subscription.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/tag.py` & `moira_python_client-4.2.1/moira_client/models/tag.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/trigger.py` & `moira_python_client-4.2.1/moira_client/models/trigger.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/models/user.py` & `moira_python_client-4.2.1/moira_client/models/user.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_client/moira.py` & `moira_python_client-4.2.1/moira_client/moira.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/moira_python_client.egg-info/PKG-INFO` & `moira_python_client-4.2.1/moira_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moira-python-client
-Version: 4.2.0
+Version: 4.2.1
 Summary: Client for Moira - Alerting system based on Graphite data
 Home-page: https://github.com/moira-alert/python-moira-client
 Author: Alexander Lukyanchenko
 Author-email: al.lukyanchenko@gmail.com
 Keywords: moira monitoring client metrics alerting
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moira-python-client-4.2.0/moira_python_client.egg-info/SOURCES.txt` & `moira_python_client-4.2.1/moira_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/setup.py` & `moira_python_client-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-4.2.0/tests/test_client.py` & `moira_python_client-4.2.1/tests/test_client.py`

 * *Files identical despite different names*

