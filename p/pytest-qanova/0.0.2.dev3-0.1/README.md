# Comparing `tmp/pytest_qanova-0.0.2.dev3.tar.gz` & `tmp/pytest_qanova-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_qanova-0.0.2.dev3.tar", last modified: Thu May 30 15:41:14 2024, max compression
+gzip compressed data, was "pytest_qanova-0.1.tar", last modified: Sun May 26 13:52:05 2024, max compression
```

## Comparing `pytest_qanova-0.0.2.dev3.tar` & `pytest_qanova-0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sa         (501) staff       (20)        0 2024-05-30 15:41:14.275285 pytest_qanova-0.0.2.dev3/
--rw-r--r--   0 sa         (501) staff       (20)     1073 2024-05-26 13:34:57.000000 pytest_qanova-0.0.2.dev3/LICENSE
--rw-r--r--   0 sa         (501) staff       (20)       30 2024-05-26 12:57:31.000000 pytest_qanova-0.0.2.dev3/MANIFEST.in
--rw-r--r--   0 sa         (501) staff       (20)      790 2024-05-30 15:41:14.274880 pytest_qanova-0.0.2.dev3/PKG-INFO
--rw-r--r--   0 sa         (501) staff       (20)       15 2024-05-26 13:42:57.000000 pytest_qanova-0.0.2.dev3/README.md
-drwxr-xr-x   0 sa         (501) staff       (20)        0 2024-05-30 15:41:14.271962 pytest_qanova-0.0.2.dev3/pytest_qanova/
--rw-r--r--   0 sa         (501) staff       (20)        0 2024-05-26 12:54:25.000000 pytest_qanova-0.0.2.dev3/pytest_qanova/__init__.py
--rw-r--r--   0 sa         (501) staff       (20)     2323 2024-05-30 15:40:55.000000 pytest_qanova-0.0.2.dev3/pytest_qanova/plugin.py
-drwxr-xr-x   0 sa         (501) staff       (20)        0 2024-05-30 15:41:14.274463 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/
--rw-r--r--   0 sa         (501) staff       (20)      790 2024-05-30 15:41:14.000000 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/PKG-INFO
--rw-r--r--   0 sa         (501) staff       (20)      312 2024-05-30 15:41:14.000000 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/SOURCES.txt
--rw-r--r--   0 sa         (501) staff       (20)        1 2024-05-30 15:41:14.000000 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/dependency_links.txt
--rw-r--r--   0 sa         (501) staff       (20)       48 2024-05-30 15:41:14.000000 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/entry_points.txt
--rw-r--r--   0 sa         (501) staff       (20)        7 2024-05-30 15:41:14.000000 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/requires.txt
--rw-r--r--   0 sa         (501) staff       (20)       14 2024-05-30 15:41:14.000000 pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/top_level.txt
--rw-r--r--   0 sa         (501) staff       (20)       38 2024-05-30 15:41:14.275362 pytest_qanova-0.0.2.dev3/setup.cfg
--rw-r--r--   0 sa         (501) staff       (20)     1103 2024-05-30 15:41:05.000000 pytest_qanova-0.0.2.dev3/setup.py
+drwxr-xr-x   0 sa         (501) staff       (20)        0 2024-05-26 13:52:05.570230 pytest_qanova-0.1/
+-rw-r--r--   0 sa         (501) staff       (20)     1073 2024-05-26 13:34:57.000000 pytest_qanova-0.1/LICENSE
+-rw-r--r--   0 sa         (501) staff       (20)       30 2024-05-26 12:57:31.000000 pytest_qanova-0.1/MANIFEST.in
+-rw-r--r--   0 sa         (501) staff       (20)      783 2024-05-26 13:52:05.569884 pytest_qanova-0.1/PKG-INFO
+-rw-r--r--   0 sa         (501) staff       (20)       15 2024-05-26 13:42:57.000000 pytest_qanova-0.1/README.md
+drwxr-xr-x   0 sa         (501) staff       (20)        0 2024-05-26 13:52:05.566985 pytest_qanova-0.1/pytest_qanova/
+-rw-r--r--   0 sa         (501) staff       (20)        0 2024-05-26 12:54:25.000000 pytest_qanova-0.1/pytest_qanova/__init__.py
+-rw-r--r--   0 sa         (501) staff       (20)     1677 2024-05-26 12:55:35.000000 pytest_qanova-0.1/pytest_qanova/plugin.py
+drwxr-xr-x   0 sa         (501) staff       (20)        0 2024-05-26 13:52:05.569535 pytest_qanova-0.1/pytest_qanova.egg-info/
+-rw-r--r--   0 sa         (501) staff       (20)      783 2024-05-26 13:52:05.000000 pytest_qanova-0.1/pytest_qanova.egg-info/PKG-INFO
+-rw-r--r--   0 sa         (501) staff       (20)      312 2024-05-26 13:52:05.000000 pytest_qanova-0.1/pytest_qanova.egg-info/SOURCES.txt
+-rw-r--r--   0 sa         (501) staff       (20)        1 2024-05-26 13:52:05.000000 pytest_qanova-0.1/pytest_qanova.egg-info/dependency_links.txt
+-rw-r--r--   0 sa         (501) staff       (20)       48 2024-05-26 13:52:05.000000 pytest_qanova-0.1/pytest_qanova.egg-info/entry_points.txt
+-rw-r--r--   0 sa         (501) staff       (20)        7 2024-05-26 13:52:05.000000 pytest_qanova-0.1/pytest_qanova.egg-info/requires.txt
+-rw-r--r--   0 sa         (501) staff       (20)       14 2024-05-26 13:52:05.000000 pytest_qanova-0.1/pytest_qanova.egg-info/top_level.txt
+-rw-r--r--   0 sa         (501) staff       (20)       38 2024-05-26 13:52:05.570299 pytest_qanova-0.1/setup.cfg
+-rw-r--r--   0 sa         (501) staff       (20)     1097 2024-05-26 13:45:13.000000 pytest_qanova-0.1/setup.py
```

### Comparing `pytest_qanova-0.0.2.dev3/LICENSE` & `pytest_qanova-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_qanova-0.0.2.dev3/PKG-INFO` & `pytest_qanova-0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_qanova
-Version: 0.0.2.dev3
+Version: 0.1
 Summary: A pytest plugin to collect test information
 Home-page: https://github.com/davidamirkhanyan/pytest-qanova
 Author: Davit Amirkhanyan
 Author-email: davit.amirkhanyan95@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytest_qanova-0.0.2.dev3/pytest_qanova/plugin.py` & `pytest_qanova-0.1/pytest_qanova/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,11 @@
 import pytest
 import json
-import os
 
 test_info_dict = {}
-session_info = {}
-
-
-def pytest_configure(config):
-    """Hook to configure pytest and collect starting variables."""
-    session_info['command_line'] = ' '.join(config.invocation_params.args)
-    session_info['rootdir'] = str(config.rootdir)
-    session_info['inifile'] = str(config.inifile) if config.inifile else None
-    session_info['args'] = config.args
-    session_info['options'] = {key: value for key, value in vars(config.option).items()}
 
 
 def pytest_collection_modifyitems(config, items):
     for item in items:
         nodeid = item.nodeid
         test_info_dict[nodeid] = {
             'nodeid': nodeid,
@@ -49,15 +38,10 @@
             error_type, error_message = report.longrepr.reprcrash.message.split(': ')
             return error_type, error_message
     else:
         return None, None
 
 
 def pytest_sessionfinish(session, exitstatus):
-    pytest_worker = os.environ.get("PYTEST_XDIST_WORKER")
-    if pytest_worker == 'gw0':
-        with open('test_results.json', 'w') as f:
-            json.dump({
-                'session_info': session_info,
-                'tests': list(test_info_dict.values())
-                }, f, indent=4)
+    with open('test_results.json', 'w') as f:
+        json.dump(list(test_info_dict.values()), f, indent=4)
```

### Comparing `pytest_qanova-0.0.2.dev3/pytest_qanova.egg-info/PKG-INFO` & `pytest_qanova-0.1/pytest_qanova.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_qanova
-Version: 0.0.2.dev3
+Version: 0.1
 Summary: A pytest plugin to collect test information
 Home-page: https://github.com/davidamirkhanyan/pytest-qanova
 Author: Davit Amirkhanyan
 Author-email: davit.amirkhanyan95@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytest_qanova-0.0.2.dev3/setup.py` & `pytest_qanova-0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytest_qanova',
-    version='0.0.2dev3',
+    version='0.1',
     author='Davit Amirkhanyan',
     author_email='davit.amirkhanyan95@gmail.com',
     description='A pytest plugin to collect test information',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davidamirkhanyan/pytest-qanova',  # Your project URL
     packages=find_packages(),
```

