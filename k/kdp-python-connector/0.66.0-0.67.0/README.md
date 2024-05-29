# Comparing `tmp/kdp-python-connector-0.66.0.tar.gz` & `tmp/kdp-python-connector-0.67.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-python-connector-0.66.0.tar", last modified: Fri Apr  5 01:48:26 2024, max compression
+gzip compressed data, was "kdp-python-connector-0.67.0.tar", last modified: Wed May 29 23:32:45 2024, max compression
```

## Comparing `kdp-python-connector-0.66.0.tar` & `kdp-python-connector-0.67.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.868216 kdp-python-connector-0.66.0/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.860216 kdp-python-connector-0.66.0/.github/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-04-05 01:48:15.000000 kdp-python-connector-0.66.0/.github/pull_request_template.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.860216 kdp-python-connector-0.66.0/.github/workflows/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7347 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.github/workflows/build-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6903 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.github/workflows/build-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.github/workflows/release-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.github/workflows/release-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.github/workflows/release.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.gitignore
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-05 01:48:26.868216 kdp-python-connector-0.66.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.860216 kdp-python-connector-0.66.0/datafiles/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/datafiles/actorfilms.csv
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.860216 kdp-python-connector-0.66.0/docs/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/Makefile
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/conf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/index.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/kdp_connector.configuration.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/kdp_connector.connectors.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/kdp_connector.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/make.bat
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/docs/modules.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.864215 kdp-python-connector-0.66.0/kdp_connector/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.864215 kdp-python-connector-0.66.0/kdp_connector/configuration/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/configuration/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/configuration/authenticationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/configuration/configurationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/configuration/keycloak_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/configuration/proxy_authentication.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.864215 kdp-python-connector-0.66.0/kdp_connector/connectors/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/Storage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1624 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/audit_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/audit_log_configs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7805 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/batch_write.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2276 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/index_management.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2388 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/ingest_job_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8921 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/kdp_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2311 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4782 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/read.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/connectors/upload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25560 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/kdp_connector/main.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.868216 kdp-python-connector-0.66.0/kdp_python_connector.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-05 01:48:26.000000 kdp-python-connector-0.66.0/kdp_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-04-05 01:48:26.000000 kdp-python-connector-0.66.0/kdp_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-05 01:48:26.000000 kdp-python-connector-0.66.0/kdp_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-05 01:48:26.000000 kdp-python-connector-0.66.0/kdp_python_connector.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-05 01:48:26.000000 kdp-python-connector-0.66.0/kdp_python_connector.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-05 01:48:26.868216 kdp-python-connector-0.66.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 01:48:26.868216 kdp-python-connector-0.66.0/test/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/test/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4263 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/test/test_ingest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/test/test_keycloak.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4719 2024-04-05 01:48:16.000000 kdp-python-connector-0.66.0/test/test_read.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.503394 kdp-python-connector-0.67.0/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.491393 kdp-python-connector-0.67.0/.github/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.github/pull_request_template.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.495394 kdp-python-connector-0.67.0/.github/workflows/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7347 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.github/workflows/build-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6903 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.github/workflows/build-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.github/workflows/release-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.github/workflows/release-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.github/workflows/release.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.gitignore
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-05-29 23:32:45.503394 kdp-python-connector-0.67.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.495394 kdp-python-connector-0.67.0/datafiles/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/datafiles/actorfilms.csv
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.495394 kdp-python-connector-0.67.0/docs/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/Makefile
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/conf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/index.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/kdp_connector.configuration.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/kdp_connector.connectors.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/kdp_connector.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/make.bat
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/docs/modules.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.495394 kdp-python-connector-0.67.0/kdp_connector/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.499394 kdp-python-connector-0.67.0/kdp_connector/configuration/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/configuration/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/configuration/authenticationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/configuration/configurationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/configuration/keycloak_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/configuration/proxy_authentication.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.499394 kdp-python-connector-0.67.0/kdp_connector/connectors/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/Storage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1624 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/audit_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/audit_log_configs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7805 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/batch_write.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2276 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/index_management.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2388 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/ingest_job_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8921 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/kdp_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2311 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4782 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/read.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/connectors/upload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25560 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/kdp_connector/main.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.503394 kdp-python-connector-0.67.0/kdp_python_connector.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-05-29 23:32:45.000000 kdp-python-connector-0.67.0/kdp_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-05-29 23:32:45.000000 kdp-python-connector-0.67.0/kdp_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-29 23:32:45.000000 kdp-python-connector-0.67.0/kdp_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-05-29 23:32:45.000000 kdp-python-connector-0.67.0/kdp_python_connector.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-05-29 23:32:45.000000 kdp-python-connector-0.67.0/kdp_python_connector.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-29 23:32:45.503394 kdp-python-connector-0.67.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 23:32:45.503394 kdp-python-connector-0.67.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/test/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4263 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/test/test_ingest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/test/test_keycloak.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4719 2024-05-29 23:32:35.000000 kdp-python-connector-0.67.0/test/test_read.py
```

### Comparing `kdp-python-connector-0.66.0/.github/workflows/build-internal.yaml` & `kdp-python-connector-0.67.0/.github/workflows/build-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/.github/workflows/build-public.yaml` & `kdp-python-connector-0.67.0/.github/workflows/build-public.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/.github/workflows/release-internal.yaml` & `kdp-python-connector-0.67.0/.github/workflows/release-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/.github/workflows/release-public.yaml` & `kdp-python-connector-0.67.0/.github/workflows/release-public.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/.github/workflows/release.yaml` & `kdp-python-connector-0.67.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/.gitignore` & `kdp-python-connector-0.67.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/PKG-INFO` & `kdp-python-connector-0.67.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.66.0
+Version: 0.67.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: kdp-api-python-client~=4.127.0
+Requires-Dist: kdp-api-python-client~=4.128.0
 Requires-Dist: pandas~=1.4.2
 Requires-Dist: numpy~=1.22.4
 
 # kdp-python-connector
 
 ## Prequisites
 * Python version 3.8.5
```

### Comparing `kdp-python-connector-0.66.0/datafiles/actorfilms.csv` & `kdp-python-connector-0.67.0/datafiles/actorfilms.csv`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/docs/Makefile` & `kdp-python-connector-0.67.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/docs/conf.py` & `kdp-python-connector-0.67.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/docs/kdp_connector.configuration.rst` & `kdp-python-connector-0.67.0/docs/kdp_connector.configuration.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/docs/kdp_connector.connectors.rst` & `kdp-python-connector-0.67.0/docs/kdp_connector.connectors.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/docs/make.bat` & `kdp-python-connector-0.67.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/configuration/authenticationUtil.py` & `kdp-python-connector-0.67.0/kdp_connector/configuration/authenticationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/configuration/configurationUtil.py` & `kdp-python-connector-0.67.0/kdp_connector/configuration/configurationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/configuration/keycloak_authentication.py` & `kdp-python-connector-0.67.0/kdp_connector/configuration/keycloak_authentication.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/Storage.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/Storage.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/audit_log.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/audit_log.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/audit_log_configs.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/audit_log_configs.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/batch_write.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/batch_write.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/index_management.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/index_management.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/ingest_job_api.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/ingest_job_api.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/kdp_api.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/kdp_api.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/query.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/query.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/read.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/read.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/connectors/upload.py` & `kdp-python-connector-0.67.0/kdp_connector/connectors/upload.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_connector/main.py` & `kdp-python-connector-0.67.0/kdp_connector/main.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/kdp_python_connector.egg-info/PKG-INFO` & `kdp-python-connector-0.67.0/kdp_python_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.66.0
+Version: 0.67.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: kdp-api-python-client~=4.127.0
+Requires-Dist: kdp-api-python-client~=4.128.0
 Requires-Dist: pandas~=1.4.2
 Requires-Dist: numpy~=1.22.4
 
 # kdp-python-connector
 
 ## Prequisites
 * Python version 3.8.5
```

### Comparing `kdp-python-connector-0.66.0/kdp_python_connector.egg-info/SOURCES.txt` & `kdp-python-connector-0.67.0/kdp_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/pyproject.toml` & `kdp-python-connector-0.67.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.66.0"
+version = "0.67.0"
 dependencies = [
-  'kdp-api-python-client ~= 4.127.0',
+  'kdp-api-python-client ~= 4.128.0',
   'pandas ~= 1.4.2',
   'numpy ~= 1.22.4'
 ]
 
 [tool.setuptools.packages.find]
 include = ["kdp_connector"]
```

### Comparing `kdp-python-connector-0.66.0/test/test_ingest.py` & `kdp-python-connector-0.67.0/test/test_ingest.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/test/test_keycloak.py` & `kdp-python-connector-0.67.0/test/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.66.0/test/test_read.py` & `kdp-python-connector-0.67.0/test/test_read.py`

 * *Files identical despite different names*

