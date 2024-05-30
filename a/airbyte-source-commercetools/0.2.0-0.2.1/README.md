# Comparing `tmp/airbyte-source-commercetools-0.2.0.tar.gz` & `tmp/airbyte_source_commercetools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-commercetools-0.2.0.tar", last modified: Wed Jan 31 01:06:11 2024, max compression
+gzip compressed data, was "airbyte_source_commercetools-0.2.1.tar", max compression
```

## Comparing `airbyte-source-commercetools-0.2.0.tar` & `airbyte_source_commercetools-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:06:11.084424 airbyte-source-commercetools-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4296 2024-01-31 01:06:11.084424 airbyte-source-commercetools-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4107 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:06:11.084424 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4296 2024-01-31 01:06:11.000000 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2046 2024-01-31 01:06:11.000000 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 01:06:11.000000 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-01-31 01:06:11.000000 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 01:06:11.000000 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-01-31 01:06:11.000000 airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:06:11.072424 airbyte-source-commercetools-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1857 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      168 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      168 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4153 2024-01-31 01:06:11.084424 airbyte-source-commercetools-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      920 2024-01-31 01:06:09.000000 airbyte-source-commercetools-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:06:11.076424 airbyte-source-commercetools-0.2.0/source_commercetools/
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/components.py
--rw-r--r--   0 root         (0) root         (0)     4617 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      251 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:06:11.076424 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/
--rw-r--r--   0 root         (0) root         (0)     2354 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/customers.json
--rw-r--r--   0 root         (0) root         (0)     2001 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/discount_codes.json
--rw-r--r--   0 root         (0) root         (0)    13199 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/orders.json
--rw-r--r--   0 root         (0) root         (0)     2344 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/payments.json
--rw-r--r--   0 root         (0) root         (0)     1947 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/products.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:06:11.080423 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/
--rw-r--r--   0 root         (0) root         (0)     1578 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/address.json
--rw-r--r--   0 root         (0) root         (0)      316 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/created_by.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/custom.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/dimension.json
--rw-r--r--   0 root         (0) root         (0)      647 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/discounted_price_per_quantity.json
--rw-r--r--   0 root         (0) root         (0)      109 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/field_type.json
--rw-r--r--   0 root         (0) root         (0)      164 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/key_reference.json
--rw-r--r--   0 root         (0) root         (0)      284 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/last_modified_by.json
--rw-r--r--   0 root         (0) root         (0)      109 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/localized_string.json
--rw-r--r--   0 root         (0) root         (0)      295 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/money.json
--rw-r--r--   0 root         (0) root         (0)     1076 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/price.json
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/price_scoped.json
--rw-r--r--   0 root         (0) root         (0)     1053 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/product_data.json
--rw-r--r--   0 root         (0) root         (0)     2990 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/product_variant.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/reference.json
--rw-r--r--   0 root         (0) root         (0)      416 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/shipping_details.json
--rw-r--r--   0 root         (0) root         (0)      166 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/state.json
--rw-r--r--   0 root         (0) root         (0)      161 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/taxed_item_price.json
--rw-r--r--   0 root         (0) root         (0)      528 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/taxed_price.json
--rw-r--r--   0 root         (0) root         (0)      693 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/taxrate.json
--rw-r--r--   0 root         (0) root         (0)      482 2024-01-31 00:49:03.000000 airbyte-source-commercetools-0.2.0/source_commercetools/source.py
+-rw-r--r--   0        0        0     4622 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/README.md
+-rw-r--r--   0        0        0      784 2024-05-30 14:08:39.567190 airbyte_source_commercetools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/__init__.py
+-rw-r--r--   0        0        0     1585 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/components.py
+-rw-r--r--   0        0        0     4617 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/manifest.yaml
+-rw-r--r--   0        0        0      251 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/run.py
+-rw-r--r--   0        0        0     2354 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/customers.json
+-rw-r--r--   0        0        0     2001 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/discount_codes.json
+-rw-r--r--   0        0        0    13199 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/orders.json
+-rw-r--r--   0        0        0     2344 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/payments.json
+-rw-r--r--   0        0        0     1947 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/products.json
+-rw-r--r--   0        0        0     1578 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/address.json
+-rw-r--r--   0        0        0      316 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/created_by.json
+-rw-r--r--   0        0        0      606 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/custom.json
+-rw-r--r--   0        0        0      157 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/dimension.json
+-rw-r--r--   0        0        0      647 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/discounted_price_per_quantity.json
+-rw-r--r--   0        0        0      109 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/field_type.json
+-rw-r--r--   0        0        0      164 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/key_reference.json
+-rw-r--r--   0        0        0      284 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/last_modified_by.json
+-rw-r--r--   0        0        0      109 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/localized_string.json
+-rw-r--r--   0        0        0      295 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/money.json
+-rw-r--r--   0        0        0     1076 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/price.json
+-rw-r--r--   0        0        0      844 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/price_scoped.json
+-rw-r--r--   0        0        0     1053 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/product_data.json
+-rw-r--r--   0        0        0     2990 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/product_variant.json
+-rw-r--r--   0        0        0      378 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/reference.json
+-rw-r--r--   0        0        0      416 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/shipping_details.json
+-rw-r--r--   0        0        0      166 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/state.json
+-rw-r--r--   0        0        0      161 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/taxed_item_price.json
+-rw-r--r--   0        0        0      528 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/taxed_price.json
+-rw-r--r--   0        0        0      693 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/taxrate.json
+-rw-r--r--   0        0        0      482 2024-05-30 13:47:38.000000 airbyte_source_commercetools-0.2.1/source_commercetools/source.py
+-rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 airbyte_source_commercetools-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-commercetools-0.2.0/PKG-INFO` & `airbyte_source_commercetools-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-commercetools
-Version: 0.2.0
-Summary: Source implementation for Commercetools.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Commercetools source connector
 
-# Commercetools Source
 
-This is the repository for the Commercetools configuration based source connector.
+This is the repository for the Commercetools source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/commercetools).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/commercetools)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_commercetools/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source commercetools test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-commercetools spec
+poetry run source-commercetools check --config secrets/config.json
+poetry run source-commercetools discover --config secrets/config.json
+poetry run source-commercetools read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-commercetools build
 ```
 
-An image will be built with the tag `airbyte/source-commercetools:dev`.
+An image will be available on your host with the tag `airbyte/source-commercetools:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-commercetools:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-commercetools:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-commercetools:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-commercetools:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-commercetools:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-commercetools test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-commercetools test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/commercetools.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/commercetools.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-commercetools-0.2.0/airbyte_source_commercetools.egg-info/PKG-INFO` & `airbyte_source_commercetools-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-commercetools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Source implementation for Commercetools.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/commercetools
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Commercetools Source
+# Commercetools source connector
 
-This is the repository for the Commercetools configuration based source connector.
+
+This is the repository for the Commercetools source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/commercetools).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/commercetools)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_commercetools/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source commercetools test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-commercetools spec
+poetry run source-commercetools check --config secrets/config.json
+poetry run source-commercetools discover --config secrets/config.json
+poetry run source-commercetools read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-commercetools build
 ```
 
-An image will be built with the tag `airbyte/source-commercetools:dev`.
+An image will be available on your host with the tag `airbyte/source-commercetools:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-commercetools:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-commercetools:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-commercetools:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-commercetools:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-commercetools:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-commercetools test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-commercetools test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/commercetools.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/commercetools.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/components.py` & `airbyte_source_commercetools-0.2.1/source_commercetools/components.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/manifest.yaml` & `airbyte_source_commercetools-0.2.1/source_commercetools/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/customers.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/discount_codes.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/orders.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/payments.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/payments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/products.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/address.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/address.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/custom.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/custom.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/discounted_price_per_quantity.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/discounted_price_per_quantity.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/price.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/price.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/price_scoped.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/price_scoped.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/product_data.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/product_data.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/product_variant.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/product_variant.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/taxed_price.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/taxed_price.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-commercetools-0.2.0/source_commercetools/schemas/shared/taxrate.json` & `airbyte_source_commercetools-0.2.1/source_commercetools/schemas/shared/taxrate.json`

 * *Files identical despite different names*

