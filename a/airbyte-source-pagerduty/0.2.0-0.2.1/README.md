# Comparing `tmp/airbyte-source-pagerduty-0.2.0.tar.gz` & `tmp/airbyte_source_pagerduty-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-pagerduty-0.2.0.tar", last modified: Wed Jan 31 15:49:23 2024, max compression
+gzip compressed data, was "airbyte_source_pagerduty-0.2.1.tar", max compression
```

## Comparing `airbyte-source-pagerduty-0.2.0.tar` & `airbyte_source_pagerduty-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:49:23.139324 airbyte-source-pagerduty-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4219 2024-01-31 15:49:23.139324 airbyte-source-pagerduty-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4043 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:49:23.139324 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4219 2024-01-31 15:49:23.000000 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      945 2024-01-31 15:49:23.000000 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 15:49:23.000000 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 15:49:23.000000 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-31 15:49:23.000000 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-01-31 15:49:23.000000 airbyte-source-pagerduty-0.2.0/airbyte_source_pagerduty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:49:23.135324 airbyte-source-pagerduty-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1356 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       25 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4085 2024-01-31 15:49:23.139324 airbyte-source-pagerduty-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      918 2024-01-31 15:49:20.000000 airbyte-source-pagerduty-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:49:23.135324 airbyte-source-pagerduty-0.2.0/source_pagerduty/
--rw-r--r--   0 root         (0) root         (0)      130 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      239 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:49:23.139324 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/
--rw-r--r--   0 root         (0) root         (0)     8873 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/incident_logs.json
--rw-r--r--   0 root         (0) root         (0)    14878 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/incidents.json
--rw-r--r--   0 root         (0) root         (0)      919 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/priorities.json
--rw-r--r--   0 root         (0) root         (0)     3287 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/services.json
--rw-r--r--   0 root         (0) root         (0)      678 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/teams.json
--rw-r--r--   0 root         (0) root         (0)     4050 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      478 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/source.py
--rw-r--r--   0 root         (0) root         (0)     2162 2024-01-31 15:33:11.000000 airbyte-source-pagerduty-0.2.0/source_pagerduty/spec.yaml
+-rw-r--r--   0        0        0     4550 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/README.md
+-rw-r--r--   0        0        0      760 2024-05-30 12:55:48.935533 airbyte_source_pagerduty-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/__init__.py
+-rw-r--r--   0        0        0     2583 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/run.py
+-rw-r--r--   0        0        0     8873 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/incident_logs.json
+-rw-r--r--   0        0        0    14878 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/incidents.json
+-rw-r--r--   0        0        0      919 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/priorities.json
+-rw-r--r--   0        0        0     3287 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/services.json
+-rw-r--r--   0        0        0      678 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/teams.json
+-rw-r--r--   0        0        0     4050 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/users.json
+-rw-r--r--   0        0        0      478 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/source.py
+-rw-r--r--   0        0        0     2162 2024-05-30 12:43:27.000000 airbyte_source_pagerduty-0.2.1/source_pagerduty/spec.yaml
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_pagerduty-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-pagerduty-0.2.0/PKG-INFO` & `airbyte_source_pagerduty-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-pagerduty
-Version: 0.2.0
-Summary: Source implementation for Pagerduty.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Pagerduty source connector
 
-# Pagerduty Source
 
-This is the repository for the Pagerduty configuration based source connector.
+This is the repository for the Pagerduty source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pagerduty).
 
+## Local development
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pagerduty)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pagerduty/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pagerduty test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-pagerduty spec
+poetry run source-pagerduty check --config secrets/config.json
+poetry run source-pagerduty discover --config secrets/config.json
+poetry run source-pagerduty read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-pagerduty build
 ```
 
-An image will be built with the tag `airbyte/source-pagerduty:dev`.
+An image will be available on your host with the tag `airbyte/source-pagerduty:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-pagerduty:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pagerduty:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pagerduty:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pagerduty:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pagerduty:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-pagerduty test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pagerduty test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pagerduty.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pagerduty.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-pagerduty-0.2.0/README.md` & `airbyte_source_pagerduty-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,110 @@
-# Pagerduty Source
+Metadata-Version: 2.1
+Name: airbyte-source-pagerduty
+Version: 0.2.1
+Summary: Source implementation for Pagerduty.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pagerduty
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
-This is the repository for the Pagerduty configuration based source connector.
+# Pagerduty source connector
+
+
+This is the repository for the Pagerduty source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pagerduty).
 
 ## Local development
 
-#### Create credentials
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pagerduty)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pagerduty/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pagerduty test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-pagerduty spec
+poetry run source-pagerduty check --config secrets/config.json
+poetry run source-pagerduty discover --config secrets/config.json
+poetry run source-pagerduty read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-pagerduty build
 ```
 
-An image will be built with the tag `airbyte/source-pagerduty:dev`.
+An image will be available on your host with the tag `airbyte/source-pagerduty:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-pagerduty:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pagerduty:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pagerduty:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pagerduty:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pagerduty:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-pagerduty test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pagerduty test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pagerduty.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pagerduty.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/manifest.yaml` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/incident_logs.json` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/incident_logs.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/incidents.json` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/incidents.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/priorities.json` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/priorities.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/services.json` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/services.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/teams.json` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/schemas/users.json` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pagerduty-0.2.0/source_pagerduty/spec.yaml` & `airbyte_source_pagerduty-0.2.1/source_pagerduty/spec.yaml`

 * *Files identical despite different names*

