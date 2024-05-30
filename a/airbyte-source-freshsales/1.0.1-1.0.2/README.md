# Comparing `tmp/airbyte_source_freshsales-1.0.1.tar.gz` & `tmp/airbyte_source_freshsales-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_freshsales-1.0.1.tar", max compression
+gzip compressed data, was "airbyte_source_freshsales-1.0.2.tar", max compression
```

## Comparing `airbyte_source_freshsales-1.0.1.tar` & `airbyte_source_freshsales-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4567 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/README.md
--rw-r--r--   0        0        0      138 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/main.py
--rw-r--r--   0        0        0      779 2024-05-28 22:09:45.105685 airbyte_source_freshsales-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      132 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/__init__.py
--rw-r--r--   0        0        0    47946 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/manifest.yaml
--rw-r--r--   0        0        0      233 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/run.py
--rw-r--r--   0        0        0      479 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/source.py
--rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 airbyte_source_freshsales-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4569 2024-05-30 09:46:12.000000 airbyte_source_freshsales-1.0.2/README.md
+-rw-r--r--   0        0        0      753 2024-05-30 12:55:02.434794 airbyte_source_freshsales-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-30 09:46:12.000000 airbyte_source_freshsales-1.0.2/source_freshsales/__init__.py
+-rw-r--r--   0        0        0    47946 2024-05-30 09:46:12.000000 airbyte_source_freshsales-1.0.2/source_freshsales/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-30 09:46:12.000000 airbyte_source_freshsales-1.0.2/source_freshsales/run.py
+-rw-r--r--   0        0        0      479 2024-05-30 09:46:12.000000 airbyte_source_freshsales-1.0.2/source_freshsales/source.py
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 airbyte_source_freshsales-1.0.2/PKG-INFO
```

### Comparing `airbyte_source_freshsales-1.0.1/README.md` & `airbyte_source_freshsales-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,88 @@
-# Freshsales Source
+# Freshsales source connector
 
-This is the repository for the Freshsales configuration based source connector.
+
+This is the repository for the Freshsales source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/freshsales).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/freshsales)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_freshsales/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_freshsales/spec.yaml` file.
+
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
-
 ```
 poetry run source-freshsales spec
 poetry run source-freshsales check --config secrets/config.json
 poetry run source-freshsales discover --config secrets/config.json
-poetry run source-freshsales read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-freshsales read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-freshsales build
 ```
 
 An image will be available on your host with the tag `airbyte/source-freshsales:dev`.
 
 
 ### Running as a docker container
-
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-freshsales:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-freshsales:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
-
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-freshsales test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-freshsales test`
 2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
     - bump the `dockerImageTag` value in in `metadata.yaml`
     - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/freshsales.md`).
```

### Comparing `airbyte_source_freshsales-1.0.1/pyproject.toml` & `airbyte_source_freshsales-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.0.1"
+version = "1.0.2"
 name = "airbyte-source-freshsales"
 description = "Source implementation for freshsales."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://docs.airbyte.com/integrations/sources/freshsales"
 homepage = "https://airbyte.com"
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_freshsales" },
-    { include = "main.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "1.0.0"
 
 [tool.poetry.scripts]
 source-freshsales = "source_freshsales.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "*"
 pytest-mock = "*"
```

### Comparing `airbyte_source_freshsales-1.0.1/source_freshsales/manifest.yaml` & `airbyte_source_freshsales-1.0.2/source_freshsales/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshsales-1.0.1/PKG-INFO` & `airbyte_source_freshsales-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,118 +1,107 @@
 Metadata-Version: 2.1
 Name: airbyte-source-freshsales
-Version: 1.0.1
+Version: 1.0.2
 Summary: Source implementation for freshsales.
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
+Requires-Dist: airbyte-cdk (==1.0.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/freshsales
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
-# Freshsales Source
+# Freshsales source connector
 
-This is the repository for the Freshsales configuration based source connector.
+
+This is the repository for the Freshsales source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/freshsales).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/freshsales)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_freshsales/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_freshsales/spec.yaml` file.
+
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
-
 ```
 poetry run source-freshsales spec
 poetry run source-freshsales check --config secrets/config.json
 poetry run source-freshsales discover --config secrets/config.json
-poetry run source-freshsales read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-freshsales read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-freshsales build
 ```
 
 An image will be available on your host with the tag `airbyte/source-freshsales:dev`.
 
 
 ### Running as a docker container
-
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-freshsales:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-freshsales:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
-
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-freshsales test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-freshsales test`
 2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
     - bump the `dockerImageTag` value in in `metadata.yaml`
     - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/freshsales.md`).
```

