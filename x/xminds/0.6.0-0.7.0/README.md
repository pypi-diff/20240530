# Comparing `tmp/xminds-0.6.0.tar.gz` & `tmp/xminds-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xminds-0.6.0.tar", last modified: Wed Apr 19 02:31:20 2023, max compression
+gzip compressed data, was "dist/xminds-0.7.0.tar", last modified: Wed May 29 22:09:19 2024, max compression
```

## Comparing `xminds-0.6.0.tar` & `xminds-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/
--rw-r--r--   0 emile      (502) staff       (20)      750 2023-04-19 02:31:20.000000 xminds-0.6.0/PKG-INFO
--rw-r--r--   0 emile      (502) staff       (20)      289 2021-03-06 05:56:48.000000 xminds-0.6.0/README.rst
--rw-r--r--   0 emile      (502) staff       (20)       38 2023-04-19 02:31:20.000000 xminds-0.6.0/setup.cfg
--rw-r--r--   0 emile      (502) staff       (20)     1141 2021-09-29 16:05:53.000000 xminds-0.6.0/setup.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/
--rw-r--r--   0 emile      (502) staff       (20)       77 2023-04-19 02:29:24.000000 xminds-0.6.0/xminds/__init__.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/_lib/
--rw-r--r--   0 emile      (502) staff       (20)        0 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/_lib/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)      937 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/_lib/compat.py
--rw-r--r--   0 emile      (502) staff       (20)    30299 2021-09-29 16:05:53.000000 xminds-0.6.0/xminds/_lib/hashmap.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/api/
--rw-r--r--   0 emile      (502) staff       (20)      184 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/api/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)     5537 2023-04-19 02:29:24.000000 xminds-0.6.0/xminds/api/apirequest.py
--rw-r--r--   0 emile      (502) staff       (20)   106531 2023-04-19 02:29:24.000000 xminds-0.6.0/xminds/api/client.py
--rw-r--r--   0 emile      (502) staff       (20)     3109 2022-08-23 22:05:50.000000 xminds-0.6.0/xminds/api/exceptions.py
--rw-r--r--   0 emile      (502) staff       (20)      517 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/compat.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/ds/
--rw-r--r--   0 emile      (502) staff       (20)       47 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/ds/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)     2875 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/ds/scaling.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/lib/
--rw-r--r--   0 emile      (502) staff       (20)       53 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/lib/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)    23723 2022-01-27 18:13:19.000000 xminds-0.6.0/xminds/lib/aggregate.py
--rw-r--r--   0 emile      (502) staff       (20)     8506 2022-01-27 18:13:19.000000 xminds-0.6.0/xminds/lib/arraybase.py
--rw-r--r--   0 emile      (502) staff       (20)    17756 2021-09-29 16:05:53.000000 xminds-0.6.0/xminds/lib/arrays.py
--rw-r--r--   0 emile      (502) staff       (20)     4080 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/lib/iterable.py
--rw-r--r--   0 emile      (502) staff       (20)     8594 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/lib/utils.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/
--rw-r--r--   0 emile      (502) staff       (20)      750 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/PKG-INFO
--rw-r--r--   0 emile      (502) staff       (20)      545 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/SOURCES.txt
--rw-r--r--   0 emile      (502) staff       (20)        1 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/dependency_links.txt
--rw-r--r--   0 emile      (502) staff       (20)       29 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/requires.txt
--rw-r--r--   0 emile      (502) staff       (20)        7 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/top_level.txt
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/
+-rw-r--r--   0 emile      (502) staff       (20)      750 2024-05-29 22:09:19.000000 xminds-0.7.0/PKG-INFO
+-rw-r--r--   0 emile      (502) staff       (20)      289 2021-03-06 05:56:48.000000 xminds-0.7.0/README.rst
+-rw-r--r--   0 emile      (502) staff       (20)       38 2024-05-29 22:09:19.000000 xminds-0.7.0/setup.cfg
+-rw-r--r--   0 emile      (502) staff       (20)     1141 2021-09-29 16:05:53.000000 xminds-0.7.0/setup.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds/
+-rw-r--r--   0 emile      (502) staff       (20)       77 2024-05-29 22:05:47.000000 xminds-0.7.0/xminds/__init__.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds/_lib/
+-rw-r--r--   0 emile      (502) staff       (20)        0 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/_lib/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)      937 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/_lib/compat.py
+-rw-r--r--   0 emile      (502) staff       (20)    30299 2021-09-29 16:05:53.000000 xminds-0.7.0/xminds/_lib/hashmap.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds/api/
+-rw-r--r--   0 emile      (502) staff       (20)      184 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/api/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)     5709 2024-05-29 22:05:47.000000 xminds-0.7.0/xminds/api/apirequest.py
+-rw-r--r--   0 emile      (502) staff       (20)   120718 2024-05-29 22:05:47.000000 xminds-0.7.0/xminds/api/client.py
+-rw-r--r--   0 emile      (502) staff       (20)     3109 2022-08-23 22:05:50.000000 xminds-0.7.0/xminds/api/exceptions.py
+-rw-r--r--   0 emile      (502) staff       (20)      517 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/compat.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds/ds/
+-rw-r--r--   0 emile      (502) staff       (20)       47 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/ds/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)     2875 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/ds/scaling.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds/lib/
+-rw-r--r--   0 emile      (502) staff       (20)       53 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/lib/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)    23743 2024-05-29 22:05:47.000000 xminds-0.7.0/xminds/lib/aggregate.py
+-rw-r--r--   0 emile      (502) staff       (20)     8506 2022-01-27 18:13:19.000000 xminds-0.7.0/xminds/lib/arraybase.py
+-rw-r--r--   0 emile      (502) staff       (20)    17756 2021-09-29 16:05:53.000000 xminds-0.7.0/xminds/lib/arrays.py
+-rw-r--r--   0 emile      (502) staff       (20)     4080 2021-03-06 05:56:48.000000 xminds-0.7.0/xminds/lib/iterable.py
+-rw-r--r--   0 emile      (502) staff       (20)     8592 2024-05-29 22:05:47.000000 xminds-0.7.0/xminds/lib/utils.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds.egg-info/
+-rw-r--r--   0 emile      (502) staff       (20)      750 2024-05-29 22:09:18.000000 xminds-0.7.0/xminds.egg-info/PKG-INFO
+-rw-r--r--   0 emile      (502) staff       (20)      545 2024-05-29 22:09:19.000000 xminds-0.7.0/xminds.egg-info/SOURCES.txt
+-rw-r--r--   0 emile      (502) staff       (20)        1 2024-05-29 22:09:18.000000 xminds-0.7.0/xminds.egg-info/dependency_links.txt
+-rw-r--r--   0 emile      (502) staff       (20)       29 2024-05-29 22:09:18.000000 xminds-0.7.0/xminds.egg-info/requires.txt
+-rw-r--r--   0 emile      (502) staff       (20)        7 2024-05-29 22:09:18.000000 xminds-0.7.0/xminds.egg-info/top_level.txt
```

### Comparing `xminds-0.6.0/PKG-INFO` & `xminds-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminds
-Version: 0.6.0
+Version: 0.7.0
 Summary:  Crossing Minds data science python library and API client
 Home-page: https://github.com/Crossing-Minds/xminds-python
 Author: Crossing Minds, Inc
 Author-email: contact@crossingminds.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xminds-0.6.0/setup.py` & `xminds-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/_lib/compat.py` & `xminds-0.7.0/xminds/_lib/compat.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/_lib/hashmap.py` & `xminds-0.7.0/xminds/_lib/hashmap.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/api/apirequest.py` & `xminds-0.7.0/xminds/api/apirequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,29 +94,32 @@
         if resp.status_code >= 500:
             exc_payload = self._parse_response(resp, fallback=True)
             if exc_payload:
                 logging.error(exc_payload)
             raise ServerError(exc_payload)
         elif resp.status_code >= 400:
             data = self._parse_response(resp, fallback=True)
-            try:
-                exc = XMindsError.from_code(data.get('error_code', 0), data.get('error_data'))
-            except (KeyError, AttributeError, TypeError, ValueError):
-                exc = ServerError({'response': data})
-            raise exc
+            raise self._error_to_xminds_exc(data)
 
         data = self._parse_response(resp)
         return data
 
     def _serialize_data(self, data):
         raise NotImplementedError()
 
     def _parse_response(self, response, fallback=False):
         raise NotImplementedError()
 
+    def _error_to_xminds_exc(self, data):
+        try:
+            exc = XMindsError.from_code(data.get('error_code', 0), data['error_data'])
+        except (KeyError, AttributeError, TypeError, ValueError):
+            exc = ServerError({'response': data})
+        return exc
+
     @staticmethod
     def _parse_token(headers):
         if 'Authorization' not in headers:
             return None
 
         authorization_header = headers['Authorization']
         token_start_index = authorization_header.index('Bearer') + len('Bearer ')
@@ -157,18 +160,21 @@
     }
     PICKLE_PROTOCOL = 4
 
     def _serialize_data(self, data):
         return zlib.compress(pickle.dumps(data, protocol=self.PICKLE_PROTOCOL))
 
     def _parse_response(self, response, fallback=False):
+        """
+        SECURITY WARNING: never deserialize un-trusted data
+        """
         if response.status_code == 204:
             return None
         # decode gzip in case it is used
         response.raw.decode_content = True
         # un-pickle from iterable
         if not fallback:
-            return pickle.load(response.raw)
+            return pickle.load(response.raw)  # nosem
         try:
-            return pickle.load(response.raw)
+            return pickle.load(response.raw)  # nosem
         except pickle.UnpicklingError:
             return response.raw.read()
```

### Comparing `xminds-0.6.0/xminds/api/client.py` & `xminds-0.7.0/xminds/api/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,119 +51,179 @@
         else:
             raise NotImplementedError(f'unknown serializer {serializer}')
         self.api = cls(**api_kwargs)
 
     # === Account ===
 
     @require_login
-    def create_individual_account(self, first_name, last_name, email, password, role='backend'):
+    def create_individual_account(self, email, password=None, first_name=None, last_name=None,
+                                  role='backend', metadata=None, email_redirect_url=None):
         """
         Create a new individual account
 
-        :param str first_name:
-        :param str last_name:
         :param str email:
-        :param str password:
+        :param str? password:
+        :param str? first_name:
+        :param str? last_name:
+        :param str? role:
+        :param dict? metadata:
+        :param str? email_redirect_url:
         :returns: {'id': str, 'warnings?': [str]}
         """
         path = f'accounts/individual/'
         data = {
-            'first_name': first_name,
-            'last_name': last_name,
             'email': email,
-            'password': password,
             'role': role,
         }
+        if password is not None:
+            data['password'] = password
+        if first_name is not None:
+            data['first_name'] = first_name
+        if last_name is not None:
+            data['last_name'] = last_name
+        if metadata is not None:
+            data['metadata'] = metadata
+        if email_redirect_url is not None:
+            data['email_redirect_url'] = email_redirect_url
         return self.api.post(path=path, data=data)
 
     @require_login
     def partial_update_individual_account(
-            self, email, password=None, first_name=None, last_name=None):
+            self, email, password=None, first_name=None, last_name=None, metadata=None):
         """
         Update the password or other editable property of an individual account,
         identified by an email.
         Editable properties not provided will not be modified.
 
         :param str email:
         :param str? password:
         :param str? first_name:
         :param str? last_name:
+        :param dict? metadata:
         :returns: {'warnings?': [str]}
         """
         path = f'accounts/individual/'
         data = {
             'email': email
         }
         if password:
             data['password'] = password
         if first_name:
-            data['first_name'] = first_name,
+            data['first_name'] = first_name
         if last_name:
-            data['last_name'] = last_name,
+            data['last_name'] = last_name
+        if metadata is not None:
+            data['metadata'] = metadata
         return self.api.patch(path=path, data=data)
 
     @require_login
-    def create_service_account(self, name, password, role='frontend'):
+    def create_service_account(self, name, password=None, role='frontend', metadata=None):
         """
         Create a new service account
 
         :param str name:
-        :param str password:
+        :param str? password:
         :param str? role:
+        :param dict? metadata:
         :returns: {'id': str, 'warnings?': [str]}
         """
         path = f'accounts/service/'
         data = {
             'name': name,
-            'password': password,
             'role': role,
         }
+        if password is not None:
+            data['password'] = password
+        if metadata is not None:
+            data['metadata'] = metadata
         return self.api.post(path=path, data=data)
 
     @require_login
-    def partial_update_service_account(self, name, password):
+    def create_service_account_key(self, name, expiration_timestamp=None, metadata=None):
         """
-        Update the password or other editable property of an existing service account,
-        identified by a service name.
-        Editable properties not provided will not be modified.
+        Create a new service account key
 
         :param str name:
-        :param str password:
-        :returns: {'warnings?': [str]}
+        :param float? expiration_timestamp:
+        :param dict? metadata:
+        :returns: {'id': str, 'warnings?': [str]}
         """
-        path = f'accounts/service/'
-        data = {
-            'name': name,
-            'password': password
-        }
-        return self.api.patch(path=path, data=data)
+        path = f'accounts/service/keys/'
+        data = {'name': name}
+        if expiration_timestamp is not None:
+            data['expiration_timestamp'] = expiration_timestamp
+        if metadata is not None:
+            data['metadata'] = metadata
+        return self.api.post(path=path, data=data)
+
+    @require_login
+    def delete_service_account_key(self, key_id):
+        """
+        delete a service account key
+
+        :param str key_id:
+        """
+        path = f'accounts/service/keys/{key_id}/'
+        return self.api.delete(path=path)
 
-    def resend_verification_code(self, email):
+    def send_reset_password_email(self, email, email_redirect_url):
         """
-        Resend the verification code to the account email
+        Send password request code by email
 
         :param str email:
+        :param str email_redirect_url:
         """
-        path = f'accounts/resend-verification-code/'
-        return self.api.put(path=path, data={'email': email})
+        path = 'accounts/individual/send-reset-password-email/'
+        data = {
+            'email': email,
+            'email_redirect_url': email_redirect_url
+        }
+        return self.api.post(path=path, data=data)
 
-    def verify_account(self, code, email):
+    def set_or_reset_password(self, email, new_password, code, code_expiration_timestamp):
         """
-        Verify the email of an account by entering the verification code
+        reset the password of an individual account using a code.
 
-        :param str code:
         :param str email:
-        :returns: {'verified': bool, 'email': str, 'warnings?': [str]}
+        :param str new_password:
+        :param str code:
+        :param float code_expiration_timestamp:
         """
-        path = f'accounts/verify/'
+        path = f'accounts/individual/reset/'
         data = {
             'code': code,
             'email': email,
+            'new_password': new_password,
+            'code_expiration_timestamp': code_expiration_timestamp
+        }
+        return self.api.post(path=path, data=data)
+
+    @require_login
+    def login_jwt(self):
+        """
+        Verify login using JWT. Returns authentication context information.
+
+        :return: {
+            'org_id': str,
+            'account': {
+                'id': str,
+                'role': str,
+            },
+            'database?': {
+                'id': str,
+                'item_id_type': str,
+                'user_id_type': str,
+                'session_id_type': str
+            },
+            'frontend_user_id?': any,
+            'frontend_session_id?': any,
         }
-        return self.api.get(path=path, params=data)
+        """
+        path = 'login/jwt/'
+        return self.api.post(path=path, data=None)
 
     @require_login
     def list_accounts(self):
         """
         Get all accounts on the current organization
 
         :returns: {
@@ -176,14 +236,21 @@
                     'verified': bool,
                 },
             ],
             'service_accounts': [
                 {
                     'name': str,
                     'role': str,
+                    'keys' [
+                        {
+                            'id': 'aeF32..',
+                            'created_timestamp': 12341234.4,
+                            'metadata': {'description': 'key for test'}
+                        }
+                    ]
                 },
             ],
             'warnings?': [str]
         }
         """
         path = f'organizations/accounts/'
         return self.api.get(path=path)
@@ -212,14 +279,52 @@
         """
         path = 'accounts/service/'
         data = {
             'name': name,
         }
         return self.api.delete(path=path, data=data)
 
+    @require_login
+    def create_service_account_key(self, name, expiration_timestamp=None, metadata=None):
+        """
+        Create a service account key
+
+        :param str name: Service name
+        :param float? expiration_timestamp:
+        :param dict? metadata:
+        :return {
+            'id': 'aeF32..',
+            'key': 'UB8gW9zxuV9D',
+            'created_timestamp': 12341234.4,
+            'expire_timestamp': 12345234.4,
+            'metadata': {'description': 'key for test'}
+        }
+        :raises: NotFoundError
+        """
+        path = 'accounts/service/keys/'
+        data = {
+            'name': name,
+        }
+        if expiration_timestamp is not None:
+            data['expiration_timestamp'] = expiration_timestamp
+        if metadata is not None:
+            data['metadata'] = metadata
+        return self.api.post(path=path, data=data)
+
+    @require_login
+    def delete_service_account_key(self, key_id):
+        """
+        Delete a service account key
+
+        :param str key_id:
+        :raises: NotFoundError
+        """
+        path = f'accounts/service/keys/{key_id}/'
+        return self.api.delete(path=path)
+
     # === Login ===
 
     def login_root(self, email, password):
         """
         [DEPRECATED] please use `login_individual` without `db_id`
         :param email:
         :param password:
@@ -239,26 +344,27 @@
         jwt_token = resp['token']
         self.set_jwt_token(jwt_token)
         self._database = None
         self._refresh_token = None
         return resp
 
     def login_individual(self, email, password, db_id=None, frontend_user_id=None,
-                         frontend_session_id=None):
+                         frontend_session_id=None, db_name=None):
         """
         Login on a database with an account.
 
         When ``frontend_user_id`` and ``frontend_session_id`` are in the request it
         will resolve the anonymous session.
 
         :param str email:
         :param str password:
         :param str? db_id:
         :param ID? frontend_user_id: user ID
         :param ID? frontend_session_id: anonymous session ID
+        :param str? db_name:
         :returns: {
             'token': str,
             'refresh_token': str,
             `role`: str,
             'org_id': str,
             'database?': {
                 'id': str,
@@ -274,39 +380,42 @@
         path = f'login/individual/'
         data = {
             'email': email,
             'password': password,
         }
         if db_id is not None:
             data['db_id'] = db_id
+        if db_name is not None:
+            data['db_name'] = db_name
         if frontend_user_id is not None:
             # cannot use `_userid2body` since we are not logged in yet
             if isinstance(frontend_user_id, bytes) and self.b64_encode_bytes:
                 frontend_user_id = self._b64_encode(frontend_user_id)
             data['frontend_user_id'] = frontend_user_id
         if frontend_session_id is not None:
             # cannot use `_sessionid2body` since we are not logged in yet
             if isinstance(frontend_session_id, bytes) and self.b64_encode_bytes:
                 frontend_session_id = self._b64_encode(frontend_session_id)
             data['frontend_session_id'] = frontend_session_id
         return self._login(path, data)
 
     def login_service(self, name, password, db_id=None, frontend_user_id=None,
-                      frontend_session_id=None):
+                      frontend_session_id=None, db_name=None):
         """
         Login on a database with a service account.
 
         When ``frontend_user_id`` and ``frontend_session_id`` are in the request it
         will resolve the anonymous session.
 
         :param str name:
         :param str password:
         :param str? db_id:
         :param ID? frontend_user_id: user ID
         :param ID? frontend_session_id: anonymous session ID
+        :param str? db_name:
         :returns: {
             'token': str,
             'refresh_token': str,
             `role`: str,
             'org_id': str,
             'database?': {
                 'id': str,
@@ -322,32 +431,35 @@
         path = f'login/service/'
         data = {
             'name': name,
             'password': password,
         }
         if db_id is not None:
             data['db_id'] = db_id
+        if db_name is not None:
+            data['db_name'] = db_name
         if frontend_user_id is not None:
             # cannot use `_userid2body` since we are not logged in yet
             if isinstance(frontend_user_id, bytes) and self.b64_encode_bytes:
                 frontend_user_id = self._b64_encode(frontend_user_id)
             data['frontend_user_id'] = frontend_user_id
         if frontend_session_id is not None:
             # cannot use `_sessionid2body` since we are not logged in yet
             if isinstance(frontend_session_id, bytes) and self.b64_encode_bytes:
                 frontend_session_id = self._b64_encode(frontend_session_id)
             data['frontend_session_id'] = frontend_session_id
         return self._login(path, data)
 
-    def login_refresh_token(self, refresh_token=None, db_id=None):
+    def login_refresh_token(self, refresh_token=None, db_id=None, db_name=None):
         """
         Login again using a refresh token
 
         :param str? refresh_token: (default: self._refresh_token)
         :param str? db_id:
+        :param str? db_name:
         :returns: {
             'token': str,
             'refresh_token': str,
             `role`: str,
             'org_id': str,
             'database?': {
                 'id': str,
@@ -363,20 +475,23 @@
         refresh_token = refresh_token or self._refresh_token
         path = f'login/refresh-token/'
         data = {
             'refresh_token': refresh_token
         }
         if db_id:
             data['db_id'] = db_id
+        if db_name is not None:
+            data['db_name'] = db_name
         return self._login(path, data)
 
     def _login(self, path, data):
         resp = self.api.post(path=path, data=data)
         jwt_token = resp['token']
         self.set_jwt_token(jwt_token)
+        self._org_id = resp.get('org_id')
         self._database = resp.get('database')
         self._refresh_token = resp['refresh_token']
         return resp
 
     # === Org metadata ===
 
     @require_login
@@ -425,37 +540,41 @@
             data['preserve'] = preserve
         return self.api.patch(path=path, data=data)
 
     # === Database ===
 
     @require_login
     def create_database(self, name, description, item_id_type, user_id_type, session_id_type=None,
-                        item_filter_cache_expiration=None):
+                        core_config=None, metadata=None):
         """
         Create a new database
 
         :param str name: Database name, must be unique
         :param str description:
         :param str item_id_type: Item ID type
         :param str user_id_type: User ID type
         :param str? session_id_type: Anonymous Session ID type
         :param float? item_filter_cache_expiration: Refresh cache time of items filters (in seconds)
+        :param dict? core_config: Internal config
+        :param dict? metadata: Extra meta data, as unvalidated JSON
         :returns: {'id': str, 'warnings?': str}
         """
         path = f'databases/'
         data = {
             'name': name,
             'description': description,
             'item_id_type': item_id_type,
             'user_id_type': user_id_type,
         }
-        if item_filter_cache_expiration:
-            data['item_filter_cache_expiration'] = item_filter_cache_expiration
         if session_id_type:
             data['session_id_type'] = session_id_type
+        if core_config is not None:
+            data['core_config'] = core_config
+        if metadata is not None:
+            data['metadata'] = metadata
         return self.api.post(path=path, data=data)
 
     @require_login
     def get_all_databases(self, amt=None, page=None):
         """
         Get all databases on the current organization
 
@@ -498,64 +617,74 @@
             'user_id_type': str,
             'session_id_type': str,
             'counters': {
                 'rating': int,
                 'user': int,
                 'item': int,
             },
+            'core_config': {**key: val},
             'metadata': {**any-key: any-val},
             'warnings?': [str]
         }
         """
         path = f'databases/current/'
         return self.api.get(path=path)
 
     @require_login
-    def partial_update_database(self, description=None, metadata=None, preserve=None):
+    def partial_update_database(
+            self, description=None, core_config=None, metadata=None, preserve=None):
         """
         update description, and apply deep partial update of extra meta-data
         :param str? description: description of DB
+        :param dict? core_config: internal config
         :param dict? metadata: extra data to store structured as unvalidated JSON-compatible dict
         :param bool? preserve: set to `True` to append values instead of replace as in RFC7396
         """
         path = f'databases/current/'
         data = {}
-        assert description is not None or metadata is not None
         if description is not None:
             data['description'] = description
+        if core_config is not None:
+            data['core_config'] = core_config
         if metadata is not None:
             data['metadata'] = metadata
         if preserve is not None:
             data['preserve'] = preserve
         return self.api.patch(path=path, data=data)
 
     @require_login
-    def partial_update_database_preview(self, description=None, metadata=None, preserve=None):
+    def partial_update_database_preview(
+            self, description=None, core_config=None, metadata=None, preserve=None):
         """
         Preview deep partial update of extra data, without changing any state
         :param str? description: description of DB
+        :param dict? core_config: internal config
         :param dict? metadata: extra data to store structured as unvalidated JSON-compatible dict
         :param bool? preserve: set to `True` to append values instead of replace as in RFC7396
         :returns: {
             'metadata_old': {
                 'description': str,
+                'core_config': {**key: val},
                 'metadata': {**any-key: any-val},
             },
             'metadata_new': {
                 'description': str,
+                'core_config': {**key: val},
                 'metadata': {**any-key: any-val},
             },
             'warnings?': [str]
         }
         """
         path = f'databases/current/preview/'
         data = {}
         assert description is not None or metadata is not None
         if description is not None:
             data['description'] = description
+        if core_config is not None:
+            data['core_config'] = core_config
         if metadata is not None:
             data['metadata'] = metadata
         if preserve is not None:
             data['preserve'] = preserve
         return self.api.patch(path=path, data=data)
 
     @require_login
@@ -583,14 +712,15 @@
         Get one user-property.
 
         :param str property_name: property name
         :returns: {
             'property_name': str,
             'value_type': str,
             'repeated': bool,
+            'indexed': bool,
             'warnings?': [str]
         }
         """
         path = f'users-properties/{self.escape_url(property_name)}/'
         return self.api.get(path=path)
 
     @require_login
@@ -599,35 +729,38 @@
         Get all user-properties for the current database.
 
         :returns: {
             'properties': [{
                 'property_name': str,
                 'value_type': str,
                 'repeated': bool,
+                'indexed': bool,
             }],
             'warnings?': [str]
         }
         """
         path = f'users-properties/'
         return self.api.get(path=path)
 
     @require_login
-    def create_user_property(self, property_name, value_type, repeated=False):
+    def create_user_property(self, property_name, value_type, repeated=False, indexed=False):
         """
         Create a new user-property.
 
         :param str property_name: property name
         :param str value_type: property type
         :param bool? repeated: whether the property has many values (default: False)
+        :param bool? indexed: whether the property is indexed for filters (default: False)
         """
         path = f'users-properties/'
         data = {
             'property_name': property_name,
             'value_type': value_type,
             'repeated': repeated,
+            'indexed': indexed,
         }
         return self.api.post(path=path, data=data)
 
     @require_login
     def delete_user_property(self, property_name):
         """
         Delete an user-property given by its name
@@ -638,35 +771,35 @@
         return self.api.delete(path=path)
 
     # === User ===
 
     @require_login
     def get_user(self, user_id):
         """
-        Get one user given its ID.
+        Get property values of one user given its ID.
 
         :param ID user_id: user ID
         :returns: {
             'item': {
                 'id': ID,
                 *<property_name: property_value>,
             },
             'warnings?': [str]
         }
         """
         user_id = self._userid2url(user_id)
-        path = f'users/{user_id}/'
+        path = f'users/{user_id}/properties/'
         resp = self.api.get(path=path)
         resp['user']['user_id'] = self._body2userid(resp['user']['user_id'])
         return resp
 
     @require_login
     def list_users(self, users_id):
         """
-        Get multiple users given their IDs.
+        Get property values of multiple users given their IDs.
         The users in the response are not aligned with the input.
         In particular this endpoint does not raise NotFoundError if any user in missing.
         Instead, the missing users are simply not present in the response.
 
         :param ID-array users_id: users IDs
         :returns: {
             'users': array with fields ['id': ID, *<property_name: value_type>]
@@ -678,29 +811,31 @@
                         'array': array with fields ['user_index': uint32, 'value_id': value_type],
                     }>
                 },
             'warnings?': [str]
         }
         """
         users_id = self._userid2body(users_id)
-        path = f'users-bulk/list/'
+        path = f'users-bulk/properties/list/'
         data = {'users_id': users_id}
         resp = self.api.post(path=path, data=data)
         resp['users'] = self._body2itemid(resp['users'])
         return resp
 
     @require_login
-    def list_users_paginated(self, amt=None, cursor=None):
+    def list_users_paginated(self, amt=None, cursor=None, properties=None, filters=None):
         """
-        Get multiple users by page.
+        Get property values of multiple users by page.
         The response is paginated, you can control the response amount and offset
         using the query parameters ``amt`` and ``cursor``.
 
         :param int? amt: amount to return (default: use the API default)
         :param str? cursor: Pagination cursor
+        :param list-of-str? properties: properties to return (default: all)
+        :param list-of-str? filters: User-property filters. Filter format: ['<PROP_NAME>:<OPERATOR>:<OPTIONAL_VALUE>',...]
         :returns: {
             'users': array with fields ['id': ID, *<property_name: value_type>]
                 contains only the non-repeated values,
             'users_m2m': dict of arrays for repeated values:
                 {
                     *<repeated_property_name: {
                         'name': str,
@@ -708,114 +843,125 @@
                     }>
                 },
             'has_next': bool,
             'next_cursor': str, pagination cursor to use in next request to get more users,
             'warnings?': [str],
         }
         """
-        path = f'users-bulk/'
+        path = f'users-bulk/properties/'
         params = {}
         if amt is not None:
             params['amt'] = amt
         if cursor:
             params['cursor'] = cursor
+        if properties:
+            params['properties'] = properties
+        if filters:
+            params['filters'] = self._clean_filters_to_urlsafe(filters)
         resp = self.api.get(path=path, params=params)
         resp['users'] = self._body2userid(resp['users'])
         return resp
 
     @require_login
-    def create_or_update_user(self, user):
+    def create_or_replace_user(self, user):
         """
-        Create a new user, or update it if the ID already exists.
+        Create property values for one user, or replace them if the ID already exists.
 
         :param dict user: user ID and properties {'user_id': ID, *<property_name: property_value>}
         """
         user = dict(user)
         user_id = self._userid2url(user.pop('user_id'))
-        path = f'users/{user_id}/'
+        path = f'users/{user_id}/properties/'
         data = {
             'user': user,
         }
         return self.api.put(path=path, data=data)
 
+    create_or_update_user = create_or_replace_user
+
     @require_login
-    def create_or_update_users_bulk(self, users, users_m2m=None, wait_for_completion=None,
-                                    chunk_size=(1 << 10)):
+    def create_or_replace_users_bulk(self, users, users_m2m=None, wait_for_completion=None,
+                                     chunk_size=(1 << 10)):
         """
-        Create many users in bulk, or update the ones for which the id already exist.
+        Create property values for many users in bulk, or update the ones for which the ID already exist.
 
         :param array users: array with fields ['id': ID, *<property_name: value_type>]
             contains only the non-repeated values,
         :param dict? users_m2m: dict of arrays for repeated values:
             {
                 *<repeated_property_name: {
                     'name': str,
                     'array': array with fields ['user_index': uint32, 'value_id': value_type],
                 }>
             }
         :param int? chunk_size: split the requests in chunks of this size (default: 1K)
         :param bool? wait_for_completion: (default: True)
         """
-        path = f'users-bulk/'
+        path = f'users-bulk/properties/'
         for users_chunk, users_m2m_chunk in self._chunk_users(users, users_m2m, chunk_size):
             data = {
                 'users': users_chunk,
                 'users_m2m': users_m2m_chunk
             }
             if wait_for_completion is not None:
                 data['wait_for_completion'] = wait_for_completion
             self.api.put(path=path, data=data, timeout=60)
 
+    create_or_update_users_bulk = create_or_replace_users_bulk
+
     @require_login
     def partial_update_user(self, user, create_if_missing=None):
         """
-        Partially update some properties of an user
+        Partially update some property values of one user.
 
         :param dict user: user ID and properties {'user_id': ID, *<property_name: property_value>}
         :param bool? create_if_missing: control whether an error should be returned or a new user
         should be created when the ``user_id`` does not already exist. (default: False)
         :returns: {
             'user_created': bool, True if the user did not exist and was created,
             'user_modified': bool True if the user already exists and was modified,
             'warnings?': [str],
         }
         """
         user = dict(user)
         user_id = self._userid2url(user.pop('user_id'))
-        path = f'users/{user_id}/'
+        path = f'users/{user_id}/properties/'
         data = {
             'user': user,
         }
         if create_if_missing is not None:
             data['create_if_missing'] = create_if_missing
         return self.api.patch(path=path, data=data)
 
     @require_login
     def partial_update_users_bulk(self, users, users_m2m=None, create_if_missing=None,
-                                  chunk_size=(1 << 10)):
+                                  chunk_size=(1 << 10), wait_for_completion=None):
         """
-        Partially update some properties of many users.
+        Partially update some property values of many users.
 
         :param array users: array with fields ['id': ID, *<property_name: value_type>]
             contains only the non-repeated values,
         :param dict? users_m2m: dict of arrays for repeated values:
             {
                 *<repeated_property_name: {
                     'name': str,
                     'array': array with fields ['user_index': uint32, 'value_id': value_type],
                 }>
             }
         :param bool? create_if_missing: to control whether an error should be returned or new users
             should be created when the ``user_id`` does not already exist. (default: False)
         :param int? chunk_size: split the requests in chunks of this size (default: 1K)
+        :param bool? wait_for_completion: (default: True)
         """
-        path = f'users-bulk/'
+        path = f'users-bulk/properties/'
         data = {}
         if create_if_missing is not None:
             data['create_if_missing'] = create_if_missing
+        if wait_for_completion is not None:
+            data['wait_for_completion'] = wait_for_completion
         for users_chunk, users_m2m_chunk in self._chunk_users(users, users_m2m, chunk_size):
             data['users'] = users_chunk
             data['users_m2m'] = users_m2m_chunk
             self.api.patch(path=path, data=data, timeout=60)
 
     @require_login
     def delete_user(self, user_id):
@@ -848,20 +994,21 @@
         """
         user_id_url = self._userid2url(user_id)
         self.api.delete(f'users/{user_id_url}/*')
 
     @require_login
     def delete_users(self, users_id):
         """
-        Delete users; doesn't wait for task completion
+        Delete property values of many users in bulk. Ratings and interactions are not deleted.
+        Doesn't wait for task completion
 
         :param ID-array users_id: user IDs
         """
         data = {'users_id': self._userid2body(users_id)}
-        self.api.delete(path='users-bulk/', data=data)
+        self.api.delete(path='users-bulk/properties/', data=data)
 
     def _chunk_users(self, users, users_m2m, chunk_size):
         users_m2m = users_m2m or []
         # cast dict to list of dict
         if isinstance(users_m2m, dict):
             users_m2m = [{'name': name, 'array': array}
                          for name, array in users_m2m.items()]
@@ -952,35 +1099,35 @@
         return self.api.delete(path=path)
 
     # === Item ===
 
     @require_login
     def get_item(self, item_id):
         """
-        Get one item given its ID.
+        Get property values of one item given its ID.
 
         :param ID item_id: item ID
         :returns: {
             'item': {
                 'id': ID,
                 *<property_name: property_value>,
             },
             'warnings?': [str],
         }
         """
         item_id = self._itemid2url(item_id)
-        path = f'items/{item_id}/'
+        path = f'items/{item_id}/properties/'
         resp = self.api.get(path=path)
         resp['item']['item_id'] = self._body2itemid(resp['item']['item_id'])
         return resp
 
     @require_login
     def list_items(self, items_id, properties=None):
         """
-        Get multiple items given their IDs.
+        Get property values of multiple items given their IDs.
         The items in the response are not aligned with the input.
         In particular this endpoint does not raise NotFoundError if any item in missing.
         Instead, the missing items are simply not present in the response.
 
         :param ID-array items_id: items IDs
         :param list-of-str? properties: properties to return (default: all)
         :returns: {
@@ -993,131 +1140,141 @@
                         'array': array with fields ['item_index': uint32, 'value_id': value_type],
                     }>
                 },
             'warnings?': [str],
         }
         """
         items_id = self._itemid2body(items_id)
-        path = f'items-bulk/list/'
+        path = f'items-bulk/properties/list/'
         data = {'items_id': items_id}
         if properties is not None:
             data['properties'] = properties
         resp = self.api.post(path=path, data=data)
         resp['items'] = self._body2itemid(resp['items'])
         return resp
 
     @require_login
-    def list_items_paginated(self, amt=None, cursor=None):
+    def list_items_paginated(self, amt=None, cursor=None, properties=None, filters=None):
         """
-        Get multiple items by page.
+        Get property values of multiple items by page.
         The response is paginated, you can control the response amount and offset
         using the query parameters ``amt`` and ``cursor``.
 
         :param int? amt: amount to return (default: use the API default)
         :param str? cursor: Pagination cursor
+        :param list-of-str? properties: properties to return (default: all)
+        :param list-of-str? filters: Item-property filters. Filter format: ['<PROP_NAME>:<OPERATOR>:<OPTIONAL_VALUE>',...]
         :returns: {
-            'items': array with fields ['id': ID, *<property_name: value_type>]
+            'items': array with fields ['item_id': ID, *<property_name: value_type>]
                 contains only the non-repeated values,
             'items_m2m': dict of arrays for repeated values:
                 {
                     *<repeated_property_name: {
                         'name': str,
                         'array': array with fields ['item_index': uint32, 'value_id': value_type],
                     }>
                 },
             'has_next': bool,
             'next_cursor': str, pagination cursor to use in next request to get more items,
             'warnings?': [str],
         }
         """
-        path = f'items-bulk/'
+        path = f'items-bulk/properties/'
         params = {}
         if amt is not None:
             params['amt'] = amt
         if cursor:
             params['cursor'] = cursor
+        if properties:
+            params['properties'] = properties
+        if filters:
+            params['filters'] = self._clean_filters_to_urlsafe(filters)
         resp = self.api.get(path=path, params=params)
         resp['items'] = self._body2itemid(resp['items'])
         return resp
 
     @require_login
-    def create_or_update_item(self, item, wait_for_completion=None):
+    def create_or_replace_item(self, item, wait_for_completion=None):
         """
-        Create a new item, or update it if the ID already exists.
+        Create property values for one item, or replace them if the ID already exists.
 
         :param dict item: item ID and properties {'item_id': ID, *<property_name: property_value>}
         :param bool? wait_for_completion: (default: True)
         """
         item = dict(item)
         item_id = self._itemid2url(item.pop('item_id'))
-        path = f'items/{item_id}/'
+        path = f'items/{item_id}/properties/'
         data = {
             'item': item,
         }
         if wait_for_completion is not None:
             data['wait_for_completion'] = wait_for_completion
         return self.api.put(path=path, data=data)
 
+    create_or_update_item = create_or_replace_item
+
     @require_login
-    def create_or_update_items_bulk(self, items, items_m2m=None, wait_for_completion=None,
-                                    chunk_size=(1 << 10)):
+    def create_or_replace_items_bulk(self, items, items_m2m=None, wait_for_completion=None,
+                                     chunk_size=(1 << 10)):
         """
-        Create many items in bulk, or update the ones for which the id already exist.
+        Create property values for many items in bulk, or replace the ones for which the ID already exist.
 
         :param array items: array with fields ['id': ID, *<property_name: value_type>]
             contains only the non-repeated values,
         :param array? items_m2m: dict of arrays for repeated values:
             {
                 *<repeated_property_name: {
                     'name': str,
                     'array': array with fields ['item_index': uint32, 'value_id': value_type],
                 }>
             }
         :param bool? wait_for_completion: (default: True)
         :param int? chunk_size: split the requests in chunks of this size (default: 1000)
         """
-        path = f'items-bulk/'
+        path = f'items-bulk/properties/'
         for items_chunk, items_m2m_chunk in self._chunk_items(items, items_m2m, chunk_size):
             data = {
                 'items': items_chunk,
                 'items_m2m': items_m2m_chunk,
             }
             if wait_for_completion is not None:
                 data['wait_for_completion'] = wait_for_completion
             self.api.put(path=path, data=data, timeout=60)
 
+    create_or_update_items_bulk = create_or_replace_items_bulk
+
     @require_login
     def partial_update_item(self, item, create_if_missing=None):
         """
-        Partially update some properties of an item.
+        Partially update some property values of one item.
 
         :param dict item: item ID and properties {'item_id': ID, *<property_name: property_value>}
         :param bool? create_if_missing: control whether an error should be returned or a new item
             should be created when the ``item_id`` does not already exist. (default: false)
         :returns: {
             'item_created': bool, True if the item did not exist and was created
             'item_modified': bool, True if the item already exists and was modified
             'warnings?': [str],
         }
         """
         item = dict(item)
         item_id = self._itemid2url(item.pop('item_id'))
-        path = f'items/{item_id}/'
+        path = f'items/{item_id}/properties/'
         data = {
             'item': item,
         }
         if create_if_missing is not None:
             data['create_if_missing'] = create_if_missing
         return self.api.patch(path=path, data=data)
 
     @require_login
     def partial_update_items_bulk(self, items, items_m2m=None, create_if_missing=None,
                                   chunk_size=(1 << 10), wait_for_completion=None):
         """
-        Partially update some properties of many items.
+        Partially update some property values of many items.
 
         :param array items: array with fields ['id': ID, *<property_name: value_type>]
             contains only the non-repeated values,
         :param array? items_m2m: dict of arrays for repeated values:
             {
                 *<repeated_property_name: {
                     'name': str,
@@ -1125,44 +1282,46 @@
                 }>
             }
         :param bool? create_if_missing: control whether an error should be returned or a new item
         should be created when the ``item_id`` does not already exist. (default: False)
         :param int? chunk_size: split the requests in chunks of this size (default: 1000)
         :param bool? wait_for_completion: (default: True)
         """
-        path = f'items-bulk/'
+        path = f'items-bulk/properties/'
         data = {}
         if create_if_missing is not None:
             data['create_if_missing'] = create_if_missing
         if wait_for_completion is not None:
             data['wait_for_completion'] = wait_for_completion
         for items_chunk, items_m2m_chunk in self._chunk_items(items, items_m2m, chunk_size):
             data['items'] = items_chunk
             data['items_m2m'] = items_m2m_chunk
             self.api.patch(path=path, data=data, timeout=60)
 
     @require_login
     def delete_item_props(self, item_id):
         """
-        Delete a single item;  doesn't wait for task completion
+        Delete the property values of one item given its ID. Ratings and interactions are not deleted.
+        Doesn't wait for task completion.
 
         :param bytes item_id:
         """
         item_id_url = self._itemid2url(item_id)
-        self.api.delete(path=f'items/{item_id_url}/')
+        self.api.delete(path=f'items/{item_id_url}/properties/')
 
     @require_login
     def delete_items(self, items_id):
         """
-        Delete items; doesn't wait for task completion
+        Delete the property values of many items in bulk. Ratings and interactions are not deleted.
+        Doesn't wait for task completion
 
         :param ID-array items_id: items IDs
         """
         data = {'items_id': self._itemid2body(items_id)}
-        self.api.delete(path='items-bulk/', data=data)
+        self.api.delete(path='items-bulk/properties/', data=data)
 
     def _chunk_items(self, items, items_m2m, chunk_size):
         items_m2m = items_m2m or []
         # cast dict to list of dict
         if isinstance(items_m2m, dict):
             items_m2m = [{'name': name, 'array': array}
                          for name, array in items_m2m.items()]
@@ -1186,14 +1345,105 @@
                         {'item_index': row['item_index'] - start_idx, 'value_id': row['value_id']}
                         for row in array
                         if start_idx <= row['item_index'] < end_idx
                     ]
                 items_m2m_chunk.append({'name': m2m['name'], 'array': array_chunk})
             yield self._itemid2body(items_chunk), items_m2m_chunk
 
+    # === Reco: *-to-item ===
+
+    @require_login
+    def get_reco_generic_to_items(
+            self, user_id=None, item_id=None, session_id=None, scenario=None,
+            skip_default_scenario=None, cursor=None, amt=None,
+            interactions=None, ratings=None, user_properties=None, item_properties=None,
+            context_items=None, filters=None, reranking=None, exclude_rated_items=None,
+            table=None
+    ):
+        """
+        Get items recommendations from any reco type.
+
+        :param ID? user_id: User ID. Used to personalize recommendations when the generic input
+        resolves to: profile_to_items, profile_to_items_w_ctx_items, precomputed_profile_to_items.
+        Otherwise used in the context of an A/B test scenario to select the group A or B and keep
+        track of the respective group in analytics.
+        :param ID? item_id: Item ID. Used to get similar items when the generic input
+        resolves to: item_to_items, precomputed_item_to_items
+        :param ID? session_id: Anonymous Session ID. Used to personalize recommendations when the
+        generic input resolves to: session_to_items, session_to_items_w_ctx_items.
+        Otherwise used in the context of an A/B test scenario to select the group A or B and
+        keep track of the respective group in analytics, when a user_id is not available.
+        :param str? scenario: name of scenario
+        :param bool? skip_default_scenario: True to skip default scenario if any
+        :param str? cursor: Pagination cursor
+        :param int? amt: amount to return (default: use the API default)
+        :param array? interactions: interactions to calculate ratings from.
+            Timestamp is optional and defaults to now.
+            ['item_id': ID, 'interaction_type': 'O' 'timestamp?': float]
+        :param array? ratings: ratings array with fields ['item_id': ID, 'rating': float]
+        :param dict? user_properties: user properties {**property_name: property_value(s)}
+        :param dict? item_properties: {**property_name: property_value(s)}
+        :param array? context_items: context items ID array with fields ['item_id': ID]
+        :param list-of-dict? filters: Item-property filters. Filter format:
+            [{'property_name': str, 'op': str , 'value?': any}]
+        :param list-of-dict? reranking: Item-property reranking. Format:
+            [{'property_name': str, 'op': str , 'weight': float, 'options': dict}]
+        :param bool? exclude_rated_items: exclude rated items from response
+        :param str? table: table name
+        :returns: {
+            'items_id': array of items IDs,
+            'next_cursor': str, pagination cursor to use in next request to get more items,
+            'warnings?': [str],
+            'evaluated_scenarios': {
+                'generic_runtime?': [{'scenario_type': str, 'to?': str, 'scenario_name': str}],
+                'generic_default?': [{'scenario_type': str, 'to?': str, 'scenario_name': str}],
+                'reco_type': str,
+                'runtime?': [{'scenario_type': str, 'to?': str, 'scenario_name': str}],
+                'default?': [{'scenario_type': str, 'to?': str, 'scenario_name': str}]
+            }
+        }
+        """
+        path = f'recommendation/generic/items/'
+        data = {}
+        if amt is not None:
+            data['amt'] = amt
+        if cursor is not None:
+            data['cursor'] = cursor
+        if scenario is not None:
+            data['scenario'] = scenario
+        if skip_default_scenario is not None:
+            data['skip_default_scenario'] = skip_default_scenario
+        if user_id is not None:
+            data['user_id'] = self._userid2body(user_id)
+        if item_id is not None:
+            data['item_id'] = self._itemid2body(item_id)
+        if session_id is not None:
+            data['session_id'] = self._sessionid2body(session_id)
+        if filters is not None:
+            data['filters'] = filters
+        if reranking is not None:
+            data['reranking'] = reranking
+        if exclude_rated_items is not None:
+            data['exclude_rated_items'] = exclude_rated_items
+        if ratings is not None:
+            data['ratings'] = self._itemid2body(ratings)
+        if interactions is not None:
+            data['interactions'] = interactions
+        if user_properties is not None:
+            data['user_properties'] = user_properties
+        if item_properties is not None:
+            data['item_properties'] = item_properties
+        if context_items is not None:
+            data['context_items'] = context_items
+        if table:
+            data['table'] = table
+        resp = self.api.post(path=path, data=data)
+        resp['items_id'] = self._body2itemid(resp['items_id'])
+        return resp
+
     # === Reco: Item-to-item ===
 
     @require_login
     def get_reco_item_to_items(
             self, item_id, amt=None, cursor=None,
             scenario=None, filters=None, reranking=None,
             skip_default_scenario=None,
@@ -1243,14 +1493,57 @@
         if session_id:
             params['session_id'] = session_id
         resp = self.api.get(path=path, params=params)
         resp['items_id'] = self._body2itemid(resp['items_id'])
         return resp
 
     @require_login
+    def get_reco_item_properties_to_items(
+            self, item_properties, amt=None,
+            scenario=None, filters=None, reranking=None,
+            skip_default_scenario=None,
+    ):
+        """
+        Get similar items using item properties.
+
+        :param dict item_properties: {**property_name: property_value(s)}
+        :param int? amt: amount to return (default: use the API default)
+        :param str? scenario: name of scenario
+        :param list-of-dict? filters: Item-property filters. Filter format:
+            [{'property_name': str, 'op': str , 'value?': any}]
+        :param list-of-dict? reranking: Item-property reranking. Format:
+            [{'property_name': str, 'op': str , 'weight': float, 'options': dict}]
+        :param bool? skip_default_scenario: True to skip default scenario if any
+        :returns: {
+            'items_id': array of items IDs,
+            'next_cursor': str, pagination cursor to use in next request to get more items,
+            'warnings?': [str],
+            'evaluated_scenarios': {
+                'runtime?': [{'scenario_type': str, 'to?': str, 'scenario_name': str}],
+                'default?': [{'scenario_type': str, 'to?': str, 'scenario_name': str}]
+            }
+        }
+        """
+        path = f'recommendation/items-properties/items/'
+        data = {'item_properties': item_properties}
+        if amt is not None:
+            data['amt'] = amt
+        if filters:
+            data['filters'] = filters
+        if reranking:
+            data['reranking'] = reranking
+        if scenario:
+            data['scenario'] = scenario
+        if skip_default_scenario is not None:
+            data['skip_default_scenario'] = skip_default_scenario
+        resp = self.api.post(path=path, data=data)
+        resp['items_id'] = self._body2itemid(resp['items_id'])
+        return resp
+
+    @require_login
     def get_precomputed_reco_item_to_items(self, item_id, table=None, scenario=None,
                                            skip_default_scenario=None, user_id=None, session_id=None):
         """
         Get similar items, from a file of precomputed recommendations (stored as a ``table``).
 
         The table must be with ``LOCAL`` connection, have no compressions and have resource equal to
         ``ITEM_TO_ITEMS_RECO``.
@@ -1572,28 +1865,34 @@
 
     # === Reco: Session-to-item with Context Items ===
 
     @require_login
     def get_reco_session_to_items_w_ctx_items(
             self, context_items, ratings=None, user_properties=None, amt=None, cursor=None,
             scenario=None, filters=None, reranking=None, exclude_rated_items=None,
-            skip_default_scenario=None):
+            skip_default_scenario=None, user_id=None, session_id=None, interactions=None):
         """
         Get items recommendations given the ratings of an anonymous session and context items ID.
 
         :param array context_items: context items ID array with fields ['item_id': ID]
         :param array? ratings: ratings array with fields ['item_id': ID, 'rating': float]
         :param dict? user_properties: user properties {**property_name: property_value(s)}
         :param int? amt: amount to return (default: use the API default)
         :param str? cursor: Pagination cursor
         :param str? scenario: scenario name
         :param list-str? filters: Item-property filters. Filter format: ['<PROP_NAME>:<OPERATOR>:<OPTIONAL_VALUE>',...]
         :param list-str? reranking: Item-property reranking. Format: ['<PROP_NAME>:<OPERATOR>:<OPTIONAL_WEIGHT>:<OPTIONS>']
         :param bool? exclude_rated_items: exclude rated items from response
         :param bool? skip_default_scenario: True to skip default scenario if any
+        :param ID? user_id: user ID. Only used in the context of an A/B test scenario to select the group A or B
+            and keep track of the respective group in analytics, NOT used to personalize recommendations
+        :param ID? session_id: Anonymous Session ID.
+        :param array? interactions: interactions to calculate ratings from.
+            Timestamp is optional and defaults to now.
+            ['item_id': ID, 'interaction_type': 'O' 'timestamp?': float]
         :returns: {
             'items_id': array of items IDs,
             'next_cursor': str, pagination cursor to use in next request to get more items,
             'warnings?': [str],
         }
         """
         path = f'recommendation/context-items/sessions/items/'
@@ -1614,14 +1913,20 @@
             data['reranking'] = reranking
         if exclude_rated_items is not None:
             data['exclude_rated_items'] = exclude_rated_items
         if scenario:
             data['scenario'] = scenario
         if skip_default_scenario is not None:
             data['skip_default_scenario'] = skip_default_scenario
+        if user_id:
+            data['user_id'] = user_id
+        if session_id:
+            data['session_id'] = session_id
+        if interactions is not None:
+            data['interactions'] = interactions
         resp = self.api.post(path=path, data=data)
         resp['items_id'] = self._body2itemid(resp['items_id'])
         return resp
 
     # === Reco: User-to-item with Context Items ===
 
     @require_login
@@ -1951,21 +2256,23 @@
             params['end_timestamp'] = end_timestamp
         resp = self.api.get(path=path, params=params)
         resp['interactions'] = self._body2userid(self._body2itemid(resp['interactions']))
         return resp
 
     @require_login
     def list_user_interactions(
-            self, user_id, amt=None, cursor=None,
+            self, user_id, amt=None, cursor=None, interaction_types=None
     ):
         """
         List the interactions of one user
 
         :param int? amt: amount to return (default: use the API default)
         :param str? cursor: Pagination cursor
+        :param list-of-str? interaction_types: When provided, only retruns interactions
+            from those types
         :returns: {
             'has_next': bool,
             'next_cursor': str,
             'interactions': array with fields
                 ['item_id': ID, 'interaction_type': str, 'timestamp': float,
                  'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
             'warnings?': [str],
@@ -1974,14 +2281,16 @@
         user_id = self._userid2url(user_id)
         path = f'users/{user_id}/interactions-bulk/'
         params = {}
         if amt is not None:
             params['amt'] = amt
         if cursor:
             params['cursor'] = cursor
+        if interaction_types:
+            params['interaction_types'] = interaction_types
         resp = self.api.get(path=path, params=params)
         resp['interactions'] = self._body2itemid(resp['interactions'])
         return resp
 
     # === Session Interactions ===
 
     @require_login
@@ -2206,17 +2515,17 @@
         if payload:
             data['payload'] = payload
         return self.api.post(path=path, data=data)
 
     @require_login
     def get_background_tasks(self, task_name, page=None, amt=None):
         """
-        List currently running background tasks such as ML models training.
+        List recent background tasks such as ML models training.
 
-        :param str task_name: names allowed ``ml_model_retrain``,
+        :param str task_name: names allowed are ``ml_model_retrain``,
         ``item_popularity_score_recalibrate``, ``ml_new_users``, ``ml_new_items``
         :param int? page: page number (default: 1)
         :param int? amt: amount of tasks by page (default: 50)
         :returns: {
             'tasks': [{
                 'task_id': str,
                 'name': str,
@@ -2734,14 +3043,16 @@
                 _f = f
             elif isinstance(f, dict):
                 _f = f"{f['property_name']}:{f['op']}"
                 if 'value' in f:
                     v = f['value']
                     if isinstance(v, dict):
                         raise TypeError('Advanced filtering features are reserved to scenarios')
+                    if isinstance(v, list):
+                        v = ','.join(str(x) for x in v)
                     _f += f':{v}'
             else:
                 raise TypeError(
                     f'only strings and dict are allowed but one is a {type(f)}')
             _filters.append(_f)
         return _filters
```

### Comparing `xminds-0.6.0/xminds/api/exceptions.py` & `xminds-0.7.0/xminds/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/compat.py` & `xminds-0.7.0/xminds/compat.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/ds/scaling.py` & `xminds-0.7.0/xminds/ds/scaling.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/lib/aggregate.py` & `xminds-0.7.0/xminds/lib/aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     array([ 4, 6,  -1,  6])
     >>> ufunc_group_by_idx(idx, values, numpy.add, -1)
     array([ 9, 11, -1,  9])
     >>> ufunc_group_by_idx(idx, values, numpy.add, 0)
     array([ 10, 12, -0,  10])
     """
     length = max(idx.max() + 1 if idx.size else 0, minlength or 0)
-    out = numpy.full(length, init)
+    out = numpy.full(length, init, dtype=values.dtype)
     ufunc.at(out, idx, values)
     return out
 
 
 def min_by_idx(idx, values, minlength=None, fill=None):
     """
     Given array of indexes ``idx`` and array ``values``,
```

### Comparing `xminds-0.6.0/xminds/lib/arraybase.py` & `xminds-0.7.0/xminds/lib/arraybase.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/lib/arrays.py` & `xminds-0.7.0/xminds/lib/arrays.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/lib/iterable.py` & `xminds-0.7.0/xminds/lib/iterable.py`

 * *Files identical despite different names*

### Comparing `xminds-0.6.0/xminds/lib/utils.py` & `xminds-0.7.0/xminds/lib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 def _deep_hash_update(h, value):
     if value is None:
         h.update(b'None')
     elif isinstance(value, bytes):
         h.update(value)
     elif isinstance(value, str):
-        h.update(value.encode('latin1'))
+        h.update(value.encode('utf8'))
     elif isinstance(value, (int, float, numpy.number, numpy.dtype)):
         h.update(str(value).encode('ascii'))
     elif isinstance(value, dict):
         for k, v in value.items():
             h.update(k.encode('ascii'))
             _deep_hash_update(h, v)
     elif isinstance(value, numpy.ndarray):
```

### Comparing `xminds-0.6.0/xminds.egg-info/PKG-INFO` & `xminds-0.7.0/xminds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminds
-Version: 0.6.0
+Version: 0.7.0
 Summary:  Crossing Minds data science python library and API client
 Home-page: https://github.com/Crossing-Minds/xminds-python
 Author: Crossing Minds, Inc
 Author-email: contact@crossingminds.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xminds-0.6.0/xminds.egg-info/SOURCES.txt` & `xminds-0.7.0/xminds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

