# Comparing `tmp/alyx_connector-2.1.4.tar.gz` & `tmp/alyx_connector-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alyx_connector-2.1.4.tar", last modified: Tue Mar  5 15:22:56 2024, max compression
+gzip compressed data, was "alyx_connector-2.1.5.tar", last modified: Tue Mar  5 16:40:57 2024, max compression
```

## Comparing `alyx_connector-2.1.4.tar` & `alyx_connector-2.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.451216 alyx_connector-2.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/LICENSE copy
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-05 15:22:56.451216 alyx_connector-2.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 15:22:56.451216 alyx_connector-2.1.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.443215 alyx_connector-2.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.451216 alyx_connector-2.1.4/src/alyx_connector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-05 15:22:56.000000 alyx_connector-2.1.4/src/alyx_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      806 2024-03-05 15:22:56.000000 alyx_connector-2.1.4/src/alyx_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 15:22:56.000000 alyx_connector-2.1.4/src/alyx_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-03-05 15:22:56.000000 alyx_connector-2.1.4/src/alyx_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-05 15:22:56.000000 alyx_connector-2.1.4/src/alyx_connector.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.447215 alyx_connector-2.1.4/src/one/
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.447215 alyx_connector-2.1.4/src/one/alf/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11569 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14175 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/files.py
--rw-rw-rw-   0 root         (0) root         (0)    26174 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/io.py
--rw-rw-rw-   0 root         (0) root         (0)     4200 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/migrations.py
--rw-rw-rw-   0 root         (0) root         (0)    20368 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/alf/spec.py
--rw-rw-rw-   0 root         (0) root         (0)   105320 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/api.py
--rw-rw-rw-   0 root         (0) root         (0)    26408 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/converters.py
--rw-rw-rw-   0 root         (0) root         (0)     3256 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/models.py
--rw-rw-rw-   0 root         (0) root         (0)    13430 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/params.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/pd_accessors.py
--rw-rw-rw-   0 root         (0) root         (0)    31795 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.447215 alyx_connector-2.1.4/src/one/remote/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4064 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/remote/base.py
--rw-rw-rw-   0 root         (0) root         (0)    22504 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/util.py
--rw-rw-rw-   0 root         (0) root         (0)    50484 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/src/one/webclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:22:56.451216 alyx_connector-2.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)    27622 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/tests/test_alyxclient.py
--rw-rw-rw-   0 root         (0) root         (0)     4731 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/tests/test_alyxrest.py
--rw-rw-rw-   0 root         (0) root         (0)    19366 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/tests/test_converters.py
--rw-rw-rw-   0 root         (0) root         (0)    81598 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/tests/test_one.py
--rw-rw-rw-   0 root         (0) root         (0)     4760 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/tests/test_params.py
--rw-rw-rw-   0 root         (0) root         (0)    11823 2024-03-05 15:22:46.000000 alyx_connector-2.1.4/tests/test_registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/LICENSE copy
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.985522 alyx_connector-2.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/src/alyx_connector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-03-05 16:40:57.000000 alyx_connector-2.1.5/src/alyx_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      806 2024-03-05 16:40:57.000000 alyx_connector-2.1.5/src/alyx_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 16:40:57.000000 alyx_connector-2.1.5/src/alyx_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-03-05 16:40:57.000000 alyx_connector-2.1.5/src/alyx_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-03-05 16:40:57.000000 alyx_connector-2.1.5/src/alyx_connector.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/src/one/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/src/one/alf/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11569 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14175 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    26174 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/migrations.py
+-rw-rw-rw-   0 root         (0) root         (0)    20368 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/alf/spec.py
+-rw-rw-rw-   0 root         (0) root         (0)   105320 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    26408 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/converters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    13430 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/params.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/pd_accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)    31795 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/src/one/remote/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4064 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/remote/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    22504 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    50484 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/src/one/webclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 16:40:57.989522 alyx_connector-2.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    27622 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/tests/test_alyxclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     4731 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/tests/test_alyxrest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19366 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/tests/test_converters.py
+-rw-rw-rw-   0 root         (0) root         (0)    81598 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/tests/test_one.py
+-rw-rw-rw-   0 root         (0) root         (0)     4760 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/tests/test_params.py
+-rw-rw-rw-   0 root         (0) root         (0)    11823 2024-03-05 16:40:47.000000 alyx_connector-2.1.5/tests/test_registration.py
```

### Comparing `alyx_connector-2.1.4/LICENSE` & `alyx_connector-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/LICENSE copy` & `alyx_connector-2.1.5/LICENSE copy`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/PKG-INFO` & `alyx_connector-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alyx_connector
-Version: 2.1.4
+Version: 2.1.5
 Summary: Alyx Connector, based on the Open Neurophysiology Environment
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/ONE
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/ONE
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/ONE
```

### Comparing `alyx_connector-2.1.4/README.md` & `alyx_connector-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/pyproject.toml` & `alyx_connector-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/alyx_connector.egg-info/PKG-INFO` & `alyx_connector-2.1.5/src/alyx_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alyx_connector
-Version: 2.1.4
+Version: 2.1.5
 Summary: Alyx Connector, based on the Open Neurophysiology Environment
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/ONE
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/ONE
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/ONE
```

### Comparing `alyx_connector-2.1.4/src/alyx_connector.egg-info/SOURCES.txt` & `alyx_connector-2.1.5/src/alyx_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/alf/cache.py` & `alyx_connector-2.1.5/src/one/alf/cache.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/alf/exceptions.py` & `alyx_connector-2.1.5/src/one/alf/exceptions.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/alf/files.py` & `alyx_connector-2.1.5/src/one/alf/files.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/alf/io.py` & `alyx_connector-2.1.5/src/one/alf/io.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/alf/migrations.py` & `alyx_connector-2.1.5/src/one/alf/migrations.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/alf/spec.py` & `alyx_connector-2.1.5/src/one/alf/spec.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/api.py` & `alyx_connector-2.1.5/src/one/api.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/converters.py` & `alyx_connector-2.1.5/src/one/converters.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/models.py` & `alyx_connector-2.1.5/src/one/models.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/params.py` & `alyx_connector-2.1.5/src/one/params.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/pd_accessors.py` & `alyx_connector-2.1.5/src/one/pd_accessors.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/registration.py` & `alyx_connector-2.1.5/src/one/registration.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/remote/base.py` & `alyx_connector-2.1.5/src/one/remote/base.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/util.py` & `alyx_connector-2.1.5/src/one/util.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/src/one/webclient.py` & `alyx_connector-2.1.5/src/one/webclient.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/tests/test_alyxclient.py` & `alyx_connector-2.1.5/tests/test_alyxclient.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/tests/test_alyxrest.py` & `alyx_connector-2.1.5/tests/test_alyxrest.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/tests/test_converters.py` & `alyx_connector-2.1.5/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/tests/test_one.py` & `alyx_connector-2.1.5/tests/test_one.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/tests/test_params.py` & `alyx_connector-2.1.5/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `alyx_connector-2.1.4/tests/test_registration.py` & `alyx_connector-2.1.5/tests/test_registration.py`

 * *Files identical despite different names*

