# Comparing `tmp/qase_pytest-6.0.0b1.tar.gz` & `tmp/qase_pytest-6.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_pytest-6.0.0b1.tar", last modified: Mon May  6 08:53:15 2024, max compression
+gzip compressed data, was "qase_pytest-6.0.0b2.tar", last modified: Tue May  7 18:05:02 2024, max compression
```

## Comparing `qase_pytest-6.0.0b1.tar` & `qase_pytest-6.0.0b2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.684541 qase_pytest-6.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.684541 qase_pytest-6.0.0b1/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.684541 qase_pytest-6.0.0b1/src/qase/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:02.933830 qase_pytest-6.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-07 18:05:02.933830 qase_pytest-6.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:05:02.933830 qase_pytest-6.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:02.929830 qase_pytest-6.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:02.929830 qase_pytest-6.0.0b2/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:02.933830 qase_pytest-6.0.0b2/src/qase/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/src/qase/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/src/qase/pytest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/src/qase/pytest/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/src/qase/pytest/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/src/qase/pytest/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-05-07 18:04:55.000000 qase_pytest-6.0.0b2/src/qase/pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:02.933830 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-07 18:05:02.000000 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 18:05:02.000000 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:05:02.000000 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 18:05:02.000000 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 18:05:02.000000 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 18:05:02.000000 qase_pytest-6.0.0b2/src/qase_pytest.egg-info/top_level.txt
```

### Comparing `qase_pytest-6.0.0b1/LICENSE.txt` & `qase_pytest-6.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qase_pytest-6.0.0b1/PKG-INFO` & `qase_pytest-6.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://qase.io
 Project-URL: Repository, https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Project-URL: Documentation, https://developers.qase.io
 Keywords: qase,pytest,plugin,testops,report,qase reporting,test observability
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 ```sh
 pip install qase-pytest
 ```
 
 ## Upgrade from 4.x to 5.x and to 6.x
 
 The new version 6.x of the Pytest reporter has breaking changes.
-To migrate from versions 4.x or 5.x, follow the [upgrade guide](UPGRADE.md).
+To migrate from versions 4.x or 5.x, follow the [upgrade guide](docs/UPGRADE.md).
 
 ## Configuration
 
 Qase Pytest Reporter is configured in multiple ways:
 
 - using a config file `qase.config.json`
 - using environment variables
```

### Comparing `qase_pytest-6.0.0b1/README.md` & `qase_pytest-6.0.0b2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```sh
 pip install qase-pytest
 ```
 
 ## Upgrade from 4.x to 5.x and to 6.x
 
 The new version 6.x of the Pytest reporter has breaking changes.
-To migrate from versions 4.x or 5.x, follow the [upgrade guide](UPGRADE.md).
+To migrate from versions 4.x or 5.x, follow the [upgrade guide](docs/UPGRADE.md).
 
 ## Configuration
 
 Qase Pytest Reporter is configured in multiple ways:
 
 - using a config file `qase.config.json`
 - using environment variables
@@ -225,8 +225,8 @@
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
     --qase-testops-project=PRJCODE \ # project, where your testrun exists in
     --qase-testops-plan-id=3 # testplan id
-```
+```
```

### Comparing `qase_pytest-6.0.0b1/pyproject.toml` & `qase_pytest-6.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-pytest"
-version = "6.0.0b1"
+version = "6.0.0b2"
 description = "Qase Pytest Plugin for Qase TestOps and Qase Report"
 readme = "README.md"
 keywords = ["qase", "pytest", "plugin", "testops", "report", "qase reporting", "test observability"]
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `qase_pytest-6.0.0b1/src/qase/pytest/conftest.py` & `qase_pytest-6.0.0b2/src/qase/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `qase_pytest-6.0.0b1/src/qase/pytest/context_manager.py` & `qase_pytest-6.0.0b2/src/qase/pytest/context_manager.py`

 * *Files identical despite different names*

### Comparing `qase_pytest-6.0.0b1/src/qase/pytest/decorators.py` & `qase_pytest-6.0.0b2/src/qase/pytest/decorators.py`

 * *Files identical despite different names*

### Comparing `qase_pytest-6.0.0b1/src/qase/pytest/options.py` & `qase_pytest-6.0.0b2/src/qase/pytest/options.py`

 * *Files identical despite different names*

### Comparing `qase_pytest-6.0.0b1/src/qase/pytest/plugin.py` & `qase_pytest-6.0.0b2/src/qase/pytest/plugin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -96,16 +96,16 @@
     def pytest_runtest_protocol(self, item):
         self.ignore = True if item.get_closest_marker("qase_ignore") else False
 
         if not self.ignore:
             self.reporter.enable_profilers()
             self.start_pytest_item(item)
             yield
-            self.reporter.disable_profilers()
             self.finish_pytest_item(item)
+            self.reporter.disable_profilers()
         else:
             yield
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(self, item, call):
         if not self.ignore:
             report = (yield).get_result()
```

### Comparing `qase_pytest-6.0.0b1/src/qase_pytest.egg-info/PKG-INFO` & `qase_pytest-6.0.0b2/src/qase_pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://qase.io
 Project-URL: Repository, https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Project-URL: Documentation, https://developers.qase.io
 Keywords: qase,pytest,plugin,testops,report,qase reporting,test observability
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 ```sh
 pip install qase-pytest
 ```
 
 ## Upgrade from 4.x to 5.x and to 6.x
 
 The new version 6.x of the Pytest reporter has breaking changes.
-To migrate from versions 4.x or 5.x, follow the [upgrade guide](UPGRADE.md).
+To migrate from versions 4.x or 5.x, follow the [upgrade guide](docs/UPGRADE.md).
 
 ## Configuration
 
 Qase Pytest Reporter is configured in multiple ways:
 
 - using a config file `qase.config.json`
 - using environment variables
```

