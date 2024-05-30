# Comparing `tmp/pyobas-1.0.4.tar.gz` & `tmp/pyobas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.4.tar", last modified: Tue May 28 22:00:56 2024, max compression
+gzip compressed data, was "pyobas-1.0.5.tar", last modified: Wed May 29 19:55:33 2024, max compression
```

## Comparing `pyobas-1.0.4.tar` & `pyobas-1.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.120499 pyobas-1.0.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-28 22:00:43.000000 pyobas-1.0.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-28 22:00:56.120499 pyobas-1.0.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-28 22:00:43.000000 pyobas-1.0.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.112499 pyobas-1.0.4/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/inject_expectation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15283 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-05-28 22:00:56.120499 pyobas-1.0.4/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.364380 pyobas-1.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-29 19:55:21.000000 pyobas-1.0.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-29 19:55:33.364380 pyobas-1.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-29 19:55:21.000000 pyobas-1.0.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.356379 pyobas-1.0.5/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/collector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/inject.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/inject_expectation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/injector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/me.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/organization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/team.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/apis/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/backends/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/backends/backend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/backends/protocol.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas/contracts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/contract_builder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/contract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/contract_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/contracts/variable_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15283 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-29 19:55:33.360380 pyobas-1.0.5/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-29 19:55:33.000000 pyobas-1.0.5/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-29 19:55:21.000000 pyobas-1.0.5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-05-29 19:55:33.364380 pyobas-1.0.5/setup.cfg
```

### Comparing `pyobas-1.0.4/LICENSE` & `pyobas-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/PKG-INFO` & `pyobas-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,16 +27,16 @@
 Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=70.0.0
 Requires-Dist: cachetools~=5.3.0
 Requires-Dist: prometheus-client~=0.20.0
-Requires-Dist: opentelemetry-api~=1.22.0
-Requires-Dist: opentelemetry-sdk~=1.22.0
+Requires-Dist: opentelemetry-api~=1.24.0
+Requires-Dist: opentelemetry-sdk~=1.24.0
 Requires-Dist: requests-toolbelt~=1.0.0
 Requires-Dist: dataclasses-json~=0.6.4
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
```

### Comparing `pyobas-1.0.4/README.md` & `pyobas-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/__init__.py` & `pyobas-1.0.5/pyobas/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 from pyobas._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
```

### Comparing `pyobas-1.0.4/pyobas/apis/__init__.py` & `pyobas-1.0.5/pyobas/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/attack_pattern.py` & `pyobas-1.0.5/pyobas/apis/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/collector.py` & `pyobas-1.0.5/pyobas/apis/collector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/document.py` & `pyobas-1.0.5/pyobas/apis/document.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/inject.py` & `pyobas-1.0.5/pyobas/apis/inject.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/inject_expectation.py` & `pyobas-1.0.5/pyobas/apis/inject_expectation.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/injector.py` & `pyobas-1.0.5/pyobas/apis/injector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/kill_chain_phase.py` & `pyobas-1.0.5/pyobas/apis/kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/team.py` & `pyobas-1.0.5/pyobas/apis/team.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/apis/user.py` & `pyobas-1.0.5/pyobas/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/backends/backend.py` & `pyobas-1.0.5/pyobas/backends/backend.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/backends/protocol.py` & `pyobas-1.0.5/pyobas/backends/protocol.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/base.py` & `pyobas-1.0.5/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/client.py` & `pyobas-1.0.5/pyobas/client.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/contracts/contract_builder.py` & `pyobas-1.0.5/pyobas/contracts/contract_builder.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/contracts/contract_config.py` & `pyobas-1.0.5/pyobas/contracts/contract_config.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/contracts/variable_helper.py` & `pyobas-1.0.5/pyobas/contracts/variable_helper.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/exceptions.py` & `pyobas-1.0.5/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/helpers.py` & `pyobas-1.0.5/pyobas/helpers.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/mixins.py` & `pyobas-1.0.5/pyobas/mixins.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas/utils.py` & `pyobas-1.0.5/pyobas/utils.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas.egg-info/PKG-INFO` & `pyobas-1.0.5/pyobas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,16 +27,16 @@
 Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=70.0.0
 Requires-Dist: cachetools~=5.3.0
 Requires-Dist: prometheus-client~=0.20.0
-Requires-Dist: opentelemetry-api~=1.22.0
-Requires-Dist: opentelemetry-sdk~=1.22.0
+Requires-Dist: opentelemetry-api~=1.24.0
+Requires-Dist: opentelemetry-sdk~=1.24.0
 Requires-Dist: requests-toolbelt~=1.0.0
 Requires-Dist: dataclasses-json~=0.6.4
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
```

### Comparing `pyobas-1.0.4/pyobas.egg-info/SOURCES.txt` & `pyobas-1.0.5/pyobas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/pyobas.egg-info/requires.txt` & `pyobas-1.0.5/pyobas.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 pika~=1.3.0
 python_json_logger~=2.0.4
 PyYAML~=6.0
 requests~=2.31.0
 setuptools~=70.0.0
 cachetools~=5.3.0
 prometheus-client~=0.20.0
-opentelemetry-api~=1.22.0
-opentelemetry-sdk~=1.22.0
+opentelemetry-api~=1.24.0
+opentelemetry-sdk~=1.24.0
 requests-toolbelt~=1.0.0
 dataclasses-json~=0.6.4
 
 [:sys_platform == "linux" or sys_platform == "darwin"]
 python-magic~=0.4.27
 
 [:sys_platform == "win32"]
```

### Comparing `pyobas-1.0.4/pyproject.toml` & `pyobas-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.4/setup.cfg` & `pyobas-1.0.5/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 	python-magic-bin~=0.4.14; sys_platform == 'win32'
 	python_json_logger~=2.0.4
 	PyYAML~=6.0
 	requests~=2.31.0
 	setuptools~=70.0.0
 	cachetools~=5.3.0
 	prometheus-client~=0.20.0
-	opentelemetry-api~=1.22.0
-	opentelemetry-sdk~=1.22.0
+	opentelemetry-api~=1.24.0
+	opentelemetry-sdk~=1.24.0
 	requests-toolbelt~=1.0.0
 	dataclasses-json~=0.6.4
 
 [options.extras_require]
 dev = 
 	black~=24.4.0
 	build~=1.2.1
```

