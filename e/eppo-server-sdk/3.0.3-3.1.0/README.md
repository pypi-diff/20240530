# Comparing `tmp/eppo_server_sdk-3.0.3.tar.gz` & `tmp/eppo_server_sdk-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo_server_sdk-3.0.3.tar", last modified: Tue May 14 16:43:09 2024, max compression
+gzip compressed data, was "eppo_server_sdk-3.1.0.tar", last modified: Thu May 30 05:18:42 2024, max compression
```

## Comparing `eppo_server_sdk-3.0.3.tar` & `eppo_server_sdk-3.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/eppo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/assignment_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/configuration_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/configuration_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/read_write_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/sharders.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 16:43:09.923875 eppo_server_sdk-3.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:18:42.890961 eppo_server_sdk-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-30 05:18:42.886961 eppo_server_sdk-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:18:42.886961 eppo_server_sdk-3.1.0/eppo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/assignment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/configuration_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/configuration_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/read_write_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/sharders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:18:42.886961 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 05:18:42.890961 eppo_server_sdk-3.1.0/setup.cfg
```

### Comparing `eppo_server_sdk-3.0.3/LICENSE` & `eppo_server_sdk-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/PKG-INFO` & `eppo_server_sdk-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 3.0.3
+Version: 3.1.0
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: requests
 Requires-Dist: cachetools
+Requires-Dist: semver
 
 # Eppo Python SDK
 
 [![Test and lint SDK](https://github.com/Eppo-exp/python-sdk/actions/workflows/test-and-lint-sdk.yml/badge.svg)](https://github.com/Eppo-exp/python-sdk/actions/workflows/test-and-lint-sdk.yml)
 
 [Eppo](https://www.geteppo.com/) is a modular flagging and experimentation analysis tool. Eppo's Python SDK is built to make assignments in multi-user server side contexts. Before proceeding you'll need an Eppo account.
```

### Comparing `eppo_server_sdk-3.0.3/README.md` & `eppo_server_sdk-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_client/__init__.py` & `eppo_server_sdk-3.1.0/eppo_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from eppo_client.client import EppoClient
 from eppo_client.config import Config
 from eppo_client.configuration_requestor import (
     ExperimentConfigurationRequestor,
 )
 from eppo_client.configuration_store import ConfigurationStore
 from eppo_client.http_client import HttpClient, SdkParams
-from eppo_client.models import Flag
+from eppo_client.models import BanditData, Flag
 from eppo_client.read_write_lock import ReadWriteLock
 from eppo_client.version import __version__
 
 
 __client: Optional[EppoClient] = None
 __lock = ReadWriteLock()
 
@@ -26,17 +26,20 @@
     :type config: Config
     """
     config._validate()
     sdk_params = SdkParams(
         apiKey=config.api_key, sdkName="python", sdkVersion=__version__
     )
     http_client = HttpClient(base_url=config.base_url, sdk_params=sdk_params)
-    config_store: ConfigurationStore[Flag] = ConfigurationStore()
+    flag_config_store: ConfigurationStore[Flag] = ConfigurationStore()
+    bandit_config_store: ConfigurationStore[BanditData] = ConfigurationStore()
     config_requestor = ExperimentConfigurationRequestor(
-        http_client=http_client, config_store=config_store
+        http_client=http_client,
+        flag_config_store=flag_config_store,
+        bandit_config_store=bandit_config_store,
     )
     assignment_logger = config.assignment_logger
     is_graceful_mode = config.is_graceful_mode
     global __client
     global __lock
     with __lock.writer():
         if __client:
```

### Comparing `eppo_server_sdk-3.0.3/eppo_client/configuration_store.py` & `eppo_server_sdk-3.1.0/eppo_client/configuration_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
     def set_configurations(self, configs: Dict[str, T]):
         with self.__lock.writer():
             self.__cache = configs
 
     def get_keys(self):
         with self.__lock.reader():
-            return list(self.__cache.keys())
+            return set(self.__cache.keys())
```

### Comparing `eppo_server_sdk-3.0.3/eppo_client/eval.py` & `eppo_server_sdk-3.1.0/eppo_client/eval.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_client/http_client.py` & `eppo_server_sdk-3.1.0/eppo_client/http_client.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_client/poller.py` & `eppo_server_sdk-3.1.0/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_client/read_write_lock.py` & `eppo_server_sdk-3.1.0/eppo_client/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_client/rules.py` & `eppo_server_sdk-3.1.0/eppo_client/rules.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_client/sharders.py` & `eppo_server_sdk-3.1.0/eppo_client/sharders.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/PKG-INFO` & `eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 3.0.3
+Version: 3.1.0
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: requests
 Requires-Dist: cachetools
+Requires-Dist: semver
 
 # Eppo Python SDK
 
 [![Test and lint SDK](https://github.com/Eppo-exp/python-sdk/actions/workflows/test-and-lint-sdk.yml/badge.svg)](https://github.com/Eppo-exp/python-sdk/actions/workflows/test-and-lint-sdk.yml)
 
 [Eppo](https://www.geteppo.com/) is a modular flagging and experimentation analysis tool. Eppo's Python SDK is built to make assignments in multi-user server side contexts. Before proceeding you'll need an Eppo account.
```

### Comparing `eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 requirements-test.txt
 requirements.txt
 setup.cfg
 eppo_client/__init__.py
 eppo_client/assignment_logger.py
+eppo_client/bandit.py
 eppo_client/base_model.py
 eppo_client/client.py
 eppo_client/config.py
 eppo_client/configuration_requestor.py
 eppo_client/configuration_store.py
 eppo_client/constants.py
 eppo_client/eval.py
```

### Comparing `eppo_server_sdk-3.0.3/setup.cfg` & `eppo_server_sdk-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 python_requires = >=3.6
 include_package_data = True
 install_requires = 
 	pydantic
 	pydantic-settings
 	requests
 	cachetools
+	semver
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

