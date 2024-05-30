# Comparing `tmp/PyPowerFlex-1.8.0.tar.gz` & `tmp/PyPowerFlex-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyPowerFlex-1.8.0.tar", last modified: Wed Jun 28 12:02:23 2023, max compression
+gzip compressed data, was "dist/PyPowerFlex-1.9.0.tar", last modified: Thu Feb 29 09:32:57 2024, max compression
```

## Comparing `PyPowerFlex-1.8.0.tar` & `PyPowerFlex-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:02:23.000000 PyPowerFlex-1.8.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:02:23.000000 PyPowerFlex-1.8.0/PyPowerFlex/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:02:23.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/acceleration_pool.py
--rw-r--r--   0 root         (0) root         (0)     4404 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/device.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/fault_set.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/protection_domain.py
--rw-r--r--   0 root         (0) root         (0)     9528 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/replication_consistency_group.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/replication_pair.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/sdc.py
--rw-r--r--   0 root         (0) root         (0)    14512 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/sds.py
--rw-r--r--   0 root         (0) root         (0)     8878 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/snapshot_policy.py
--rw-r--r--   0 root         (0) root         (0)    18584 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/storage_pool.py
--rw-r--r--   0 root         (0) root         (0)    16344 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/system.py
--rw-r--r--   0 root         (0) root         (0)     4450 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/utility.py
--rw-r--r--   0 root         (0) root         (0)    18894 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/objects/volume.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13227 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/base_client.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/configuration.py
--rw-r--r--   0 root         (0) root         (0)     9621 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/constants.py
--rw-r--r--   0 root         (0) root         (0)     4175 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/token.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/PyPowerFlex/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:02:23.000000 PyPowerFlex-1.8.0/PyPowerFlex.egg-info/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-28 12:02:22.000000 PyPowerFlex-1.8.0/PyPowerFlex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-28 12:02:22.000000 PyPowerFlex-1.8.0/PyPowerFlex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 12:02:22.000000 PyPowerFlex-1.8.0/PyPowerFlex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-28 12:02:22.000000 PyPowerFlex-1.8.0/PyPowerFlex.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-28 12:02:22.000000 PyPowerFlex-1.8.0/PyPowerFlex.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     7607 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-28 12:02:20.000000 PyPowerFlex-1.8.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-28 12:02:23.000000 PyPowerFlex-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 12:02:23.000000 PyPowerFlex-1.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/acceleration_pool.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/device.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/fault_set.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/managed_device.py
+-rw-r--r--   0 root         (0) root         (0)     8986 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/protection_domain.py
+-rw-r--r--   0 root         (0) root         (0)     9528 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/replication_consistency_group.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/replication_pair.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/sdc.py
+-rw-r--r--   0 root         (0) root         (0)    14512 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/sds.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/service_template.py
+-rw-r--r--   0 root         (0) root         (0)     8878 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/snapshot_policy.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/storage_pool.py
+-rw-r--r--   0 root         (0) root         (0)    16344 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/system.py
+-rw-r--r--   0 root         (0) root         (0)     4450 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/utility.py
+-rw-r--r--   0 root         (0) root         (0)    18894 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/objects/volume.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13859 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/base_client.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     9621 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4175 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      793 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/token.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/PyPowerFlex/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      324 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      967 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PyPowerFlex.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     7654 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-02-29 09:32:55.000000 PyPowerFlex-1.9.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 09:32:57.000000 PyPowerFlex-1.9.0/setup.cfg
```

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/__init__.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Dell Inc. or its subsidiaries.
+# Copyright (c) 2024 Dell Inc. or its subsidiaries.
 # All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -22,14 +22,17 @@
 from PyPowerFlex.objects.storage_pool import StoragePool
 from PyPowerFlex.objects.acceleration_pool import AccelerationPool
 from PyPowerFlex.objects.system import System
 from PyPowerFlex.objects.volume import Volume
 from PyPowerFlex.objects.utility import PowerFlexUtility
 from PyPowerFlex.objects.replication_consistency_group import ReplicationConsistencyGroup
 from PyPowerFlex.objects.replication_pair import ReplicationPair
+from PyPowerFlex.objects.service_template import ServiceTemplate
+from PyPowerFlex.objects.managed_device import ManagedDevice
+from PyPowerFlex.objects.deployment import Deployment
 
 
 __all__ = [
     'Device',
     'FaultSet',
     'ProtectionDomain',
     'Sdc',
@@ -37,9 +40,12 @@
     'SnapshotPolicy',
     'StoragePool',
     'AccelerationPool',
     'System',
     'Volume',
     'PowerFlexUtility',
     'ReplicationConsistencyGroup',
-    'ReplicationPair'
+    'ReplicationPair',
+    'ServiceTemplate',
+    'ManagedDevice',
+    'Deployment',
 ]
```

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/acceleration_pool.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/acceleration_pool.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/device.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/device.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/fault_set.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/fault_set.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/protection_domain.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/protection_domain.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/replication_consistency_group.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/replication_consistency_group.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/replication_pair.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/replication_pair.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/sdc.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/sdc.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/sds.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/sds.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/snapshot_policy.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/snapshot_policy.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/storage_pool.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/storage_pool.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/system.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/system.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/utility.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/utility.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/objects/volume.py` & `PyPowerFlex-1.9.0/PyPowerFlex/objects/volume.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/__init__.py` & `PyPowerFlex-1.9.0/PyPowerFlex/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Dell Inc. or its subsidiaries.
+# Copyright (c) 2024 Dell Inc. or its subsidiaries.
 # All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -40,15 +40,18 @@
         'snapshot_policy',
         'storage_pool',
         'acceleration_pool',
         'system',
         'volume',
         'utility',
         'replication_consistency_group',
-        'replication_pair'
+        'replication_pair',
+        'service_template',
+        'managed_device',
+        'deployment'
     )
 
     def __init__(self,
                  gateway_address=None,
                  gateway_port=443,
                  username=None,
                  password=None,
@@ -88,14 +91,17 @@
         self.__add_storage_entity('acceleration_pool',
                                   objects.AccelerationPool)
         self.__add_storage_entity('system', objects.System)
         self.__add_storage_entity('volume', objects.Volume)
         self.__add_storage_entity('utility', objects.PowerFlexUtility)
         self.__add_storage_entity('replication_consistency_group', objects.ReplicationConsistencyGroup)
         self.__add_storage_entity('replication_pair', objects.ReplicationPair)
+        self.__add_storage_entity('service_template', objects.ServiceTemplate)
+        self.__add_storage_entity('managed_device', objects.ManagedDevice)
+        self.__add_storage_entity('deployment', objects.Deployment)
         utils.init_logger(self.configuration.log_level)
         if version.parse(self.system.api_version()) < version.Version('3.0'):
             raise exceptions.PowerFlexClientException(
                 'PowerFlex (VxFlex OS) versions lower than '
                 '3.0 are not supported.'
             )
         self.__is_initialized = True
```

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/base_client.py` & `PyPowerFlex-1.9.0/PyPowerFlex/base_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Dell Inc. or its subsidiaries.
+# Copyright (c) 2024 Dell Inc. or its subsidiaries.
 # All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -17,20 +17,21 @@
 
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
 from PyPowerFlex import exceptions
 from PyPowerFlex import utils
 
-
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 LOG = logging.getLogger(__name__)
 
 
 class Request:
+    GET = "get"
+
     def __init__(self, token, configuration):
         self.token = token
         self.configuration = configuration
         self.__refresh_token = None
 
     @property
     def base_url(self):
@@ -56,25 +57,32 @@
         if (
                 self.configuration.verify_certificate
                 and self.configuration.certificate_path
         ):
             verify_certificate = self.configuration.certificate_path
         return verify_certificate
 
+    def get_auth_headers(self, request_type=None):
+        if request_type == self.GET:
+            return {'Authorization': 'Bearer {0}'.format(self.token.get())}
+        return {'Authorization': 'Bearer {0}'.format(self.token.get()),
+                'content-type': 'application/json'}
+
     def send_get_request(self, url, **url_params):
         request_url = self.base_url + url.format(**url_params)
         version = self.login()
-        r = requests.get(request_url,
-                         auth=(
-                             self.configuration.username,
-                             self.token.get()
-                         ),
-                         verify=self.verify_certificate,
-                         timeout=self.configuration.timeout)
-
+        request_params = {'url': request_url,
+                          'headers': self.get_auth_headers(request_type=self.GET),
+                          'verify': self.verify_certificate,
+                          'timeout': self.configuration.timeout}
+        if utils.is_version_3(version):
+            request_params['auth'] = (self.configuration.username,
+                                      self.token.get())
+            request_params['headers'] = None
+        r = requests.get(**request_params)
         self.logout(version)
         response = r.json()
         return r, response
 
     def send_post_request(self, url, params=None, **url_params):
         if params is None:
             params = dict()
@@ -113,26 +121,26 @@
             response = r.json()
         self.logout(version)
         return r, response
 
     # To perform login based on the API version
     def login(self):
         version = self.get_api_version()
-        if utils.check_version(version=version):
-            self._appliance_login()
-        else:
+        if utils.is_version_3(version=version):
             self._login()
+        else:
+            self._appliance_login()
         return version
 
     # To perform logout based on the API version
     def logout(self, version):
-        if utils.check_version(version=version):
-            self._appliance_logout()
-        else:
+        if utils.is_version_3(version=version):
             self._logout()
+        else:
+            self._appliance_logout()
 
     # Get the Current API version
     def get_api_version(self):
         request_url = self.base_url + '/version'
         self._login()
         r = requests.get(request_url,
                          auth=(
@@ -161,47 +169,44 @@
         token = response['access_token']
         self.token.set(token)
         self.__refresh_token = response['refresh_token']
 
     # API logout method for 4.0 and above.
     def _appliance_logout(self):
         request_url = self.auth_url + '/logout'
-        token = self.token.get()
-        headers = {'Authorization': 'Bearer {0}'.format(token),
-                   'content-type': 'application/json'
-                   }
         data = {'refresh_token': '{0}'.format(self.__refresh_token)}
-        r = requests.post(request_url, headers=headers, json=data,
+        r = requests.post(request_url, headers=self.get_auth_headers(), json=data,
                           verify=self.verify_certificate,
                           timeout=self.configuration.timeout
                           )
 
         if r.status_code != requests.codes.no_content:
             exc = exceptions.PowerFlexFailQuerying('token')
             LOG.error(exc.message)
             raise exc
         self.token.set("")
         self.__refresh_token = None
 
     def _login(self):
         request_url = self.base_url + '/login'
-
-        r = requests.get(request_url,
-                         auth=(
-                             self.configuration.username,
-                             self.configuration.password
-                         ),
-                         verify=self.verify_certificate,
-                         timeout=self.configuration.timeout)
-        if r.status_code != requests.codes.ok:
-            exc = exceptions.PowerFlexFailQuerying('token')
-            LOG.error(exc.message)
-            raise exc
-        token = r.json()
-        self.token.set(token)
+        try:
+            r = requests.get(request_url,
+                            auth=(
+                                self.configuration.username,
+                                self.configuration.password
+                            ),
+                            verify=self.verify_certificate,
+                            timeout=self.configuration.timeout)
+            r.raise_for_status()
+            token = r.json()
+            self.token.set(token)
+        except requests.exceptions.RequestException as e:
+            error_msg = f'Login failed with error:{e.response.content}' if e.response else f'Login failed with error:{str(e)}'
+            LOG.error(error_msg)
+            raise Exception(error_msg)
 
     def _logout(self):
         token = self.token.get()
 
         if token:
             request_url = self.base_url + '/logout'
             r = requests.get(request_url,
@@ -222,14 +227,17 @@
     base_action_url = '/instances/{entity}::{entity_id}/action/{action}'
     base_entity_url = '/instances/{entity}::{entity_id}'
     base_entity_list_or_create_url = '/types/{entity}/instances'
     base_relationship_url = base_entity_url + '/relationships/{related}'
     base_object_url = '/instances/{entity}/action/{action}'
     query_mdm_cluster_url = '/instances/{entity}/queryMdmCluster'
     list_statistics_url = '/types/{entity}/instances/action/{action}'
+    service_template_url = '/V1/ServiceTemplate'
+    managed_device_url = '/V1/ManagedDevice'
+    deployment_url = '/V1/Deployment'
     entity_name = None
 
     @property
     def entity(self):
         return self.entity_name or self.__class__.__name__
 
     def _create_entity(self, params=None):
```

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/configuration.py` & `PyPowerFlex-1.9.0/PyPowerFlex/configuration.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/constants.py` & `PyPowerFlex-1.9.0/PyPowerFlex/constants.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/exceptions.py` & `PyPowerFlex-1.9.0/PyPowerFlex/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/token.py` & `PyPowerFlex-1.9.0/PyPowerFlex/token.py`

 * *Files identical despite different names*

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex/utils.py` & `PyPowerFlex-1.9.0/PyPowerFlex/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Dell Inc. or its subsidiaries.
+# Copyright (c) 2024 Dell Inc. or its subsidiaries.
 # All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -16,15 +16,14 @@
 import json
 import logging
 import numbers
 import sys
 
 from PyPowerFlex import exceptions
 
-
 def init_logger(log_level):
     """Initialize logger for PowerFlex client.
 
     :param log_level: logging level (e. g. logging.DEBUG)
     :type log_level: int
     :rtype: None
     """
@@ -126,18 +125,24 @@
         if value is not None:
             prepared[name] = convert(value)
     if dump:
         return json.dumps(prepared)
     return prepared
 
 
-def check_version(version):
+def is_version_3(version):
     """ Check the API version.
 
     :param version: Specifies the current API version
-    :return: True if API version is greater than or equal to 4.0
+    :return: True if API version is lesser than 4.0
     :rtype: bool
     """
     appliance_version = "4.0"
-    if version >= appliance_version:
+    if version < appliance_version:
         return True
     return False
+
+def build_uri_with_params(uri, **url_params):
+    query_params = [f"{key}={item}" if isinstance(value, list) else f"{key}={value}" for key, value in url_params.items() for item in (value if isinstance(value, list) else [value]) if item is not None]
+    if query_params:
+        uri += '?' + '&'.join(query_params)
+    return uri
```

### Comparing `PyPowerFlex-1.8.0/PyPowerFlex.egg-info/SOURCES.txt` & `PyPowerFlex-1.9.0/PyPowerFlex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 PyPowerFlex.egg-info/PKG-INFO
 PyPowerFlex.egg-info/SOURCES.txt
 PyPowerFlex.egg-info/dependency_links.txt
 PyPowerFlex.egg-info/requires.txt
 PyPowerFlex.egg-info/top_level.txt
 PyPowerFlex/objects/__init__.py
 PyPowerFlex/objects/acceleration_pool.py
+PyPowerFlex/objects/deployment.py
 PyPowerFlex/objects/device.py
 PyPowerFlex/objects/fault_set.py
+PyPowerFlex/objects/managed_device.py
 PyPowerFlex/objects/protection_domain.py
 PyPowerFlex/objects/replication_consistency_group.py
 PyPowerFlex/objects/replication_pair.py
 PyPowerFlex/objects/sdc.py
 PyPowerFlex/objects/sds.py
+PyPowerFlex/objects/service_template.py
 PyPowerFlex/objects/snapshot_policy.py
 PyPowerFlex/objects/storage_pool.py
 PyPowerFlex/objects/system.py
 PyPowerFlex/objects/utility.py
 PyPowerFlex/objects/volume.py
```

### Comparing `PyPowerFlex-1.8.0/README.md` & `PyPowerFlex-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 * ReplicationPair
 * System
 * StoragePool
 * AccelerationPool
 * Sdc
 * FaultSet
 * Volume
+* ManagedDevice
+* Deployment
+* ServiceTemplate
 
 #### Initialize PowerFlex client
 
 ```python
 from PyPowerFlex import PowerFlexClient
 
 client = PowerFlexClient(gateway_address='1.2.3.4',
```

### Comparing `PyPowerFlex-1.8.0/setup.py` & `PyPowerFlex-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Dell Inc. or its subsidiaries.
+# Copyright (c) 2024 Dell Inc. or its subsidiaries.
 # All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +13,15 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from setuptools import setup
 
 setup(
     name='PyPowerFlex',
-    version='1.8.0',
+    version='1.9.0',
     description='Python library for Dell PowerFlex',
     author='Ansible Team at Dell',
     author_email='ansible.team@dell.com',
     install_requires=[
         'packaging>=20.4',
         'requests>=2.23.0',
     ],
```

