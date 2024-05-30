# Comparing `tmp/airbyte-source-microsoft-dataverse-0.1.2.tar.gz` & `tmp/airbyte_source_microsoft_dataverse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-microsoft-dataverse-0.1.2.tar", last modified: Wed Jan 31 13:30:42 2024, max compression
+gzip compressed data, was "airbyte_source_microsoft_dataverse-0.1.3.tar", max compression
```

## Comparing `airbyte-source-microsoft-dataverse-0.1.2.tar` & `airbyte_source_microsoft_dataverse-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:30:42.732226 airbyte-source-microsoft-dataverse-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     5606 2024-01-31 13:30:42.732226 airbyte-source-microsoft-dataverse-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5571 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:30:42.728226 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5606 2024-01-31 13:30:42.000000 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1000 2024-01-31 13:30:42.000000 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 13:30:42.000000 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-01-31 13:30:42.000000 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 13:30:42.000000 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-31 13:30:42.000000 airbyte-source-microsoft-dataverse-0.1.2/airbyte_source_microsoft_dataverse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:30:42.728226 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       82 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      347 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      161 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      154 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       82 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5486 2024-01-31 13:30:42.732226 airbyte-source-microsoft-dataverse-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      960 2024-01-31 13:30:40.000000 airbyte-source-microsoft-dataverse-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:30:42.728226 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/
--rw-r--r--   0 root         (0) root         (0)      148 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/dataverse.py
--rw-r--r--   0 root         (0) root         (0)      267 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/run.py
--rw-r--r--   0 root         (0) root         (0)     4435 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/source.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/spec.yaml
--rw-r--r--   0 root         (0) root         (0)     6168 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:30:42.728226 airbyte-source-microsoft-dataverse-0.1.2/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      525 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/unit_tests/test_dataverse.py
--rw-r--r--   0 root         (0) root         (0)     3713 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)     5019 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     3716 2024-01-31 13:14:34.000000 airbyte-source-microsoft-dataverse-0.1.2/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4730 2024-05-30 01:28:52.933139 airbyte_source_microsoft_dataverse-0.1.3/README.md
+-rw-r--r--   0        0        0      821 2024-05-30 01:35:32.380409 airbyte_source_microsoft_dataverse-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-05-30 01:28:52.937139 airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-30 01:28:52.937139 airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/dataverse.py
+-rw-r--r--   0        0        0      267 2024-05-30 01:28:52.937139 airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/run.py
+-rw-r--r--   0        0        0     4435 2024-05-30 01:28:52.937139 airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/source.py
+-rw-r--r--   0        0        0     1147 2024-05-30 01:28:52.937139 airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/spec.yaml
+-rw-r--r--   0        0        0     6168 2024-05-30 01:28:52.937139 airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/streams.py
+-rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 airbyte_source_microsoft_dataverse-0.1.3/PKG-INFO
```

### Comparing `airbyte-source-microsoft-dataverse-0.1.2/PKG-INFO` & `airbyte_source_microsoft_dataverse-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-microsoft-dataverse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Source implementation for Microsoft Dataverse.
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
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/microsoft-dataverse
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.2
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Microsoft Dataverse Source
+# Microsoft-Dataverse source connector
 
-This is the repository for the Microsoft Dataverse source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/microsoft-dataverse).
 
+This is the repository for the Microsoft-Dataverse source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/microsoft-dataverse).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/microsoft-dataverse)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/microsoft-dataverse)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_microsoft_dataverse/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source microsoft-dataverse test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-microsoft-dataverse spec
+poetry run source-microsoft-dataverse check --config secrets/config.json
+poetry run source-microsoft-dataverse discover --config secrets/config.json
+poetry run source-microsoft-dataverse read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-microsoft-dataverse build
 ```
 
-An image will be built with the tag `airbyte/source-microsoft-dataverse:dev`.
+An image will be available on your host with the tag `airbyte/source-microsoft-dataverse:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-microsoft-dataverse:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-microsoft-dataverse:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-dataverse:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-dataverse:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-microsoft-dataverse:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-microsoft-dataverse test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-microsoft-dataverse test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/microsoft-dataverse.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/microsoft-dataverse.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-microsoft-dataverse-0.1.2/setup.cfg` & `airbyte_source_microsoft_dataverse-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,91 @@
-[metadata]
-name = airbyte-source-microsoft-dataverse
-version = 0.1.2
-author = Airbyte
-author_email = contact@airbyte.io
-long_description = # Microsoft Dataverse Source
-	
-	This is the repository for the Microsoft Dataverse source connector, written in Python.
-	For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/microsoft-dataverse).
-	
-	
-	**To iterate on this connector, make sure to complete this prerequisites section.**
-	
-	
-	From this connector directory, create a virtual environment:
-	```
-	python -m venv .venv
-	```
-	
-	This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-	development environment of choice. To activate it from the terminal, run:
-	```
-	source .venv/bin/activate
-	pip install -r requirements.txt
-	pip install '.[tests]'
-	```
-	If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
-	
-	Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-	used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-	If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-	should work as you expect.
-	
-	**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/microsoft-dataverse)
-	to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_microsoft_dataverse/spec.yaml` file.
-	Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-	See `integration_tests/sample_config.json` for a sample config file.
-	
-	**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source microsoft-dataverse test creds`
-	and place them into `secrets/config.json`.
-	
-	```
-	python main.py spec
-	python main.py check --config secrets/config.json
-	python main.py discover --config secrets/config.json
-	python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
-	```
-	
-	
-	
-	**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-	```bash
-	airbyte-ci connectors --name=source-microsoft-dataverse build
-	```
-	
-	An image will be built with the tag `airbyte/source-microsoft-dataverse:dev`.
-	
-	**Via `docker build`:**
-	```bash
-	docker build -t airbyte/source-microsoft-dataverse:dev .
-	```
-	
-	Then run any of the connector commands as follows:
-	```
-	docker run --rm airbyte/source-microsoft-dataverse:dev spec
-	docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-dataverse:dev check --config /secrets/config.json
-	docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-dataverse:dev discover --config /secrets/config.json
-	docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-microsoft-dataverse:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
-	```
-	
-	You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
-	```bash
-	airbyte-ci connectors --name=source-microsoft-dataverse test
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
-	1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-microsoft-dataverse test`
-	2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
-	3. Make sure the `metadata.yaml` content is up to date.
-	4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/microsoft-dataverse.md`).
-	5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
-	6. Pat yourself on the back for being an awesome contributor.
-	7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-long_description_content_type = text/markdown
-
-[egg_info]
-tag_build = 
-tag_date = 0
+# Microsoft-Dataverse source connector
 
+
+This is the repository for the Microsoft-Dataverse source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/microsoft-dataverse).
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/microsoft-dataverse)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_microsoft_dataverse/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+```
+poetry run source-microsoft-dataverse spec
+poetry run source-microsoft-dataverse check --config secrets/config.json
+poetry run source-microsoft-dataverse discover --config secrets/config.json
+poetry run source-microsoft-dataverse read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
+airbyte-ci connectors --name=source-microsoft-dataverse build
+```
+
+An image will be available on your host with the tag `airbyte/source-microsoft-dataverse:dev`.
+
+
+### Running as a docker container
+Then run any of the connector commands as follows:
+```
+docker run --rm airbyte/source-microsoft-dataverse:dev spec
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-dataverse:dev check --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-dataverse:dev discover --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-microsoft-dataverse:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
+```
+
+### Running our CI test suite
+You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+```bash
+airbyte-ci connectors --name=source-microsoft-dataverse test
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
+1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-microsoft-dataverse test`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
+3. Make sure the `metadata.yaml` content is up to date.
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/microsoft-dataverse.md`).
+5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
+6. Pat yourself on the back for being an awesome contributor.
+7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/dataverse.py` & `airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/dataverse.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/source.py` & `airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/spec.yaml` & `airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-microsoft-dataverse-0.1.2/source_microsoft_dataverse/streams.py` & `airbyte_source_microsoft_dataverse-0.1.3/source_microsoft_dataverse/streams.py`

 * *Files identical despite different names*

