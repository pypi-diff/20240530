# Comparing `tmp/airbyte-source-workramp-0.1.0.tar.gz` & `tmp/airbyte_source_workramp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-workramp-0.1.0.tar", last modified: Thu Feb  1 09:46:35 2024, max compression
+gzip compressed data, was "airbyte_source_workramp-0.1.1.tar", max compression
```

## Comparing `airbyte-source-workramp-0.1.0.tar` & `airbyte_source_workramp-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:46:35.945911 airbyte-source-workramp-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4204 2024-02-01 09:46:35.945911 airbyte-source-workramp-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4025 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:46:35.945911 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4204 2024-02-01 09:46:35.000000 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      916 2024-02-01 09:46:35.000000 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 09:46:35.000000 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-02-01 09:46:35.000000 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-01 09:46:35.000000 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-02-01 09:46:35.000000 airbyte-source-workramp-0.1.0/airbyte_source_workramp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:46:35.941911 airbyte-source-workramp-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1380 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       65 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/integration_tests/simple_catalog.json
--rw-r--r--   0 root         (0) root         (0)     4066 2024-02-01 09:46:35.945911 airbyte-source-workramp-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      927 2024-02-01 09:46:34.000000 airbyte-source-workramp-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:46:35.945911 airbyte-source-workramp-0.1.0/source_workramp/
--rw-r--r--   0 root         (0) root         (0)      128 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:46:35.945911 airbyte-source-workramp-0.1.0/source_workramp/schemas/
--rw-r--r--   0 root         (0) root         (0)      504 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/schemas/awarded_certifications.json
--rw-r--r--   0 root         (0) root         (0)      488 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/schemas/certifications.json
--rw-r--r--   0 root         (0) root         (0)      153 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/schemas/paths_users.json
--rw-r--r--   0 root         (0) root         (0)      750 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/schemas/registrations.json
--rw-r--r--   0 root         (0) root         (0)      321 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/schemas/trainings.json
--rw-r--r--   0 root         (0) root         (0)      587 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      477 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/source.py
--rw-r--r--   0 root         (0) root         (0)      501 2024-02-01 09:38:30.000000 airbyte-source-workramp-0.1.0/source_workramp/spec.yaml
+-rw-r--r--   0        0        0     4532 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/README.md
+-rw-r--r--   0        0        0      754 2024-05-30 01:45:24.773543 airbyte_source_workramp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/__init__.py
+-rw-r--r--   0        0        0     2101 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/run.py
+-rw-r--r--   0        0        0      504 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/schemas/awarded_certifications.json
+-rw-r--r--   0        0        0      488 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/schemas/certifications.json
+-rw-r--r--   0        0        0      153 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/schemas/paths_users.json
+-rw-r--r--   0        0        0      750 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/schemas/registrations.json
+-rw-r--r--   0        0        0      321 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/schemas/trainings.json
+-rw-r--r--   0        0        0      587 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/schemas/users.json
+-rw-r--r--   0        0        0      477 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/source.py
+-rw-r--r--   0        0        0      501 2024-05-30 01:30:33.000000 airbyte_source_workramp-0.1.1/source_workramp/spec.yaml
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 airbyte_source_workramp-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-workramp-0.1.0/PKG-INFO` & `airbyte_source_workramp-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-workramp
-Version: 0.1.0
-Summary: Source implementation for Workramp.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Workramp source connector
 
-# Workramp Source
 
-This is the repository for the Workramp configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/workramp).
+This is the repository for the Workramp source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/workramp).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/workramp)
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/workramp)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_workramp/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source workramp test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-workramp spec
+poetry run source-workramp check --config secrets/config.json
+poetry run source-workramp discover --config secrets/config.json
+poetry run source-workramp read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-workramp build
 ```
 
-An image will be built with the tag `airbyte/source-workramp:dev`.
+An image will be available on your host with the tag `airbyte/source-workramp:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-workramp:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-workramp:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-workramp:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-workramp:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-workramp:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-workramp test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-workramp test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/workramp.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/workramp.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-workramp-0.1.0/README.md` & `airbyte_source_workramp-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,110 @@
-# Workramp Source
+Metadata-Version: 2.1
+Name: airbyte-source-workramp
+Version: 0.1.1
+Summary: Source implementation for Workramp.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==1.0.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/workramp
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
-This is the repository for the Workramp configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/workramp).
+# Workramp source connector
+
+
+This is the repository for the Workramp source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/workramp).
 
 ## Local development
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/workramp)
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/workramp)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_workramp/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source workramp test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-workramp spec
+poetry run source-workramp check --config secrets/config.json
+poetry run source-workramp discover --config secrets/config.json
+poetry run source-workramp read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-workramp build
 ```
 
-An image will be built with the tag `airbyte/source-workramp:dev`.
+An image will be available on your host with the tag `airbyte/source-workramp:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-workramp:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-workramp:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-workramp:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-workramp:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-workramp:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-workramp test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
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
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-workramp test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/workramp.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/workramp.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-workramp-0.1.0/source_workramp/manifest.yaml` & `airbyte_source_workramp-0.1.1/source_workramp/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-workramp-0.1.0/source_workramp/schemas/registrations.json` & `airbyte_source_workramp-0.1.1/source_workramp/schemas/registrations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-workramp-0.1.0/source_workramp/schemas/users.json` & `airbyte_source_workramp-0.1.1/source_workramp/schemas/users.json`

 * *Files identical despite different names*

