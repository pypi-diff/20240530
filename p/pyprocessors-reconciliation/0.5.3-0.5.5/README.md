# Comparing `tmp/pyprocessors_reconciliation-0.5.3.tar.gz` & `tmp/pyprocessors_reconciliation-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_reconciliation-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors_reconciliation-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors_reconciliation-0.5.3.tar` & `pyprocessors_reconciliation-0.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1731 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/.gitignore
--rwxr-xr-x   0        0        0      123 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/AUTHORS.md
--rwxr-xr-x   0        0        0      268 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/CHANGELOG.md
--rwxr-xr-x   0        0        0      476 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/Dockerfile
--rwxr-xr-x   0        0        0    10236 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/Jenkinsfile
--rwxr-xr-x   0        0        0     1082 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/LICENSE
--rwxr-xr-x   0        0        0     1660 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/README.md
--rwxr-xr-x   0        0        0      953 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/RELEASE.md
--rwxr-xr-x   0        0        0     1559 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/bumpversion.py
--rwxr-xr-x   0        0        0       62 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/.gitignore
--rwxr-xr-x   0        0        0      268 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/CHANGELOG.md
--rwxr-xr-x   0        0        0     1082 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/LICENSE
--rwxr-xr-x   0        0        0        0 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/_static/.gitkeep
--rwxr-xr-x   0        0        0        0 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/_templates/.gitkeep
--rwxr-xr-x   0        0        0     2909 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/conf.py
--rwxr-xr-x   0        0        0      148 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/docs/index.rst
--rwxr-xr-x   0        0        0       98 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/mypy.ini
--rwxr-xr-x   0        0        0     2314 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/pyproject.toml
--rwxr-xr-x   0        0        0     1921 2024-05-30 07:17:16.895024 pyprocessors_reconciliation-0.5.3/results.xml
--rwxr-xr-x   0        0        0       60 2024-05-30 07:18:49.778024 pyprocessors_reconciliation-0.5.3/src/pyprocessors_reconciliation/__init__.py
--rwxr-xr-x   0        0        0    12237 2024-05-30 07:17:16.895024 pyprocessors_reconciliation-0.5.3/src/pyprocessors_reconciliation/reconciliation.py
--rwxr-xr-x   0        0        0        0 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/tests/__init__.py
--rwxr-xr-x   0        0        0     6824 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/tests/data/afp_ner_fr-document-test-whitelist2.json
--rw-r--r--   0        0        0    20748 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/tests/data/x_cago_ner_en-document-test.json
--rw-r--r--   0        0        0    17283 2024-05-30 07:18:46.985934 pyprocessors_reconciliation-0.5.3/tests/data/x_cago_ner_en-document_conso.json
--rwxr-xr-x   0        0        0     2243 2024-05-30 07:17:16.899025 pyprocessors_reconciliation-0.5.3/tests/test_reconciliation.py
--rwxr-xr-x   0        0        0      893 2024-05-30 06:58:18.374180 pyprocessors_reconciliation-0.5.3/tox.ini
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.3/setup.py
--rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1774 2024-05-30 17:31:20.484068 pyprocessors_reconciliation-0.5.5/.gitignore
+-rwxr-xr-x   0        0        0      123 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/AUTHORS.md
+-rwxr-xr-x   0        0        0      268 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/CHANGELOG.md
+-rwxr-xr-x   0        0        0      476 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/Dockerfile
+-rw-r--r--   0        0        0    13995 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/Jenkinsfile
+-rwxr-xr-x   0        0        0     1082 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/LICENSE
+-rwxr-xr-x   0        0        0     1660 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/README.md
+-rwxr-xr-x   0        0        0      953 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/RELEASE.md
+-rwxr-xr-x   0        0        0     1559 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/bumpversion.py
+-rwxr-xr-x   0        0        0       62 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/.gitignore
+-rwxr-xr-x   0        0        0      268 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1082 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/LICENSE
+-rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/_static/.gitkeep
+-rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/_templates/.gitkeep
+-rwxr-xr-x   0        0        0     2909 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/conf.py
+-rwxr-xr-x   0        0        0      148 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/docs/index.rst
+-rwxr-xr-x   0        0        0       98 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/mypy.ini
+-rwxr-xr-x   0        0        0     2314 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/pyproject.toml
+-rwxr-xr-x   0        0        0     1921 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/results.xml
+-rwxr-xr-x   0        0        0       60 2024-05-30 17:43:14.710453 pyprocessors_reconciliation-0.5.5/src/pyprocessors_reconciliation/__init__.py
+-rwxr-xr-x   0        0        0    12237 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/src/pyprocessors_reconciliation/reconciliation.py
+-rwxr-xr-x   0        0        0        0 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/tests/__init__.py
+-rwxr-xr-x   0        0        0     6824 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/tests/data/afp_ner_fr-document-test-whitelist2.json
+-rw-r--r--   0        0        0    20748 2024-05-30 17:41:23.210952 pyprocessors_reconciliation-0.5.5/tests/data/x_cago_ner_en-document-test.json
+-rw-r--r--   0        0        0    17283 2024-05-30 17:43:12.106371 pyprocessors_reconciliation-0.5.5/tests/data/x_cago_ner_en-document_conso.json
+-rwxr-xr-x   0        0        0     2243 2024-05-30 17:41:23.214952 pyprocessors_reconciliation-0.5.5/tests/test_reconciliation.py
+-rwxr-xr-x   0        0        0      893 2024-05-30 17:41:23.214952 pyprocessors_reconciliation-0.5.5/tox.ini
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.5/setup.py
+-rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 pyprocessors_reconciliation-0.5.5/PKG-INFO
```

### Comparing `pyprocessors_reconciliation-0.5.3/.gitignore` & `pyprocessors_reconciliation-0.5.5/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -120,7 +120,11 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Specific
+.groovylintrc.json
+.emailNotif
```

### Comparing `pyprocessors_reconciliation-0.5.3/LICENSE` & `pyprocessors_reconciliation-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/README.md` & `pyprocessors_reconciliation-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/RELEASE.md` & `pyprocessors_reconciliation-0.5.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/bumpversion.py` & `pyprocessors_reconciliation-0.5.5/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/docs/LICENSE` & `pyprocessors_reconciliation-0.5.5/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/docs/conf.py` & `pyprocessors_reconciliation-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/pyproject.toml` & `pyprocessors_reconciliation-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/results.xml` & `pyprocessors_reconciliation-0.5.5/results.xml`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/src/pyprocessors_reconciliation/reconciliation.py` & `pyprocessors_reconciliation-0.5.5/src/pyprocessors_reconciliation/reconciliation.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/tests/data/afp_ner_fr-document-test-whitelist2.json` & `pyprocessors_reconciliation-0.5.5/tests/data/afp_ner_fr-document-test-whitelist2.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/tests/data/x_cago_ner_en-document-test.json` & `pyprocessors_reconciliation-0.5.5/tests/data/x_cago_ner_en-document-test.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/tests/data/x_cago_ner_en-document_conso.json` & `pyprocessors_reconciliation-0.5.5/tests/data/x_cago_ner_en-document_conso.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/tests/test_reconciliation.py` & `pyprocessors_reconciliation-0.5.5/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/tox.ini` & `pyprocessors_reconciliation-0.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_reconciliation-0.5.3/setup.py` & `pyprocessors_reconciliation-0.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['reconciliation = '
                           'pyprocessors_reconciliation.reconciliation:ReconciliationProcessor']}
 
 setup(name='pyprocessors-reconciliation',
-      version='0.5.3',
+      version='0.5.5',
       description='Sherpa reconciliation processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_reconciliation/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors_reconciliation-0.5.3/PKG-INFO` & `pyprocessors_reconciliation-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-reconciliation
-Version: 0.5.3
+Version: 0.5.5
 Summary: Sherpa reconciliation processor
 Home-page: https://github.com/oterrier/pyprocessors_reconciliation/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

