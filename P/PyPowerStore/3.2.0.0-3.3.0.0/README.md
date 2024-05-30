# Comparing `tmp/PyPowerStore-3.2.0.0.tar.gz` & `tmp/PyPowerStore-3.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyPowerStore-3.2.0.0.tar", last modified: Mon Apr 29 12:11:23 2024, max compression
+gzip compressed data, was "dist/PyPowerStore-3.3.0.0.tar", last modified: Thu May 30 16:14:26 2024, max compression
```

## Comparing `PyPowerStore-3.2.0.0.tar` & `PyPowerStore-3.3.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/
--rw-r--r--   0 root         (0) root         (0)      991 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5629 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/file_dns.py
--rw-r--r--   0 root         (0) root         (0)     6357 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/file_interface.py
--rw-r--r--   0 root         (0) root         (0)     5666 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/file_nis.py
--rw-r--r--   0 root         (0) root         (0)     6005 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/nfs_server.py
--rw-r--r--   0 root         (0) root         (0)     5882 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/smb_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37909 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/exception.py
--rw-r--r--   0 root         (0) root         (0)     7269 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/helpers.py
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16271 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/client.py
--rw-r--r--   0 root         (0) root         (0)    96987 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/configuration.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/powerstore_conn.py
--rw-r--r--   0 root         (0) root         (0)    61608 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/protection.py
--rw-r--r--   0 root         (0) root         (0)   105129 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/provisioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      729 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/
+-rw-r--r--   0 root         (0) root         (0)      991 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/file_dns.py
+-rw-r--r--   0 root         (0) root         (0)     6357 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/file_interface.py
+-rw-r--r--   0 root         (0) root         (0)     5666 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/file_nis.py
+-rw-r--r--   0 root         (0) root         (0)     6005 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/nfs_server.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/objects/smb_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38062 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/utils/exception.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/utils/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16271 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/client.py
+-rw-r--r--   0 root         (0) root         (0)    96987 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/powerstore_conn.py
+-rw-r--r--   0 root         (0) root         (0)    61608 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/protection.py
+-rw-r--r--   0 root         (0) root         (0)   106662 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/PyPowerStore/provisioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PyPowerStore.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      729 2024-05-30 16:14:25.000000 PyPowerStore-3.3.0.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      339 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 16:14:26.000000 PyPowerStore-3.3.0.0/setup.cfg
```

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/objects/__init__.py` & `PyPowerStore-3.3.0.0/PyPowerStore/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/objects/file_dns.py` & `PyPowerStore-3.3.0.0/PyPowerStore/objects/file_dns.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/objects/file_interface.py` & `PyPowerStore-3.3.0.0/PyPowerStore/objects/file_interface.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/objects/file_nis.py` & `PyPowerStore-3.3.0.0/PyPowerStore/objects/file_nis.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/objects/nfs_server.py` & `PyPowerStore-3.3.0.0/PyPowerStore/objects/nfs_server.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/objects/smb_server.py` & `PyPowerStore-3.3.0.0/PyPowerStore/objects/smb_server.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/utils/constants.py` & `PyPowerStore-3.3.0.0/PyPowerStore/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,14 +636,18 @@
 # SMB Share endpoints
 GET_SMB_SHARE_LIST_URL = 'https://{0}/api/rest/smb_share'
 CREATE_SMB_SHARE_URL = GET_SMB_SHARE_LIST_URL
 GET_SMB_SHARE_DETAILS_URL = 'https://{0}/api/rest/smb_share/{1}'
 MODIFY_SMB_SHARE_URL = GET_SMB_SHARE_DETAILS_URL
 DELETE_SMB_SHARE_URL = GET_SMB_SHARE_DETAILS_URL
 
+# SMB Share ACL endpoints
+GET_ACL_DETAILS = 'https://{0}/api/rest/smb_share/{1}/get_acl'
+SET_ACL_DETAILS = 'https://{0}/api/rest/smb_share/{1}/set_acl'
+
 # File Tree Quota endpoints
 GET_TREE_QUOTA_LIST_URL = 'https://{0}/api/rest/file_tree_quota'
 CREATE_TREE_QUOTA_URL = GET_TREE_QUOTA_LIST_URL
 GET_TREE_QUOTA_DETAILS_URL = 'https://{0}/api/rest/file_tree_quota/{1}'
 MODIFY_TREE_QUOTA_URL = GET_TREE_QUOTA_DETAILS_URL
 DELETE_TREE_QUOTA_URL = GET_TREE_QUOTA_DETAILS_URL
```

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/utils/exception.py` & `PyPowerStore-3.3.0.0/PyPowerStore/utils/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright: (c) 2019, Dell Technologies
+# Copyright: (c) 2024, Dell Technologies
 
 """PowerStore exceptions"""
 
 
 class PowerStoreException(Exception):
     """Class for PowerStore exceptions"""
     HTTP_ERR = 1
```

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/utils/helpers.py` & `PyPowerStore-3.3.0.0/PyPowerStore/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/client.py` & `PyPowerStore-3.3.0.0/PyPowerStore/client.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/configuration.py` & `PyPowerStore-3.3.0.0/PyPowerStore/configuration.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/powerstore_conn.py` & `PyPowerStore-3.3.0.0/PyPowerStore/powerstore_conn.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/protection.py` & `PyPowerStore-3.3.0.0/PyPowerStore/protection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# Copyright: (c) 2019, Dell Technologies
-# Copyright: (c) 2019, Ivan Pchelintsev <Ivan.Pchelintsev@emc.com>
+# Copyright: (c) 2024, Dell Technologies
+# Copyright: (c) 2024, Ivan Pchelintsev <Ivan.Pchelintsev@emc.com>
 
 """Collection of protection related functions for PowerStore"""
 
 from collections import namedtuple
 
 from PyPowerStore.utils import constants, helpers
```

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore/provisioning.py` & `PyPowerStore-3.3.0.0/PyPowerStore/provisioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -2006,15 +2006,15 @@
 
         :returns: SMB shares
         :rtype: list of dict
         """
         LOG.info("Getting smbshares with filter: '%s' and all_pages: %s"
                  % (filter_dict, all_pages))
         querystring = helpers.prepare_querystring(
-            constants.SELECT_ID_AND_NAME, filter_dict)
+            constants.SELECT_ALL_SMB_SHARE, filter_dict)
         LOG.info("Querystring: '%s'" % querystring)
         return self.client.request(constants.GET,
                                    constants.GET_SMB_SHARE_LIST_URL.format
                                    (self.server_ip), payload=None,
                                    querystring=querystring,
                                    all_pages=all_pages)
 
@@ -2105,14 +2105,55 @@
         LOG.info("Deleting smbshare: '%s'" % share_id)
         return self.client.request(constants.DELETE,
                                    constants.DELETE_SMB_SHARE_URL
                                    .format(
                                        self.server_ip, share_id))
     # SMB Share Methods End
 
+    # ACL Methods
+
+    def get_acl(self, share_id):
+        """
+        Retrieves the Access Control List (ACL) details for a given share ID.
+
+        :param share_id: The ID of the share for which to retrieve the ACL details.
+        :type share_id: str
+        :return: The response from the client's request to retrieve the ACL details.
+        :rtype: dict
+        """
+        LOG.info(f"Getting ACL details: '{share_id}'")
+        return self.client.request(
+            constants.POST,
+            constants.GET_ACL_DETAILS.format(self.server_ip, share_id),
+        )
+
+    def set_acl(self, share_id, add_aces=None, remove_aces=None):
+        """
+        Sets the access control list (ACL) for a given share.
+        Args:
+            share_id (str): The ID of the share.
+            add_aces (list, optional): A list of access control entries
+              (ACEs) to add to the ACL. Defaults to None.
+            remove_aces (list, optional): A list of access control entries
+              (ACEs) to remove from the ACL. Defaults to None.
+
+        Returns:
+            dict: The response from the server after setting the ACL.
+        """
+        payload = dict()
+        if add_aces:
+            payload["add_aces"] = add_aces
+        if remove_aces:
+            payload["remove_aces"] = remove_aces
+        return self.client.request(
+            constants.POST, constants.SET_ACL_DETAILS.format(
+                self.server_ip, share_id), payload=payload)
+
+    # ACL Methods End
+
     # FS Quota Methods
     def get_file_tree_quotas(self, filter_dict=None, all_pages=False):
         """Get a list of file tree quotas.
 
         :param filter_dict: (optional) Filter detail
         :type filter_dict: dict
         :param all_pages: (optional) Indicates whether to return all element
```

### Comparing `PyPowerStore-3.2.0.0/PyPowerStore.egg-info/SOURCES.txt` & `PyPowerStore-3.3.0.0/PyPowerStore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/README.md` & `PyPowerStore-3.3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.2.0.0/setup.py` & `PyPowerStore-3.3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
 setup(name='PyPowerStore',
-      version='3.2.0.0',
+      version='3.3.0.0',
       description='Python Library for Dell PowerStore',
       author='Ansible Team at Dell',
       author_email='ansible.team@dell.com',
       install_requires=[
         'urllib3>=1.26.7',
         'requests>=2.23.0'
       ],
```

