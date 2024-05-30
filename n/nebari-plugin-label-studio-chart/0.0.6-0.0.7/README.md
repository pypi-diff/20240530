# Comparing `tmp/nebari_plugin_label_studio_chart-0.0.6.tar.gz` & `tmp/nebari_plugin_label_studio_chart-0.0.7.tar.gz`

## Comparing `nebari_plugin_label_studio_chart-0.0.6.tar` & `nebari_plugin_label_studio_chart-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/__about__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/__init__.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/plugin.py
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/main.tf
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/variables.tf
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/versions.tf
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/chart/Chart.yaml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/chart/values.yaml
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/chart/templates/auth.yaml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/chart/templates/ingress.yaml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/.gitignore
--rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/README.md
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/__about__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/__init__.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/plugin.py
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/main.tf
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/variables.tf
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/versions.tf
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/chart/Chart.yaml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/chart/values.yaml
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/chart/templates/auth.yaml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/.gitignore
+-rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/README.md
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.7/PKG-INFO
```

### Comparing `nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/plugin.py` & `nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/plugin.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/main.tf` & `nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/outputs.tf` & `nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/variables.tf` & `nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/chart/templates/auth.yaml` & `nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/chart/templates/auth.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/src/nebari_plugin_label_studio_chart/template/chart/templates/ingress.yaml` & `nebari_plugin_label_studio_chart-0.0.7/src/nebari_plugin_label_studio_chart/template/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/LICENSE.md` & `nebari_plugin_label_studio_chart-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/pyproject.toml` & `nebari_plugin_label_studio_chart-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.6/PKG-INFO` & `nebari_plugin_label_studio_chart-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nebari-plugin-label-studio-chart
-Version: 0.0.6
+Version: 0.0.7
 Summary: MetroStar Onyx - Label Studio plugin for Nebari platform
 Project-URL: Documentation, https://github.com/MetroStar/nebari-label-studio#readme
 Project-URL: Issues, https://github.com/MetroStar/nebari-label-studio/issues
 Project-URL: Source, https://github.com/MetroStar/nebari-label-studio
 Author-email: Scott Blair <sblair@metrostar.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -19,14 +19,19 @@
 Requires-Python: >=3.8
 Requires-Dist: nebari
 Description-Content-Type: text/markdown
 
 
 # Nebari Plugin Label-Studio Chart
 
+[![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-label-studio-chart.svg)](https://pypi.org/project/nebari-plugin-label-studio-chart)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-label-studio-chart.svg)](https://pypi.org/project/nebari-plugin-label-studio-chart)
+
+-----
+
 ## Overview
 This plugin integrates Label Studio into the Nebari platform, allowing seamless labeling functionality within Nebari. Utilizing Python, Terraform, Kubernetes, and Helm charts, the plugin provides a configurable deployment and authentication through Keycloak.
 
 ## Design and Architecture
 The plugin follows a modular design, leveraging Terraform to define the deployment of Label Studio within a Kubernetes cluster. Key components include:
 - **Terraform Configuration**: Defines variables, outputs, and resources for deployment, including Helm release, Keycloak authentication, and Kubernetes secrets.
 - **Helm Chart Integration**: Deploys Label Studio as a Helm chart within the specified Kubernetes namespace.
@@ -54,14 +59,24 @@
     # helm release name - default label-studio
     name: label-studio
     # target namespace - default (nebari global namespace)
     namespace: label-studio
     # enable or disable traefik auth proxy and keycloak integration
     auth:
         enabled: true
+    # configure default affinity/selector for chart components
+    affinity:
+        enabled: true # default
+        selector: general # default
+        # -- or --
+        selector:
+            default: general
+            worker: worker
+            db: general
+            auth: general
     # helm chart values overrides
     values: {}
 ```
 
 ### Internal
 The following configuration values apply to the internally managed terraform module and are indirectly controlled through related values in `nebari-config.yaml`.
 
@@ -70,21 +85,46 @@
 - `realm_id`, `client_id`: Keycloak authentication settings.
 - `base_url`, `external_url`, `valid_redirect_uris`: OpenID URLs.
 - `signing_key_ref`: Signing key reference information.
 - `create_namespace`, `namespace`: Kubernetes namespace configuration.
 - `overrides`: Map for overriding default configurations.
 - `auth_enabled`: Flag to enable/disable authentication.
 
+### Label Studio Version
+
+Label Studio is deployed via its offical Helm chart and will default to using the `develop` image tag if not specified.
+
+To set a Label Studio version, update your `nebari-config.yaml` to override the app image tag used in the helm chart.
+
+``` yaml
+label_studio:
+  namespace: label-studio
+  values:
+    # Deploy Label Studio 1.8.1
+    global:
+      image:
+        tag: "1.8.1"
+```
+See the [Label Studio helm chart documentation](https://labelstud.io/guide/helm_values) for all available configurations.
+
+## Usage
+Once the extension is installed, the Label Studio Community Edition will be available at `https://[your-project-domain]/label-studio`.
+
+If authentication is enabled, any user attempting to access Label Studio will be required to login first with valid, active Nebari (Keycloak) credentials.  However, Label Studio accounts are separate from Nebari accounts.  Any user who has passed the authentication step above will then be able to create their own account.
+
+> NOTE: The Community Edition of Label Studio does not include role-based access permissions.  All users have access to the same functionality and can see all projects.
+
+Once a user has created their account, they can join the Label Studio 101 tutorial at the step [Label Studio 101 - Creating Your Project](https://labelstud.io/blog/zero-to-one-getting-started-with-label-studio/#creating-your-project).
+
+For more information on using Label Studio, refer to the [Label Studio documentation](https://labelstud.io/guide/).
+
 ## Testing Overview
 
 The plugin includes unit tests to validate its core functionalities:
 
 - **Constructor Test**: Verifies the default name and priority.
 - **Input Variables Test**: Validates domain, realm ID, client ID, and external URL settings.
 - **Default Namespace Test**: Tests the default namespace configuration.
 
-## Version Information
-- **Plugin Version**: 0.0.5
-
 ## License
 
 `nebari-plugin-label-studio-chart` is distributed under the terms of the [Apache](./LICENSE.md) license.
```

