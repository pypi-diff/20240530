# Comparing `tmp/apache_airflow_providers_common_io-1.3.1rc1.tar.gz` & `tmp/apache_airflow_providers_common_io-1.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_common_io-1.3.1rc1.tar", last modified: Tue Apr  9 12:23:20 2024, max compression
+gzip compressed data, was "apache_airflow_providers_common_io-1.3.2rc1.tar", last modified: Tue May 21 10:26:31 2024, max compression
```

## Comparing `apache_airflow_providers_common_io-1.3.1rc1.tar` & `apache_airflow_providers_common_io-1.3.2rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4074 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/LICENSE
--rw-r--r--   0        0        0     1584 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/__init__.py
--rw-r--r--   0        0        0     3799 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/__init__.py
--rw-r--r--   0        0        0     3479 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/file_transfer.py
--rw-r--r--   0        0        0     1362 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/__init__.py
--rw-r--r--   0        0        0     5979 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/backend.py
--rw-r--r--   0        0        0     3058 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/pyproject.toml
--rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 apache_airflow_providers_common_io-1.3.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     4074 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/LICENSE
+-rw-r--r--   0        0        0     1496 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/__init__.py
+-rw-r--r--   0        0        0     3808 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/operators/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/operators/file_transfer.py
+-rw-r--r--   0        0        0     1273 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/xcom/__init__.py
+-rw-r--r--   0        0        0     5979 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/xcom/backend.py
+-rw-r--r--   0        0        0     3058 2024-05-21 10:26:31.000000 apache_airflow_providers_common_io-1.3.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 apache_airflow_providers_common_io-1.3.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/README.rst` & `apache_airflow_providers_common_io-1.3.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-common-io``
 
-Release: ``1.3.1.rc1``
+Release: ``1.3.2.rc1``
 
 
 ``Common IO Provider``
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.io`` provider. All classes for this provider package
 are in ``airflow.providers.common.io`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-io``
@@ -91,8 +91,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2/changelog.html>`_.
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/LICENSE` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/__init__.py` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "1.3.1"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "1.3.2"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.8.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-common-io:{__version__}` needs Apache Airflow 2.8.0+"
     )
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/get_provider_info.py` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-io",
         "name": "Common IO",
         "description": "``Common IO Provider``\n",
         "state": "ready",
-        "source-date-epoch": 1712665400,
-        "versions": ["1.3.1", "1.3.0", "1.2.0", "1.1.0", "1.0.1", "1.0.0"],
+        "source-date-epoch": 1716287191,
+        "versions": ["1.3.2", "1.3.1", "1.3.0", "1.2.0", "1.1.0", "1.0.1", "1.0.0"],
         "dependencies": ["apache-airflow>=2.8.0"],
         "integrations": [
             {
                 "integration-name": "Common IO",
                 "external-doc-url": "https://filesystem-spec.readthedocs.io/en/latest/index.html",
                 "how-to-guide": ["/docs/apache-airflow-providers-common-io/operators.rst"],
                 "tags": ["software"],
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/__init__.py` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/file_transfer.py` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/operators/file_transfer.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,19 +75,29 @@
         src.copy(dst)
 
     def get_openlineage_facets_on_start(self) -> OperatorLineage:
         from openlineage.client.run import Dataset
 
         from airflow.providers.openlineage.extractors import OperatorLineage
 
+        def _prepare_ol_dataset(path: ObjectStoragePath) -> Dataset:
+            if hasattr(path, "namespace"):
+                # namespace has been added in Airflow 2.9.0; #36410
+                return Dataset(namespace=path.namespace, name=path.key)
+            # manually recreating namespace
+            return Dataset(
+                namespace=f"{path.protocol}://{path.bucket}" if path.bucket else path.protocol,
+                name=path.key.lstrip(path.sep),
+            )
+
         src: ObjectStoragePath = self._get_path(self.src, self.source_conn_id)
         dst: ObjectStoragePath = self._get_path(self.dst, self.dst_conn_id)
 
-        input_dataset = Dataset(namespace=src.namespace, name=src.key)
-        output_dataset = Dataset(namespace=dst.namespace, name=dst.key)
+        input_dataset = _prepare_ol_dataset(src)
+        output_dataset = _prepare_ol_dataset(dst)
 
         return OperatorLineage(
             inputs=[input_dataset],
             outputs=[output_dataset],
         )
 
     @staticmethod
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/__init__.py` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/xcom/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,21 +14,17 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import packaging.version
 
+from airflow import __version__ as airflow_version
 from airflow.exceptions import AirflowOptionalProviderFeatureException
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
-
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.9.0"
 ):
     raise AirflowOptionalProviderFeatureException(
         "The package xcom backend feature of `apache-airflow-providers-common-io` needs "
         "Apache Airflow 2.9.0+"
     )
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/backend.py` & `apache_airflow_providers_common_io-1.3.2rc1/airflow/providers/common/io/xcom/backend.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/pyproject.toml` & `apache_airflow_providers_common_io-1.3.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-common-io"
-version = "1.3.1.rc1"
+version = "1.3.2.rc1"
 description = "Provider package apache-airflow-providers-common-io for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -56,16 +56,16 @@
 ]
 requires-python = "~=3.8"
 dependencies = [
     "apache-airflow>=2.8.0rc0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_common_io-1.3.1rc1/PKG-INFO` & `apache_airflow_providers_common_io-1.3.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-io
-Version: 1.3.1rc1
+Version: 1.3.2rc1
 Summary: Provider package apache-airflow-providers-common-io for Apache Airflow
 Keywords: airflow-provider,common.io,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow>=2.8.0rc0
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: openlineage
 
 
@@ -72,28 +72,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-common-io``
 
-Release: ``1.3.1.rc1``
+Release: ``1.3.2.rc1``
 
 
 ``Common IO Provider``
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.io`` provider. All classes for this provider package
 are in ``airflow.providers.common.io`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-io``
@@ -125,8 +125,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.2/changelog.html>`_.
```

