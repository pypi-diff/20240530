# Comparing `tmp/python3_commons-0.5.3.tar.gz` & `tmp/python3_commons-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.3.tar", last modified: Wed May 29 20:49:10 2024, max compression
+gzip compressed data, was "python3_commons-0.5.4.tar", last modified: Wed May 29 21:01:36 2024, max compression
```

## Comparing `python3_commons-0.5.3.tar` & `python3_commons-0.5.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 20:49:02.000000 python3_commons-0.5.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.254893 python3_commons-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.254893 python3_commons-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 20:49:02.000000 python3_commons-0.5.3/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 20:49:02.000000 python3_commons-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 20:49:02.000000 python3_commons-0.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 20:49:02.000000 python3_commons-0.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 20:49:02.000000 python3_commons-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 20:49:10.262893 python3_commons-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 20:49:02.000000 python3_commons-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 20:49:02.000000 python3_commons-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 20:49:02.000000 python3_commons-0.5.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 20:49:02.000000 python3_commons-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 20:49:02.000000 python3_commons-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 20:49:02.000000 python3_commons-0.5.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 20:49:02.000000 python3_commons-0.5.3/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 20:49:10.262893 python3_commons-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 20:49:02.000000 python3_commons-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.254893 python3_commons-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.258893 python3_commons-0.5.3/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 20:49:02.000000 python3_commons-0.5.3/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 20:49:10.000000 python3_commons-0.5.3/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:49:10.262893 python3_commons-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 20:49:02.000000 python3_commons-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 20:49:02.000000 python3_commons-0.5.3/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 20:49:02.000000 python3_commons-0.5.3/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.765667 python3_commons-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 21:01:31.000000 python3_commons-0.5.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.753667 python3_commons-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.757667 python3_commons-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 21:01:31.000000 python3_commons-0.5.4/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 21:01:31.000000 python3_commons-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:01:31.000000 python3_commons-0.5.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 21:01:31.000000 python3_commons-0.5.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 21:01:31.000000 python3_commons-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 21:01:36.765667 python3_commons-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 21:01:31.000000 python3_commons-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 21:01:31.000000 python3_commons-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.757667 python3_commons-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.757667 python3_commons-0.5.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 21:01:31.000000 python3_commons-0.5.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:01:31.000000 python3_commons-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 21:01:31.000000 python3_commons-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 21:01:31.000000 python3_commons-0.5.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 21:01:31.000000 python3_commons-0.5.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 21:01:36.765667 python3_commons-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 21:01:31.000000 python3_commons-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.753667 python3_commons-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 21:01:31.000000 python3_commons-0.5.4/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 21:01:36.000000 python3_commons-0.5.4/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:01:36.761667 python3_commons-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 21:01:31.000000 python3_commons-0.5.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 21:01:31.000000 python3_commons-0.5.4/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 21:01:31.000000 python3_commons-0.5.4/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.3/.coveragerc` & `python3_commons-0.5.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/.github/workflows/python-publish.yaml` & `python3_commons-0.5.4/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/.gitignore` & `python3_commons-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/LICENSE` & `python3_commons-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/PKG-INFO` & `python3_commons-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.3
+Version: 0.5.4
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.3/docs/Makefile` & `python3_commons-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/docs/conf.py` & `python3_commons-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/docs/index.rst` & `python3_commons-0.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/setup.cfg` & `python3_commons-0.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.3
+version = 0.5.4
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.3/src/python3_commons/audit.py` & `python3_commons-0.5.4/src/python3_commons/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 archive.addfile(info, BytesIO(content))
                 object_names.append(name)
 
     fo.seek(0)
 
     if object_names:
         archive_path = object_storage.get_absolute_path(
-            f'.archive/{year}_{month:02}_{day:02}.tar.bz2')
+            f'audit/.archive/{year}_{month:02}_{day:02}.tar.bz2')
         object_storage.put_object(bucket_name, archive_path, fo, fo.getbuffer().nbytes)
 
         if errors := object_storage.remove_objects(bucket_name, object_names=object_names):
             for error in errors:
                 logger.error(f'Failed to delete object in {bucket_name=}: {error}')
     else:
         logger.info('No objects to archive found.')
```

### Comparing `python3_commons-0.5.3/src/python3_commons/conf.py` & `python3_commons-0.5.4/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/db.py` & `python3_commons-0.5.4/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/helpers.py` & `python3_commons-0.5.4/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.4/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/object_storage.py` & `python3_commons-0.5.4/src/python3_commons/object_storage.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/serializers/json.py` & `python3_commons-0.5.4/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.4/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.4/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.4/src/python3_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.3
+Version: 0.5.4
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.3/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.4/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/tests/conftest.py` & `python3_commons-0.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/tests/test_msgpack.py` & `python3_commons-0.5.4/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.3/tests/test_msgspec.py` & `python3_commons-0.5.4/tests/test_msgspec.py`

 * *Files identical despite different names*

