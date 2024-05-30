# Comparing `tmp/airbyte-source-secoda-0.1.0.tar.gz` & `tmp/airbyte_source_secoda-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-secoda-0.1.0.tar", last modified: Wed Jan 31 18:06:49 2024, max compression
+gzip compressed data, was "airbyte_source_secoda-0.1.1.tar", max compression
```

## Comparing `airbyte-source-secoda-0.1.0.tar` & `airbyte_source_secoda-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4168 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3993 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4168 2024-01-31 18:06:49.000000 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      782 2024-01-31 18:06:49.000000 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 18:06:49.000000 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-31 18:06:49.000000 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 18:06:49.000000 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-31 18:06:49.000000 airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      686 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       33 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4032 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      921 2024-01-31 18:06:47.000000 airbyte-source-secoda-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/source_secoda/
--rw-r--r--   0 root         (0) root         (0)      124 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:06:49.471565 airbyte-source-secoda-0.1.0/source_secoda/schemas/
--rw-r--r--   0 root         (0) root         (0)      684 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/schemas/collections.json
--rw-r--r--   0 root         (0) root         (0)     1010 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/schemas/tables.json
--rw-r--r--   0 root         (0) root         (0)      637 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/schemas/terms.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/source.py
--rw-r--r--   0 root         (0) root         (0)      660 2024-01-31 17:51:56.000000 airbyte-source-secoda-0.1.0/source_secoda/spec.yaml
+-rw-r--r--   0        0        0     4496 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/README.md
+-rw-r--r--   0        0        0      742 2024-05-30 17:05:54.339114 airbyte_source_secoda-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/__init__.py
+-rw-r--r--   0        0        0     1689 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/run.py
+-rw-r--r--   0        0        0      684 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/schemas/collections.json
+-rw-r--r--   0        0        0     1010 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/schemas/tables.json
+-rw-r--r--   0        0        0      637 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/schemas/terms.json
+-rw-r--r--   0        0        0      475 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/source.py
+-rw-r--r--   0        0        0      660 2024-05-30 14:44:42.000000 airbyte_source_secoda-0.1.1/source_secoda/spec.yaml
+-rw-r--r--   0        0        0     5199 1970-01-01 00:00:00.000000 airbyte_source_secoda-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-secoda-0.1.0/PKG-INFO` & `airbyte_source_secoda-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-secoda
-Version: 0.1.0
-Summary: Source implementation for Secoda.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Secoda source connector
 
-# Secoda Source
 
-This is the repository for the Secoda configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/secoda).
+This is the repository for the Secoda source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/secoda).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/secoda)
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/secoda)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_secoda/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source secoda test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-secoda spec
+poetry run source-secoda check --config secrets/config.json
+poetry run source-secoda discover --config secrets/config.json
+poetry run source-secoda read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-secoda build
 ```
 
-An image will be built with the tag `airbyte/source-secoda:dev`.
+An image will be available on your host with the tag `airbyte/source-secoda:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-secoda:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-secoda:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-secoda:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-secoda:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-secoda:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-secoda test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-secoda test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/secoda.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/secoda.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-secoda-0.1.0/airbyte_source_secoda.egg-info/PKG-INFO` & `airbyte_source_secoda-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-secoda
-Version: 0.1.0
+Version: 0.1.1
 Summary: Source implementation for Secoda.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==1.0.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/secoda
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Secoda Source
+# Secoda source connector
 
-This is the repository for the Secoda configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/secoda).
 
+This is the repository for the Secoda source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/secoda).
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/secoda)
+## Local development
+
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/secoda)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_secoda/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source secoda test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-secoda spec
+poetry run source-secoda check --config secrets/config.json
+poetry run source-secoda discover --config secrets/config.json
+poetry run source-secoda read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-secoda build
 ```
 
-An image will be built with the tag `airbyte/source-secoda:dev`.
+An image will be available on your host with the tag `airbyte/source-secoda:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-secoda:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-secoda:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-secoda:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-secoda:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-secoda:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-secoda test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-secoda test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/secoda.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/secoda.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-secoda-0.1.0/source_secoda/manifest.yaml` & `airbyte_source_secoda-0.1.1/source_secoda/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-secoda-0.1.0/source_secoda/schemas/collections.json` & `airbyte_source_secoda-0.1.1/source_secoda/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-secoda-0.1.0/source_secoda/schemas/tables.json` & `airbyte_source_secoda-0.1.1/source_secoda/schemas/tables.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-secoda-0.1.0/source_secoda/schemas/terms.json` & `airbyte_source_secoda-0.1.1/source_secoda/schemas/terms.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-secoda-0.1.0/source_secoda/spec.yaml` & `airbyte_source_secoda-0.1.1/source_secoda/spec.yaml`

 * *Files identical despite different names*

