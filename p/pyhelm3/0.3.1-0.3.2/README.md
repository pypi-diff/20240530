# Comparing `tmp/pyhelm3-0.3.1.tar.gz` & `tmp/pyhelm3-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelm3-0.3.1.tar", last modified: Thu May 23 15:05:29 2024, max compression
+gzip compressed data, was "pyhelm3-0.3.2.tar", last modified: Thu May 30 15:53:16 2024, max compression
```

## Comparing `pyhelm3-0.3.1.tar` & `pyhelm3-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.587798 pyhelm3-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/pyhelm3/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32859 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/pyhelm3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:16.302773 pyhelm3-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:16.298773 pyhelm3-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:16.298773 pyhelm3-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-30 15:53:16.302773 pyhelm3-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:16.298773 pyhelm3-0.3.2/pyhelm3/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/pyhelm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/pyhelm3/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32859 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/pyhelm3/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/pyhelm3/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/pyhelm3/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:16.302773 pyhelm3-0.3.2/pyhelm3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-30 15:53:16.000000 pyhelm3-0.3.2/pyhelm3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 15:53:16.000000 pyhelm3-0.3.2/pyhelm3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:53:16.000000 pyhelm3-0.3.2/pyhelm3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:53:16.000000 pyhelm3-0.3.2/pyhelm3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 15:53:16.000000 pyhelm3-0.3.2/pyhelm3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 15:53:16.000000 pyhelm3-0.3.2/pyhelm3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-30 15:53:16.302773 pyhelm3-0.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-30 15:53:12.000000 pyhelm3-0.3.2/setup.py
```

### Comparing `pyhelm3-0.3.1/.github/workflows/pypi-publish.yaml` & `pyhelm3-0.3.2/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.1/PKG-INFO` & `pyhelm3-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyhelm3
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library for managing Helm releases using Helm 3.
 Home-page: https://github.com/stackhpc/pyhelm3
 Author: Matt Pryor
 Author-email: matt@stackhpc.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
 
 # pyhelm3
 
 Python library for managing Helm releases using Helm 3 (i.e. Tiller-less Helm).
```

### Comparing `pyhelm3-0.3.1/README.md` & `pyhelm3-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.1/pyhelm3/client.py` & `pyhelm3-0.3.2/pyhelm3/client.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.1/pyhelm3/command.py` & `pyhelm3-0.3.2/pyhelm3/command.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.1/pyhelm3/errors.py` & `pyhelm3-0.3.2/pyhelm3/errors.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.1/pyhelm3/models.py` & `pyhelm3-0.3.2/pyhelm3/models.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.1/pyhelm3.egg-info/PKG-INFO` & `pyhelm3-0.3.2/pyhelm3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyhelm3
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library for managing Helm releases using Helm 3.
 Home-page: https://github.com/stackhpc/pyhelm3
 Author: Matt Pryor
 Author-email: matt@stackhpc.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
 
 # pyhelm3
 
 Python library for managing Helm releases using Helm 3 (i.e. Tiller-less Helm).
```

