# Comparing `tmp/apache_airflow_providers_asana-2.5.1rc1.tar.gz` & `tmp/apache-airflow-providers-asana-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_asana-2.5.1rc1.tar", last modified: Tue May 21 10:20:43 2024, max compression
+gzip compressed data, was "dist/apache-airflow-providers-asana-3.0.0rc1.tar", last modified: Tue Nov 15 00:14:08 2022, max compression
```

## Comparing `apache_airflow_providers_asana-2.5.1rc1.tar` & `apache-airflow-providers-asana-3.0.0rc1.tar`

### file list

```diff
@@ -1,11 +1,28 @@
--rw-r--r--   0        0        0     3046 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/LICENSE
--rw-r--r--   0        0        0      779 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/README.md
--rw-r--r--   0        0        0     1492 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/__init__.py
--rw-r--r--   0        0        0     2466 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/hooks/__init__.py
--rw-r--r--   0        0        0    12406 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/hooks/asana.py
--rw-r--r--   0        0        0      787 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/operators/__init__.py
--rw-r--r--   0        0        0     5491 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/operators/asana_tasks.py
--rw-r--r--   0        0        0     2960 2024-05-21 10:20:43.000000 apache_airflow_providers_asana-2.5.1rc1/pyproject.toml
--rw-r--r--   0        0        0     4735 1970-01-01 00:00:00.000000 apache_airflow_providers_asana-2.5.1rc1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7480 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13369 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2022-09-14 19:22:24.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1832 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1460 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/LICENSE` & `apache-airflow-providers-asana-3.0.0rc1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -195,59 +195,7 @@
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
-============================================================================
-   APACHE AIRFLOW SUBCOMPONENTS:
-
-   The Apache Airflow project contains subcomponents with separate copyright
-   notices and license terms. Your use of the source code for the these
-   subcomponents is subject to the terms and conditions of the following
-   licenses.
-
-
-========================================================================
-Third party Apache 2.0 licenses
-========================================================================
-
-The following components are provided under the Apache 2.0 License.
-See project link for details. The text of each license is also included
-at licenses/LICENSE-[project].txt.
-
-    (ALv2 License) hue v4.3.0 (https://github.com/cloudera/hue/)
-    (ALv2 License) jqclock v2.3.0 (https://github.com/JohnRDOrazio/jQuery-Clock-Plugin)
-    (ALv2 License) bootstrap3-typeahead v4.0.2 (https://github.com/bassjobsen/Bootstrap-3-Typeahead)
-    (ALv2 License) connexion v2.7.0 (https://github.com/zalando/connexion)
-
-========================================================================
-MIT licenses
-========================================================================
-
-The following components are provided under the MIT License. See project link for details.
-The text of each license is also included at licenses/LICENSE-[project].txt.
-
-    (MIT License) jquery v3.5.1 (https://jquery.org/license/)
-    (MIT License) dagre-d3 v0.6.4 (https://github.com/cpettitt/dagre-d3)
-    (MIT License) bootstrap v3.4.1 (https://github.com/twbs/bootstrap/)
-    (MIT License) d3-tip v0.9.1 (https://github.com/Caged/d3-tip)
-    (MIT License) dataTables v1.10.25 (https://datatables.net)
-    (MIT License) normalize.css v3.0.2 (http://necolas.github.io/normalize.css/)
-    (MIT License) ElasticMock v1.3.2 (https://github.com/vrcmarcos/elasticmock)
-    (MIT License) MomentJS v2.24.0 (http://momentjs.com/)
-    (MIT License) eonasdan-bootstrap-datetimepicker v4.17.49 (https://github.com/eonasdan/bootstrap-datetimepicker/)
-
-========================================================================
-BSD 3-Clause licenses
-========================================================================
-The following components are provided under the BSD 3-Clause license. See project links for details.
-The text of each license is also included at licenses/LICENSE-[project].txt.
-
-    (BSD 3 License) d3 v5.16.0 (https://d3js.org)
-    (BSD 3 License) d3-shape v2.1.0 (https://github.com/d3/d3-shape)
-    (BSD 3 License) cgroupspy 0.2.1 (https://github.com/cloudsigma/cgroupspy)
-
-========================================================================
-See licenses/LICENSES-ui.txt for packages used in `/airflow/www`
```

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/README.md` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-<!--
- Licensed to the Apache Software Foundation (ASF) under one
- or more contributor license agreements.  See the NOTICE file
- distributed with this work for additional information
- regarding copyright ownership.  The ASF licenses this file
- to you under the Apache License, Version 2.0 (the
- "License"); you may not use this file except in compliance
- with the License.  You may obtain a copy of the License at
-
-   http://www.apache.org/licenses/LICENSE-2.0
-
- Unless required by applicable law or agreed to in writing,
- software distributed under the License is distributed on an
- "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
- KIND, either express or implied.  See the License for the
- specific language governing permissions and limitations
- under the License.
- -->
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
```

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -10,30 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-#
+
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
-# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
+# OVERWRITTEN WHEN PREPARING PACKAGES.
 #
-# IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
-# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
-#
-from __future__ import annotations
+# IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
+# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
-import packaging.version
+"""Setup.py for the apache-airflow-providers-asana package."""
 
-from airflow import __version__ as airflow_version
+from setuptools import find_namespace_packages, setup
 
-__all__ = ["__version__"]
+version = "3.0.0"
 
-__version__ = "2.5.1"
 
-if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
-    "2.7.0"
-):
-    raise RuntimeError(
-        f"The package `apache-airflow-providers-asana:{__version__}` needs Apache Airflow 2.7.0+"
+def do_setup():
+    """Perform the package apache-airflow-providers-asana setup."""
+    setup(
+        version=version,
+        extras_require={},
+        packages=find_namespace_packages(include=["airflow.providers.asana", "airflow.providers.asana.*"]),
     )
+
+
+if __name__ == "__main__":
+    do_setup()
```

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/get_provider_info.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,44 +14,25 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
 # OVERWRITTEN WHEN PREPARING PACKAGES.
 #
-# IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
-# `get_provider_info_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
+# IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
+# `get_provider_info_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-asana",
         "name": "Asana",
-        "description": "`Asana <https://asana.com/>`__\n",
-        "state": "ready",
-        "source-date-epoch": 1716286843,
-        "versions": [
-            "2.5.1",
-            "2.5.0",
-            "2.4.1",
-            "2.4.0",
-            "2.3.0",
-            "2.2.2",
-            "2.2.1",
-            "2.2.0",
-            "2.1.0",
-            "2.0.1",
-            "2.0.0",
-            "1.1.3",
-            "1.1.2",
-            "1.1.1",
-            "1.1.0",
-            "1.0.0",
-        ],
-        "dependencies": ["apache-airflow>=2.7.0", "asana>=0.10,<4.0.0"],
+        "description": "`Asana <https://app.asana.com/>`__\n",
+        "versions": ["3.0.0", "2.0.1", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.3.0", "asana>=0.10"],
         "integrations": [
             {
                 "integration-name": "Asana",
                 "external-doc-url": "https://developers.asana.com/docs",
                 "how-to-guide": ["/docs/apache-airflow-providers-asana/operators/asana.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/hooks/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/hooks/asana.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,54 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Connect to Asana."""
-
 from __future__ import annotations
 
-from functools import cached_property
+from functools import wraps
 from typing import Any
 
 from asana import Client  # type: ignore[attr-defined]
 from asana.error import NotFoundError  # type: ignore[attr-defined]
 
+from airflow.compat.functools import cached_property
 from airflow.hooks.base import BaseHook
 
 
+def _ensure_prefixes(conn_type):
+    """
+    Remove when provider min airflow version >= 2.5.0 since this is handled by
+    provider manager from that version.
+    """
+
+    def dec(func):
+        @wraps(func)
+        def inner():
+            field_behaviors = func()
+            conn_attrs = {"host", "schema", "login", "password", "port", "extra"}
+
+            def _ensure_prefix(field):
+                if field not in conn_attrs and not field.startswith("extra__"):
+                    return f"extra__{conn_type}__{field}"
+                else:
+                    return field
+
+            if "placeholders" in field_behaviors:
+                placeholders = field_behaviors["placeholders"]
+                field_behaviors["placeholders"] = {_ensure_prefix(k): v for k, v in placeholders.items()}
+            return field_behaviors
+
+        return inner
+
+    return dec
+
+
 class AsanaHook(BaseHook):
     """Wrapper around Asana Python client library."""
 
     conn_name_attr = "asana_conn_id"
     default_conn_name = "asana_default"
     conn_type = "asana"
     hook_name = "Asana"
@@ -55,53 +83,54 @@
             return extras[field_name] or None
         prefixed_name = f"{backcompat_prefix}{field_name}"
         return extras.get(prefixed_name) or None
 
     def get_conn(self) -> Client:
         return self.client
 
-    @classmethod
-    def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Return connection widgets to add to connection form."""
+    @staticmethod
+    def get_connection_form_widgets() -> dict[str, Any]:
+        """Returns connection widgets to add to connection form"""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
 
         return {
             "workspace": StringField(lazy_gettext("Workspace"), widget=BS3TextFieldWidget()),
             "project": StringField(lazy_gettext("Project"), widget=BS3TextFieldWidget()),
         }
 
-    @classmethod
-    def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom field behaviour."""
+    @staticmethod
+    @_ensure_prefixes(conn_type="asana")
+    def get_ui_field_behaviour() -> dict[str, Any]:
+        """Returns custom field behaviour"""
         return {
             "hidden_fields": ["port", "host", "login", "schema"],
             "relabeling": {},
             "placeholders": {
                 "password": "Asana personal access token",
                 "workspace": "Asana workspace gid",
                 "project": "Asana project gid",
             },
         }
 
     @cached_property
     def client(self) -> Client:
-        """Instantiate python-asana Client."""
+        """Instantiates python-asana Client"""
         if not self.connection.password:
             raise ValueError(
                 "Asana connection password must contain a personal access token: "
                 "https://developers.asana.com/docs/personal-access-token"
             )
 
         return Client.access_token(self.connection.password)
 
     def create_task(self, task_name: str, params: dict | None) -> dict:
         """
-        Create an Asana task.
+        Creates an Asana task.
 
         :param task_name: Name of the new task
         :param params: Other task attributes, such as due_on, parent, and notes. For a complete list
             of possible parameters, see https://developers.asana.com/docs/create-a-task
         :return: A dict of attributes of the created task, including its gid
         """
         merged_params = self._merge_create_task_parameters(task_name, params)
@@ -139,29 +168,29 @@
         if required_parameters.isdisjoint(params):
             raise ValueError(
                 f"You must specify at least one of {required_parameters} in the create_task parameters"
             )
 
     def delete_task(self, task_id: str) -> dict:
         """
-        Delete an Asana task.
+        Deletes an Asana task.
 
         :param task_id: Asana GID of the task to delete
         :return: A dict containing the response from Asana
         """
         try:
             response = self.client.tasks.delete_task(task_id)
             return response
         except NotFoundError:
             self.log.info("Asana task %s not found for deletion.", task_id)
             return {}
 
     def find_task(self, params: dict | None) -> list:
         """
-        Retrieve a list of Asana tasks that match search parameters.
+        Retrieves a list of Asana tasks that match search parameters.
 
         :param params: Attributes that matching tasks should have. For a list of possible parameters,
             see https://developers.asana.com/docs/get-multiple-tasks
         :return: A list of dicts containing attributes of matching Asana tasks
         """
         merged_params = self._merge_find_task_parameters(params)
         self._validate_find_task_parameters(merged_params)
@@ -202,42 +231,42 @@
             raise ValueError(
                 f"You must specify at least one of {one_of_list} "
                 f"or both of {both_of_list} in the find_task parameters."
             )
 
     def update_task(self, task_id: str, params: dict) -> dict:
         """
-        Update an existing Asana task.
+        Updates an existing Asana task.
 
         :param task_id: Asana GID of task to update
         :param params: New values of the task's attributes. For a list of possible parameters, see
             https://developers.asana.com/docs/update-a-task
         :return: A dict containing the updated task's attributes
         """
         response = self.client.tasks.update(task_id, params)
         return response
 
     def create_project(self, params: dict) -> dict:
         """
-        Create a new project.
+        Creates a new project.
 
         :param params: Attributes that the new project should have. See
             https://developers.asana.com/docs/create-a-project#create-a-project-parameters
             for a list of possible parameters.
         :return: A dict containing the new project's attributes, including its GID.
         """
         merged_params = self._merge_project_parameters(params)
         self._validate_create_project_parameters(merged_params)
         response = self.client.projects.create(merged_params)
         return response
 
     @staticmethod
     def _validate_create_project_parameters(params: dict) -> None:
         """
-        Check that user provided the minimum required parameters for project creation.
+        Check that user provided the minimum required parameters for project creation
 
         :param params: Attributes that the new project should have
         :return: None; raises a ValueError if `params` does not contain the minimum required attributes.
         """
         required_parameters = {"workspace", "team"}
         if required_parameters.isdisjoint(params):
             raise ValueError(
@@ -254,41 +283,41 @@
         """
         merged_params = {} if self.workspace is None else {"workspace": self.workspace}
         merged_params.update(params)
         return merged_params
 
     def find_project(self, params: dict) -> list:
         """
-        Retrieve a list of Asana projects that match search parameters.
+        Retrieves a list of Asana projects that match search parameters.
 
         :param params: Attributes which matching projects should have. See
             https://developers.asana.com/docs/get-multiple-projects
             for a list of possible parameters.
         :return: A list of dicts containing attributes of matching Asana projects
         """
         merged_params = self._merge_project_parameters(params)
         response = self.client.projects.find_all(merged_params)
         return list(response)
 
     def update_project(self, project_id: str, params: dict) -> dict:
         """
-        Update an existing project.
+        Updates an existing project.
 
         :param project_id: Asana GID of the project to update
         :param params: New attributes that the project should have. See
             https://developers.asana.com/docs/update-a-project#update-a-project-parameters
             for a list of possible parameters
         :return: A dict containing the updated project's attributes
         """
         response = self.client.projects.update(project_id, params)
         return response
 
     def delete_project(self, project_id: str) -> dict:
         """
-        Delete a project.
+        Deletes a project.
 
         :param project_id: Asana GID of the project to delete
         :return: A dict containing the response from Asana
         """
         try:
             response = self.client.projects.delete(project_id)
             return response
```

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/operators/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_asana-2.5.1rc1/airflow/providers/asana/operators/asana_tasks.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,16 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class AsanaCreateTaskOperator(BaseOperator):
     """
-    This operator can be used to create Asana tasks.
-
-    .. seealso::
-        For more information on Asana optional task parameters:
-        https://developers.asana.com/docs/create-a-task
+    This operator can be used to create Asana tasks. For more information on
+    Asana optional task parameters, see https://developers.asana.com/docs/create-a-task
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaCreateTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param name: Name of the Asana task.
@@ -66,18 +63,16 @@
         self.log.info(response)
         return response["gid"]
 
 
 class AsanaUpdateTaskOperator(BaseOperator):
     """
     This operator can be used to update Asana tasks.
-
-    .. seealso::
-        For more information on Asana optional task parameters:
-        https://developers.asana.com/docs/update-a-task
+    For more information on Asana optional task parameters, see
+    https://developers.asana.com/docs/update-a-task
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaUpdateTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param asana_task_gid: Asana task ID to update
@@ -134,18 +129,15 @@
         response = hook.delete_task(self.asana_task_gid)
         self.log.info(response)
 
 
 class AsanaFindTaskOperator(BaseOperator):
     """
     This operator can be used to retrieve Asana tasks that match various filters.
-
-    .. seealso::
-        For a list of possible filters:
-        https://developers.asana.com/docs/update-a-task
+    See https://developers.asana.com/docs/update-a-task for a list of possible filters.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaFindTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param search_parameters: The parameters used to find relevant tasks. You must
```

