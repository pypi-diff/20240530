# Comparing `tmp/contact-persons-local-0.0.8.tar.gz` & `tmp/contact_persons_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-persons-local-0.0.8.tar", last modified: Tue Feb 20 17:03:25 2024, max compression
+gzip compressed data, was "contact_persons_local-0.0.9.tar", last modified: Thu May  9 06:41:13 2024, max compression
```

## Comparing `contact-persons-local-0.0.8.tar` & `contact_persons_local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 17:03:25.066428 contact-persons-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-20 17:03:25.066428 contact-persons-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-20 17:02:40.000000 contact-persons-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 17:03:25.062428 contact-persons-local-0.0.8/contact_persons_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 17:03:25.066428 contact-persons-local-0.0.8/contact_persons_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-02-20 17:02:40.000000 contact-persons-local-0.0.8/contact_persons_local/src/contact_persons_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-20 17:02:40.000000 contact-persons-local-0.0.8/contact_persons_local/src/contact_persons_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 17:03:25.066428 contact-persons-local-0.0.8/contact_persons_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-20 17:03:25.000000 contact-persons-local-0.0.8/contact_persons_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-20 17:03:25.000000 contact-persons-local-0.0.8/contact_persons_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 17:03:25.000000 contact-persons-local-0.0.8/contact_persons_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-20 17:03:25.000000 contact-persons-local-0.0.8/contact_persons_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-20 17:03:25.000000 contact-persons-local-0.0.8/contact_persons_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-20 17:02:40.000000 contact-persons-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 17:03:25.066428 contact-persons-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-20 17:02:40.000000 contact-persons-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:41:13.981045 contact_persons_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 06:41:13.981045 contact_persons_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-09 06:40:48.000000 contact_persons_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:41:13.977045 contact_persons_local-0.0.9/contact_persons_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:41:13.981045 contact_persons_local-0.0.9/contact_persons_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-09 06:40:48.000000 contact_persons_local-0.0.9/contact_persons_local/src/contact_persons_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 06:40:48.000000 contact_persons_local-0.0.9/contact_persons_local/src/contact_persons_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:41:13.981045 contact_persons_local-0.0.9/contact_persons_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 06:41:13.000000 contact_persons_local-0.0.9/contact_persons_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 06:41:13.000000 contact_persons_local-0.0.9/contact_persons_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:41:13.000000 contact_persons_local-0.0.9/contact_persons_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 06:41:13.000000 contact_persons_local-0.0.9/contact_persons_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 06:41:13.000000 contact_persons_local-0.0.9/contact_persons_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-09 06:40:48.000000 contact_persons_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:41:13.981045 contact_persons_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 06:40:48.000000 contact_persons_local-0.0.9/setup.py
```

### Comparing `contact-persons-local-0.0.8/PKG-INFO` & `contact_persons_local-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: contact-persons-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-person-local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: person-local>=0.0.37
+Requires-Dist: person-local>=0.0.52
 Requires-Dist: python-sdk-remote>=0.0.27
+Requires-Dist: language-remote
```

### Comparing `contact-persons-local-0.0.8/README.md` & `contact_persons_local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `contact-persons-local-0.0.8/contact_persons_local/src/contact_persons_local.py` & `contact_persons_local-0.0.9/contact_persons_local/src/contact_persons_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .contact_persons_local_constants import CONTACT_PERSONS_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
 from logger_local.LoggerLocal import Logger
 from database_mysql_local.generic_mapping import GenericMapping
-from person_local.src.persons_local import PersonsLocal
-from person_local.src.persons_local import Person
+from person_local.persons_local import PersonsLocal
+from person_local.persons_local import Person
 
 logger = Logger.create_logger(object=CONTACT_PERSONS_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 
 DEFAULT_SCHEMA_NAME = 'contact_person'
 DEFAULT_ENTITY_NAME1 = 'contact'
 DEFAULT_ENTITY_NAME2 = 'person'
 DEFAULT_ID_COLUMN_NAME = 'contact_person_id'
@@ -36,18 +36,20 @@
         :param contact_id: contact id
         :param is_test_data: is test data
         :return: contact_person_id
         """
         logger.start(object={"contact_dict": contact_dict, "contact_email_address": contact_email_address,
                              "contact_id": contact_id})
         # TODO: also check if contact_person_id by phone number
-        if not contact_email_address:
-            logger.end(log_message="contact_email_address is None")
-            return None
-        person_id = self.persons_local.get_person_id_by_email_address(email_address=contact_email_address)
+        person_id = self.select_one_value_by_id(select_clause_value="person_id",
+                                                id_column_name="contact_id",
+                                                id_column_value=contact_id)
+        if contact_email_address and person_id is None:
+            # TODO: use upsert with both email_addresses and phone_numbers
+            person_id = self.persons_local.get_person_id_by_email_address(email_address=contact_email_address)
         if person_id is None:
             # create new person and add it to person_table
             logger.info(log_message="person_id is None, creating new person")
             person_object = self._proccess_contact_dict_to_person_class(contact_dict=contact_dict,
                                                                         contact_email_address=contact_email_address)
             result = self.persons_local.insert_if_not_exists(person=person_object)
             if result:
```

### Comparing `contact-persons-local-0.0.8/contact_persons_local/src/contact_persons_local_constants.py` & `contact_persons_local-0.0.9/contact_persons_local/src/contact_persons_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact-persons-local-0.0.8/contact_persons_local.egg-info/PKG-INFO` & `contact_persons_local-0.0.9/contact_persons_local.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: contact-persons-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-person-local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: person-local>=0.0.37
+Requires-Dist: person-local>=0.0.52
 Requires-Dist: python-sdk-remote>=0.0.27
+Requires-Dist: language-remote
```

### Comparing `contact-persons-local-0.0.8/setup.py` & `contact_persons_local-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 PACKAGE_NAME = "contact-persons-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/contact-person-local
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/contact-persons-local
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-person-local Python",
     long_description="",
     long_description_content_type='text/markdown',
     url="https://github.com/circles",  # https://pypi.org/project/contact-person-local
     packages=[package_dir],
@@ -21,11 +21,12 @@
     ],
     # TODO: Update which packages to include with this package
     install_requires=[
         'PyMySQL>=1.0.2',
         'pytest>=7.4.0',
         'mysql-connector>=2.2.9',
         'logzio-python-handler>= 4.1.0',
-        'person-local>=0.0.37',
-        'python-sdk-remote>=0.0.27'
+        'person-local>=0.0.52',
+        'python-sdk-remote>=0.0.27',
+        'language-remote'
     ],
 )
```

