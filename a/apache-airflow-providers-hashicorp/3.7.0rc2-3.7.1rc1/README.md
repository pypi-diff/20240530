# Comparing `tmp/apache_airflow_providers_hashicorp-3.7.0rc2.tar.gz` & `tmp/apache_airflow_providers_hashicorp-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_hashicorp-3.7.0rc2.tar", last modified: Tue Apr 30 11:29:25 2024, max compression
+gzip compressed data, was "apache_airflow_providers_hashicorp-3.7.1rc1.tar", last modified: Tue May 21 10:38:55 2024, max compression
```

## Comparing `apache_airflow_providers_hashicorp-3.7.0rc2.tar` & `apache_airflow_providers_hashicorp-3.7.1rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4079 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/LICENSE
--rw-r--r--   0        0        0     1584 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/__init__.py
--rw-r--r--   0        0        0      785 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/__init__.py
--rw-r--r--   0        0        0    22534 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/vault_client.py
--rw-r--r--   0        0        0     2887 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/__init__.py
--rw-r--r--   0        0        0    18790 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/vault.py
--rw-r--r--   0        0        0      785 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/__init__.py
--rw-r--r--   0        0        0    12245 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/vault.py
--rw-r--r--   0        0        0     3102 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 apache_airflow_providers_hashicorp-3.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     4079 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/LICENSE
+-rw-r--r--   0        0        0     1496 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py
+-rw-r--r--   0        0        0    22645 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
+-rw-r--r--   0        0        0     2908 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/hooks/__init__.py
+-rw-r--r--   0        0        0    18790 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/hooks/vault.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/secrets/__init__.py
+-rw-r--r--   0        0        0    12245 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/secrets/vault.py
+-rw-r--r--   0        0        0     3102 2024-05-21 10:38:55.000000 apache_airflow_providers_hashicorp-3.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 apache_airflow_providers_hashicorp-3.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/README.rst` & `apache_airflow_providers_hashicorp-3.7.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.7.0.rc2``
+Release: ``3.7.1.rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``hashicorp`` provider. All classes for this provider package
 are in ``airflow.providers.hashicorp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-hashicorp``
@@ -92,8 +92,8 @@
 ====================================================================================================  ==========
 Dependent package                                                                                     Extra
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/LICENSE` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/__init__.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "3.7.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "3.7.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-hashicorp:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/__init__.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/vault_client.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,16 @@
                     status_forcelist=[412, 500, 502, 503],
                     raise_on_status=False,
                 )
             )
             session = Session()
             session.mount("http://", adapter)
             session.mount("https://", adapter)
+            if self.kwargs and "verify" in self.kwargs:
+                session.verify = self.kwargs["verify"]
             self.kwargs["session"] = session
 
         _client = hvac.Client(url=self.url, **self.kwargs)
         if self.auth_type == "approle":
             self._auth_approle(_client)
         elif self.auth_type == "aws_iam":
             self._auth_aws_iam(_client)
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/get_provider_info.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-hashicorp",
         "name": "Hashicorp",
         "description": "Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714476565,
+        "source-date-epoch": 1716287935,
         "versions": [
+            "3.7.1",
             "3.7.0",
             "3.6.4",
             "3.6.3",
             "3.6.2",
             "3.6.1",
             "3.6.0",
             "3.5.0",
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/__init__.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/vault.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/hooks/vault.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/__init__.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/vault.py` & `apache_airflow_providers_hashicorp-3.7.1rc1/airflow/providers/hashicorp/secrets/vault.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/pyproject.toml` & `apache_airflow_providers_hashicorp-3.7.1rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-hashicorp"
-version = "3.7.0.rc2"
+version = "3.7.1.rc1"
 description = "Provider package apache-airflow-providers-hashicorp for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -57,16 +57,16 @@
 requires-python = "~=3.8"
 dependencies = [
     "apache-airflow>=2.7.0rc0",
     "hvac>=1.1.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc2/PKG-INFO` & `apache_airflow_providers_hashicorp-3.7.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.7.0rc2
+Version: 3.7.1rc1
 Summary: Provider package apache-airflow-providers-hashicorp for Apache Airflow
 Keywords: airflow-provider,hashicorp,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: hvac>=1.1.0
 Requires-Dist: boto3>=1.33.0 ; extra == "boto3"
 Requires-Dist: apache-airflow-providers-google ; extra == "google"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: boto3
 Provides-Extra: google
 
@@ -75,28 +75,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.7.0.rc2``
+Release: ``3.7.1.rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``hashicorp`` provider. All classes for this provider package
 are in ``airflow.providers.hashicorp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-hashicorp``
@@ -129,8 +129,8 @@
 ====================================================================================================  ==========
 Dependent package                                                                                     Extra
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.1/changelog.html>`_.
```

