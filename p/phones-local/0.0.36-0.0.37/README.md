# Comparing `tmp/phones_local-0.0.36.tar.gz` & `tmp/phones_local-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.36.tar", last modified: Wed May 29 19:24:13 2024, max compression
+gzip compressed data, was "phones_local-0.0.37.tar", last modified: Thu May 30 15:30:07 2024, max compression
```

## Comparing `phones_local-0.0.36.tar` & `phones_local-0.0.37.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.944059 phones_local-0.0.36/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 19:24:13.944059 phones_local-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-29 19:23:43.000000 phones_local-0.0.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.940059 phones_local-0.0.36/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.944059 phones_local-0.0.36/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:23:43.000000 phones_local-0.0.36/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-29 19:23:43.000000 phones_local-0.0.36/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-29 19:23:43.000000 phones_local-0.0.36/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:13.944059 phones_local-0.0.36/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 19:24:13.000000 phones_local-0.0.36/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-29 19:23:50.000000 phones_local-0.0.36/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:24:13.944059 phones_local-0.0.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 19:23:43.000000 phones_local-0.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.197425 phones_local-0.0.37/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 15:30:07.197425 phones_local-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-30 15:29:23.000000 phones_local-0.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.193425 phones_local-0.0.37/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.197425 phones_local-0.0.37/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:29:23.000000 phones_local-0.0.37/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 15:29:23.000000 phones_local-0.0.37/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-30 15:29:23.000000 phones_local-0.0.37/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:30:07.197425 phones_local-0.0.37/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:30:07.000000 phones_local-0.0.37/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 15:29:43.000000 phones_local-0.0.37/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:30:07.197425 phones_local-0.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:29:23.000000 phones_local-0.0.37/setup.py
```

### Comparing `phones_local-0.0.36/PKG-INFO` & `phones_local-0.0.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.36
+Version: 0.0.37
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.36/README.md` & `phones_local-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.36/phones_local/src/phone_local_constans.py` & `phones_local-0.0.37/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.36/phones_local/src/phones_local.py` & `phones_local-0.0.37/phones_local/src/phones_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
             assert location_id, "location_id is required for getting country_id"
             country_id = self.select_one_value_by_column_and_value(
                 schema_name="location", view_table_name='location_view', select_clause_value='country_id',
                 column_name='location_id', column_value=location_id)
 
         country_iso_code = self.select_one_value_by_column_and_value(
-            schema_name="country", view_table_name='country_ml_view', select_clause_value='iso',
+            schema_name="location", view_table_name='country_ml_view', select_clause_value='iso',
             column_name='country_id', column_value=country_id)
         return country_iso_code
 
     # TODO: Is it really necessary to access the database for location?
     # I think it's possible to get the normalized phone number and the international code
     # from original_phone_number
     def process_phone(self, original_phone_number: str, country_iso_code: str = None, contact_id: int = None,
```

### Comparing `phones_local-0.0.36/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.37/phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.36
+Version: 0.0.37
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.36/pyproject.toml` & `phones_local-0.0.37/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.36/setup.py` & `phones_local-0.0.37/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.36',  # https://pypi.org/project/phones-local/
+    version='0.0.37',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

