# Comparing `tmp/airbyte-source-salesloft-1.2.0.tar.gz` & `tmp/airbyte_source_salesloft-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-salesloft-1.2.0.tar", last modified: Wed Jan 31 18:09:28 2024, max compression
+gzip compressed data, was "airbyte_source_salesloft-1.2.1.tar", max compression
```

## Comparing `airbyte-source-salesloft-1.2.0.tar` & `airbyte_source_salesloft-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:09:28.283239 airbyte-source-salesloft-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     5415 2024-01-31 18:09:28.283239 airbyte-source-salesloft-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5388 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:09:28.283239 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5415 2024-01-31 18:09:28.000000 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1664 2024-01-31 18:09:28.000000 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 18:09:28.000000 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 18:09:28.000000 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       75 2024-01-31 18:09:28.000000 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-01-31 18:09:28.000000 airbyte-source-salesloft-1.2.0/airbyte_source_salesloft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5292 2024-01-31 18:09:28.283239 airbyte-source-salesloft-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      923 2024-01-31 18:09:26.000000 airbyte-source-salesloft-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:09:28.275239 airbyte-source-salesloft-1.2.0/source_salesloft/
--rw-r--r--   0 root         (0) root         (0)      130 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/__init__.py
--rw-r--r--   0 root         (0) root         (0)      239 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:09:28.283239 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/
--rw-r--r--   0 root         (0) root         (0)      432 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/account_stages.json
--rw-r--r--   0 root         (0) root         (0)      422 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/account_tiers.json
--rw-r--r--   0 root         (0) root         (0)     3841 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/accounts.json
--rw-r--r--   0 root         (0) root         (0)     1896 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/actions.json
--rw-r--r--   0 root         (0) root         (0)     2151 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/cadence_memberships.json
--rw-r--r--   0 root         (0) root         (0)     2822 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/cadences.json
--rw-r--r--   0 root         (0) root         (0)     1863 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/call_data_records.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/call_dispositions.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/call_sentiments.json
--rw-r--r--   0 root         (0) root         (0)     2252 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/calls.json
--rw-r--r--   0 root         (0) root         (0)     1167 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/crm_activities.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/crm_users.json
--rw-r--r--   0 root         (0) root         (0)      538 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/custom_fields.json
--rw-r--r--   0 root         (0) root         (0)      656 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/email_template_attachments.json
--rw-r--r--   0 root         (0) root         (0)     2616 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/email_templates.json
--rw-r--r--   0 root         (0) root         (0)     3872 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/emails.json
--rw-r--r--   0 root         (0) root         (0)      258 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/groups.json
--rw-r--r--   0 root         (0) root         (0)      509 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/import.json
--rw-r--r--   0 root         (0) root         (0)     4180 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/meetings.json
--rw-r--r--   0 root         (0) root         (0)     1126 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/notes.json
--rw-r--r--   0 root         (0) root         (0)     5588 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/people.json
--rw-r--r--   0 root         (0) root         (0)      422 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/person_stages.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/phone_number_assignments.json
--rw-r--r--   0 root         (0) root         (0)     2804 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/searches.json
--rw-r--r--   0 root         (0) root         (0)     1177 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/steps.json
--rw-r--r--   0 root         (0) root         (0)     2590 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/successes.json
--rw-r--r--   0 root         (0) root         (0)      655 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/team_template_attachments.json
--rw-r--r--   0 root         (0) root         (0)     2019 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/team_templates.json
--rw-r--r--   0 root         (0) root         (0)     3235 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)     9550 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/source.py
--rw-r--r--   0 root         (0) root         (0)     3217 2024-01-31 17:51:56.000000 airbyte-source-salesloft-1.2.0/source_salesloft/spec.json
+-rw-r--r--   0        0        0     4550 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/README.md
+-rw-r--r--   0        0        0      783 2024-05-30 02:03:43.443510 airbyte_source_salesloft-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/__init__.py
+-rw-r--r--   0        0        0      239 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/run.py
+-rw-r--r--   0        0        0      432 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/account_stages.json
+-rw-r--r--   0        0        0      422 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/account_tiers.json
+-rw-r--r--   0        0        0     3841 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/accounts.json
+-rw-r--r--   0        0        0     1896 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/actions.json
+-rw-r--r--   0        0        0     2151 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/cadence_memberships.json
+-rw-r--r--   0        0        0     2822 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/cadences.json
+-rw-r--r--   0        0        0     1863 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/call_data_records.json
+-rw-r--r--   0        0        0      418 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/call_dispositions.json
+-rw-r--r--   0        0        0      418 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/call_sentiments.json
+-rw-r--r--   0        0        0     2252 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/calls.json
+-rw-r--r--   0        0        0     1167 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/crm_activities.json
+-rw-r--r--   0        0        0      620 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/crm_users.json
+-rw-r--r--   0        0        0      538 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/custom_fields.json
+-rw-r--r--   0        0        0      656 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/email_template_attachments.json
+-rw-r--r--   0        0        0     2616 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/email_templates.json
+-rw-r--r--   0        0        0     3872 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/emails.json
+-rw-r--r--   0        0        0      258 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/groups.json
+-rw-r--r--   0        0        0      509 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/import.json
+-rw-r--r--   0        0        0     4180 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/meetings.json
+-rw-r--r--   0        0        0     1126 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/notes.json
+-rw-r--r--   0        0        0     5588 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/people.json
+-rw-r--r--   0        0        0      422 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/person_stages.json
+-rw-r--r--   0        0        0      452 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/phone_number_assignments.json
+-rw-r--r--   0        0        0     2804 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/searches.json
+-rw-r--r--   0        0        0     1177 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/steps.json
+-rw-r--r--   0        0        0     2590 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/successes.json
+-rw-r--r--   0        0        0      655 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/team_template_attachments.json
+-rw-r--r--   0        0        0     2019 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/team_templates.json
+-rw-r--r--   0        0        0     3235 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/schemas/users.json
+-rw-r--r--   0        0        0     9550 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/source.py
+-rw-r--r--   0        0        0     3217 2024-05-30 01:47:37.000000 airbyte_source_salesloft-1.2.1/source_salesloft/spec.json
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 airbyte_source_salesloft-1.2.1/PKG-INFO
```

### Comparing `airbyte-source-salesloft-1.2.0/PKG-INFO` & `airbyte_source_salesloft-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,111 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesloft
-Version: 1.2.0
+Version: 1.2.1
 Summary: Source implementation for Salesloft.
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
+Requires-Dist: airbyte-cdk (==0.83.0)
+Requires-Dist: pendulum (==2.1.2)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/salesloft
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Requires-Dist: pendulum
-Provides-Extra: tests
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: requests-mock; extra == "tests"
 
-# Salesloft Source
+# Salesloft source connector
 
-This is the repository for the Salesloft source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/salesloft).
 
+This is the repository for the Salesloft source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/salesloft).
 
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
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/salesloft)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_salesloft/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/salesloft)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_salesloft/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source salesloft test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-salesloft spec
+poetry run source-salesloft check --config secrets/config.json
+poetry run source-salesloft discover --config secrets/config.json
+poetry run source-salesloft read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-salesloft build
 ```
 
-An image will be built with the tag `airbyte/source-salesloft:dev`.
+An image will be available on your host with the tag `airbyte/source-salesloft:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-salesloft:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-salesloft:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-salesloft:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-salesloft:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-salesloft:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-salesloft test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-salesloft test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/salesloft.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/salesloft.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/accounts.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/actions.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/actions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/cadence_memberships.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/cadence_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/cadences.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/cadences.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/call_data_records.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/call_data_records.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/calls.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/calls.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/crm_activities.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/crm_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/crm_users.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/crm_users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/custom_fields.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/custom_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/email_template_attachments.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/email_template_attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/email_templates.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/email_templates.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/emails.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/emails.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/meetings.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/meetings.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/notes.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/notes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/people.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/people.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/searches.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/searches.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/steps.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/steps.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/successes.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/successes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/team_template_attachments.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/team_template_attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/team_templates.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/team_templates.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/schemas/users.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/source.py` & `airbyte_source_salesloft-1.2.1/source_salesloft/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-salesloft-1.2.0/source_salesloft/spec.json` & `airbyte_source_salesloft-1.2.1/source_salesloft/spec.json`

 * *Files identical despite different names*

