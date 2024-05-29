# Comparing `tmp/airbyte-source-tmdb-0.1.0.tar.gz` & `tmp/airbyte_source_tmdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-tmdb-0.1.0.tar", last modified: Thu Feb  1 08:05:36 2024, max compression
+gzip compressed data, was "airbyte_source_tmdb-0.1.1.tar", max compression
```

## Comparing `airbyte-source-tmdb-0.1.0.tar` & `airbyte_source_tmdb-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:05:36.590790 airbyte-source-tmdb-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     5082 2024-02-01 08:05:36.590790 airbyte-source-tmdb-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5043 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:05:36.590790 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5082 2024-02-01 08:05:36.000000 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2028 2024-02-01 08:05:36.000000 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 08:05:36.000000 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-02-01 08:05:36.000000 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-01 08:05:36.000000 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-02-01 08:05:36.000000 airbyte-source-tmdb-0.1.0/airbyte_source_tmdb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:05:36.578790 airbyte-source-tmdb-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     7372 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      151 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      122 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4970 2024-02-01 08:05:36.590790 airbyte-source-tmdb-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      915 2024-02-01 08:05:34.000000 airbyte-source-tmdb-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:05:36.582790 airbyte-source-tmdb-0.1.0/source_tmdb/
--rw-r--r--   0 root         (0) root         (0)      120 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8437 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      224 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:05:36.590790 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/
--rw-r--r--   0 root         (0) root         (0)    20718 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/certification_movie.json
--rw-r--r--   0 root         (0) root         (0)    13634 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/certification_tv.json
--rw-r--r--   0 root         (0) root         (0)     1443 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/changes_movie.json
--rw-r--r--   0 root         (0) root         (0)     1443 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/changes_person.json
--rw-r--r--   0 root         (0) root         (0)     1441 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/changes_tv.json
--rw-r--r--   0 root         (0) root         (0)     1217 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_alternative_titles.json
--rw-r--r--   0 root         (0) root         (0)     2500 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_changes.json
--rw-r--r--   0 root         (0) root         (0)     5293 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_credits.json
--rw-r--r--   0 root         (0) root         (0)     6601 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_details.json
--rw-r--r--   0 root         (0) root         (0)      956 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_external_ids.json
--rw-r--r--   0 root         (0) root         (0)     3551 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_images.json
--rw-r--r--   0 root         (0) root         (0)      937 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_keywords.json
--rw-r--r--   0 root         (0) root         (0)     4332 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_latest.json
--rw-r--r--   0 root         (0) root         (0)     5154 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_lists.json
--rw-r--r--   0 root         (0) root         (0)     4308 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_now_playing.json
--rw-r--r--   0 root         (0) root         (0)     3815 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_popular.json
--rw-r--r--   0 root         (0) root         (0)     3798 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_recommendations.json
--rw-r--r--   0 root         (0) root         (0)     2253 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_releases_dates.json
--rw-r--r--   0 root         (0) root         (0)     3400 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_reviews.json
--rw-r--r--   0 root         (0) root         (0)     3798 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_similar_movies.json
--rw-r--r--   0 root         (0) root         (0)    15218 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_top_rated.json
--rw-r--r--   0 root         (0) root         (0)    32178 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_translations.json
--rw-r--r--   0 root         (0) root         (0)     4318 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_upcoming.json
--rw-r--r--   0 root         (0) root         (0)     3751 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_videos.json
--rw-r--r--   0 root         (0) root         (0)   209095 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_watch_providers.json
--rw-r--r--   0 root         (0) root         (0)     1655 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_collections.json
--rw-r--r--   0 root         (0) root         (0)     1436 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_companies.json
--rw-r--r--   0 root         (0) root         (0)     1215 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_keywords.json
--rw-r--r--   0 root         (0) root         (0)     3835 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_movies.json
--rw-r--r--   0 root         (0) root         (0)     3902 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_multi.json
--rw-r--r--   0 root         (0) root         (0)     6244 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_people.json
--rw-r--r--   0 root         (0) root         (0)     3975 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_tv_shows.json
--rw-r--r--   0 root         (0) root         (0)     3814 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/schemas/trending.json
--rw-r--r--   0 root         (0) root         (0)      473 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/source.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-02-01 07:53:30.000000 airbyte-source-tmdb-0.1.0/source_tmdb/spec.yaml
+-rw-r--r--   0        0        0     4460 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/README.md
+-rw-r--r--   0        0        0      730 2024-05-29 22:05:56.792406 airbyte_source_tmdb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/__init__.py
+-rw-r--r--   0        0        0     8471 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/manifest.yaml
+-rw-r--r--   0        0        0      224 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/run.py
+-rw-r--r--   0        0        0    20718 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/certification_movie.json
+-rw-r--r--   0        0        0    13634 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/certification_tv.json
+-rw-r--r--   0        0        0     1443 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/changes_movie.json
+-rw-r--r--   0        0        0     1443 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/changes_person.json
+-rw-r--r--   0        0        0     1441 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/changes_tv.json
+-rw-r--r--   0        0        0     1217 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_alternative_titles.json
+-rw-r--r--   0        0        0     2500 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_changes.json
+-rw-r--r--   0        0        0     5293 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_credits.json
+-rw-r--r--   0        0        0     6601 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_details.json
+-rw-r--r--   0        0        0      956 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_external_ids.json
+-rw-r--r--   0        0        0     3551 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_images.json
+-rw-r--r--   0        0        0      937 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_keywords.json
+-rw-r--r--   0        0        0     4332 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_latest.json
+-rw-r--r--   0        0        0     5154 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_lists.json
+-rw-r--r--   0        0        0     4308 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_now_playing.json
+-rw-r--r--   0        0        0     3815 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_popular.json
+-rw-r--r--   0        0        0     3798 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_recommendations.json
+-rw-r--r--   0        0        0     2253 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_releases_dates.json
+-rw-r--r--   0        0        0     3378 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_reviews.json
+-rw-r--r--   0        0        0     3798 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_similar_movies.json
+-rw-r--r--   0        0        0    15218 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_top_rated.json
+-rw-r--r--   0        0        0    32180 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_translations.json
+-rw-r--r--   0        0        0     4318 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_upcoming.json
+-rw-r--r--   0        0        0     3751 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_videos.json
+-rw-r--r--   0        0        0   209095 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_watch_providers.json
+-rw-r--r--   0        0        0     1655 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_collections.json
+-rw-r--r--   0        0        0     1436 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_companies.json
+-rw-r--r--   0        0        0     1215 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_keywords.json
+-rw-r--r--   0        0        0     3835 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_movies.json
+-rw-r--r--   0        0        0     3902 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_multi.json
+-rw-r--r--   0        0        0     6244 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_people.json
+-rw-r--r--   0        0        0     3975 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_tv_shows.json
+-rw-r--r--   0        0        0     3814 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/schemas/trending.json
+-rw-r--r--   0        0        0      473 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/source.py
+-rw-r--r--   0        0        0     1043 2024-05-29 21:37:39.000000 airbyte_source_tmdb-0.1.1/source_tmdb/spec.yaml
+-rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 airbyte_source_tmdb-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-tmdb-0.1.0/PKG-INFO` & `airbyte_source_tmdb-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-tmdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Source implementation for Tmdb.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/tmdb
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Tmdb Source
+# Tmdb source connector
 
-This is the repository for the Tmdb configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/tmdb).
 
+This is the repository for the Tmdb source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/tmdb).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
-
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
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/tmdb)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/tmdb)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_tmdb/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source tmdb test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-tmdb spec
+poetry run source-tmdb check --config secrets/config.json
+poetry run source-tmdb discover --config secrets/config.json
+poetry run source-tmdb read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-tmdb build
 ```
 
-An image will be built with the tag `airbyte/source-tmdb:dev`.
+An image will be available on your host with the tag `airbyte/source-tmdb:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-tmdb:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-tmdb:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-tmdb:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-tmdb:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-tmdb:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-tmdb test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-tmdb test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/tmdb.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/tmdb.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-tmdb-0.1.0/README.md` & `airbyte_source_tmdb-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-# Tmdb Source
+# Tmdb source connector
 
-This is the repository for the Tmdb configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/tmdb).
+
+This is the repository for the Tmdb source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/tmdb).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Minimum Python version required `= 3.9.0`
-
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
-
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
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/tmdb)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/tmdb)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_tmdb/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source tmdb test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-tmdb spec
+poetry run source-tmdb check --config secrets/config.json
+poetry run source-tmdb discover --config secrets/config.json
+poetry run source-tmdb read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-tmdb build
 ```
 
-An image will be built with the tag `airbyte/source-tmdb:dev`.
+An image will be available on your host with the tag `airbyte/source-tmdb:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-tmdb:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-tmdb:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-tmdb:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-tmdb:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-tmdb:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-tmdb test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-tmdb test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/tmdb.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/tmdb.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/manifest.yaml` & `airbyte_source_tmdb-0.1.1/source_tmdb/manifest.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 version: "0.29.0"
 
 definitions:
   selector:
     extractor:
       field_path: []
+    schema_normalization: Default
   requester:
     url_base: "https://api.themoviedb.org/3/"
     http_method: "GET"
     request_parameters:
       api_key: "{{ config['api_key'] }}"
       language: |
         {{
```

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/certification_movie.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/certification_movie.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/certification_tv.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/certification_tv.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/changes_movie.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/changes_movie.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/changes_person.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/changes_person.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/changes_tv.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/changes_tv.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_alternative_titles.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_alternative_titles.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_changes.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_changes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_credits.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_credits.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_details.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_details.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_external_ids.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_external_ids.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_images.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_images.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_keywords.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_keywords.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_latest.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_latest.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_lists.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_lists.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_now_playing.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_now_playing.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_popular.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_popular.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_recommendations.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_recommendations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_releases_dates.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_releases_dates.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_reviews.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_reviews.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999991280692%*

 * *Differences: {"'properties'": "{'results': {'items': {'properties': {'author_details': {'properties': "*

 * *                 "{'avatar_path': {'type': {delete: [2]}}, 'rating': {'type': {delete: [2]}}}}}}}}"}*

```diff
@@ -34,16 +34,15 @@
                             "avatar_path": {
                                 "$id": "#root/results/items/author_details/avatar_path",
                                 "default": "",
                                 "pattern": "^.*$",
                                 "title": "Avatar_path",
                                 "type": [
                                     "null",
-                                    "string",
-                                    "integer"
+                                    "string"
                                 ]
                             },
                             "name": {
                                 "$id": "#root/results/items/author_details/name",
                                 "default": "",
                                 "pattern": "^.*$",
                                 "title": "Name",
@@ -51,16 +50,15 @@
                             },
                             "rating": {
                                 "$id": "#root/results/items/author_details/rating",
                                 "default": null,
                                 "title": "Rating",
                                 "type": [
                                     "null",
-                                    "string",
-                                    "integer"
+                                    "string"
                                 ]
                             },
                             "username": {
                                 "$id": "#root/results/items/author_details/username",
                                 "default": "",
                                 "pattern": "^.*$",
                                 "title": "Username",
```

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_similar_movies.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_similar_movies.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_top_rated.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_top_rated.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_translations.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_translations.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997967479674796%*

 * *Differences: {"'translations'": "{2: {'data': {'homepage': 'https://www.welcometofc.com/'}}, 31: {'data': "*

 * *                   "{'homepage': 'https://www.foxmovies.com/movies/fight-club'}}}"}*

```diff
@@ -21,15 +21,15 @@
             "english_name": "German",
             "iso_3166_1": "DE",
             "iso_639_1": "de",
             "name": "Deutsch"
         },
         {
             "data": {
-                "homepage": "http://www.welcometofc.com/",
+                "homepage": "https://www.welcometofc.com/",
                 "overview": "Jack (Edward Norton) \u00e9 um executivo que trabalha como investigador de seguros, tem uma boa vida financeira, mas sofre com problemas de ins\u00f4nia. Para tentar se curar, ele come\u00e7a a freq\u00fcentar terapias em grupo, mas sua vida vira de cabe\u00e7a para baixo quando ele conhece Tyler (Brad Pitt). Com ele, forma um clube da luta, onde pessoas s\u00e3o amigas, mas se esmurram violentamente em algumas noites. Tudo ganha prop\u00f3sitos maiores quando as coisas come\u00e7am a ficar loucas e surreais.",
                 "title": "Clube de Combate"
             },
             "english_name": "Portuguese",
             "iso_3166_1": "PT",
             "iso_639_1": "pt",
             "name": "Portugu\u00eas"
@@ -340,15 +340,15 @@
             "english_name": "Thai",
             "iso_3166_1": "TH",
             "iso_639_1": "th",
             "name": "\u0e20\u0e32\u0e29\u0e32\u0e44\u0e17\u0e22"
         },
         {
             "data": {
-                "homepage": "http://www.foxmovies.com/movies/fight-club",
+                "homepage": "https://www.foxmovies.com/movies/fight-club",
                 "overview": "A ticking-time-bomb insomniac and a slippery soap salesman channel primal male aggression into a shocking new form of therapy. Their concept catches on, with underground \"fight clubs\" forming in every town, until an eccentric gets in the way and ignites an out-of-control spiral toward oblivion.",
                 "title": ""
             },
             "english_name": "English",
             "iso_3166_1": "US",
             "iso_639_1": "en",
             "name": "English"
```

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_upcoming.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_upcoming.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_videos.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_videos.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/movies_watch_providers.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/movies_watch_providers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_collections.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_companies.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_companies.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_keywords.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_keywords.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_movies.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_movies.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_multi.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_multi.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_people.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_people.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/search_tv_shows.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/search_tv_shows.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/schemas/trending.json` & `airbyte_source_tmdb-0.1.1/source_tmdb/schemas/trending.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tmdb-0.1.0/source_tmdb/spec.yaml` & `airbyte_source_tmdb-0.1.1/source_tmdb/spec.yaml`

 * *Files identical despite different names*

