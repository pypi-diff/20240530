# Comparing `tmp/airbyte_source_mailerlite-1.0.0.tar.gz` & `tmp/airbyte_source_mailerlite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_mailerlite-1.0.0.tar", max compression
+gzip compressed data, was "airbyte_source_mailerlite-1.0.1.tar", max compression
```

## Comparing `airbyte_source_mailerlite-1.0.0.tar` & `airbyte_source_mailerlite-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4572 2024-05-28 22:04:33.065757 airbyte_source_mailerlite-1.0.0/README.md
--rw-r--r--   0        0        0      138 2024-05-28 22:04:33.069757 airbyte_source_mailerlite-1.0.0/main.py
--rw-r--r--   0        0        0      779 2024-05-28 22:08:28.832216 airbyte_source_mailerlite-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      132 2024-05-28 22:04:33.069757 airbyte_source_mailerlite-1.0.0/source_mailerlite/__init__.py
--rw-r--r--   0        0        0    45634 2024-05-28 22:04:33.069757 airbyte_source_mailerlite-1.0.0/source_mailerlite/manifest.yaml
--rw-r--r--   0        0        0      233 2024-05-28 22:04:33.069757 airbyte_source_mailerlite-1.0.0/source_mailerlite/run.py
--rw-r--r--   0        0        0      479 2024-05-28 22:04:33.069757 airbyte_source_mailerlite-1.0.0/source_mailerlite/source.py
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 airbyte_source_mailerlite-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4565 2024-05-30 00:24:42.000000 airbyte_source_mailerlite-1.0.1/README.md
+-rw-r--r--   0        0        0      763 2024-05-30 00:53:09.080311 airbyte_source_mailerlite-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-30 00:24:42.000000 airbyte_source_mailerlite-1.0.1/source_mailerlite/__init__.py
+-rw-r--r--   0        0        0    45634 2024-05-30 00:24:42.000000 airbyte_source_mailerlite-1.0.1/source_mailerlite/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-30 00:24:42.000000 airbyte_source_mailerlite-1.0.1/source_mailerlite/run.py
+-rw-r--r--   0        0        0      479 2024-05-30 00:24:42.000000 airbyte_source_mailerlite-1.0.1/source_mailerlite/source.py
+-rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 airbyte_source_mailerlite-1.0.1/PKG-INFO
```

### Comparing `airbyte_source_mailerlite-1.0.0/README.md` & `airbyte_source_mailerlite-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,103 +1,91 @@
-# Mailerlite Source
+# Mailerlite source connector
 
-This is the repository for the Mailerlite configuration based source connector.
+
+This is the repository for the Mailerlite source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/mailerlite).
 
 ## Local development
 
 ### Prerequisites
-
-* Python (`^3.9`)
-* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
-
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
 ### Installing the connector
-
 From this connector directory, run:
 ```bash
 poetry install --with dev
 ```
 
 
 ### Create credentials
-
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/mailerlite)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_mailerlite/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_mailerlite/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
-
 ```
 poetry run source-mailerlite spec
 poetry run source-mailerlite check --config secrets/config.json
 poetry run source-mailerlite discover --config secrets/config.json
-poetry run source-mailerlite read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-mailerlite read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Running tests
-
-To run tests locally, from the connector directory run:
-
+### Running unit tests
+To run unit tests locally, from the connector directory run:
 ```
-poetry run pytest tests
+poetry run pytest unit_tests
 ```
 
 ### Building the docker image
-
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-mailerlite build
 ```
 
 An image will be available on your host with the tag `airbyte/source-mailerlite:dev`.
 
 
 ### Running as a docker container
-
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-mailerlite:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-mailerlite:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-mailerlite:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-mailerlite:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
-
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-mailerlite test
 ```
 
 ### Customizing acceptance Tests
-
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-
 All of your dependencies should be managed via Poetry. 
 To add a new dependency, run:
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
-
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-mailerlite test`
 2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `dockerImageTag` value in `metadata.yaml`
     - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/mailerlite.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_mailerlite-1.0.0/pyproject.toml` & `airbyte_source_mailerlite-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.0.0"
+version = "1.0.1"
 name = "airbyte-source-mailerlite"
-description = "Source implementation for mailerlite."
+description = "Source implementation for Mailerlite."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://docs.airbyte.com/integrations/sources/mailerlite"
 homepage = "https://airbyte.com"
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_mailerlite" },
-    { include = "main.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "^1"
 
 [tool.poetry.scripts]
 source-mailerlite = "source_mailerlite.run:run"
 
 [tool.poetry.group.dev.dependencies]
-requests-mock = "*"
-pytest-mock = "*"
-pytest = "*"
+requests-mock = "^1.9.3"
+pytest = "^6.1"
+pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_mailerlite-1.0.0/source_mailerlite/manifest.yaml` & `airbyte_source_mailerlite-1.0.1/source_mailerlite/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailerlite-1.0.0/PKG-INFO` & `airbyte_source_mailerlite-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,122 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-mailerlite
-Version: 1.0.0
-Summary: Source implementation for mailerlite.
+Version: 1.0.1
+Summary: Source implementation for Mailerlite.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (>=1,<2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/mailerlite
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
-# Mailerlite Source
+# Mailerlite source connector
 
-This is the repository for the Mailerlite configuration based source connector.
+
+This is the repository for the Mailerlite source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/mailerlite).
 
 ## Local development
 
 ### Prerequisites
-
-* Python (`^3.9`)
-* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
-
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
 ### Installing the connector
-
 From this connector directory, run:
 ```bash
 poetry install --with dev
 ```
 
 
 ### Create credentials
-
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/mailerlite)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_mailerlite/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_mailerlite/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
-
 ```
 poetry run source-mailerlite spec
 poetry run source-mailerlite check --config secrets/config.json
 poetry run source-mailerlite discover --config secrets/config.json
-poetry run source-mailerlite read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-mailerlite read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Running tests
-
-To run tests locally, from the connector directory run:
-
+### Running unit tests
+To run unit tests locally, from the connector directory run:
 ```
-poetry run pytest tests
+poetry run pytest unit_tests
 ```
 
 ### Building the docker image
-
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-mailerlite build
 ```
 
 An image will be available on your host with the tag `airbyte/source-mailerlite:dev`.
 
 
 ### Running as a docker container
-
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-mailerlite:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-mailerlite:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-mailerlite:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-mailerlite:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
-
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-mailerlite test
 ```
 
 ### Customizing acceptance Tests
-
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-
 All of your dependencies should be managed via Poetry. 
 To add a new dependency, run:
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
-
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-mailerlite test`
 2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `dockerImageTag` value in `metadata.yaml`
     - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/mailerlite.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

