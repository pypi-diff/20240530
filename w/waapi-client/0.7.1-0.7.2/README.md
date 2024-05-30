# Comparing `tmp/waapi-client-0.7.1.tar.gz` & `tmp/waapi_client-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waapi-client-0.7.1.tar", last modified: Tue Jan 23 15:07:45 2024, max compression
+gzip compressed data, was "waapi_client-0.7.2.tar", last modified: Thu May 30 20:49:00 2024, max compression
```

## Comparing `waapi-client-0.7.1.tar` & `waapi_client-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-23 15:07:45.089659 waapi-client-0.7.1/
--rw-rw-rw-   0        0        0    11558 2022-10-26 22:05:27.000000 waapi-client-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     3520 2024-01-23 15:07:45.086695 waapi-client-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2573 2024-01-23 14:38:26.000000 waapi-client-0.7.1/README.md
--rw-rw-rw-   0        0        0       86 2024-01-23 15:07:45.093702 waapi-client-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1414 2024-01-23 14:38:48.000000 waapi-client-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-23 15:07:44.962688 waapi-client-0.7.1/waapi/
--rw-rw-rw-   0        0        0      101 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-23 15:07:45.012772 waapi-client-0.7.1/waapi/client/
--rw-rw-rw-   0        0        0      106 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/client/__init__.py
--rw-rw-rw-   0        0        0    12145 2023-06-12 13:12:32.000000 waapi-client-0.7.1/waapi/client/client.py
--rw-rw-rw-   0        0        0     2775 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/client/event.py
--rw-rw-rw-   0        0        0     1637 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/client/executor.py
--rw-rw-rw-   0        0        0      917 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/client/interface.py
-drwxrwxrwx   0        0        0        0 2024-01-23 15:07:45.052689 waapi-client-0.7.1/waapi/wamp/
--rw-rw-rw-   0        0        0        0 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/wamp/__init__.py
--rw-rw-rw-   0        0        0     9880 2023-06-12 13:12:32.000000 waapi-client-0.7.1/waapi/wamp/ak_autobahn.py
--rw-rw-rw-   0        0        0       89 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/wamp/async_compatibility.py
--rw-rw-rw-   0        0        0     5634 2023-06-12 13:12:32.000000 waapi-client-0.7.1/waapi/wamp/async_decoupled_client.py
--rw-rw-rw-   0        0        0     1566 2022-10-26 22:05:27.000000 waapi-client-0.7.1/waapi/wamp/interface.py
-drwxrwxrwx   0        0        0        0 2024-01-23 15:07:45.081782 waapi-client-0.7.1/waapi_client.egg-info/
--rw-rw-rw-   0        0        0     3520 2024-01-23 15:07:44.000000 waapi-client-0.7.1/waapi_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-01-23 15:07:44.000000 waapi-client-0.7.1/waapi_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-23 15:07:44.000000 waapi-client-0.7.1/waapi_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-23 15:07:44.000000 waapi-client-0.7.1/waapi_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-23 15:07:44.000000 waapi-client-0.7.1/waapi_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 20:49:00.902181 waapi_client-0.7.2/
+-rw-rw-rw-   0        0        0    11558 2022-10-26 22:05:27.000000 waapi_client-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     3626 2024-05-30 20:49:00.902181 waapi_client-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2679 2024-05-30 20:44:07.000000 waapi_client-0.7.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-30 20:49:00.902181 waapi_client-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2024-05-30 20:44:07.000000 waapi_client-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:49:00.870906 waapi_client-0.7.2/waapi/
+-rw-rw-rw-   0        0        0      101 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:49:00.886643 waapi_client-0.7.2/waapi/client/
+-rw-rw-rw-   0        0        0      106 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/client/__init__.py
+-rw-rw-rw-   0        0        0    12145 2023-06-12 13:12:32.000000 waapi_client-0.7.2/waapi/client/client.py
+-rw-rw-rw-   0        0        0     2775 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/client/event.py
+-rw-rw-rw-   0        0        0     1637 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/client/executor.py
+-rw-rw-rw-   0        0        0      917 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/client/interface.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:49:00.886643 waapi_client-0.7.2/waapi/wamp/
+-rw-rw-rw-   0        0        0        0 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/wamp/__init__.py
+-rw-rw-rw-   0        0        0     9880 2023-06-12 13:12:32.000000 waapi_client-0.7.2/waapi/wamp/ak_autobahn.py
+-rw-rw-rw-   0        0        0       89 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/wamp/async_compatibility.py
+-rw-rw-rw-   0        0        0     5634 2023-06-12 13:12:32.000000 waapi_client-0.7.2/waapi/wamp/async_decoupled_client.py
+-rw-rw-rw-   0        0        0     1566 2022-10-26 22:05:27.000000 waapi_client-0.7.2/waapi/wamp/interface.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:49:00.902181 waapi_client-0.7.2/waapi_client.egg-info/
+-rw-rw-rw-   0        0        0     3626 2024-05-30 20:49:00.000000 waapi_client-0.7.2/waapi_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-30 20:49:00.000000 waapi_client-0.7.2/waapi_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 20:49:00.000000 waapi_client-0.7.2/waapi_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 20:49:00.000000 waapi_client-0.7.2/waapi_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 20:49:00.000000 waapi_client-0.7.2/waapi_client.egg-info/top_level.txt
```

### Comparing `waapi-client-0.7.1/LICENSE` & `waapi_client-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/PKG-INFO` & `waapi_client-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waapi-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: Wwise Authoring API client.
 Home-page: https://github.com/audiokinetic/waapi-client-python
 Download-URL: https://github.com/audiokinetic/waapi-client-python/releases
 Author: Audiokinetic
 Maintainer: Samuel Longchamps
 Maintainer-email: slongchamps@audiokinetic.com
 License: Apache License 2.0
@@ -22,15 +22,15 @@
 License-File: LICENSE
 Requires-Dist: autobahn
 
 # Wwise Authoring API (Waapi) Client for Python
 Decoupled autobahn WAMP client with support for plain options and bindable subscription callbacks.
 
 ## Requirements
-* Python 3.7+ (see `tox.ini` for versions tested)
+* Non-EOL Python 3.x version (see `tox.ini` for versions tested). Refer to the official [Status of Python versions](https://devguide.python.org/versions)
 * [Wwise](https://www.audiokinetic.com/en/download) instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
 
 ## Setup
 On Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
 
 * Windows: `py -3 -m pip install waapi-client`
 * Other platforms: `python3 -m pip install waapi-client`
@@ -98,8 +98,8 @@
 
 * Windows: `py -3 -m pip install tox`
 * Other platforms: `python3 -m pip install tox`
 
 Open a blank project in Wwise, then you may execute `tox` in the terminal from the root of the repository
 
 The test suite will run for all supported versions of Python.
-Use `-e pyXX` to run for a single version, e.g., `tox -e py37` for Python 3.7).
+Use `-e pyXX` to run for a single version, e.g., `tox -e py312` for Python 3.12).
```

### Comparing `waapi-client-0.7.1/README.md` & `waapi_client-0.7.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Wwise Authoring API (Waapi) Client for Python
 Decoupled autobahn WAMP client with support for plain options and bindable subscription callbacks.
 
 ## Requirements
-* Python 3.7+ (see `tox.ini` for versions tested)
+* Non-EOL Python 3.x version (see `tox.ini` for versions tested). Refer to the official [Status of Python versions](https://devguide.python.org/versions)
 * [Wwise](https://www.audiokinetic.com/en/download) instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
 
 ## Setup
 On Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
 
 * Windows: `py -3 -m pip install waapi-client`
 * Other platforms: `python3 -m pip install waapi-client`
@@ -74,8 +74,8 @@
 
 * Windows: `py -3 -m pip install tox`
 * Other platforms: `python3 -m pip install tox`
 
 Open a blank project in Wwise, then you may execute `tox` in the terminal from the root of the repository
 
 The test suite will run for all supported versions of Python.
-Use `-e pyXX` to run for a single version, e.g., `tox -e py37` for Python 3.7).
+Use `-e pyXX` to run for a single version, e.g., `tox -e py312` for Python 3.12).
```

### Comparing `waapi-client-0.7.1/setup.py` & `waapi_client-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     test_suite='waapi.test',
     install_requires=[
       'autobahn'
     ],
     license='Apache License 2.0',
     platforms=['any'],
     scripts=[],
-    version='0.7.1',
+    version='0.7.2',
     description='Wwise Authoring API client.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Audiokinetic',
     maintainer='Samuel Longchamps',
     maintainer_email='slongchamps@audiokinetic.com',
     url='https://github.com/audiokinetic/waapi-client-python',
```

### Comparing `waapi-client-0.7.1/waapi/client/client.py` & `waapi_client-0.7.2/waapi/client/client.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi/client/event.py` & `waapi_client-0.7.2/waapi/client/event.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi/client/executor.py` & `waapi_client-0.7.2/waapi/client/executor.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi/client/interface.py` & `waapi_client-0.7.2/waapi/client/interface.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi/wamp/ak_autobahn.py` & `waapi_client-0.7.2/waapi/wamp/ak_autobahn.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi/wamp/async_decoupled_client.py` & `waapi_client-0.7.2/waapi/wamp/async_decoupled_client.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi/wamp/interface.py` & `waapi_client-0.7.2/waapi/wamp/interface.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.7.1/waapi_client.egg-info/PKG-INFO` & `waapi_client-0.7.2/waapi_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waapi-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: Wwise Authoring API client.
 Home-page: https://github.com/audiokinetic/waapi-client-python
 Download-URL: https://github.com/audiokinetic/waapi-client-python/releases
 Author: Audiokinetic
 Maintainer: Samuel Longchamps
 Maintainer-email: slongchamps@audiokinetic.com
 License: Apache License 2.0
@@ -22,15 +22,15 @@
 License-File: LICENSE
 Requires-Dist: autobahn
 
 # Wwise Authoring API (Waapi) Client for Python
 Decoupled autobahn WAMP client with support for plain options and bindable subscription callbacks.
 
 ## Requirements
-* Python 3.7+ (see `tox.ini` for versions tested)
+* Non-EOL Python 3.x version (see `tox.ini` for versions tested). Refer to the official [Status of Python versions](https://devguide.python.org/versions)
 * [Wwise](https://www.audiokinetic.com/en/download) instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
 
 ## Setup
 On Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
 
 * Windows: `py -3 -m pip install waapi-client`
 * Other platforms: `python3 -m pip install waapi-client`
@@ -98,8 +98,8 @@
 
 * Windows: `py -3 -m pip install tox`
 * Other platforms: `python3 -m pip install tox`
 
 Open a blank project in Wwise, then you may execute `tox` in the terminal from the root of the repository
 
 The test suite will run for all supported versions of Python.
-Use `-e pyXX` to run for a single version, e.g., `tox -e py37` for Python 3.7).
+Use `-e pyXX` to run for a single version, e.g., `tox -e py312` for Python 3.12).
```

