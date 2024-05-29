# Comparing `tmp/heaserver_organizations-1.4.2.tar.gz` & `tmp/heaserver_organizations-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_organizations-1.4.2.tar", last modified: Thu May 23 22:34:27 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.4.3.tar", last modified: Wed May 29 22:42:28 2024, max compression
```

## Comparing `heaserver_organizations-1.4.2.tar` & `heaserver_organizations-1.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.898150 heaserver_organizations-1.4.2/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5667 2024-05-23 22:34:27.896500 heaserver_organizations-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4244 2024-05-23 22:33:21.000000 heaserver_organizations-1.4.2/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/RELEASING.md
--rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.733137 heaserver_organizations-1.4.2/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.733137 heaserver_organizations-1.4.2/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.831032 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-23 22:34:27.898675 heaserver_organizations-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1931 2024-05-23 22:33:35.000000 heaserver_organizations-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.735136 heaserver_organizations-1.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.734137 heaserver_organizations-1.4.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.833387 heaserver_organizations-1.4.2/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    52582 2024-05-22 19:00:26.000000 heaserver_organizations-1.4.2/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.843820 heaserver_organizations-1.4.2/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    24887 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.895444 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     5667 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.736137 heaserver_organizations-1.4.2/tests/
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.737137 heaserver_organizations-1.4.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.892443 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.911460 heaserver_organizations-1.4.3/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5772 2024-05-29 22:42:28.909459 heaserver_organizations-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4349 2024-05-29 21:46:35.000000 heaserver_organizations-1.4.3/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/RELEASING.md
+-rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.668980 heaserver_organizations-1.4.3/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.669512 heaserver_organizations-1.4.3/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.812252 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 22:42:28.911460 heaserver_organizations-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1931 2024-05-29 22:41:49.000000 heaserver_organizations-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.671629 heaserver_organizations-1.4.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.670570 heaserver_organizations-1.4.3/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.829071 heaserver_organizations-1.4.3/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    52582 2024-05-23 22:35:54.000000 heaserver_organizations-1.4.3/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.841800 heaserver_organizations-1.4.3/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    26704 2024-05-29 21:15:39.000000 heaserver_organizations-1.4.3/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.907937 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     5772 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.672677 heaserver_organizations-1.4.3/tests/
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.672677 heaserver_organizations-1.4.3/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.905850 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver_organizations-1.4.2/Dockerfile` & `heaserver_organizations-1.4.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/LICENSE` & `heaserver_organizations-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/PKG-INFO` & `heaserver_organizations-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.2
+Version: 1.4.3
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,17 @@
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.3
+* Send the account ids and group id fields when submitting the members editor form.
+
 ## Version 1.4.2
 * Corrected heaobject.organization.Organization permissions.
 
 ## Version 1.4.1
 * Generate the correct name attribute for heaobject.keychain.AWSCredentials objects.
 
 ## Version 1.4.0
```

### Comparing `heaserver_organizations-1.4.2/README.md` & `heaserver_organizations-1.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.3
+* Send the account ids and group id fields when submitting the members editor form.
+
 ## Version 1.4.2
 * Corrected heaobject.organization.Organization permissions.
 
 ## Version 1.4.1
 * Generate the correct name attribute for heaobject.keychain.AWSCredentials objects.
 
 ## Version 1.4.0
```

### Comparing `heaserver_organizations-1.4.2/RELEASING.md` & `heaserver_organizations-1.4.3/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/docker-entrypoint.sh` & `heaserver_organizations-1.4.3/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/test_all.py` & `heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/run-swaggerui.py` & `heaserver_organizations-1.4.3/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/setup.py` & `heaserver_organizations-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.4.2',
+    version='1.4.3',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
```

### Comparing `heaserver_organizations-1.4.2/src/heaserver/organization/service.py` & `heaserver_organizations-1.4.3/src/heaserver/organization/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.4.3/src/heaserver/organization/wstl/all.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998794367283951%*

 * *Differences: {"'wstl'": "{'actions': {8: {'inputs': {6: {'hea': {'optionsFromUrl': {'path': 'accounts/'}}, "*

 * *           "'name': 'account_ids', 'prompt': 'Accounts', 'readOnly': True}, insert: [(18, "*

 * *           "OrderedDict([('hea', OrderedDict([('cardinality', 'multiple'), ('optionsFromUrl', "*

 * *           "OrderedDict([('path', 'groups/'), ('value', 'id'), ('text', 'display_name')])), "*

 * *           "('display', False)])), ('name', 'admin_group_ids'), ('prompt', 'Admin groups'), "*

 * *           "('type', 'select')])), (19,  […]*

```diff
@@ -380,21 +380,22 @@
                         "readOnly": true
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
                             "display": false,
                             "optionsFromUrl": {
-                                "path": "awsaccounts/",
+                                "path": "accounts/",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
-                        "name": "aws_account_ids",
-                        "prompt": "AWS Accounts",
+                        "name": "account_ids",
+                        "prompt": "Accounts",
+                        "readOnly": true,
                         "type": "select"
                     },
                     {
                         "hea": {
                             "optionsFromUrl": {
                                 "path": "people/",
                                 "text": "display_name",
@@ -545,14 +546,56 @@
                             "section": "shares"
                         },
                         "name": "type",
                         "prompt": "Type",
                         "readOnly": true,
                         "required": true,
                         "value": "heaobject.root.ShareImpl"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "display": false,
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "admin_group_ids",
+                        "prompt": "Admin groups",
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "display": false,
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "manager_group_ids",
+                        "prompt": "Manager groups",
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "display": false,
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "member_group_ids",
+                        "prompt": "Member groups",
+                        "type": "select"
                     }
                 ],
                 "name": "heaserver-organizations-organization-edit-membership",
                 "prompt": "Membership",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
```

### Comparing `heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.2
+Version: 1.4.3
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,17 @@
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.3
+* Send the account ids and group id fields when submitting the members editor form.
+
 ## Version 1.4.2
 * Corrected heaobject.organization.Organization permissions.
 
 ## Version 1.4.1
 * Generate the correct name attribute for heaobject.keychain.AWSCredentials objects.
 
 ## Version 1.4.0
```

### Comparing `heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.4.3/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.2/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.4.3/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*

