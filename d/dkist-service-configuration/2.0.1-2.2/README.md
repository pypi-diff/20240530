# Comparing `tmp/dkist_service_configuration-2.0.1.tar.gz` & `tmp/dkist_service_configuration-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_service_configuration-2.0.1.tar", last modified: Wed May 22 14:56:05 2024, max compression
+gzip compressed data, was "dkist_service_configuration-2.2.tar", last modified: Thu May 30 14:08:57 2024, max compression
```

## Comparing `dkist_service_configuration-2.0.1.tar` & `dkist_service_configuration-2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2116 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.341018 dkist_service_configuration-2.0.1/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2116 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:56:04.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 14:08:57.908816 dkist_service_configuration-2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-30 14:08:57.908816 dkist_service_configuration-2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 14:08:57.904816 dkist_service_configuration-2.2/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 14:08:57.904816 dkist_service_configuration-2.2/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 14:08:57.908816 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-30 14:08:57.000000 dkist_service_configuration-2.2/dkist_service_configuration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-30 14:08:57.908816 dkist_service_configuration-2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-30 14:08:45.000000 dkist_service_configuration-2.2/tox.ini
```

### Comparing `dkist_service_configuration-2.0.1/.gitignore` & `dkist_service_configuration-2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/.pre-commit-config.yaml` & `dkist_service_configuration-2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/LICENSE` & `dkist_service_configuration-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/PKG-INFO` & `dkist_service_configuration-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 2.0.1
+Version: 2.2
 Summary: Library for retrieving configurations for DKIST services
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist_service_configuration
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dkist_service_configuration-2.0.1/README.rst` & `dkist_service_configuration-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/bitbucket-pipelines.yml` & `dkist_service_configuration-2.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/dkist_service_configuration/logging.py` & `dkist_service_configuration-2.2/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/dkist_service_configuration/settings.py` & `dkist_service_configuration-2.2/dkist_service_configuration/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Wrapper for retrieving configurations and safely logging their retrieval
 """
+import logging
 import re
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic_settings import BaseSettings
 from pydantic_settings import SettingsConfigDict
 
-from dkist_service_configuration.logging import logger
+
+logger = logging.getLogger(__name__)
 
 
 class ConfigurationBase(BaseSettings):
     """Settings base which logs configured settings while censoring secrets"""
 
     log_level: str = Field(default="INFO", validation_alias="LOGURU_LEVEL")
```

### Comparing `dkist_service_configuration-2.0.1/dkist_service_configuration/tests/test_settings.py` & `dkist_service_configuration-2.2/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/PKG-INFO` & `dkist_service_configuration-2.2/dkist_service_configuration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 2.0.1
+Version: 2.2
 Summary: Library for retrieving configurations for DKIST services
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist_service_configuration
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist_service_configuration-2.2/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/pyproject.toml` & `dkist_service_configuration-2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.1/tox.ini` & `dkist_service_configuration-2.2/tox.ini`

 * *Files identical despite different names*

