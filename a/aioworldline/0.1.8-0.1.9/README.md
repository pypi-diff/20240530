# Comparing `tmp/aioworldline-0.1.8.tar.gz` & `tmp/aioworldline-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworldline-0.1.8.tar", last modified: Mon Apr 22 06:18:27 2024, max compression
+gzip compressed data, was "aioworldline-0.1.9.tar", last modified: Wed May  8 09:06:48 2024, max compression
```

## Comparing `aioworldline-0.1.8.tar` & `aioworldline-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.192019 aioworldline-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-22 06:18:17.000000 aioworldline-0.1.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.188019 aioworldline-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.188019 aioworldline-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-22 06:18:17.000000 aioworldline-0.1.8/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-22 06:18:17.000000 aioworldline-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 06:18:17.000000 aioworldline-0.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 06:18:17.000000 aioworldline-0.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-04-22 06:18:17.000000 aioworldline-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-22 06:18:27.192019 aioworldline-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 06:18:17.000000 aioworldline-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 06:18:17.000000 aioworldline-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.192019 aioworldline-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.192019 aioworldline-0.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 06:18:17.000000 aioworldline-0.1.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 06:18:17.000000 aioworldline-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 06:18:17.000000 aioworldline-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 06:18:17.000000 aioworldline-0.1.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-22 06:18:27.196019 aioworldline-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-22 06:18:17.000000 aioworldline-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.188019 aioworldline-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.192019 aioworldline-0.1.8/src/aioworldline/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-22 06:18:17.000000 aioworldline-0.1.8/src/aioworldline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 06:18:17.000000 aioworldline-0.1.8/src/aioworldline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-22 06:18:17.000000 aioworldline-0.1.8/src/aioworldline/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-22 06:18:17.000000 aioworldline-0.1.8/src/aioworldline/worldline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.192019 aioworldline-0.1.8/src/aioworldline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-22 06:18:27.000000 aioworldline-0.1.8/src/aioworldline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 06:18:27.000000 aioworldline-0.1.8/src/aioworldline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:18:27.000000 aioworldline-0.1.8/src/aioworldline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:18:27.000000 aioworldline-0.1.8/src/aioworldline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 06:18:27.000000 aioworldline-0.1.8/src/aioworldline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 06:18:27.000000 aioworldline-0.1.8/src/aioworldline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:18:27.192019 aioworldline-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-22 06:18:17.000000 aioworldline-0.1.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.520148 aioworldline-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 09:06:40.000000 aioworldline-0.1.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.512148 aioworldline-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.516148 aioworldline-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 09:06:40.000000 aioworldline-0.1.9/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-08 09:06:40.000000 aioworldline-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 09:06:40.000000 aioworldline-0.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 09:06:40.000000 aioworldline-0.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-08 09:06:40.000000 aioworldline-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-08 09:06:48.520148 aioworldline-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 09:06:40.000000 aioworldline-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 09:06:40.000000 aioworldline-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.516148 aioworldline-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.516148 aioworldline-0.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 09:06:40.000000 aioworldline-0.1.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 09:06:40.000000 aioworldline-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 09:06:40.000000 aioworldline-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 09:06:40.000000 aioworldline-0.1.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-08 09:06:48.520148 aioworldline-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-08 09:06:40.000000 aioworldline-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.512148 aioworldline-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.516148 aioworldline-0.1.9/src/aioworldline/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 09:06:40.000000 aioworldline-0.1.9/src/aioworldline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-08 09:06:40.000000 aioworldline-0.1.9/src/aioworldline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-08 09:06:40.000000 aioworldline-0.1.9/src/aioworldline/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-08 09:06:40.000000 aioworldline-0.1.9/src/aioworldline/worldline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.516148 aioworldline-0.1.9/src/aioworldline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-08 09:06:48.000000 aioworldline-0.1.9/src/aioworldline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 09:06:48.000000 aioworldline-0.1.9/src/aioworldline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:06:48.000000 aioworldline-0.1.9/src/aioworldline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:06:48.000000 aioworldline-0.1.9/src/aioworldline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 09:06:48.000000 aioworldline-0.1.9/src/aioworldline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 09:06:48.000000 aioworldline-0.1.9/src/aioworldline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:06:48.516148 aioworldline-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 09:06:40.000000 aioworldline-0.1.9/tests/conftest.py
```

### Comparing `aioworldline-0.1.8/.coveragerc` & `aioworldline-0.1.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/.github/workflows/python-publish.yaml` & `aioworldline-0.1.9/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/.gitignore` & `aioworldline-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/LICENSE` & `aioworldline-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/PKG-INFO` & `aioworldline-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: aioworldline
-Version: 0.1.8
+Version: 0.1.9
 Summary: Unofficial Worldline portal data retrieving client
 Home-page: https://github.com/kamikaze/aioworldline
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/aioworldline/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: aiohttp[speedups]==3.9.5
-Requires-Dist: pydantic==2.7.0
-Requires-Dist: pydantic_settings==2.2.1
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pydantic-settings==2.2.1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 aioworldline
 ============
```

### Comparing `aioworldline-0.1.8/docs/Makefile` & `aioworldline-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/docs/conf.py` & `aioworldline-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/docs/index.rst` & `aioworldline-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/setup.cfg` & `aioworldline-0.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aioworldline
-version = 0.1.8
+version = 0.1.9
 description = Unofficial Worldline portal data retrieving client
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/aioworldline
@@ -20,16 +20,16 @@
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	aiohttp[speedups]==3.9.5
-	pydantic==2.7.0
-	pydantic_settings==2.2.1
+	pydantic==2.7.1
+	pydantic-settings==2.2.1
 python_requires = >=3.12
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `aioworldline-0.1.8/src/aioworldline/worldline.py` & `aioworldline-0.1.9/src/aioworldline/worldline.py`

 * *Files identical despite different names*

### Comparing `aioworldline-0.1.8/src/aioworldline.egg-info/PKG-INFO` & `aioworldline-0.1.9/src/aioworldline.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: aioworldline
-Version: 0.1.8
+Version: 0.1.9
 Summary: Unofficial Worldline portal data retrieving client
 Home-page: https://github.com/kamikaze/aioworldline
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/aioworldline/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: aiohttp[speedups]==3.9.5
-Requires-Dist: pydantic==2.7.0
-Requires-Dist: pydantic_settings==2.2.1
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pydantic-settings==2.2.1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 aioworldline
 ============
```

### Comparing `aioworldline-0.1.8/src/aioworldline.egg-info/SOURCES.txt` & `aioworldline-0.1.9/src/aioworldline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

