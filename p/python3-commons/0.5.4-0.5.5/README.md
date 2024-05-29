# Comparing `tmp/python3_commons-0.5.4.tar.gz` & `tmp/python3_commons-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.4.tar", last modified: Wed May 29 21:01:36 2024, max compression
+gzip compressed data, was "python3_commons-0.5.5.tar", last modified: Wed May 29 22:21:32 2024, max compression
```

## Comparing `python3_commons-0.5.4.tar` & `python3_commons-0.5.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.765667 python3_commons-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 21:01:31.000000 python3_commons-0.5.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.753667 python3_commons-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.757667 python3_commons-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 21:01:31.000000 python3_commons-0.5.4/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 21:01:31.000000 python3_commons-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:01:31.000000 python3_commons-0.5.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 21:01:31.000000 python3_commons-0.5.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 21:01:31.000000 python3_commons-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 21:01:36.765667 python3_commons-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 21:01:31.000000 python3_commons-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 21:01:31.000000 python3_commons-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.757667 python3_commons-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.757667 python3_commons-0.5.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:01:31.000000 python3_commons-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 21:01:31.000000 python3_commons-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 21:01:31.000000 python3_commons-0.5.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 21:01:31.000000 python3_commons-0.5.4/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 21:01:36.765667 python3_commons-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 21:01:31.000000 python3_commons-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.753667 python3_commons-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 21:01:31.000000 python3_commons-0.5.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 21:01:31.000000 python3_commons-0.5.4/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 21:01:31.000000 python3_commons-0.5.4/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.851035 python3_commons-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 22:21:19.000000 python3_commons-0.5.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.843035 python3_commons-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.843035 python3_commons-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 22:21:19.000000 python3_commons-0.5.5/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 22:21:19.000000 python3_commons-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 22:21:19.000000 python3_commons-0.5.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 22:21:19.000000 python3_commons-0.5.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 22:21:19.000000 python3_commons-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 22:21:32.851035 python3_commons-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 22:21:19.000000 python3_commons-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 22:21:19.000000 python3_commons-0.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.847035 python3_commons-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.847035 python3_commons-0.5.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 22:21:19.000000 python3_commons-0.5.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 22:21:19.000000 python3_commons-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 22:21:19.000000 python3_commons-0.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 22:21:19.000000 python3_commons-0.5.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 22:21:19.000000 python3_commons-0.5.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 22:21:32.851035 python3_commons-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 22:21:19.000000 python3_commons-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.843035 python3_commons-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.847035 python3_commons-0.5.5/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.847035 python3_commons-0.5.5/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.847035 python3_commons-0.5.5/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 22:21:19.000000 python3_commons-0.5.5/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.851035 python3_commons-0.5.5/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 22:21:32.000000 python3_commons-0.5.5/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 22:21:32.000000 python3_commons-0.5.5/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:21:32.000000 python3_commons-0.5.5/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:21:32.000000 python3_commons-0.5.5/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 22:21:32.000000 python3_commons-0.5.5/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 22:21:32.000000 python3_commons-0.5.5/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:21:32.851035 python3_commons-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 22:21:19.000000 python3_commons-0.5.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 22:21:19.000000 python3_commons-0.5.5/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 22:21:19.000000 python3_commons-0.5.5/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.4/.coveragerc` & `python3_commons-0.5.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/.github/workflows/python-publish.yaml` & `python3_commons-0.5.5/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/.gitignore` & `python3_commons-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/LICENSE` & `python3_commons-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/PKG-INFO` & `python3_commons-0.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.4
+Version: 0.5.5
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.4/docs/Makefile` & `python3_commons-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/docs/conf.py` & `python3_commons-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/docs/index.rst` & `python3_commons-0.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/setup.cfg` & `python3_commons-0.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.4
+version = 0.5.5
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.4/src/python3_commons/audit.py` & `python3_commons-0.5.5/src/python3_commons/audit.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 logger = logging.getLogger(__name__)
 
 
 async def write_audit_data(settings: S3Settings, key: str, data: bytes):
     if settings.s3_secret_access_key:
         try:
             client = get_s3_client(settings)
+            absolute_path = object_storage.get_absolute_path(f'audit/{key}')
 
-            client.put_object(settings.s3_bucket, f'audit/{key}', io.BytesIO(data), len(data))
+            client.put_object(settings.s3_bucket, absolute_path, io.BytesIO(data), len(data))
         except S3Error as e:
             logger.error(f'Failed storing object in storage: {e}')
         else:
             logger.debug(f'Stored object in storage: {key}')
     else:
         logger.debug(f'S3 is not configured, not storing object in storage: {key}')
```

### Comparing `python3_commons-0.5.4/src/python3_commons/conf.py` & `python3_commons-0.5.5/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons/db.py` & `python3_commons-0.5.5/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons/helpers.py` & `python3_commons-0.5.5/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.5/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons/object_storage.py` & `python3_commons-0.5.5/src/python3_commons/object_storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import logging
 from datetime import datetime
 from typing import Generator, Iterable
 
-from minio import Minio, S3Error
+from minio import Minio
 from minio.datatypes import Object
 from minio.deleteobjects import DeleteObject, DeleteError
 
 from python3_commons.conf import s3_settings, S3Settings
 
 logger = logging.getLogger(__name__)
 __CLIENT = None
@@ -39,27 +39,29 @@
     return path
 
 
 def put_object(bucket_name: str, path: str, data: io.BytesIO, length: int) -> str:
     s3_client = get_s3_client(s3_settings)
 
     if s3_client:
+        path = get_absolute_path(path)
         result = s3_client.put_object(bucket_name, path, data, length)
 
         logger.debug(f'Stored object into object storage: {bucket_name}:{path}')
 
         return result.location
     else:
         logger.warning(f'No S3 client available, skipping object put')
 
 
 def get_object_stream(bucket_name: str, path: str):
     s3_client = get_s3_client(s3_settings)
 
     if s3_client:
+        path = get_absolute_path(path)
         logger.debug(f'Getting object from object storage: {bucket_name}:{path}')
 
         try:
             response = s3_client.get_object(bucket_name, path)
         except Exception as e:
             logger.debug(f'Failed getting object from object storage: {bucket_name}:{path}', exc_info=e)
 
@@ -88,14 +90,16 @@
     s3_client = get_s3_client(s3_settings)
 
     yield from s3_client.list_objects(bucket_name, prefix=prefix, recursive=recursive)
 
 
 def get_objects(bucket_name: str, path: str,
                 recursive: bool = True) -> Generator[tuple[str, datetime, bytes], None, None]:
+    path = get_absolute_path(path)
+
     for obj in list_objects(bucket_name, path, recursive):
         object_name = obj.object_name
 
         if obj.size:
             data = get_object(bucket_name, object_name)
         else:
             data = b''
@@ -109,14 +113,15 @@
 
 
 def remove_objects(bucket_name: str, prefix: str = None,
                    object_names: Iterable[str] = None) -> Iterable[DeleteError] | None:
     s3_client = get_s3_client(s3_settings)
 
     if prefix:
+        prefix = get_absolute_path(prefix)
         delete_object_list = map(
             lambda obj: DeleteObject(obj.object_name), s3_client.list_objects(bucket_name, prefix=prefix,
                                                                               recursive=True)
         )
     elif object_names:
         delete_object_list = map(DeleteObject, object_names)
     else:
```

### Comparing `python3_commons-0.5.4/src/python3_commons/serializers/json.py` & `python3_commons-0.5.5/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.5/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.5/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.5/src/python3_commons.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.4
+Version: 0.5.5
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.4/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.5/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/tests/conftest.py` & `python3_commons-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/tests/test_msgpack.py` & `python3_commons-0.5.5/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.4/tests/test_msgspec.py` & `python3_commons-0.5.5/tests/test_msgspec.py`

 * *Files identical despite different names*

