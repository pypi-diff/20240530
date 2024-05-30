# Comparing `tmp/airbyte-source-bigcommerce-0.2.0.tar.gz` & `tmp/airbyte_source_bigcommerce-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-bigcommerce-0.2.0.tar", last modified: Tue Jan 30 14:48:18 2024, max compression
+gzip compressed data, was "airbyte_source_bigcommerce-0.2.1.tar", max compression
```

## Comparing `airbyte-source-bigcommerce-0.2.0.tar` & `airbyte_source_bigcommerce-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:48:18.196337 airbyte-source-bigcommerce-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4260 2024-01-30 14:48:18.196337 airbyte-source-bigcommerce-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4075 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:48:18.192337 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4260 2024-01-30 14:48:18.000000 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1192 2024-01-30 14:48:18.000000 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 14:48:18.000000 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-30 14:48:18.000000 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-30 14:48:18.000000 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-01-30 14:48:18.000000 airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:48:18.192337 airbyte-source-bigcommerce-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1911 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     3548 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       97 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       97 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     1815 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4119 2024-01-30 14:48:18.196337 airbyte-source-bigcommerce-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      936 2024-01-30 14:48:16.000000 airbyte-source-bigcommerce-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:48:18.192337 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/
--rw-r--r--   0 root         (0) root         (0)      134 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1000 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/components.py
--rw-r--r--   0 root         (0) root         (0)     9716 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:48:18.192337 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/
--rw-r--r--   0 root         (0) root         (0)      812 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/brands.json
--rw-r--r--   0 root         (0) root         (0)     1275 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/categories.json
--rw-r--r--   0 root         (0) root         (0)      870 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/channels.json
--rw-r--r--   0 root         (0) root         (0)     4371 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/customers.json
--rw-r--r--   0 root         (0) root         (0)     3670 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/order_products.json
--rw-r--r--   0 root         (0) root         (0)     6000 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/orders.json
--rw-r--r--   0 root         (0) root         (0)     1223 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/pages.json
--rw-r--r--   0 root         (0) root         (0)    21299 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/products.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:48:18.192337 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/shared/
--rw-r--r--   0 root         (0) root         (0)      727 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/shared/meta.json
--rw-r--r--   0 root         (0) root         (0)     4079 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/store.json
--rw-r--r--   0 root         (0) root         (0)     3042 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/transactions.json
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-30 14:29:13.000000 airbyte-source-bigcommerce-0.2.0/source_bigcommerce/source.py
+-rw-r--r--   0        0        0     4586 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/README.md
+-rw-r--r--   0        0        0      772 2024-05-30 14:07:41.143517 airbyte_source_bigcommerce-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/__init__.py
+-rw-r--r--   0        0        0     1000 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/components.py
+-rw-r--r--   0        0        0     9716 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/manifest.yaml
+-rw-r--r--   0        0        0      245 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/run.py
+-rw-r--r--   0        0        0      812 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/brands.json
+-rw-r--r--   0        0        0     1275 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/categories.json
+-rw-r--r--   0        0        0      870 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/channels.json
+-rw-r--r--   0        0        0     4371 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/customers.json
+-rw-r--r--   0        0        0     3670 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/order_products.json
+-rw-r--r--   0        0        0     6000 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/orders.json
+-rw-r--r--   0        0        0     1223 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/pages.json
+-rw-r--r--   0        0        0    21299 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/products.json
+-rw-r--r--   0        0        0      727 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/shared/meta.json
+-rw-r--r--   0        0        0     4079 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/store.json
+-rw-r--r--   0        0        0     3042 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/transactions.json
+-rw-r--r--   0        0        0      480 2024-05-30 13:53:52.000000 airbyte_source_bigcommerce-0.2.1/source_bigcommerce/source.py
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 airbyte_source_bigcommerce-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-bigcommerce-0.2.0/PKG-INFO` & `airbyte_source_bigcommerce-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-bigcommerce
-Version: 0.2.0
-Summary: Source implementation for Bigcommerce.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Bigcommerce source connector
 
-# Bigcommerce Source
 
-This is the repository for the Bigcommerce configuration based source connector.
+This is the repository for the Bigcommerce source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/bigcommerce).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/bigcommerce)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_bigcommerce/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source bigcommerce test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-bigcommerce spec
+poetry run source-bigcommerce check --config secrets/config.json
+poetry run source-bigcommerce discover --config secrets/config.json
+poetry run source-bigcommerce read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-bigcommerce build
 ```
 
-An image will be built with the tag `airbyte/source-bigcommerce:dev`.
+An image will be available on your host with the tag `airbyte/source-bigcommerce:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-bigcommerce:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-bigcommerce:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-bigcommerce:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-bigcommerce:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-bigcommerce:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-bigcommerce test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-bigcommerce test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/bigcommerce.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/bigcommerce.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-bigcommerce-0.2.0/airbyte_source_bigcommerce.egg-info/PKG-INFO` & `airbyte_source_bigcommerce-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-bigcommerce
-Version: 0.2.0
+Version: 0.2.1
 Summary: Source implementation for Bigcommerce.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/bigcommerce
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Bigcommerce Source
+# Bigcommerce source connector
 
-This is the repository for the Bigcommerce configuration based source connector.
+
+This is the repository for the Bigcommerce source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/bigcommerce).
 
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
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/bigcommerce)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_bigcommerce/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source bigcommerce test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-bigcommerce spec
+poetry run source-bigcommerce check --config secrets/config.json
+poetry run source-bigcommerce discover --config secrets/config.json
+poetry run source-bigcommerce read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-bigcommerce build
 ```
 
-An image will be built with the tag `airbyte/source-bigcommerce:dev`.
+An image will be available on your host with the tag `airbyte/source-bigcommerce:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-bigcommerce:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-bigcommerce:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-bigcommerce:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-bigcommerce:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-bigcommerce:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-bigcommerce test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-bigcommerce test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/bigcommerce.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/bigcommerce.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/components.py` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/components.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/manifest.yaml` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/brands.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/brands.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/categories.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/categories.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/channels.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/channels.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/customers.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/order_products.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/order_products.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/orders.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/pages.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/products.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/shared/meta.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/shared/meta.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/store.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/store.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-bigcommerce-0.2.0/source_bigcommerce/schemas/transactions.json` & `airbyte_source_bigcommerce-0.2.1/source_bigcommerce/schemas/transactions.json`

 * *Files identical despite different names*

