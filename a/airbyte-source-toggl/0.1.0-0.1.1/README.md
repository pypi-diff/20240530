# Comparing `tmp/airbyte-source-toggl-0.1.0.tar.gz` & `tmp/airbyte_source_toggl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-toggl-0.1.0.tar", last modified: Thu Feb  1 08:03:50 2024, max compression
+gzip compressed data, was "airbyte_source_toggl-0.1.1.tar", max compression
```

## Comparing `airbyte-source-toggl-0.1.0.tar` & `airbyte_source_toggl-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:03:50.738335 airbyte-source-toggl-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4150 2024-02-01 08:03:50.738335 airbyte-source-toggl-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3977 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:03:50.738335 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4150 2024-02-01 08:03:50.000000 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1004 2024-02-01 08:03:50.000000 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 08:03:50.000000 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-02-01 08:03:50.000000 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-01 08:03:50.000000 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-02-01 08:03:50.000000 airbyte-source-toggl-0.1.0/airbyte_source_toggl.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:03:50.734334 airbyte-source-toggl-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1857 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       40 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      169 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4015 2024-02-01 08:03:50.738335 airbyte-source-toggl-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      918 2024-02-01 08:03:48.000000 airbyte-source-toggl-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:03:50.734334 airbyte-source-toggl-0.1.0/source_toggl/
--rw-r--r--   0 root         (0) root         (0)      122 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3247 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      227 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:03:50.738335 airbyte-source-toggl-0.1.0/source_toggl/schemas/
--rw-r--r--   0 root         (0) root         (0)      938 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/organizations.json
--rw-r--r--   0 root         (0) root         (0)      339 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/organizations_groups.json
--rw-r--r--   0 root         (0) root         (0)      743 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/organizations_users.json
--rw-r--r--   0 root         (0) root         (0)     1054 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/time_entries.json
--rw-r--r--   0 root         (0) root         (0)      253 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/workspace.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/workspace_clients.json
--rw-r--r--   0 root         (0) root         (0)     1490 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/workspace_projects.json
--rw-r--r--   0 root         (0) root         (0)      680 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/schemas/workspace_tasks.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/source.py
--rw-r--r--   0 root         (0) root         (0)     1431 2024-02-01 07:53:30.000000 airbyte-source-toggl-0.1.0/source_toggl/spec.yaml
+-rw-r--r--   0        0        0     4478 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/README.md
+-rw-r--r--   0        0        0      736 2024-05-30 17:26:37.043427 airbyte_source_toggl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/__init__.py
+-rw-r--r--   0        0        0     3247 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/run.py
+-rw-r--r--   0        0        0      938 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/organizations.json
+-rw-r--r--   0        0        0      339 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/organizations_groups.json
+-rw-r--r--   0        0        0      743 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/organizations_users.json
+-rw-r--r--   0        0        0     1054 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/time_entries.json
+-rw-r--r--   0        0        0      253 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/workspace.json
+-rw-r--r--   0        0        0      380 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/workspace_clients.json
+-rw-r--r--   0        0        0     1490 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/workspace_projects.json
+-rw-r--r--   0        0        0      680 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/schemas/workspace_tasks.json
+-rw-r--r--   0        0        0      474 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/source.py
+-rw-r--r--   0        0        0     1431 2024-05-30 15:06:24.000000 airbyte_source_toggl-0.1.1/source_toggl/spec.yaml
+-rw-r--r--   0        0        0     5178 1970-01-01 00:00:00.000000 airbyte_source_toggl-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-toggl-0.1.0/PKG-INFO` & `airbyte_source_toggl-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-toggl
-Version: 0.1.0
-Summary: Source implementation for Toggl.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Toggl source connector
 
-# Toggl Source
 
-This is the repository for the Toggl configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/toggl).
+This is the repository for the Toggl source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/toggl).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/toggl)
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/toggl)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_toggl/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source toggl test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-toggl spec
+poetry run source-toggl check --config secrets/config.json
+poetry run source-toggl discover --config secrets/config.json
+poetry run source-toggl read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-toggl build
 ```
 
-An image will be built with the tag `airbyte/source-toggl:dev`.
+An image will be available on your host with the tag `airbyte/source-toggl:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-toggl:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-toggl:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-toggl:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-toggl:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-toggl:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-toggl test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-toggl test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/toggl.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/toggl.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-toggl-0.1.0/setup.cfg` & `airbyte_source_toggl-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,110 @@
-[metadata]
-name = airbyte-source-toggl
-version = 0.1.0
-author = Airbyte
-author_email = contact@airbyte.io
-long_description = # Toggl Source
-	
-	This is the repository for the Toggl configuration based source connector.
-	For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/toggl).
-	
-	
-	**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/toggl)
-	to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_toggl/spec.yaml` file.
-	Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-	See `integration_tests/sample_config.json` for a sample config file.
-	
-	**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source toggl test creds`
-	and place them into `secrets/config.json`.
-	
-	
-	
-	**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-	```bash
-	airbyte-ci connectors --name=source-toggl build
-	```
-	
-	An image will be built with the tag `airbyte/source-toggl:dev`.
-	
-	**Via `docker build`:**
-	```bash
-	docker build -t airbyte/source-toggl:dev .
-	```
-	
-	Then run any of the connector commands as follows:
-	```
-	docker run --rm airbyte/source-toggl:dev spec
-	docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-toggl:dev check --config /secrets/config.json
-	docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-toggl:dev discover --config /secrets/config.json
-	docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-toggl:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
-	```
-	
-	You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
-	```bash
-	airbyte-ci connectors --name=source-toggl test
-	```
-	
-	Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
-	If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
-	
-	All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-	We split dependencies between two groups, dependencies that are:
-	* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-	* required for the testing need to go to `TEST_REQUIREMENTS` list
-	
-	You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
-	1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-toggl test`
-	2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
-	3. Make sure the `metadata.yaml` content is up to date.
-	4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/toggl.md`).
-	5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
-	6. Pat yourself on the back for being an awesome contributor.
-	7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-long_description_content_type = text/markdown
-
-[egg_info]
-tag_build = 
-tag_date = 0
+Metadata-Version: 2.1
+Name: airbyte-source-toggl
+Version: 0.1.1
+Summary: Source implementation for Toggl.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/toggl
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
+# Toggl source connector
+
+
+This is the repository for the Toggl source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/toggl).
+
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/toggl)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_toggl/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+```
+poetry run source-toggl spec
+poetry run source-toggl check --config secrets/config.json
+poetry run source-toggl discover --config secrets/config.json
+poetry run source-toggl read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
+
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
+
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
+```bash
+airbyte-ci connectors --name=source-toggl build
+```
+
+An image will be available on your host with the tag `airbyte/source-toggl:dev`.
+
+
+### Running as a docker container
+Then run any of the connector commands as follows:
+```
+docker run --rm airbyte/source-toggl:dev spec
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-toggl:dev check --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-toggl:dev discover --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-toggl:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
+```
+
+### Running our CI test suite
+You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+```bash
+airbyte-ci connectors --name=source-toggl test
+```
+
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
+
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
+You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-toggl test`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
+3. Make sure the `metadata.yaml` content is up to date.
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/toggl.md`).
+5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
+6. Pat yourself on the back for being an awesome contributor.
+7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/manifest.yaml` & `airbyte_source_toggl-0.1.1/source_toggl/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/schemas/organizations.json` & `airbyte_source_toggl-0.1.1/source_toggl/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/schemas/organizations_users.json` & `airbyte_source_toggl-0.1.1/source_toggl/schemas/organizations_users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/schemas/time_entries.json` & `airbyte_source_toggl-0.1.1/source_toggl/schemas/time_entries.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/schemas/workspace_projects.json` & `airbyte_source_toggl-0.1.1/source_toggl/schemas/workspace_projects.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/schemas/workspace_tasks.json` & `airbyte_source_toggl-0.1.1/source_toggl/schemas/workspace_tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-toggl-0.1.0/source_toggl/spec.yaml` & `airbyte_source_toggl-0.1.1/source_toggl/spec.yaml`

 * *Files identical despite different names*

