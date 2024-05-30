# Comparing `tmp/apache_airflow_providers_teradata-2.1.1rc1.tar.gz` & `tmp/apache_airflow_providers_teradata-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_teradata-2.1.1rc1.tar", last modified: Tue May 21 10:59:21 2024, max compression
+gzip compressed data, was "apache_airflow_providers_teradata-2.2.0rc1.tar", last modified: Thu May 30 06:45:06 2024, max compression
```

## Comparing `apache_airflow_providers_teradata-2.1.1rc1.tar` & `apache_airflow_providers_teradata-2.2.0rc1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     4343 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/LICENSE
--rw-r--r--   0        0        0     1495 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/__init__.py
--rw-r--r--   0        0        0     2890 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/hooks/__init__.py
--rw-r--r--   0        0        0     7386 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/hooks/teradata.py
--rw-r--r--   0        0        0      787 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/operators/__init__.py
--rw-r--r--   0        0        0     2373 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/operators/teradata.py
--rw-r--r--   0        0        0      785 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/transfers/__init__.py
--rw-r--r--   0        0        0     3834 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/transfers/teradata_to_teradata.py
--rw-r--r--   0        0        0     3170 2024-05-21 10:59:21.000000 apache_airflow_providers_teradata-2.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0     6260 1970-01-01 00:00:00.000000 apache_airflow_providers_teradata-2.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     4675 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/LICENSE
+-rw-r--r--   0        0        0     1495 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/__init__.py
+-rw-r--r--   0        0        0     3854 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/__init__.py
+-rw-r--r--   0        0        0     9511 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/teradata.py
+-rw-r--r--   0        0        0      787 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/teradata.py
+-rw-r--r--   0        0        0      785 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/__init__.py
+-rw-r--r--   0        0        0     4293 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/azure_blob_to_teradata.py
+-rw-r--r--   0        0        0     4523 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/s3_to_teradata.py
+-rw-r--r--   0        0        0     3834 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/teradata_to_teradata.py
+-rw-r--r--   0        0        0     3296 2024-05-30 06:45:06.000000 apache_airflow_providers_teradata-2.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6799 1970-01-01 00:00:00.000000 apache_airflow_providers_teradata-2.2.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/README.rst` & `apache_airflow_providers_teradata-2.2.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-teradata``
 
-Release: ``2.1.1.rc1``
+Release: ``2.2.0.rc1``
 
 
 `Teradata <https://www.teradata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``teradata`` provider. All classes for this provider package
 are in ``airflow.providers.teradata`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-teradata``
@@ -84,18 +84,20 @@
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
-    pip install apache-airflow-providers-teradata[common.sql]
+    pip install apache-airflow-providers-teradata[amazon]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-============================================================================================================  ==============
+======================================================================================================================  ===================
+Dependent package                                                                                                       Extra
+======================================================================================================================  ===================
+`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_                    ``amazon``
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_            ``common.sql``
+`apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
+======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/LICENSE` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import packaging.version
 
 from airflow import __version__ as airflow_version
 
 __all__ = ["__version__"]
 
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-teradata:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/get_provider_info.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/get_provider_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,22 +24,26 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-teradata",
         "name": "Teradata",
         "description": "`Teradata <https://www.teradata.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1716289161,
-        "versions": ["2.1.1", "2.1.0", "2.0.0"],
+        "source-date-epoch": 1717051506,
+        "versions": ["2.2.0", "2.1.1", "2.1.0", "2.0.0"],
         "dependencies": [
             "apache-airflow>=2.7.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "teradatasqlalchemy>=17.20.0.0",
             "teradatasql>=17.20.0.28",
         ],
+        "additional-extras": [
+            {"name": "microsoft.azure", "dependencies": ["apache-airflow-providers-microsoft-azure"]},
+            {"name": "amazon", "dependencies": ["apache-airflow-providers-amazon"]},
+        ],
         "integrations": [
             {
                 "integration-name": "Teradata",
                 "external-doc-url": "https://www.teradata.com/",
                 "how-to-guide": ["/docs/apache-airflow-providers-teradata/operators/teradata.rst"],
                 "logo": "/integration-logos/teradata/Teradata.png",
                 "tags": ["software"],
@@ -56,15 +60,27 @@
         ],
         "transfers": [
             {
                 "source-integration-name": "Teradata",
                 "target-integration-name": "Teradata",
                 "python-module": "airflow.providers.teradata.transfers.teradata_to_teradata",
                 "how-to-guide": "/docs/apache-airflow-providers-teradata/operators/teradata_to_teradata.rst",
-            }
+            },
+            {
+                "source-integration-name": "Microsoft Azure Blob Storage",
+                "target-integration-name": "Teradata",
+                "python-module": "airflow.providers.teradata.transfers.azure_blob_to_teradata",
+                "how-to-guide": "/docs/apache-airflow-providers-teradata/operators/azure_blob_to_teradata.rst",
+            },
+            {
+                "source-integration-name": "Amazon Simple Storage Service (S3)",
+                "target-integration-name": "Teradata",
+                "python-module": "airflow.providers.teradata.transfers.s3_to_teradata",
+                "how-to-guide": "/docs/apache-airflow-providers-teradata/operators/s3_to_teradata.rst",
+            },
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.teradata.hooks.teradata.TeradataHook",
                 "connection-type": "teradata",
             }
         ],
```

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/hooks/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/hooks/teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/hooks/teradata.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,14 +28,25 @@
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 if TYPE_CHECKING:
     from airflow.models.connection import Connection
 
+PARAM_TYPES = {bool, float, int, str}
+
+
+def _map_param(value):
+    if value in PARAM_TYPES:
+        # In this branch, value is a Python type; calling it produces
+        # an instance of the type which is understood by the Teradata driver
+        # in the out parameter mapping mechanism.
+        value = value()
+    return value
+
 
 class TeradataHook(DbApiHook):
     """General hook for interacting with Teradata SQL Database.
 
     This module contains basic APIs to connect to and interact with Teradata SQL Database. It uses teradatasql
     client internally as a database driver for connecting to Teradata database. The config parameters like
     Teradata DB Server URL, username, password and database name are fetched from the predefined connection
@@ -183,7 +194,62 @@
                 "extra": json.dumps(
                     {"tmode": "TERA", "sslmode": "verify-ca", "sslca": "/tmp/server-ca.pem"}, indent=4
                 ),
                 "login": "dbc",
                 "password": "dbc",
             },
         }
+
+    def callproc(
+        self,
+        identifier: str,
+        autocommit: bool = False,
+        parameters: list | dict | None = None,
+    ) -> list | dict | tuple | None:
+        """
+        Call the stored procedure identified by the provided string.
+
+        Any OUT parameters must be provided with a value of either the
+        expected Python type (e.g., `int`) or an instance of that type.
+
+        :param identifier: stored procedure name
+        :param autocommit: What to set the connection's autocommit setting to
+            before executing the query.
+        :param parameters: The `IN`, `OUT` and `INOUT` parameters for Teradata
+            stored procedure
+
+        The return value is a list or mapping that includes parameters in
+        both directions; the actual return type depends on the type of the
+        provided `parameters` argument.
+
+        """
+        if parameters is None:
+            parameters = []
+
+        args = ",".join("?" for name in parameters)
+
+        sql = f"{{CALL {identifier}({(args)})}}"
+
+        def handler(cursor):
+            records = cursor.fetchall()
+
+            if records is None:
+                return
+            if isinstance(records, list):
+                return [row for row in records]
+
+            if isinstance(records, dict):
+                return {n: v for (n, v) in records.items()}
+            raise TypeError(f"Unexpected results: {records}")
+
+        result = self.run(
+            sql,
+            autocommit=autocommit,
+            parameters=(
+                [_map_param(value) for (name, value) in parameters.items()]
+                if isinstance(parameters, dict)
+                else [_map_param(value) for value in parameters]
+            ),
+            handler=handler,
+        )
+
+        return result
```

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/operators/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/transfers/__init__.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/airflow/providers/teradata/transfers/teradata_to_teradata.py` & `apache_airflow_providers_teradata-2.2.0rc1/airflow/providers/teradata/transfers/teradata_to_teradata.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/pyproject.toml` & `apache_airflow_providers_teradata-2.2.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-teradata"
-version = "2.1.1.rc1"
+version = "2.2.0.rc1"
 description = "Provider package apache-airflow-providers-teradata for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -59,24 +59,30 @@
     "apache-airflow-providers-common-sql>=1.3.1rc0",
     "apache-airflow>=2.7.0rc0",
     "teradatasql>=17.20.0.28",
     "teradatasqlalchemy>=17.20.0.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
 provider_info = "airflow.providers.teradata.get_provider_info:get_provider_info"
 [project.optional-dependencies]
+"amazon" = [
+    "apache-airflow-providers-amazon",
+]
 "common.sql" = [
     "apache-airflow-providers-common-sql",
 ]
+"microsoft.azure" = [
+    "apache-airflow-providers-microsoft-azure",
+]
 
 [tool.flit.module]
 name = "airflow.providers.teradata"
```

### Comparing `apache_airflow_providers_teradata-2.1.1rc1/PKG-INFO` & `apache_airflow_providers_teradata-2.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-teradata
-Version: 2.1.1rc1
+Version: 2.2.0rc1
 Summary: Provider package apache-airflow-providers-teradata for Apache Airflow
 Keywords: airflow-provider,teradata,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,23 +21,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: teradatasql>=17.20.0.28
 Requires-Dist: teradatasqlalchemy>=17.20.0.0
+Requires-Dist: apache-airflow-providers-amazon ; extra == "amazon"
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
+Requires-Dist: apache-airflow-providers-microsoft-azure ; extra == "microsoft.azure"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Provides-Extra: amazon
 Provides-Extra: common.sql
+Provides-Extra: microsoft.azure
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
@@ -75,28 +79,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-teradata``
 
-Release: ``2.1.1.rc1``
+Release: ``2.2.0.rc1``
 
 
 `Teradata <https://www.teradata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``teradata`` provider. All classes for this provider package
 are in ``airflow.providers.teradata`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-teradata``
@@ -121,18 +125,20 @@
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
-    pip install apache-airflow-providers-teradata[common.sql]
+    pip install apache-airflow-providers-teradata[amazon]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-============================================================================================================  ==============
+======================================================================================================================  ===================
+Dependent package                                                                                                       Extra
+======================================================================================================================  ===================
+`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_                    ``amazon``
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_            ``common.sql``
+`apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
+======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.1.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-teradata/2.2.0/changelog.html>`_.
```

