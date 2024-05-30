# Comparing `tmp/ibridges-0.1.6.tar.gz` & `tmp/ibridges-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibridges-0.1.6.tar", last modified: Tue May 14 10:25:29 2024, max compression
+gzip compressed data, was "ibridges-0.2.0.tar", last modified: Thu May 30 11:11:00 2024, max compression
```

## Comparing `ibridges-0.1.6.tar` & `ibridges-0.2.0.tar`

### file list

```diff
@@ -1,123 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.904852 ibridges-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:25:24.000000 ibridges-0.1.6/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.880852 ibridges-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/integration-tests-irods.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/integration-tests-yoda.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-14 10:25:24.000000 ibridges-0.1.6/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-14 10:25:24.000000 ibridges-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 10:25:24.000000 ibridges-0.1.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 10:25:24.000000 ibridges-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-14 10:25:29.904852 ibridges-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-14 10:25:24.000000 ibridges-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog/init-user-db.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_catalog_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/setup-4.3.1.input
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_catalog_provider/setup-4.3.2.input
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.880852 ibridges-0.1.6/docker/irods_client/environments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_client/environments/plain-irods/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/plain-irods/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/plain-irods/irods_environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.884852 ibridges-0.1.6/docker/irods_client/environments/yoda/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/yoda/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/environments/yoda/irods_environment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docker/irods_client/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/beach.rtf
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/bunny.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/example.r
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docker/irods_client/testdata/more_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/more_data/polarbear.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/plant.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/testdata/sun.rtf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docker/irods_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_data_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker/irods_client/tests/test_ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 10:25:24.000000 ibridges-0.1.6/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.888852 ibridges-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.892852 ibridges-0.1.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-14 10:25:24.000000 ibridges-0.1.6/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.892852 ibridges-0.1.6/ibridges/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/data_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/export_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/icat_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-14 10:25:24.000000 ibridges-0.1.6/ibridges/tickets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.900852 ibridges-0.1.6/ibridges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 10:25:29.000000 ibridges-0.1.6/ibridges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 10:25:24.000000 ibridges-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:25:29.904852 ibridges-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-14 10:25:24.000000 ibridges-0.1.6/tests/test_irodspath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-14 10:25:24.000000 ibridges-0.1.6/tests/testdata/bunny.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tests/testdata/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 10:25:24.000000 ibridges-0.1.6/tests/testdata/subfolder/sun.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/01-Setup-and-connect.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/02-Working-with-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/03-iRODS-Paths.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/04-Metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/05-Data-Sharing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/Data_sync.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/QuickStart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.896852 ibridges-0.1.6/tutorials/example_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/example_rules/example.r
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/iRODS_paths.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:25:29.900852 ibridges-0.1.6/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject1.png
--rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject2.png
--rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject3.png
--rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject4.png
--rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject5.png
--rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/DataObject6.png
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/Save_json.png
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-14 10:25:24.000000 ibridges-0.1.6/tutorials/img/Yoda_environment.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.827860 ibridges-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:10:55.000000 ibridges-0.2.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/workflows/integration-tests-irods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/workflows/integration-tests-yoda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-30 11:10:55.000000 ibridges-0.2.0/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 11:10:55.000000 ibridges-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 11:10:55.000000 ibridges-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 11:10:55.000000 ibridges-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-05-30 11:11:00.827860 ibridges-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-30 11:10:55.000000 ibridges-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/docker/irods_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_catalog/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_catalog/init-user-db.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/docker/irods_catalog_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_catalog_provider/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_catalog_provider/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_catalog_provider/setup-4.3.1.input
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_catalog_provider/setup-4.3.2.input
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/docker/irods_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.807860 ibridges-0.2.0/docker/irods_client/environments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/docker/irods_client/environments/plain-irods/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/environments/plain-irods/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/environments/plain-irods/irods_environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.811860 ibridges-0.2.0/docker/irods_client/environments/yoda/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/environments/yoda/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/environments/yoda/irods_environment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.815860 ibridges-0.2.0/docker/irods_client/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/testdata/beach.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/testdata/bunny.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/testdata/example.r
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.815860 ibridges-0.2.0/docker/irods_client/testdata/more_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/testdata/more_data/polarbear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/testdata/plant.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/testdata/sun.rtf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.815860 ibridges-0.2.0/docker/irods_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_data_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker/irods_client/tests/test_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 11:10:55.000000 ibridges-0.2.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.815860 ibridges-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.815860 ibridges-0.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.819860 ibridges-0.2.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/api/full_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/api/user_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/ipath.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-30 11:10:55.000000 ibridges-0.2.0/docs/source/sync.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.819860 ibridges-0.2.0/ibridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21234 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/data_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/export_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/icat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20345 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/tickets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-30 11:10:55.000000 ibridges-0.2.0/ibridges/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.827860 ibridges-0.2.0/ibridges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 11:11:00.000000 ibridges-0.2.0/ibridges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 11:10:55.000000 ibridges-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:11:00.827860 ibridges-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.819860 ibridges-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-30 11:10:55.000000 ibridges-0.2.0/tests/test_irodspath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.819860 ibridges-0.2.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-30 11:10:55.000000 ibridges-0.2.0/tests/testdata/bunny.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.823860 ibridges-0.2.0/tests/testdata/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-30 11:10:55.000000 ibridges-0.2.0/tests/testdata/subfolder/sun.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.823860 ibridges-0.2.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    18483 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/00-FirstSteps.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/01-Setup-and-connect.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/02-iRODS-paths.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19207 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/03-Working-with-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/04-Metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/05-Data-Sharing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/06-Data-sync.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.823860 ibridges-0.2.0/tutorials/example_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/example_rules/example.r
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:11:00.827860 ibridges-0.2.0/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/DataObject1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/DataObject2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/DataObject3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/DataObject4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/DataObject5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/DataObject6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/Save_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-30 11:10:55.000000 ibridges-0.2.0/tutorials/img/Yoda_environment.png
```

### Comparing `ibridges-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `ibridges-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `ibridges-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/.github/dependabot.yml` & `ibridges-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/.github/workflows/integration-tests-irods.yml` & `ibridges-0.2.0/.github/workflows/integration-tests-irods.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/.github/workflows/integration-tests-yoda.yml` & `ibridges-0.2.0/.github/workflows/integration-tests-yoda.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/.github/workflows/main.yml` & `ibridges-0.2.0/.github/workflows/main.yml`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[test]
 
+    - name: Lint with Ruff
+      run: |
+        ruff check ibridges
+
     - name: Lint with PyLint
       run: |
         pylint ibridges
 
     - name: Check types with MyPy
       run: |
         mypy ibridges
```

### Comparing `ibridges-0.1.6/.github/workflows/pypi_release.yml` & `ibridges-0.2.0/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/.gitignore` & `ibridges-0.2.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Local additions
 .idea
 irods-basicGUI/logs/*
 irods-iBridgesGui.spec
 *DS_Store
-
+docs/source/api/generated
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `ibridges-0.1.6/.readthedocs.yaml` & `ibridges-0.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/LICENSE` & `ibridges-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/PKG-INFO` & `ibridges-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.6
+Version: 0.2.0
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -49,14 +49,15 @@
 Requires-Dist: types-tqdm; extra == "test"
 Requires-Dist: sphinx; extra == "test"
 Requires-Dist: sphinx-rtd-theme; extra == "test"
 Requires-Dist: sphinxcontrib-napoleon; extra == "test"
 Requires-Dist: sphinx-autodoc-typehints; extra == "test"
 Requires-Dist: sphinx_inline_tabs; extra == "test"
 Requires-Dist: sphinx_copybutton; extra == "test"
+Requires-Dist: ruff; extra == "test"
 
 # iBridges
 [![PyPI version](https://badge.fury.io/py/ibridges.svg)](https://badge.fury.io/py/ibridges)
 [![](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-irods.yml/badge.svg?branch=develop)](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-irods.yml) [![](https://github.com/UtrechtUniversity/iBridges/actions/workflows/main.yml/badge.svg?branch=develop)](https://github.com/UtrechtUniversity/iBridges/actions/workflows/main.yml) 
 [![](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-yoda.yml/badge.svg)](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-yoda.yml) ![](https://readthedocs.org/projects/ibridges/badge/?version=latest&style=flat-default)
 
 iBridges is library for scientific programmers who are working with data in iRODS. We provide a wrapper around the [python-irodsclient](https://pypi.org/project/python-irodsclient/) to facilitate easy interaction with the iRODS server. iBridges is currently still in very active development.
@@ -105,50 +106,50 @@
 
 ## Usage
 
 Below are some basic examples of the features in iBridges.
 
 ```py
 # Create an iRODS session
-from ibridges import Session
+from ibridges.interactive import interactive_auth
 
-session = Session(irods_env_path="~/.irods/irods_environment.json", password="mypassword")
+session = interactive_auth()
 
 # Upload data
 from ibridges import upload
 
 upload(session, "/your/local/path", "/irods/path")
 
 # Download data
 from ibridges import download
 
 download(session, "/irods/path", "/other/local/path")
 
 ```
 
-## Commandline interface
-To simply upload or download data you do not need to write full python program, we offer a Commandline interface
+## Command line interface
+To simply upload or download data you do not need to write full python program, we offer a command line interface
 
 - Establish a connection
 
   ```bash
   ibridges init
   ```
 
-- List a colletion
+- List a collection
   
   ```bash
   # list your home collection
   ibridges list
   
   # list a different collection in your home
   ibridges list irods:~/<collection>
   
   # list a collection on a different path than your home
-  ibridges. list irods:<full_irods_path>
+  ibridges list irods:<full_irods_path>
   ```
 
 - Upload data
 
   ```bash
   ibridges upload my_file.json irods:~/some_collection
   ```
@@ -158,30 +159,30 @@
   ```bash
   ibridges download irods:~/some_collection/some_object download_dir
   ```
 
 - Synchronise data
 
   ```bash
-      ibridges sync some_local_directory irods:~/some_collection
+  	ibridges sync some_local_directory irods:~/some_collection
   ```
 
 ## Tutorials
 ### Documentation
 - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
 
 ### Guides
-- [QuickStart](tutorials/QuickStart.ipynb)
-- [iRODS Paths](tutorials/iRODS_paths.ipynb)
-- [Data synchronisation](tutorials/Data_sync.ipynb)
+- [Manual with examples](tutorials/QuickStart.ipynb)
+- [Tutorial for iRODS paths](tutorials/01-iRODS_paths.ipynb)
+- [Data synchronisation manual](tutorials/Data_sync.ipynb)
 
 ### Beginners tutorials
 - [Setup client configuration](tutorials/01-Setup-and-connect.ipynb)
+- [iRODS Paths](tutorials/01-iRODS_paths.ipynb)
 - [Working with data](tutorials/02-Working-with-data.ipynb)
-- [iRODS and local Paths](tutorials/03-iRODS-Paths.ipynb)
 - [Metadata](tutorials/04-Metadata.ipynb)
 - [Sharing data](tutorials/05-Data-Sharing.ipynb)
 
 ## Authors
 
 **Christine Staiger (Maintainer) [ORCID](https://orcid.org/0000-0002-6754-7647)**
```

### Comparing `ibridges-0.1.6/README.md` & `ibridges-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,50 +49,50 @@
 
 ## Usage
 
 Below are some basic examples of the features in iBridges.
 
 ```py
 # Create an iRODS session
-from ibridges import Session
+from ibridges.interactive import interactive_auth
 
-session = Session(irods_env_path="~/.irods/irods_environment.json", password="mypassword")
+session = interactive_auth()
 
 # Upload data
 from ibridges import upload
 
 upload(session, "/your/local/path", "/irods/path")
 
 # Download data
 from ibridges import download
 
 download(session, "/irods/path", "/other/local/path")
 
 ```
 
-## Commandline interface
-To simply upload or download data you do not need to write full python program, we offer a Commandline interface
+## Command line interface
+To simply upload or download data you do not need to write full python program, we offer a command line interface
 
 - Establish a connection
 
   ```bash
   ibridges init
   ```
 
-- List a colletion
+- List a collection
   
   ```bash
   # list your home collection
   ibridges list
   
   # list a different collection in your home
   ibridges list irods:~/<collection>
   
   # list a collection on a different path than your home
-  ibridges. list irods:<full_irods_path>
+  ibridges list irods:<full_irods_path>
   ```
 
 - Upload data
 
   ```bash
   ibridges upload my_file.json irods:~/some_collection
   ```
@@ -102,30 +102,30 @@
   ```bash
   ibridges download irods:~/some_collection/some_object download_dir
   ```
 
 - Synchronise data
 
   ```bash
-      ibridges sync some_local_directory irods:~/some_collection
+  	ibridges sync some_local_directory irods:~/some_collection
   ```
 
 ## Tutorials
 ### Documentation
 - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
 
 ### Guides
-- [QuickStart](tutorials/QuickStart.ipynb)
-- [iRODS Paths](tutorials/iRODS_paths.ipynb)
-- [Data synchronisation](tutorials/Data_sync.ipynb)
+- [Manual with examples](tutorials/QuickStart.ipynb)
+- [Tutorial for iRODS paths](tutorials/01-iRODS_paths.ipynb)
+- [Data synchronisation manual](tutorials/Data_sync.ipynb)
 
 ### Beginners tutorials
 - [Setup client configuration](tutorials/01-Setup-and-connect.ipynb)
+- [iRODS Paths](tutorials/01-iRODS_paths.ipynb)
 - [Working with data](tutorials/02-Working-with-data.ipynb)
-- [iRODS and local Paths](tutorials/03-iRODS-Paths.ipynb)
 - [Metadata](tutorials/04-Metadata.ipynb)
 - [Sharing data](tutorials/05-Data-Sharing.ipynb)
 
 ## Authors
 
 **Christine Staiger (Maintainer) [ORCID](https://orcid.org/0000-0002-6754-7647)**
```

#### html2text {}

```diff
@@ -25,37 +25,37 @@
                                    _q_u_e_s_t_i_o_n
 ## Installation There are two main ways to install iBridges. The recommended
 way is to use the stable version that is available on PyPi: ```bash pip install
 ibridges ``` If you want to install the unstable version to test out new
 features, you can install the development branch: ```bash pip install
 git+https://github.com/UtrechtUniversity/iBridges.git@develop ``` ## Usage
 Below are some basic examples of the features in iBridges. ```py # Create an
-iRODS session from ibridges import Session session = Session
-(irods_env_path="~/.irods/irods_environment.json", password="mypassword") #
-Upload data from ibridges import upload upload(session, "/your/local/path", "/
-irods/path") # Download data from ibridges import download download(session, "/
-irods/path", "/other/local/path") ``` ## Commandline interface To simply upload
-or download data you do not need to write full python program, we offer a
-Commandline interface - Establish a connection ```bash ibridges init ``` - List
-a colletion ```bash # list your home collection ibridges list # list a
-different collection in your home ibridges list irods:~/ # list a collection on
-a different path than your home ibridges. list irods: ``` - Upload data ```bash
-ibridges upload my_file.json irods:~/some_collection ``` - Download data
-```bash ibridges download irods:~/some_collection/some_object download_dir ```
-- Synchronise data ```bash ibridges sync some_local_directory irods:~/
-some_collection ``` ## Tutorials ### Documentation - **[ReadTheDocs](https://
-ibridges.readthedocs.io/en/latest/)** ### Guides - [QuickStart](tutorials/
-QuickStart.ipynb) - [iRODS Paths](tutorials/iRODS_paths.ipynb) - [Data
-synchronisation](tutorials/Data_sync.ipynb) ### Beginners tutorials - [Setup
-client configuration](tutorials/01-Setup-and-connect.ipynb) - [Working with
-data](tutorials/02-Working-with-data.ipynb) - [iRODS and local Paths]
-(tutorials/03-iRODS-Paths.ipynb) - [Metadata](tutorials/04-Metadata.ipynb) -
-[Sharing data](tutorials/05-Data-Sharing.ipynb) ## Authors **Christine Staiger
-(Maintainer) [ORCID](https://orcid.org/0000-0002-6754-7647)** - *Wageningen
-University & Research* 2021 - 2022 - *Utrecht University* 2022 **Tim van
-Daalen**, *Wageningen University & Research* 2021 **Maarten Schermer
-(Maintainer) [ORCID](https://orcid.org/my-orcid?orcid=0000-0001-6770-3155)**,
-*Utrecht University* 2023 **Raoul Schram (Maintainer) [ORCID](https://
-orcid.org/my-orcid?orcid=0000-0001-6616-230X)**. *Utrecht University* 2023 ##
-Contributors **J.P. Mc Farland**, *University of Groningen, Center for
-Information Technology*, 2022 ## License This project is licensed under the MIT
-license. The full license can be found in [LICENSE](LICENSE).
+iRODS session from ibridges.interactive import interactive_auth session =
+interactive_auth() # Upload data from ibridges import upload upload(session, "/
+your/local/path", "/irods/path") # Download data from ibridges import download
+download(session, "/irods/path", "/other/local/path") ``` ## Command line
+interface To simply upload or download data you do not need to write full
+python program, we offer a command line interface - Establish a connection
+```bash ibridges init ``` - List a collection ```bash # list your home
+collection ibridges list # list a different collection in your home ibridges
+list irods:~/ # list a collection on a different path than your home ibridges
+list irods: ``` - Upload data ```bash ibridges upload my_file.json irods:~/
+some_collection ``` - Download data ```bash ibridges download irods:~/
+some_collection/some_object download_dir ``` - Synchronise data ```bash
+ibridges sync some_local_directory irods:~/some_collection ``` ## Tutorials ###
+Documentation - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
+### Guides - [Manual with examples](tutorials/QuickStart.ipynb) - [Tutorial for
+iRODS paths](tutorials/01-iRODS_paths.ipynb) - [Data synchronisation manual]
+(tutorials/Data_sync.ipynb) ### Beginners tutorials - [Setup client
+configuration](tutorials/01-Setup-and-connect.ipynb) - [iRODS Paths](tutorials/
+01-iRODS_paths.ipynb) - [Working with data](tutorials/02-Working-with-
+data.ipynb) - [Metadata](tutorials/04-Metadata.ipynb) - [Sharing data]
+(tutorials/05-Data-Sharing.ipynb) ## Authors **Christine Staiger (Maintainer)
+[ORCID](https://orcid.org/0000-0002-6754-7647)** - *Wageningen University &
+Research* 2021 - 2022 - *Utrecht University* 2022 **Tim van Daalen**,
+*Wageningen University & Research* 2021 **Maarten Schermer (Maintainer) [ORCID]
+(https://orcid.org/my-orcid?orcid=0000-0001-6770-3155)**, *Utrecht University*
+2023 **Raoul Schram (Maintainer) [ORCID](https://orcid.org/my-orcid?orcid=0000-
+0001-6616-230X)**. *Utrecht University* 2023 ## Contributors **J.P. Mc
+Farland**, *University of Groningen, Center for Information Technology*, 2022
+## License This project is licensed under the MIT license. The full license can
+be found in [LICENSE](LICENSE).
```

### Comparing `ibridges-0.1.6/docker/.gitattributes` & `ibridges-0.2.0/docker/.gitattributes`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/README.md` & `ibridges-0.2.0/docker/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_catalog_provider/Dockerfile` & `ibridges-0.2.0/docker/irods_catalog_provider/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_catalog_provider/entrypoint.sh` & `ibridges-0.2.0/docker/irods_catalog_provider/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/Dockerfile` & `ibridges-0.2.0/docker/irods_client/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/entrypoint.sh` & `ibridges-0.2.0/docker/irods_client/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/environments/yoda/config.toml` & `ibridges-0.2.0/docker/irods_client/environments/yoda/config.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/environments/yoda/irods_environment.json` & `ibridges-0.2.0/docker/irods_client/environments/yoda/irods_environment.json`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/testdata/beach.rtf` & `ibridges-0.2.0/docker/irods_client/testdata/beach.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/testdata/bunny.rtf` & `ibridges-0.2.0/docker/irods_client/testdata/bunny.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/testdata/more_data/polarbear.txt` & `ibridges-0.2.0/docker/irods_client/testdata/more_data/polarbear.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/testdata/plant.rtf` & `ibridges-0.2.0/docker/irods_client/testdata/plant.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/testdata/sun.rtf` & `ibridges-0.2.0/docker/irods_client/testdata/sun.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker/irods_client/tests/conftest.py` & `ibridges-0.2.0/docker/irods_client/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import json
 from pathlib import Path
-import os
 
 import pytest
 import tomli
 
 from ibridges import Session
 from ibridges.data_operations import (
     create_collection,
-    get_collection,
-    get_dataobject,
     upload,
 )
 from ibridges.path import IrodsPath
 
 
 @pytest.fixture(scope="session")
 def config_dir(request):
@@ -57,10 +54,9 @@
     return create_collection(session, IrodsPath(session, "~", "test_collection"))
 
 
 @pytest.fixture(scope="session")
 def dataobject(session, testdata):
     ipath = IrodsPath(session, "~", "bunny.rtf")
     upload(session, testdata/"bunny.rtf", IrodsPath(session, "~"), overwrite=True)
-    data_obj = get_dataobject(session, ipath)
-    yield data_obj
+    yield ipath.dataobject
     ipath.remove()
```

### Comparing `ibridges-0.1.6/docker/irods_client/tests/test_cli.py` & `ibridges-0.2.0/docker/irods_client/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,29 +48,29 @@
     ipath = IrodsPath(session, "~", "plant.rtf")
     ipath.remove()
     subprocess.run(["ibridges", "init", irods_env_file],
                    check=True, **pass_opts)
 
     if "resc2" in config["resources"]:
         subprocess.run(["ibridges", "upload", testdata/"plant.rtf", "irods:" + str(ipath),
-                        "--overwrite", "--resource resc2"],
+                        "--overwrite", "--resource", "resc2"],
                         check=True, **pass_opts)
     else:
         subprocess.run(["ibridges", "upload", testdata/"plant.rtf", "irods:" + str(ipath),
                         "--overwrite"],
                         check=True, **pass_opts)
     assert ipath.dataobject_exists()
 
     # Download the same file and check if they are equal.
     assert isinstance(testdata, Path)
     if "resc2" in config["resources"]:
         subprocess.run(["ibridges", "download", "irods:~/plant.rtf", testdata/"plant2.rtf",
-                        "--resource resc2"], check=True, **pass_opts)
+                        "--resource", "resc2"], check=True, **pass_opts)
     else:
-        subprocess.run(["ibridges", "download", "irods:~/plant.rtf", testdata/"plant2.rtf"], 
+        subprocess.run(["ibridges", "download", "irods:~/plant.rtf", testdata/"plant2.rtf"],
                         check=True, **pass_opts)
     assert Path(testdata/"plant2.rtf").is_file()
 
     _check_files_equal(testdata/"plant2.rtf", testdata/"plant.rtf")
     (testdata/"plant2.rtf").unlink()
 
     # Upload a directory and check if the dataobjects and collections are created.
```

### Comparing `ibridges-0.1.6/docker/irods_client/tests/test_meta.py` & `ibridges-0.2.0/docker/irods_client/tests/test_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import irods
 import pytest
 from pytest import mark
-import irods
 
-from ibridges.meta import MetaData
 from ibridges.export_metadata import export_metadata_to_dict
+from ibridges.meta import MetaData
+
 
 @mark.parametrize("item_name", ["collection", "dataobject"])
 def test_meta(item_name, request):
     item = request.getfixturevalue(item_name)
     meta = MetaData(item)
     meta.clear()
 
@@ -60,31 +61,36 @@
     meta.add("y", "z")
     meta.set("y", "x")
     assert "x" in meta
     assert ("y", "z") not in meta
     assert ("y", "x") in meta
 
 @mark.parametrize("item_name", ["collection", "dataobject"])
-def test_export_metadata(item_name, request):
+def test_metadata_todict(item_name, request):
     item = request.getfixturevalue(item_name)
     meta = MetaData(item)
     meta.clear()
-    
     # test against:
     test_dict = {
             'name': item.name,
             'irods_id': item.id,
             'metadata': [('x', 'z', 'm')]
             }
 
     if isinstance(item, irods.data_object.iRODSDataObject):
         test_dict['checksum'] = item.checksum
-    
+
     # Add some metadata
     meta.add("x", "z", "m")
     assert "x" in meta
     result = meta.to_dict()
 
     for key in result.keys():
         assert key in test_dict
     for value in result.values():
         assert value in test_dict.values()
+
+@mark.parametrize("item_name", ["collection", "dataobject"])
+def test_metadata_export(item_name, request, session):
+    item = request.getfixturevalue(item_name)
+    res = export_metadata_to_dict(MetaData(item), session)
+    assert isinstance(res, dict)
```

### Comparing `ibridges-0.1.6/docker/irods_client/tests/test_permissions.py` & `ibridges-0.2.0/docker/irods_client/tests/test_permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pytest
-from irods.exception import CAT_NO_ACCESS_PERMISSION
 from pytest import mark
 
-from ibridges.data_operations import download, upload
-from ibridges.permissions import Permissions
 from ibridges.path import IrodsPath
+from ibridges.permissions import Permissions
 
 
 @mark.parametrize("item_name", ["collection", "dataobject"])
 def test_perm_own(session, item_name, request, tmpdir, config):
     item = request.getfixturevalue(item_name)
     perm = Permissions(session, item)
     ipath = IrodsPath(session, item.path)
```

### Comparing `ibridges-0.1.6/docker/irods_client/tests/test_session.py` & `ibridges-0.2.0/docker/irods_client/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import pytest
 import json
 
+import pytest
+
 from ibridges import Session
 from ibridges.interactive import interactive_auth
 
+
 def test_session_from_cached_pw(config, irods_env):
     # test only for plain irods
     if config.get("create_session_from_cached_pw", True):
         session = Session(config["env_path"])
         assert session.has_valid_irods_session()
         assert ".".join(str(x) for x in session.server_version) == config["server_version"]
         assert session.home == irods_env["irods_home"]
```

### Comparing `ibridges-0.1.6/docker/irods_client/tests/test_sync.py` & `ibridges-0.2.0/docker/irods_client/tests/test_sync.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,66 @@
-from ibridges.sync import sync_data, _calc_checksum
+from ibridges.data_operations import _calc_checksum, create_collection, sync
 from ibridges.path import IrodsPath
-from ibridges.data_operations import create_collection, get_dataobject
+
 
 def test_sync_dry_run(session, testdata, capsys):
 
     ipath = IrodsPath(session, "~", "empty")
     coll = create_collection(session=session, coll_path=ipath)
+    assert len(coll.data_objects)+len(coll.subcollections)==0, "Dry run starting not empty"
 
     # upload
-    sync_data(session=session,
-         source=testdata,
-         target=ipath,
-         max_level=None,
-         dry_run=True,
-         copy_empty_folders=True)
-
-    captured = capsys.readouterr()
-    lines=sorted([x.strip() for x in captured.out.split("\n") if len(x.strip())>0])
-    
-    assert lines == ['/tempZone/home/rods/empty/more_data',
-        'Will create collection(s):',
-        "Will upload from '/tmp/testdata' to '/tempZone/home/rods/empty':",
-        'beach.rtf  727',
-        'bunny.rtf  10150',
-        'example.r  182',
-        'more_data/polarbear.txt  2717',
-        'plant.rtf  992',
-        'plant.rtf.copy  992',
-        'sun.rtf  661']
-
+    ops = sync(session=session,
+               source=testdata,
+               target=ipath,
+               max_level=None,
+               dry_run=True,
+               copy_empty_folders=True)
+
+    assert len(ops["create_collection"]) == 1
+    assert len(ops["create_dir"]) == 0
+    assert len(ops["download"]) == 0
+    assert len(ops["upload"]) == 7
     assert len(coll.data_objects)+len(coll.subcollections)==0, "Dry run did sync"
 
+
 def test_sync_upload_download(session, testdata, tmpdir):
     ipath = IrodsPath(session, "~", "empty")
     coll = create_collection(session=session, coll_path=ipath)
 
     assert len(coll.data_objects)+len(coll.subcollections)==0, "iRODS folder not empty"
 
     # upload
-    sync_data(session=session,
+    sync(session=session,
          source=testdata,
          target=ipath,
          max_level=None,
          dry_run=False,
          copy_empty_folders=True)
 
     for cur_file in list(testdata.glob("*")):
         s_ipath = IrodsPath(session, "~", "empty", cur_file.name)
         if cur_file.is_file():
             assert s_ipath.dataobject_exists(), "File not uploaded"
-            cur_obj=get_dataobject(session=session, path=s_ipath)
+            cur_obj=s_ipath.dataobject
             assert _calc_checksum(cur_file)==(cur_obj.checksum
                 if len(cur_obj.checksum)>0
                 else cur_obj.chksum()), "Checksums not identical after upload"
 
     s_ipath = IrodsPath(session, "~/empty/more_data")
     assert s_ipath.collection_exists(), "Subfolder not uploaded"
     s_ipath = IrodsPath(session, "~/empty/more_data/polarbear.txt")
     assert s_ipath.dataobject_exists(), "File in subfolder not uploaded"
-    obj = get_dataobject(session=session, path=s_ipath)
+    obj = s_ipath.dataobject
     assert _calc_checksum(testdata / "more_data" / "polarbear.txt")== \
         (obj.checksum if len(obj.checksum)>0 else obj.chksum()), \
             "Checksums not identical after upload"
 
     # download
-    sync_data(session=session,
+    sync(session=session,
         source=ipath,
         target=tmpdir,
         max_level=None,
         dry_run=False,
         copy_empty_folders=True)
 
     for cur_file in list(testdata.glob("*")):
```

### Comparing `ibridges-0.1.6/docker/irods_client/tests/test_ticket.py` & `ibridges-0.2.0/docker/irods_client/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docker-compose.yml` & `ibridges-0.2.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docs/Makefile` & `ibridges-0.2.0/docs/Makefile`

 * *Files 25% similar despite different names*

```diff
@@ -8,13 +8,16 @@
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
-.PHONY: help Makefile
+.PHONY: help Makefile clean
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+clean:
+	rm -r $(BUILDDIR) $(SOURCEDIR)/api/generated
```

### Comparing `ibridges-0.1.6/docs/make.bat` & `ibridges-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docs/source/api.rst` & `ibridges-0.2.0/docs/source/api/full_reference.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-API Reference
-=============
-
-
-Submodules
-----------
+Full Reference
+==============
 
 
 ibridges.data\_operations module
 --------------------------------
 
 .. automodule:: ibridges.data_operations
    :members:
@@ -102,32 +98,14 @@
 
 .. automodule:: ibridges.session
    :members:
    :undoc-members:
    :show-inheritance:
 
 
-ibridges.sync module
---------------------
-
-.. automodule:: ibridges.sync
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-
 ibridges.tickets module
 -----------------------
 
 .. automodule:: ibridges.tickets
    :members:
    :undoc-members:
    :show-inheritance:
-
-
-.. Module contents
-.. ---------------
-
-.. .. automodule:: ibridges
-..    :members:
-..    :undoc-members:
-..    :show-inheritance:
```

### Comparing `ibridges-0.1.6/docs/source/cli.rst` & `ibridges-0.2.0/docs/source/cli.rst`

 * *Files 6% similar despite different names*

```diff
@@ -23,39 +23,49 @@
 .. code:: shell
 
     ibridges init some_irods_env_file.json
 
 This will most likely ask for your password. After filling this in, iBridges will cache your password, so that
 you will not have to type it in every time you use an iBridges operation. This is especially useful if you want
 to execute scripts that run in the background. Note that the time your cached password is valid depends on the
-administrator settings of your iRods server.
+administrator settings of your iRODS server.
 
 iBridges stores the location of your irods environment file in `~/.ibridges/ibridges_cli.json`. You can safely delete
 this file if somehow it gets corrupted. If you have the irods environment in the default location, it can still be
 useful to cache the password so that the next commands do not ask for your password anymore:
 
 .. code:: shell
 
     ibridges init
 
 
 Listing remote files
 --------------------
 
-To list the dataobjects and collections that are available on the iRods server, you can use the `ibridges list` command:
+To list the dataobjects and collections that are available on the iRODS server, you can use the `ibridges list` command:
 
 .. code:: shell
 
-    ibridges list "irods:some_collection"
+    ibridges list "irods:/path/to/some_collection"
+
+If you don't supply a collection to display, it will list the data objects and collections in your `irods_home` directory which you can specify in your `~/.irods/irods_environment.json`.
+
+If you want to list a collection in your `irods_home`, you can use `~` as an abbreviation:
+
+.. code:: shell
+
+    ibridges list "irods:~/collection_in_home"
+
+
+Please try to avoid spaces in collection and data object names! If you really need them, you must enclose the path with `"`. That also holds true for local paths.
 
-If you don't supply a collection to display, it will list the data objects and collections in your `irods_home` directory.
 
 .. note::
 
-    Note that all data objects and collections on the iRods server are always preceded with "irods:". This is
+    Note that all data objects and collections on the iRODS server are always preceded with "irods:". This is
     done to distinguish local and remote files.
 
 
 Downloading data
 ----------------
 
 The basic command to download a data object or collection is `ibridges download`:
@@ -69,24 +79,24 @@
 There are two more options: `--overwrite` to allow the download command to overwrite a local file and
 `--resource` to set the resource to download the data from. See `ibridges download --help` for more details.
 
 
 Uploading data
 --------------
 
-The command to upload files and directories to an iRods server is similar to the `download` command:
+The command to upload files and directories to an iRODS server is similar to the `download` command:
 
 .. code:: shell
 
     ibridges upload my_file "irods:~/some_collection"
 
 .. note::
 
-    In contrast to the `download`` command, the `upload`` command always needs a desination collection or data
-    object.
+    In contrast to the `download`` command, the `upload`` command always needs a 
+    destination collection or data object.
 
 
 Synchronizing data
 ------------------
 
 In some cases, instead of downloading/uploading your data, you might want to synchronize data between local
 folders and collections. The `sync` command does this synchronization and only transfers files/directories
```

### Comparing `ibridges-0.1.6/docs/source/conf.py` & `ibridges-0.2.0/docs/source/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 author = 'Christine Staiger'
 release = '0.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.napoleon', "sphinx.ext.autodoc", "sphinx_autodoc_typehints",
-              'sphinx_rtd_theme', "sphinx_inline_tabs", "sphinx_copybutton"]
+              'sphinx_rtd_theme', "sphinx_inline_tabs", "sphinx_copybutton",
+              "sphinx.ext.autosummary"]
 
 templates_path = ['_templates']
 exclude_patterns = []
 
 
 
 # -- Options for HTML output -------------------------------------------------
```

### Comparing `ibridges-0.1.6/docs/source/faq.rst` & `ibridges-0.2.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/docs/source/index.rst` & `ibridges-0.2.0/docs/source/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -14,23 +14,29 @@
    broken or not implemented yet. We appreciate help, issues and bug report in our issue tracker on `github <https://github.com/UtrechtUniversity/iBridges>`__.
 
 
 iBridges is a wrapper around the `python-irodsclient <https://github.com/irods/python-irodsclient>`__. While the
 python-irodsclient is very powerful and feature rich, we aim to provide an easier API for users (mainly researchers)
 that do not have any technical knowledge of iRods.
 
+We provide extensive tutorials on how to work with data in iRODS. Please consult our `iBridges <https://github.com/UtrechtUniversity/iBridges/tree/main/tutorials>`__.
+
 .. toctree::
    :hidden:
    :maxdepth: 2
    :caption: Contents:
 
    quickstart
+
+   install
+   sync
+   ipath
    cli
    faq
-   api
+   api/main
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `ibridges-0.1.6/docs/source/quickstart.rst` & `ibridges-0.2.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/ibridges/data_operations.py` & `ibridges-0.2.0/ibridges/path.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,485 +1,561 @@
-"""Collections and data objects."""
+"""A class to handle iRODS paths."""
 from __future__ import annotations
 
-import os
-import warnings
-from pathlib import Path
-from typing import Optional, Union
-
-import irods.collection
-import irods.data_object
-import irods.exception
-import irods.keywords as kw
+from collections import defaultdict
+from pathlib import PurePosixPath
+from typing import Iterable, Optional, Union
+
+import irods
 from irods.models import DataObject
 
 import ibridges.icat_columns as icat
-from ibridges.path import IrodsPath
-from ibridges.session import Session
 
-NUM_THREADS = 4
 
-def get_dataobject(session: Session,
-                   path: Union[str, IrodsPath]) -> irods.data_object.iRODSDataObject:
-    """Instantiate an iRODS data object.
+class IrodsPath():
+    """A class analogous to the pathlib.Path for accessing iRods data.
 
-    Parameters
-    ----------
-    session :
-        Session with connection to the server to get the data object from.
-    path : str
-        Name of an iRODS data object.
-
-    Raises
-    ------
-    ValueError:
-        If the path is pointing to a collection and not a data object.
+    The IrodsPath can be used in much the same way as a Path from the pathlib library.
+    Not all methods and attributes are implemented, and some methods/attributes behave
+    subtly different from the pathlib implementation. They mostly do with the expansion
+    of the home directory. With the IrodsPath, the '~' is used to denote the irods_home
+    directory set in the Session object. So, for example the name of an irods path is
+    always the name of the collection/subcollection, which is different from the pathlib
+    behavior in some cases.
+    """
+
+    _current_working_path = ""
+
+    def __init__(self, session, *args):
+        """Initialize IrodsPath object similar to the Path object.
+
+        It does take an extra argument in session.
+
+        Parameters
+        ----------
+        session:
+            Session that is used for the ipath.
+        args:
+            Specification of the path. For example: "x/z" or "x", "z".
+
+        Raises
+        ------
+        ValueError:
+            If the provided session does not have an 'irods_session' attribute.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~")  # Get an iRods path of the irods_home collection.
+        >>> IrodsPath(session, "/zone/home/some_collection")  # Absolute path.
+        >>> IrodsPath(session, "some_collection")  # Relative path.
+        >>> IrodsPath(session, "~/some_collection")  # Same as above.
+
+        """
+        self.session = session
+        if not hasattr(session, "irods_session"):
+            raise ValueError(f'{str(self)} does not have a valid session.')
+        # We don't want recursive IrodsPaths, so we take the
+        # path outside of the IrodsPath object.
+        args = [a._path if isinstance(a, IrodsPath) else a
+                for a in args]
+        self._path = PurePosixPath(*args)
+        super().__init__()
+
+    def absolute(self) -> IrodsPath:
+        """Return the absolute path.
+
+        This method does the expansion of the '~' and '.' symbols.
+
+        Returns
+        -------
+            The absolute IrodsPath, without any '~' or '.'.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~").absolute()
+        IrodsPath(/, zone, user)
+
+        """
+        # absolute path
+        if len(self._path.parts) == 0:
+            return IrodsPath(self.session, self.session.home)
+        if self._path.parts[0] == "~" or self._path.parts[0] == ".":
+            begin, end = self.session.home, self._path.parts[1:]
+        elif self._path.parts[0] == "/":
+            begin, end = "/", self._path.parts[1:]
+        else:
+            begin, end = self.session.home, self._path.parts
+        abs_str = str(PurePosixPath(begin, *end))
+        return IrodsPath(self.session, abs_str)
 
-    Returns
-    -------
-    iRODSDataObject
-        Instance of the data object with `path`.
 
-    """
-    path = IrodsPath(session, path)
-    if path.dataobject_exists():
-        return session.irods_session.data_objects.get(str(path))
-    if path.collection_exists():
-        raise ValueError("Error retrieving data object, path is linked to a collection."
-                         " Use get_collection instead to retrieve the collection.")
+    def __str__(self) -> str:
+        """Get the absolute path if converting to string."""
+        return str(self.absolute()._path)
 
-    raise irods.exception.DataObjectDoesNotExist(path)
+    def __repr__(self) -> str:
+        """Representation of the IrodsPath object in line with a Path object."""
+        return f"IrodsPath({', '.join(self._path.parts)})"
 
-def get_collection(session: Session,
-                   path: Union[str, IrodsPath]) -> irods.collection.iRODSCollection:
-    """Instantiate an iRODS collection.
+    def __truediv__(self, other) -> IrodsPath:
+        """Ensure that we can append just like the Path object."""
+        return self.__class__(self.session, self._path, other)
 
-    Parameters
-    ----------
-    session :
-        Session to get the collection from.
-    path : str
-        Name of an iRODS collection.
-
-    Raises
-    ------
-    ValueError:
-        If the path points to a dataobject and not a collection.
+    def __getattribute__(self, attr):
+        """Make the IrodsPath transparent so that some Path functionality is available."""
+        if attr in ["parts"]:
+            return self._path.__getattribute__(attr)
+        return super().__getattribute__(attr)
 
-    Returns
-    -------
-    iRODSCollection
-        Instance of the collection with `path`.
+    def joinpath(self, *args) -> IrodsPath:
+        """Concatenate another path to this one.
 
-    """
-    path = IrodsPath(session, path)
-    if path.collection_exists():
-        return session.irods_session.collections.get(str(path))
-    if path.dataobject_exists():
-        raise ValueError("Error retrieving collection, path is linked to a data object."
-                         " Use get_dataobject instead to retrieve the data object.")
-    raise irods.exception.CollectionDoesNotExist(path)
+        Returns
+        -------
+            The concatenated path.
 
-def obj_replicas(obj: irods.data_object.iRODSDataObject) -> list[tuple[int, str, str, int, str]]:
-    """Retrieve information about replicas (copies of the file on different resources).
+        Examples
+        --------
+        >>> IrodsPath(session, "~").joinpath("x", "y")
+        IrodsPath(~, x, y)
 
-    It does so for a data object in the iRODS system.
+        """
+        return IrodsPath(self.session, self._path, *args)
 
-    Parameters
-    ----------
-    obj : irods.data_object.iRODSDataObject
-        The data object
+    @property
+    def parent(self) -> IrodsPath:
+        """Return the parent directory of the current directory.
 
-    Returns
-    -------
-    list(tuple(int, str, str, int, str)):
-        List with tuple where each tuple contains replica index/number, resource name on which
-        the replica is stored about one replica, replica checksum, replica size,
-        replica status of the replica
+        Returns
+        -------
+            The parent just above the current directory
 
-    """
-    #replicas = []
-    repl_states = {
-        '0': 'stale',
-        '1': 'good',
-        '2': 'intermediate',
-        '3': 'write-locked'
-    }
-
-    replicas = [(r.number, r.resource_name, r.checksum,
-                 r.size, repl_states.get(r.status, r.status)) for r in obj.replicas]
-
-    return replicas
-
-def is_dataobject(item) -> bool:
-    """Determine if item is an iRODS data object."""
-    return isinstance(item, irods.data_object.iRODSDataObject)
-
-def is_collection(item) -> bool:
-    """Determine if item is an iRODS collection."""
-    return isinstance(item, irods.collection.iRODSCollection)
-
-def _obj_put(session: Session, local_path: Union[str, Path], irods_path: Union[str, IrodsPath],
-             overwrite: bool = False, resc_name: str = '', options: Optional[dict] = None):
-    """Upload `local_path` to `irods_path` following iRODS `options`.
+        Examples
+        --------
+        >>> IrodsPath(session, "/zone/home/user").parent
+        IrodsPath("/", "zone", "home")
+        >>> IrodsPath(session, "~").parent
+        IrodsPath("/", "zone", "home")
 
-    Parameters
-    ----------
-    session :
-        Session to upload the object.
-    local_path : str or Path
-        Path of local file.
-    irods_path : str or IrodsPath
-        Path of iRODS data object or collection.
-    resc_name : str
-        Optional resource name.
-    overwrite :
-        Whether to overwrite the object if it exists.
-    options :
-        TODO: this seems currently unused?
+        """
+        return IrodsPath(self.session, self.absolute()._path.parent)  # pylint: disable=protected-access
 
-    """
-    local_path = Path(local_path)
-    irods_path = IrodsPath(session, irods_path)
+    @property
+    def name(self) -> str:
+        """Return the name of the data object or collection.
 
-    if not local_path.is_file():
-        raise ValueError("local_path must be a file.")
+        Returns
+        -------
+            The name of the object/collction, similarly to pathlib.
 
-    # Check if irods object already exists
-    obj_exists = IrodsPath(session,
-                           irods_path / local_path.name).dataobject_exists() \
-                 or irods_path.dataobject_exists()
-
-    if options is None:
-        options = {}
-    options.update({
-        kw.NUM_THREADS_KW: NUM_THREADS,
-        kw.REG_CHKSUM_KW: '',
-        kw.VERIFY_CHKSUM_KW: ''
-    })
-
-    if resc_name not in ['', None]:
-        options[kw.RESC_NAME_KW] = resc_name
-    if overwrite or not obj_exists:
-        session.irods_session.data_objects.put(local_path, str(irods_path), **options)
-    else:
-        raise irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG
-
-def _obj_get(session: Session, irods_path: Union[str, IrodsPath], local_path: Union[str, Path],
-             overwrite: bool = False, resc_name: Optional[str] = '',
-             options: Optional[dict] = None):
-    """Download `irods_path` to `local_path` following iRODS `options`.
 
-    Parameters
-    ----------
-    session :
-        Session to get the object from.
-    irods_path : str or IrodsPath
-        Path of iRODS data object.
-    local_path : str or Path
-        Path of local file or directory/folder.
-    overwrite :
-        Whether to overwrite the local file if it exists.
-    resc_name:
-        Name of the resource to get the object from.
-    options : dict
-        iRODS transfer options.
+        Examples
+        --------
+        >>> IrodsPath(session, "/zone/home/user")
+        "user"
 
-    """
-    irods_path = IrodsPath(session, irods_path)
-    if not irods_path.dataobject_exists():
-        raise ValueError("irods_path must be a data object.")
-    if options is None:
-        options = {}
-    options.update({
-        kw.NUM_THREADS_KW: NUM_THREADS,
-        kw.VERIFY_CHKSUM_KW: '',
-        })
-    if overwrite:
-        options[kw.FORCE_FLAG_KW] = ''
-    if resc_name not in ['', None]:
-        options[kw.RESC_NAME_KW] = resc_name
-    #Quick fix for #126
-    if Path(local_path).is_dir():
-        local_path = Path(local_path).joinpath(irods_path.parts[-1])
-    session.irods_session.data_objects.get(str(irods_path), local_path, **options)
-
-def _create_irods_dest(local_path: Path, irods_path: IrodsPath
-                       ) -> list[tuple[Path, IrodsPath]]:
-    """Assembles the irods destination paths for upload of a folder."""
-    upload_path = irods_path.joinpath(local_path.name)
-    paths = [(str(Path(root).relative_to(local_path)), f)
-             for root, _, files in os.walk(local_path) for f in files]
-
-    source_to_dest = [(local_path.joinpath(folder.lstrip(os.sep), file_name),
-                       upload_path.joinpath(folder.lstrip(os.sep), file_name))
-                       for folder, file_name in paths]
-
-    return source_to_dest
-
-def _create_irods_subtree(local_path: Path, irods_path: IrodsPath):
-    # create all collections from folders including empty ones
-    folders = [Path(root).relative_to(local_path).joinpath(f)
-               for root, folders, _ in os.walk(local_path) for f in folders]
-    for folder in folders:
-        IrodsPath.create_collection(irods_path.session,
-                                    irods_path.joinpath(local_path.parts[-1], *folder.parts))
-
-def _upload_collection(session: Session, local_path: Union[str, Path],
-                       irods_path: Union[str, IrodsPath],
-                       overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
-                       copy_empty_folders: bool = True, options: Optional[dict] = None):
-    """Upload a local directory to iRODS.
+        """
+        return self.absolute().parts[-1]
 
-    Parameters
-    ----------
-    session :
-        Session to upload the collection to.
-    local_path : Path
-        Absolute path to the directory to upload
-    irods_path : IrodsPath
-        Absolute irods destination path
-    overwrite : bool
-        If data already exists on iRODS, overwrite
-    ignore_err : bool
-        If an error occurs during upload, and ignore_err is set to True, any errors encountered
-        will be transformed into warnings and iBridges will continue to upload the remaining files.
-        By default all errors will stop the process of uploading.
-    resc_name : str
-        Name of the resource to which data is uploaded, by default the server will decide
-    copy_empty_folders : bool
-        Create collection even if the corresponding source folder is empty.
-    options : dict
-        More options for the upload
+    def remove(self):
+        """Remove the data behind an iRODS path.
 
-    """
-    local_path = Path(local_path)
-    irods_path = IrodsPath(session, irods_path)
-    # get all files and their relative path to local_path
-    if not local_path.is_dir():
-        raise ValueError("local_path must be a directory.")
-
-    if copy_empty_folders:
-        _create_irods_subtree(local_path, irods_path)
-    source_to_dest = _create_irods_dest(local_path, irods_path)
-    for source, dest in source_to_dest:
-        _ = create_collection(session, dest.parent)
-        try:
-            _obj_put(session, source, dest, overwrite, resc_name, options)
-        except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG:
-            warnings.warn(f'Object already exists\tSkipping {source}')
-        except KeyError as e:
-            if ignore_err is True:
-                warnings.warn(f'Upload failed: {source}\n'+repr(e))
-            else:
-                raise ValueError(f'Upload failed: {source}: '+repr(e)) from e
+        Raises
+        ------
+        PermissionError:
+            If the user has insufficient permission to remove the data.
 
-def _create_local_dest(session: Session, irods_path: IrodsPath, local_path: Path
-                       ) -> list[tuple[IrodsPath, Path]]:
-    """Assembles the local destination paths for download of a collection."""
-    # get all data objects
-    coll = get_collection(session, irods_path)
-    all_objs = _get_data_objects(session, coll)
-
-    download_path = local_path.joinpath(irods_path.name.lstrip('/'))
-    source_to_dest: list[tuple[IrodsPath, Path]] = []
-    for subcoll_path, obj_name, _, _ in all_objs:
-        cur_ipath = IrodsPath(session, subcoll_path, obj_name)
-        cur_lpath = (download_path / IrodsPath(session, subcoll_path).relative_to(irods_path)
-                                   / obj_name)
-        source_to_dest.append((cur_ipath, cur_lpath))
-    return source_to_dest
-
-def _create_local_subtree(session: Session, irods_path: IrodsPath, local_path: Path):
-
-    coll = get_collection(session, irods_path)
-    subcolls = _get_subcoll_paths(session, coll)
-    # create all folders from collections including empty ones
-    folders = [local_path.joinpath(coll.name, *sc.relative_to(irods_path).parts)
-               for sc in subcolls]
-    for folder in folders:
-        folder.mkdir(parents=True, exist_ok=True)
-
-def _download_collection(session: Session, irods_path: Union[str, IrodsPath], local_path: Path,
-                         overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
-                         copy_empty_folders: bool = True, options: Optional[dict] = None):
-    """Download a collection to the local filesystem.
+        Examples
+        --------
+        >>> IrodsPath(session, "/home/zone/user/some_collection").remove()
 
-    Parameters
-    ----------
-    session :
-        Session to download the collection from.
-    irods_path : IrodsPath
-        Absolute irods source path pointing to a collection
-    local_path : Path
-        Absolute path to the destination directory
-    overwrite : bool
-        Overwrite existing local data
-    ignore_err : bool
-        If an error occurs during download, and ignore_err is set to True, any errors encountered
-        will be transformed into warnings and iBridges will continue to download the remaining
-        files.
-        By default all errors will stop the process of uploading.
-    resc_name : str
-        Name of the resource from which data is downloaded, by default the server will decide
-    copy_empty_folders : bool 
-        Create a respective folder for empty colletions.
-    options : dict
-        More options for the download
+        """
+        try:
+            if self.collection_exists():
+                coll = self.session.irods_session.collections.get(str(self))
+                coll.remove()
+            elif self.dataobject_exists():
+                obj = self.session.irods_session.data_objects.get(str(self))
+                obj.unlink()
+        except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
+            raise PermissionError(
+                f"While removing {self}: iRODS server forbids action.") from exc
+
+    @staticmethod
+    def create_collection(session,
+                          coll_path: Union[IrodsPath, str]) -> irods.collection.iRODSCollection:
+        """Create a collection and all parent collections that do not exist yet.
+
+        Parameters
+        ----------
+        session:
+            Session for which the collection is created.
+        coll_path:
+            Irods path to the collection to be created.
+
+        Raises
+        ------
+        PermissionError:
+            If the collection cannot be created due to insufficient permissions.
+
+        Returns
+        -------
+        collection:
+            The newly created collection.
+
+        Examples
+        --------
+        >>> IrodsPath.create_collection(session, "/zone/home/user/some_collection")
+        >>> IrodsPath.create_collection(session, IrodsPath(session, "~/some_collection"))
 
-    """
-    irods_path = IrodsPath(session, irods_path)
-    if not irods_path.collection_exists():
-        raise ValueError("irods_path must be a collection.")
-
-    if copy_empty_folders:
-        _create_local_subtree(session, irods_path, local_path)
-    source_to_dest = _create_local_dest(session, irods_path, local_path)
-
-    for source, dest in source_to_dest:
-        # ensure local folder exists
-        if not dest.parent.is_dir():
-            os.makedirs(dest.parent)
+        """
         try:
-            _obj_get(session, source, dest, overwrite, resc_name, options)
-        except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG:
-            warnings.warn(f'File already exists\tSkipping {source}')
-        except KeyError as e:
-            if ignore_err is True:
-                warnings.warn(f'Download failed: {source}i\n'+repr(e))
-            else:
-                raise ValueError(f'Download failed: {source}: '+repr(e)) from e
+            return session.irods_session.collections.create(str(coll_path))
+        except irods.exception.CAT_NO_ACCESS_PERMISSION as error:
+            raise PermissionError(f"Cannot create {str(coll_path)}, no access.") from error
+        except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
+            raise PermissionError(
+                "While creating collection '{coll_path}': iRODS server forbids action.") from exc
+
+    def rename(self, new_name: Union[str, IrodsPath]) -> IrodsPath:
+        """Change the name or the path of a data object or collection.
+
+        New collections on the path will be created.
+
+        Parameters
+        ----------
+        new_name: str or IrodsPath
+            new name or a new full path
+
+
+        Raises
+        ------
+        ValueError:
+            If the new path already exists, or the path is in a different zone.
+        PermissionError:
+            If the new collection cannot be created.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/some_collection").rename("~/new_collection")
+
+        """
+        if not self.exists():
+            raise ValueError(f'str{self} does not exist.')
+
+        # Build new path
+        if str(new_name).startswith('/'+self.session.zone):
+            new_path = IrodsPath(self.session, new_name)
+        else:
+            new_path = self.parent.joinpath(new_name)
 
-def upload(session: Session, local_path: Union[str, Path], irods_path: Union[str, IrodsPath],
-           overwrite: bool = False, ignore_err: bool = False,
-           resc_name: str = '', copy_empty_folders: bool = True, options: Optional[dict] = None):
-    """Upload a local directory or file to iRODS.
+        try:
+            # Make sure new path exists on iRODS server
+            if not new_path.parent.exists():
+                self.create_collection(self.session, new_path.parent)
 
-    Parameters
-    ----------
-    session :
-        Session to upload the data to.
-    local_path : Path
-        Absolute path to the directory to upload
-    irods_path : IrodsPath
-        Absolute irods destination path
-    overwrite : bool
-        If data object or collection already exists on iRODS, overwrite
-    ignore_err : bool
-        If an error occurs during upload, and ignore_err is set to True, any errors encountered
-        will be transformed into warnings and iBridges will continue to upload the remaining files.
-        By default all errors will stop the process of uploading.
-    resc_name : str
-        Name of the resource to which data is uploaded, by default the server will decide
-    copy_empty_folders : bool
-        Create respective iRODS collection for empty folders. Default: True.
-    options : dict
-        More options for the upload
-
-    Raises
-    ------
-    ValueError:
-        If the local_path is not a valid filename of directory.
-    PermissionError:
-        If the iRODS server does not allow the collection or data object to be created.
+            if self.dataobject_exists():
+                self.session.irods_session.data_objects.move(str(self), str(new_path))
+            else:
+                self.session.irods_session.collections.move(str(self), str(new_path))
+            return new_path
 
-    """
-    local_path = Path(local_path)
-    try:
-        if local_path.is_dir():
-            _upload_collection(session, local_path, irods_path, overwrite, ignore_err,
-                               resc_name, copy_empty_folders, options)
-        elif local_path.is_file():
-            _obj_put(session, local_path, irods_path, overwrite, resc_name, options)
-        else:
-            raise FileNotFoundError(f"Cannot find local file '{local_path}', check the path.")
-    except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-        raise PermissionError(
-            f"During upload operation to '{irods_path}': iRODS server forbids action.") from exc
-    except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG as exc:
-        raise FileExistsError(f"Dataset or collection (in) {irods_path} already exists. "
-                              "Use overwrite=True to overwrite the existing file(s).") from exc
-
-def download(session: Session, irods_path: Union[str, IrodsPath], local_path: Union[str, Path],
-             overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
-             copy_empty_folders: bool = True, options: Optional[dict] = None):
-    """Download a collection or data object to the local filesystem.
+        except irods.exception.SAME_SRC_DEST_PATHS_ERR as err:
+            raise ValueError(f'Path {new_path} already exists.') from err
+        except irods.exception.SYS_CROSS_ZONE_MV_NOT_SUPPORTED as err:
+            raise ValueError(
+                    f'Path {new_path} needs to start with /{self.session.zone}/home') from err
+        except irods.exception.CAT_NO_ACCESS_PERMISSION as err:
+            raise PermissionError(f'Not allowed to move data to {new_path}') from err
+
+
+    def collection_exists(self) -> bool:
+        """Check if the path points to an iRODS collection.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/does_not_exist").collection_exists()
+        False
+        >>> IrodsPath(session, "~/some_dataobj").collection_exists()
+        False
+        >>> IrodsPath(session, "~/some_collection").collection_exists()
+        True
+
+        """
+        return self.session.irods_session.collections.exists(str(self))
+
+    def dataobject_exists(self) -> bool:
+        """Check if the path points to an iRODS data object.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/does_not_exist").dataobject_exists()
+        False
+        >>> IrodsPath(session, "~/some_collection").dataobject_exists()
+        False
+        >>> IrodsPath(session, "~/some_dataobj").dataobject_exists()
+        True
+
+        """
+        return self.session.irods_session.data_objects.exists(str(self))
+
+    def exists(self) -> bool:
+        """Check if the path already exists on the iRODS server.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/does_not_exist").exists()
+        False
+        >>> IrodsPath(session, "~/some_collection").exists()
+        True
+        >>> IrodsPath(session, "~/some_dataobj").exists()
+        True
+
+        """
+        return self.dataobject_exists() or self.collection_exists()
+
+    @property
+    def collection(self) -> irods.collection.iRODSCollection:
+        """Instantiate an iRODS collection.
+
+        Raises
+        ------
+        ValueError:
+            If the path points to a dataobject and not a collection.
+        CollectionDoesNotExist:
+            If the path does not point to a dataobject or a collection.
+
+        Returns
+        -------
+        iRODSCollection
+            Instance of the collection with `path`.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/some_collection").collection
+        <iRODSCollection 21260050 b'some_collection'>
+
+        """
+        if self.collection_exists():
+            return self.session.irods_session.collections.get(str(self))
+        if self.dataobject_exists():
+            raise ValueError("Error retrieving collection, path is linked to a data object."
+                            " Use get_dataobject instead to retrieve the data object.")
+        raise irods.exception.CollectionDoesNotExist(str(self))
+
+    @property
+    def dataobject(self) -> irods.data_object.iRODSDataObject:
+        """Instantiate an iRODS data object.
+
+        Raises
+        ------
+        ValueError:
+            If the path is pointing to a collection and not a data object.
+
+        Returns
+        -------
+        iRODSDataObject
+            Instance of the data object with `path`.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/some_dataobj.txt").dataobject
+        <iRODSDataObject 24490075 some_dataobj.txt>
+
+        """
+        if self.dataobject_exists():
+            return self.session.irods_session.data_objects.get(str(self))
+        if self.collection_exists():
+            raise ValueError("Error retrieving data object, path is linked to a collection."
+                         " Use get_collection instead to retrieve the collection.")
 
-    Parameters
-    ----------
-    session :
-        Session to download the collection from.
-    irods_path : IrodsPath
-        Absolute irods source path pointing to a collection
-    local_path : Path
-        Absolute path to the destination directory
-    overwrite : bool
-        If an error occurs during download, and ignore_err is set to True, any errors encountered
-        will be transformed into warnings and iBridges will continue to download the remaining
-        files.
-        By default all errors will stop the process of downloading.
-    ignore_err : bool
-        Collections: If download of an item fails print error and continue with next item.
-    resc_name : str
-        Name of the resource from which data is downloaded, by default the server will decide.
-    copy_empty_folders : bool
-        Create respective local directory for empty collections.
-    options : dict
-        More options for the download
-
-    Raises
-    ------
-    PermissionError:
-        If the iRODS server (for whatever reason) forbids downloading the file or
-        (part of the) collection.
-    ValueError:
-        If the irods_path is not pointing to either a collection or a data object.
+        raise irods.exception.DataObjectDoesNotExist(str(IrodsPath))
 
-    """
-    irods_path = IrodsPath(session, irods_path)
-    local_path = Path(local_path)
-    try:
-        if irods_path.collection_exists():
-            _download_collection(session, irods_path, local_path, overwrite, ignore_err, resc_name,
-                                 copy_empty_folders, options)
-        elif irods_path.dataobject_exists():
-            _obj_get(session, irods_path, local_path, overwrite, resc_name, options)
-        else:
-            raise ValueError(f"Data object or collection not found: '{irods_path}'")
-    except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-        raise PermissionError(
-            f"During download operation from '{irods_path}': iRODS server forbids action."
-            ) from exc
-    except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG as exc:
-        raise FileExistsError(f"File or directory {local_path} already exists. "
-                              "Use overwrite=True to overwrite the existing file(s).") from exc
-
-def get_size(session: Session, item: Union[irods.data_object.iRODSDataObject,
-                               irods.collection.iRODSCollection]) -> int:
-    """Collect the sizes of a data object or a collection.
 
-    Parameters
-    ----------
-    session :
-        Session with the connection to the item.
-    item : iRODSDataObject or iRODSCollection
-        Collection or data object to get the size of.
+    def walk(self, depth: Optional[int] = None) -> Iterable[IrodsPath]:
+        """Walk on a collection.
 
-    Returns
-    -------
-    int :
-        Total size [bytes] of the iRODS object or all iRODS objects in the collection.
+        This iterates over all collections and data object for the path. If the
+        path is pointing to a data object, it will simply yield this data object.
 
-    """
-    if is_dataobject(item):
-        return item.size
-    all_objs = _get_data_objects(session, item)
-    return sum(size for _, _, size, _ in all_objs)
+        Parameters
+        ----------
+        depth : int
+            The maximum depth relative to the starting collection over which is walked.
+            For example if depth equals 1, then it will iterate only over the subcollections
+            and data objects directly under the starting collection.
+
+        Returns
+        -------
+            Generator that generates all data objects and subcollections in the collection.
+
+        Examples
+        --------
+        >>> for ipath in IrodsPath(session, "~").walk():
+        >>>     print(ipath)
+        IrodsPath(~, x)
+        IrodsPath(~, x, y)
+        IrodsPath(~, x, y, z.txt)
+        >>> for ipath in IrodsPath(session, "~").walk(depth=1):
+        >>>     print(ipath)
+        IrodsPath(~, x)
+
+        """
+        all_data_objects: dict[str, list[IrodsPath]] = defaultdict(list)
+        for path, name, size, checksum in _get_data_objects(self.session, self.collection):
+            abs_path = IrodsPath(self.session, path).absolute()
+            ipath = CachedIrodsPath(self.session, size, True, checksum, path, name)
+            all_data_objects[str(abs_path)].append(ipath)
+        all_collections = _get_subcoll_paths(self.session, self.collection)
+        all_collections = sorted(all_collections, key=str)
+        sub_collections: dict[str, list[IrodsPath]] = defaultdict(list)
+        for cur_col in all_collections:
+            sub_collections[str(cur_col.parent)].append(cur_col)
+
+        yield from _recursive_walk(self, sub_collections, all_data_objects, self, 0, depth)
+
+    def relative_to(self, other: IrodsPath) -> PurePosixPath:
+        """Calculate the relative path compared to our path.
+
+        Can only calculate the relateive path compared to another irods path.
+
+        >>> IrodsPath(session, "~/col/dataobj.txt").relative_to(IrodsPath(session, "~"))
+        PurePosixPath(col, dataobj.txt)
+        >>> IrodsPath(session, "~/col/dataobj.txt").relative_to(IrodsPath(session, "~/col"))
+        PurePosixPath(dataobj.txt)
+        """
+        return PurePosixPath(str(self.absolute())).relative_to(
+            PurePosixPath(str(other.absolute())))
+
+    @property
+    def size(self) -> int:
+        """Collect the sizes of a data object or a collection.
+
+        Returns
+        -------
+        int :
+            Total size [bytes] of the iRODS object or all iRODS objects in the collection.
+
+        Raises
+        ------
+        ValueError:
+            If the path is neither a collection or data object.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/some_collection").size
+        12345
+        >>> IrodsPath(session, "~/some_dataobj.txt").size
+        623
+
+        """
+        if not self.exists():
+            raise ValueError(f"Path '{str(self)}' does not exist;"
+                             " it is neither a collection nor a dataobject.")
+        if self.dataobject_exists():
+            return self.dataobject.size
+        all_objs = _get_data_objects(self.session, self.collection)
+        return sum(size for _, _, size, _ in all_objs)
+
+    @property
+    def checksum(self) -> str:
+        """Checksum of the data object.
+
+        If not calculated yet, it will be computed on the server.
+
+        Returns
+        -------
+            The checksum of the data object.
+
+        Raises
+        ------
+        ValueError
+            When the path does not point to a data object.
+
+        Examples
+        --------
+        >>> IrodsPath(session, "~/some_dataobj.txt").checksum
+        'sha2:XGiECYZOtUfP9lnCGyZaBBkBGLaJJw1p6eoc0GxLeKU='
+
+        """
+        if self.dataobject_exists():
+            dataobj = self.dataobject
+            return dataobj.checksum if dataobj.checksum is not None else dataobj.chksum()
+        if self.collection_exists():
+            raise ValueError("Cannot take checksum of a collection.")
+        raise ValueError("Cannot take checksum of irods path neither a dataobject or collection.")
+
+
+def _recursive_walk(cur_col: IrodsPath, sub_collections: dict[str, list[IrodsPath]],
+                    all_dataobjects: dict[str, list[IrodsPath]], start_col: IrodsPath,
+                    depth: int, max_depth: Optional[int]):
+    if cur_col != start_col:
+        yield cur_col
+    if max_depth is not None and depth >= max_depth:
+        return
+    for sub_col in sub_collections[str(cur_col)]:
+        yield from _recursive_walk(sub_col, sub_collections, all_dataobjects, start_col,
+                                   depth+1, max_depth)
+    yield from sorted(all_dataobjects[str(cur_col)], key=str)
+
+class CachedIrodsPath(IrodsPath):
+    """Cached version of the IrodsPath.
+
+    This version should generally not be used by users, but is used for performance reasons.
+    It will cache the size checksum and whether it is a data object. This can be invalidated
+    when other ibridges operations are used.
+    """
+
+    def __init__(self, session, size: Optional[int], is_dataobj: bool,
+                 checksum: Optional[str], *args):
+        """Initialize CachedIrodsPath.
+
+        Parameters
+        ----------
+        session:
+            Session used for the IrodsPath
+        size:
+            Size of the dataobject, None for collections.
+        is_dataobj:
+            Whether the path points to a data object.`
+        checksum:
+            The checksum of the dataobject, None for collections.
+        args:
+            Remainder of the path
+
+        """
+        self._is_dataobj = is_dataobj
+        self._size = size
+        self._checksum = checksum
+        super().__init__(session, *args)
+
+    @property
+    def size(self) -> int:
+        """See IrodsPath."""
+        if self._size is None:
+            return super().size
+        return self._size
+
+    @property
+    def checksum(self) -> str:
+        """See IrodsPath."""
+        if self._checksum is None:
+            return super().checksum
+        return self._checksum
+
+    def dataobject_exists(self) -> bool:
+        """See IrodsPath."""
+        return self._is_dataobj
+
+    def collection_exists(self) -> bool:
+        """See IrodsPath."""
+        return not self._is_dataobj
 
-def _get_data_objects(session: Session,
+
+def _get_data_objects(session,
                       coll: irods.collection.iRODSCollection) -> list[tuple[str, str, int, str]]:
     """Retrieve all data objects in a collection and all its subcollections.
 
     Parameters
     ----------
     session:
         Session to get the data objects with.
@@ -502,40 +578,16 @@
     data_query = data_query.filter(icat.LIKE(icat.COLL_NAME, coll.path+"/%"))
     for res in data_query.get_results():
         path, name, size, checksum = res.values()
         objs.append((path, name, size, checksum))
 
     return objs
 
-def _get_subcoll_paths(session: Session,
-                     coll: irods.collection.iRODSCollection) -> list:
-    """
-    Retrieves all sub collections in a sub tree starting at coll and returns their IrodsPaths.
-    """
+
+def _get_subcoll_paths(session,
+                       coll: irods.collection.iRODSCollection) -> list:
+    """Retrieve all sub collections in a sub tree starting at coll and returns their IrodsPaths."""
     coll_query = session.irods_session.query(icat.COLL_NAME)
     coll_query = coll_query.filter(icat.LIKE(icat.COLL_NAME, coll.path+"/%"))
 
-    return [IrodsPath(session, p) for r in coll_query.get_results() for p in r.values()]
-
-def create_collection(session: Session,
-                      coll_path: Union[IrodsPath, str]) -> irods.collection.iRODSCollection:
-    """Create a collection and all collections in its path.
-
-    Parameters
-    ----------
-    session:
-        Session to create the collection for.
-    coll_path: IrodsPath
-        Collection path
-
-    Raises
-    ------
-    PermissionError:
-        If creating a collection is not allowed by the server.
-
-    """
-    try:
-        return session.irods_session.collections.create(str(coll_path))
-    except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-        raise PermissionError(
-                f"While creating collection at '{coll_path}': iRODS server forbids action."
-              ) from exc
+    return [CachedIrodsPath(session, None, False, None, p) for r in coll_query.get_results()
+            for p in r.values()]
```

### Comparing `ibridges-0.1.6/ibridges/export_metadata.py` & `ibridges-0.2.0/ibridges/export_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 """Exporting metadata."""
 from __future__ import annotations
 
 from typing import Any, Optional, Union
 
 from irods.collection import iRODSCollection
 
-from ibridges.data_operations import is_collection, is_dataobject
 from ibridges.meta import MetaData
 from ibridges.path import IrodsPath
 from ibridges.session import Session
+from ibridges.util import is_collection, is_dataobject
 
 
 def export_metadata_to_dict(meta: MetaData, session: Session,
                             recursive: bool = True, keys: Optional[list] = None) -> dict:
     """Retrieve the metadata of the item and brings it into dict form.
 
     If the item is a collection all metadata from all subcollections
```

### Comparing `ibridges-0.1.6/ibridges/icat_columns.py` & `ibridges-0.2.0/ibridges/icat_columns.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/ibridges/interactive.py` & `ibridges-0.2.0/ibridges/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Interactive authentication with iRODS server."""
 
 import os
 from getpass import getpass
 from pathlib import Path
 from typing import Optional, Union
 
-from ibridges.session import Session, LoginError, PasswordError
+from ibridges.session import LoginError, PasswordError, Session
 
 DEFAULT_IENV_PATH = Path(os.path.expanduser("~")).joinpath(".irods", "irods_environment.json")
 
 def interactive_auth(password: Optional[str] = None,
                      irods_env_path: Union[None, str, Path] = None) -> Session:
     """Interactive authentication with iRODS server.
```

### Comparing `ibridges-0.1.6/ibridges/meta.py` & `ibridges-0.2.0/ibridges/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 """metadata operations."""
 from __future__ import annotations
 
 from typing import Any, Iterator, Optional, Sequence, Union
 
+import irods
 import irods.exception
 import irods.meta
 
-from ibridges.data_operations import is_dataobject
+from ibridges.util import is_dataobject
 
 
 class MetaData():
-    """Irods metadata operations."""
+    """Irods metadata operations.
 
-    def __init__(self, item):
+    This allows for adding and deleting of metadata entries for data objects
+    and collections.
+
+    Examples
+    --------
+    >>> meta = MetaData(coll)
+    >>> "Author" in meta
+    True
+    >>> for entry in meta:
+    >>>     print(entry.key, entry.value, entry.units)
+    Author Ben
+    Mass 10 kg
+    >>> meta.add("Author", "Emma")
+    >>> meta.set("Author", "Alice")
+    >>> meta.delete("Author")
+    >>> print(meta)
+    {Mass, 10, kg}
+
+    """
+
+    def __init__(self, item: Union[irods.data_object.iRODSDataObject,
+                                   irods.collection.iRODSCollection]):
         """Initialize the metadata object.
 
         Parameters
         ----------
         item
             The data object or collection to attach the metadata object to.
 
@@ -24,15 +46,30 @@
         self.item = item
 
     def __iter__(self) -> Iterator:
         """Iterate over all metadata key/value/units pairs."""
         yield from self.item.metadata.items()
 
     def __contains__(self, val: Union[str, Sequence]) -> bool:
-        """Check whether a key, key/val, key/val/units pairs are in the metadata."""
+        """Check whether a key, key/val, key/val/units pairs are in the metadata.
+
+        Returns
+        -------
+            True if key/val/unit pairs are present in the item.
+
+        Examples
+        --------
+        >>> "Author" in meta
+        True
+        >>> ("Author", "Ben") in meta
+        False
+        >>> ("Release", "2000", "year") in meta
+        True
+
+        """
         if isinstance(val, str):
             val = [val]
         all_attrs = ["name", "value", "units"][:len(val)]
         for meta in self:
             n_same = 0
             for i_attr, attr in enumerate(all_attrs):
                 if getattr(meta, attr) == val[i_attr] or val[i_attr] is None:
@@ -77,14 +114,19 @@
         Raises
         ------
         ValueError:
             If the metadata already exists.
         PermissionError:
             If the metadata cannot be updated because the user does not have sufficient permissions.
 
+        Examples
+        --------
+        >>> meta.add("Author", "Ben")
+        >>> meta.add("Mass", "10", "kg")
+
         """
         try:
             if (key, value, units) in self:
                 raise irods.exception.CATALOG_ALREADY_HAS_ITEM_BY_THAT_NAME()
             self.item.metadata.add(key, value, units)
         except irods.exception.CATALOG_ALREADY_HAS_ITEM_BY_THAT_NAME as error:
             raise ValueError("ADD META: Metadata already present") from error
@@ -109,14 +151,19 @@
             The units of the new entry.
 
         Raises
         ------
         PermissionError:
             If the user does not have sufficient permissions to set the metadata.
 
+        Examples
+        --------
+        >>> meta.set("Author", "Ben")
+        >>> meta.set("mass", "10", "kg")
+
         """
         self.delete(key, None)
         self.add(key, value, units)
 
     def delete(self, key: str, value: Optional[str], units: Optional[str] = None):
         """Delete a metadata entry of an item.
 
@@ -132,14 +179,23 @@
         Raises
         ------
         KeyError:
             If the to be deleted key cannot be found.
         PermissionError:
             If the user has insufficient permissions to delete the metadata.
 
+        Examples
+        --------
+        >>> # Delete the metadata entry with mass 10 kg
+        >>> meta.delete("mass", "10", "kg")
+        >>> # Delete all metadata with key mass  and value 10
+        >>> meta.delete("mass", "10")
+        >>> # Delete all metadata with the key mass
+        >>> meta.delete("mass")
+
         """
         try:
             if value is None:
                 metas = self.item.metadata.get_all(key)
                 value_units = [(m.value, m.units) for m in metas]
                 if (value, units) not in value_units:
                     for meta in metas:
```

### Comparing `ibridges-0.1.6/ibridges/permissions.py` & `ibridges-0.2.0/ibridges/permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/ibridges/resources.py` & `ibridges-0.2.0/ibridges/resources.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/ibridges/rules.py` & `ibridges-0.2.0/ibridges/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Rule operations."""
 import logging
 from typing import Optional
+
 import irods.exception
 import irods.rule
 
 from ibridges.session import Session
 
 
 def execute_rule(session: Session,
```

### Comparing `ibridges-0.1.6/ibridges/search.py` & `ibridges-0.2.0/ibridges/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,28 +49,47 @@
                         + " Please supply either a path, checksum or key_vals.")
 
     # create the query for collections; we only want to return the collection name
     coll_query = session.irods_session.query(icat.COLL_NAME)
     # create the query for data objects; we need the collection name, the data name and its checksum
     data_query = session.irods_session.query(icat.COLL_NAME, icat.DATA_NAME,
                                              icat.DATA_CHECKSUM)
+    data_name_query = session.irods_session.query(icat.COLL_NAME, icat.DATA_NAME,
+                                                  icat.DATA_CHECKSUM)
+    # iRODS queries do not know the 'or' operator, so we need three searches
+    # One for the collection, and two for the data
+    # one data search in case path is a collection path and we want to retrieve all data there
+    # one in case the path is or ends with a file name
     if path:
+        path = IrodsPath(session, path)
+        parent = path.parent
+        name = path.name
+        # all collections starting with path
         coll_query = coll_query.filter(icat.LIKE(icat.COLL_NAME, str(path)))
+
+        # all data objects in path
         data_query = data_query.filter(icat.LIKE(icat.COLL_NAME, str(path)))
+        # all data objects on path.parent with name
+        data_name_query = data_name_query.filter(icat.LIKE(icat.DATA_NAME, name)).filter(
+                                                 icat.LIKE(icat.COLL_NAME, str(parent)))
     if key_vals:
         for key in key_vals:
             data_query.filter(icat.LIKE(icat.META_DATA_ATTR_NAME, key))
             coll_query.filter(icat.LIKE(icat.META_COLL_ATTR_NAME, key))
+            data_name_query.filter(icat.LIKE(icat.META_DATA_ATTR_NAME, key))
             if key_vals[key]:
                 data_query.filter(icat.LIKE(icat.META_DATA_ATTR_VALUE, key_vals[key]))
                 coll_query.filter(icat.LIKE(icat.META_COLL_ATTR_VALUE, key_vals[key]))
+                data_name_query = data_name_query.filter(
+                                    icat.LIKE(icat.META_DATA_ATTR_VALUE, key_vals[key]))
     if checksum:
         data_query = data_query.filter(icat.LIKE(icat.DATA_CHECKSUM, checksum))
+        data_name_query = data_name_query.filter(icat.LIKE(icat.DATA_CHECKSUM, checksum))
     # gather results
-    results = list(data_query.get_results())
+    results = list(data_query.get_results())+list(data_name_query.get_results())
     if checksum is None:
         coll_res = list(coll_query.get_results())
         if len(coll_res) > 0:
             results.extend(coll_res)
 
     for item in results:
         if isinstance(item, dict):
```

### Comparing `ibridges-0.1.6/ibridges/session.py` & `ibridges-0.2.0/ibridges/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,23 @@
         FileNotFoundError:
             If the irods_env parameter is interpreted as a file name and not found.
         TypeError:
             If the irods_env parameter is not a dict, str or Path.
         LoginError:
             If the connection to the iRODS server fails to establish.
 
+        Examples
+        --------
+        >>> session = Session(Path.home() / ".irods" / "irods_environment.json",
+        >>>                    password="your_password", irods_home="/zone/home/user")
+        >>> session = Session(env_dictionary)  # env_dictionary with connection info
+        >>> with Session("irods_environment.json") as session:
+        >>>     # Do operations with the session here.
+        >>>     # The session will be automatically closed on finish/error.
+
         """
         irods_env_path = None
         if isinstance(irods_env, (str, Path)):
             irods_env_path = Path(irods_env)
             if not irods_env_path.is_file():
                 raise FileNotFoundError(f"Cannot find irods environment file '{irods_env}'")
             with irods_env_path.open("r", encoding="utf-8") as envfd:
@@ -89,14 +98,20 @@
         In the iRODS community this is known as 'irods_home', in file system terms
         it would be the current working directory.
 
         Returns
         -------
             The current working directory in the current session.
 
+
+        Examples
+        --------
+        >>> session.home
+        /zone/home/user
+
         """
         return self._irods_env["irods_home"]
 
     @home.setter
     def home(self, value):
         self._irods_env["irods_home"] = value
```

### Comparing `ibridges-0.1.6/ibridges/tickets.py` & `ibridges-0.2.0/ibridges/tickets.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,19 +148,21 @@
             [(ticket string, ticket type, irods obj/coll path, expiry data in epoche)]
 
         """
         user = self.session.username
         self._all_tickets = []
         for row in self.session.irods_session.query(TicketQuery.Ticket).filter(
                 TicketQuery.Owner.name == user):
+            time = row[TicketQuery.Ticket.expiry_ts]
+            time_stamp = datetime.fromtimestamp(int(time)) if time else ""
             self._all_tickets.append(
                 TicketData(row[TicketQuery.Ticket.string],
                            row[TicketQuery.Ticket.type],
                            self._id_to_path(str(row[TicketQuery.Ticket.object_id])),
-                           datetime.fromtimestamp(int(row[TicketQuery.Ticket.expiry_ts]))
+                           time_stamp
                 ))
         return self._all_tickets
 
     def clear(self):
         """Delete all tickets."""
         for tick_data in self.update_tickets():
             self.delete_ticket(tick_data.name)
```

### Comparing `ibridges-0.1.6/ibridges.egg-info/PKG-INFO` & `ibridges-0.2.0/ibridges.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.6
+Version: 0.2.0
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -49,14 +49,15 @@
 Requires-Dist: types-tqdm; extra == "test"
 Requires-Dist: sphinx; extra == "test"
 Requires-Dist: sphinx-rtd-theme; extra == "test"
 Requires-Dist: sphinxcontrib-napoleon; extra == "test"
 Requires-Dist: sphinx-autodoc-typehints; extra == "test"
 Requires-Dist: sphinx_inline_tabs; extra == "test"
 Requires-Dist: sphinx_copybutton; extra == "test"
+Requires-Dist: ruff; extra == "test"
 
 # iBridges
 [![PyPI version](https://badge.fury.io/py/ibridges.svg)](https://badge.fury.io/py/ibridges)
 [![](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-irods.yml/badge.svg?branch=develop)](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-irods.yml) [![](https://github.com/UtrechtUniversity/iBridges/actions/workflows/main.yml/badge.svg?branch=develop)](https://github.com/UtrechtUniversity/iBridges/actions/workflows/main.yml) 
 [![](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-yoda.yml/badge.svg)](https://github.com/UtrechtUniversity/iBridges/actions/workflows/integration-tests-yoda.yml) ![](https://readthedocs.org/projects/ibridges/badge/?version=latest&style=flat-default)
 
 iBridges is library for scientific programmers who are working with data in iRODS. We provide a wrapper around the [python-irodsclient](https://pypi.org/project/python-irodsclient/) to facilitate easy interaction with the iRODS server. iBridges is currently still in very active development.
@@ -105,50 +106,50 @@
 
 ## Usage
 
 Below are some basic examples of the features in iBridges.
 
 ```py
 # Create an iRODS session
-from ibridges import Session
+from ibridges.interactive import interactive_auth
 
-session = Session(irods_env_path="~/.irods/irods_environment.json", password="mypassword")
+session = interactive_auth()
 
 # Upload data
 from ibridges import upload
 
 upload(session, "/your/local/path", "/irods/path")
 
 # Download data
 from ibridges import download
 
 download(session, "/irods/path", "/other/local/path")
 
 ```
 
-## Commandline interface
-To simply upload or download data you do not need to write full python program, we offer a Commandline interface
+## Command line interface
+To simply upload or download data you do not need to write full python program, we offer a command line interface
 
 - Establish a connection
 
   ```bash
   ibridges init
   ```
 
-- List a colletion
+- List a collection
   
   ```bash
   # list your home collection
   ibridges list
   
   # list a different collection in your home
   ibridges list irods:~/<collection>
   
   # list a collection on a different path than your home
-  ibridges. list irods:<full_irods_path>
+  ibridges list irods:<full_irods_path>
   ```
 
 - Upload data
 
   ```bash
   ibridges upload my_file.json irods:~/some_collection
   ```
@@ -158,30 +159,30 @@
   ```bash
   ibridges download irods:~/some_collection/some_object download_dir
   ```
 
 - Synchronise data
 
   ```bash
-      ibridges sync some_local_directory irods:~/some_collection
+  	ibridges sync some_local_directory irods:~/some_collection
   ```
 
 ## Tutorials
 ### Documentation
 - **[ReadTheDocs](https://ibridges.readthedocs.io/en/latest/)**
 
 ### Guides
-- [QuickStart](tutorials/QuickStart.ipynb)
-- [iRODS Paths](tutorials/iRODS_paths.ipynb)
-- [Data synchronisation](tutorials/Data_sync.ipynb)
+- [Manual with examples](tutorials/QuickStart.ipynb)
+- [Tutorial for iRODS paths](tutorials/01-iRODS_paths.ipynb)
+- [Data synchronisation manual](tutorials/Data_sync.ipynb)
 
 ### Beginners tutorials
 - [Setup client configuration](tutorials/01-Setup-and-connect.ipynb)
+- [iRODS Paths](tutorials/01-iRODS_paths.ipynb)
 - [Working with data](tutorials/02-Working-with-data.ipynb)
-- [iRODS and local Paths](tutorials/03-iRODS-Paths.ipynb)
 - [Metadata](tutorials/04-Metadata.ipynb)
 - [Sharing data](tutorials/05-Data-Sharing.ipynb)
 
 ## Authors
 
 **Christine Staiger (Maintainer) [ORCID](https://orcid.org/0000-0002-6754-7647)**
```

### Comparing `ibridges-0.1.6/ibridges.egg-info/SOURCES.txt` & `ibridges-0.2.0/ibridges.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,53 +43,57 @@
 docker/irods_client/tests/test_rules.py
 docker/irods_client/tests/test_session.py
 docker/irods_client/tests/test_sync.py
 docker/irods_client/tests/test_ticket.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
-docs/source/api.rst
 docs/source/cli.rst
 docs/source/conf.py
 docs/source/faq.rst
 docs/source/index.rst
+docs/source/install.rst
+docs/source/ipath.rst
 docs/source/quickstart.rst
+docs/source/sync.rst
+docs/source/api/full_reference.rst
+docs/source/api/main.rst
+docs/source/api/user_reference.rst
 ibridges/__init__.py
 ibridges/__main__.py
 ibridges/_version.py
 ibridges/data_operations.py
 ibridges/export_metadata.py
 ibridges/icat_columns.py
 ibridges/interactive.py
 ibridges/meta.py
 ibridges/path.py
 ibridges/permissions.py
 ibridges/resources.py
 ibridges/rules.py
 ibridges/search.py
 ibridges/session.py
-ibridges/sync.py
 ibridges/tickets.py
+ibridges/util.py
 ibridges.egg-info/PKG-INFO
 ibridges.egg-info/SOURCES.txt
 ibridges.egg-info/dependency_links.txt
 ibridges.egg-info/entry_points.txt
 ibridges.egg-info/requires.txt
 ibridges.egg-info/top_level.txt
 tests/test_irodspath.py
 tests/testdata/bunny.txt
 tests/testdata/subfolder/sun.csv
+tutorials/00-FirstSteps.ipynb
 tutorials/01-Setup-and-connect.ipynb
-tutorials/02-Working-with-data.ipynb
-tutorials/03-iRODS-Paths.ipynb
+tutorials/02-iRODS-paths.ipynb
+tutorials/03-Working-with-data.ipynb
 tutorials/04-Metadata.ipynb
 tutorials/05-Data-Sharing.ipynb
-tutorials/Data_sync.ipynb
-tutorials/QuickStart.ipynb
-tutorials/iRODS_paths.ipynb
+tutorials/06-Data-sync.ipynb
 tutorials/example_rules/example.r
 tutorials/img/DataObject1.png
 tutorials/img/DataObject2.png
 tutorials/img/DataObject3.png
 tutorials/img/DataObject4.png
 tutorials/img/DataObject5.png
 tutorials/img/DataObject6.png
```

### Comparing `ibridges-0.1.6/pyproject.toml` & `ibridges-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "pytest",
     "pytest-cov",
     "ruff",
     "mypy",
     "types-tqdm",
     "sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon",
     "sphinx-autodoc-typehints", "sphinx_inline_tabs", "sphinx_copybutton",
+    "ruff"
 ]
 
 
 [project.scripts]
 ibridges = "ibridges.__main__:main"
 
 [tool.setuptools]
@@ -73,9 +74,9 @@
 max-line-length=100
 max-locals=35
 max-args=10
 
 [tool.ruff]
 exclude = ["_version.py"]
 line-length = 100
-select = ["D", "E", "F", "W", "I", "N"]
-ignore = ["D203", "D213"]
+lint.select = ["D", "E", "F", "W", "I", "N"]
+lint.ignore = ["D203", "D213"]
```

### Comparing `ibridges-0.1.6/tests/testdata/bunny.txt` & `ibridges-0.2.0/tests/testdata/bunny.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tests/testdata/subfolder/sun.csv` & `ibridges-0.2.0/tests/testdata/subfolder/sun.csv`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/01-Setup-and-connect.ipynb` & `ibridges-0.2.0/tutorials/01-Setup-and-connect.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988692434210527%*

 * *Differences: {"'cells'": "{2: {'source': ['To connect to a specific iRODS instance you will need a so-called "*

 * *            '`irods_environment.json` file. This file contains all parameters to establish the '*

 * *            'connection. Your iRODS system administrator or service provider will give you such an '*

 * *            "environment file.']}, 9: {'source': {insert: [(6, 'The `.` shows that it is a hidden "*

 * *            'folder, which can be quite difficult to create in Windows. Below we provide a python '*

 * *            "cod […]*

```diff
@@ -17,15 +17,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "466e791e",
             "metadata": {},
             "source": [
-                "To connect to a specific iRODS instance you will need a so-called `irods_environment.json` file. This file contains all parameters to establish the connection. Your iRODS sysadmin or service provider will give you such an environment file."
+                "To connect to a specific iRODS instance you will need a so-called `irods_environment.json` file. This file contains all parameters to establish the connection. Your iRODS system administrator or service provider will give you such an environment file."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c0dec8b5",
             "metadata": {},
             "source": [
@@ -111,15 +111,15 @@
             "source": [
                 "All iRODS clients (icommands and APIs) expect the above parameters to be stored in a special folder. This folder is called `.irods` and it lies in your home directory:\n",
                 "- Mac: `/Users/<user>/.irods`\n",
                 "- Linux: `/home/<user>/.irods`\n",
                 "- Windows: `C:\\Users\\<user>\\.irods`\n",
                 "\n",
                 "In Mac and Linux you can simply create the folder manually in the file browser.\n",
-                "The `.` shows that it is a hidden folder, which can be quite difficult to create in Windows. Below we provide a python cde snippet which creates the folder:"
+                "The `.` shows that it is a hidden folder, which can be quite difficult to create in Windows. Below we provide a python code snippet which creates the folder:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5196436f",
             "metadata": {},
@@ -349,15 +349,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "33bffc91",
             "metadata": {},
             "source": [
-                "Let us verify that the current working location ineed exists:"
+                "Let us verify that the current working location indeed exists:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6d06932a",
             "metadata": {},
@@ -369,15 +369,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a06f0c7d",
             "metadata": {},
             "source": [
-                "We create an `IrodsPath` which is not a simple text or string, but which is actually connected to iRODS through the `session`. With that we can ask iRODS wether the path indeed is a collection (similar to folder, see chapter about Data).\n",
+                "We create an `IrodsPath` which is not a simple text or string, but which is actually connected to iRODS through the `session`. With that we can ask iRODS whether the path indeed is a collection (similar to folder, see chapter about Data).\n",
                 "\n",
                 "In case the last command gave you a `False`, do not despair. You can set this parameter with."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `ibridges-0.1.6/tutorials/02-Working-with-data.ipynb` & `ibridges-0.2.0/tutorials/04-Metadata.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9567743171683389%*

 * *Differences: {"'cells'": "{0: {'id': 'f9e6811a', 'source': ['# User-defined metadata']}, 1: {'id': '8564525b', "*

 * *            "'source': {insert: [(0, 'Next to system metadata, iRODS allows you to create own "*

 * *            "metadata with data objects and collections.\\n'), (2, 'You can use that metadata to "*

 * *            'describe your data and later search for this data; and it can help you keeping the '*

 * *            "overview of what was the input for an analysis and what is the outcome.\\n'), (3, "*

 * *            '\'\\n\'), […]*

```diff
@@ -1,425 +1,449 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "d3598e82",
+            "id": "f9e6811a",
             "metadata": {},
             "source": [
-                "# Working with data"
+                "# User-defined metadata"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "26ff36c3",
+            "id": "8564525b",
             "metadata": {},
             "source": [
-                "On your computer you can open an Explorer which will show you all the files and the directories. In iRODS we have something similar: we have data objects which you can see for the moment as a file and we have collections which are similar to directories.\n",
+                "Next to system metadata, iRODS allows you to create own metadata with data objects and collections.\n",
                 "\n",
-                "In the course of this and the next tutorials it will become clear that this is only an analogy and that there is more to data objects and collections."
+                "You can use that metadata to describe your data and later search for this data; and it can help you keeping the overview of what was the input for an analysis and what is the outcome.\n",
+                "\n",
+                "<img src=\"img/DataObject5.png\" width=\"400\">\n",
+                "\n",
+                "Technically, iRODS offers metadata as key-value-units triple. Let's investigate this:"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "458b2f0f",
+            "id": "bde731e4",
             "metadata": {},
             "source": [
-                "## Create an iRODS session"
+                "## Add metadata to data objects"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ed555077",
+            "id": "784fdac1",
             "metadata": {},
             "source": [
-                "Again, to work from your Laptop with data in iRODS you will need a `session` as describes in [01-Setup-and-connect](01-Setup-and-connect.ipynb)."
+                "As always: first we have to create an iRODS session:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e5ef4e10",
+            "id": "277459df",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges.interactive import interactive_auth\n",
                 "session = interactive_auth()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "172e153a",
+            "id": "81094d42",
             "metadata": {},
             "source": [
-                "## Create a collection and upload a file"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "9645865a",
-            "metadata": {},
-            "source": [
-                "We will now create a new collection on iRODS in your current iRODS working location:"
+                "Now we can retrieve a data object and insect its metadata."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "716769b9",
+            "id": "69066865",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges.path import IrodsPath\n",
-                "from ibridges.data_operations import create_collection\n",
-                "irods_path = IrodsPath(session, '~')\n",
-                "print(\"Current working location:\", irods_path)\n",
-                "irods_coll_path = irods_path.joinpath('demo')\n",
-                "print(\"New collection name:\", irods_coll_path)\n",
-                "coll = create_collection(session, irods_coll_path)\n",
-                "print(\"New collection is created:\", irods_coll_path.collection_exists())"
+                "from ibridges.meta import MetaData\n",
+                "\n",
+                "irods_coll_path = IrodsPath(session, '~').joinpath('demo')\n",
+                "obj = irods_coll_path.joinpath('demofile.txt').dataobject\n",
+                "\n",
+                "obj_metadata = MetaData(obj)\n",
+                "print(obj_metadata)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2ef9c2fd",
+            "id": "7d9a578b",
             "metadata": {},
             "source": [
-                "Now we will upload a file to that new iRODS collection. In this tutorial we assume that you have a file called `demofile.txt` in your home:\n",
-                "- Linux: `/home/<user>/demofile.txt`\n",
-                "- Mac: `/Users/<user>/demofile.txt`\n",
-                "- Windows: `C:\\Users\\<user>\\demofile.txt`\n",
+                "Most probably you will see no metadata in the above cell. **Note, that system metadata and user-defined metadata are two different entities in a data object!**\n",
+                "With the command `MetaData(obj)` we only retrieve the user-defined metadata.\n",
                 "\n",
-                "Let's check that first."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "cbe34a24",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from pathlib import Path\n",
-                "local_file = Path.expanduser(Path('~')).joinpath('demofile.txt')\n",
-                "if local_file.is_file():\n",
-                "    print('You are good to follow the next steps!')\n",
-                "else:\n",
-                "    print(f'Please create a file {local_file} before you continue')"
+                "<img src=\"img/DataObject4.png\" width=\"400\">"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "eaf9182b",
+            "id": "1fb67574",
             "metadata": {},
             "source": [
-                "Now we can upload that file:"
+                "Now we can add some own metadata. The metadata comes as key-value-units triple:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f6be04e0",
+            "id": "79a1bb89",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges import upload\n",
-                "upload(session, local_file, irods_coll_path)"
+                "obj_metadata.add('Key', 'Value', 'Units')\n",
+                "print(obj_metadata)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "94ace2c2",
+            "id": "dafbeaff",
             "metadata": {},
             "source": [
-                "We now created a new data object in iRODS:\n",
-                "\n",
-                "<img src=\"img/DataObject1.png\" width=\"400\">\n",
-                "\n",
-                "How can we now be sure that the file is uploaded? Remember, when we created the new collection `demo`, we created a python object called `coll`. Let's inspect that:"
+                "Sometimes we do not really have `units`, so we can leave this part empty:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "91b73ddd",
+            "id": "fb439f38",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(coll.name)\n",
-                "print(coll.path)"
+                "obj_metadata.add('Author', 'Christine')\n",
+                "print(obj_metadata)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e41763a3",
+            "id": "3bfbfa71",
             "metadata": {},
             "source": [
-                "Apart from information about its name and its path, a collection also carries a list of `subcollections` and `data_objects`."
+                "We can also add a second author:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "48777591",
+            "id": "bb35166a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(f'Current subcollections in {coll.path}:', coll.subcollections)\n",
-                "print(f'Current data objects in {coll.path}:', coll.data_objects)"
+                "obj_metadata.add('Author', 'Raoul')\n",
+                "print(obj_metadata)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2e3380dc",
+            "id": "116c0f10",
             "metadata": {},
             "source": [
-                "## Download the file and the collection"
+                "You see, that keys in **iRODS metadata keys can have different values**. That is different from python dictionaries where one key can only have one value. **How then to overwrite a value?**"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ef68a87a",
+            "id": "cf6d7f93",
             "metadata": {},
             "source": [
-                "Of course we can also download the data object we have just created. We will download it to your `Downloads` directory on you computer:"
+                "## Overwrite metadata"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e7e770d3",
+            "cell_type": "markdown",
+            "id": "cb5b7fef",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "local_path = Path.expanduser(Path('~')).joinpath('Downloads')\n",
-                "assert local_path.is_dir()"
+                "If you wish to *overwrite* a value, you can first add the new metadata key-value-units triple as above and subsequently remove the old one, you need to specify the whole triple if the metadata contains a units part. As you see the following command will fail:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3d4a6914",
+            "id": "d0cbd9bf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges import download\n",
-                "download(session, irods_coll_path.joinpath('demofile.txt'), local_path)"
+                "obj_metadata.delete('Key', 'Value')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "32a53bfc",
+            "id": "77993416",
             "metadata": {},
             "source": [
-                "You can verify taht the file is downloaded.\n",
-                "Now, what happens if we download the file again?"
+                "While this one will succeed:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2d67068c",
+            "id": "ce98d47c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "download(session, irods_coll_path.joinpath('demofile.txt'), local_path)"
+                "obj_metadata.delete('Key', 'Value', 'Units')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "13e5c96d",
+            "id": "e7f47a59",
             "metadata": {},
             "source": [
-                "You will receive an Exception `OVERWRITE_WITHOUT_FORCE_FLAG`. This means that the file is already there.  \n",
-                "\n",
-                "**Note, both the upload and the download function do not overwrite existing data by default.** \n",
-                "\n",
-                "You can force to overwrite the existing data by setting the flag `overwrite`:"
+                "You can also set all existing values to **one** new value:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "22496425",
+            "id": "c9f0a95b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "download(session, irods_coll_path.joinpath('demofile.txt'), local_path, overwrite=True)"
+                "print(obj_metadata)\n",
+                "obj_metadata.set('Author', 'Maarten')\n",
+                "print(obj_metadata)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bff8110e",
+            "id": "c3f54857",
             "metadata": {},
             "source": [
-                "## System metadata"
+                "## Add metadata to collections"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "74c72c43",
+            "id": "51438d57",
+            "metadata": {},
+            "source": [
+                "The same functionality we saw above, we can use for collections:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "65fb35a5",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Both, collections and data objects in iRODS are labeled automatically with some extra information. This information is called *system metadata*. We already saw the `name` and the `path` for the collection. But there is more!"
+                "coll = irods_coll_path.collection\n",
+                "coll_metadata = MetaData(coll)\n",
+                "print(coll_metadata)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "70f3e9a4",
+            "id": "2af31459",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(f'Collection {coll.name} was created on {coll.create_time}')\n",
-                "print(f'The collection was last modified on {coll.modify_time}')\n",
-                "print(f'The collection was uploaded by and is owned by {coll.owner_name}')"
+                "coll_metadata.add('TypeOfCollection', 'Results')\n",
+                "print(coll_metadata)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "19779512",
+            "id": "d7eacaba",
             "metadata": {},
             "source": [
-                "We can also get some system information about the data object we created by uploading the demo file. To insoect a data object (and also a collection) we have to retrieve it from iRODS. We will use the function `get_dataobject` to do so. Note, for collections the function is called `get_collection`."
+                "## Which metadata can help you keeping an overview?"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "cb48bb74",
+            "metadata": {},
+            "source": [
+                "iRODS metadata can help you keeping an overview while you are working with data and maybe many files which have relations to each other. There are ontologies which define keywords and links between keywords like the **[prov-o Ontology](https://www.w3.org/TR/prov-o/#prov-o-at-a-glance)**.\n",
+                "\n",
+                "Let's see how we can annotate our test data, so that we know that it is test data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bd40cf7c",
+            "id": "bbadefc7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges import get_dataobject, get_collection\n",
-                "obj = get_dataobject(session, irods_coll_path.joinpath('demofile.txt'))"
+                "from datetime import datetime\n",
+                "coll_metadata.add('prov:wasGeneratedBy', 'Christine')\n",
+                "coll_metadata.add('CollectionType', 'testcollection')\n",
+                "obj_metadata.add('prov:SoftwareAgent', 'iRODS jupyter Tutorial')\n",
+                "obj_metadata.add('prov:wasGeneratedBy', 'Maarten')\n",
+                "obj_metadata.add('DataType', 'testdata')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "58906168",
+            "id": "5be8180b",
             "metadata": {},
             "source": [
-                "Now we can inspect the object:"
+                "Now we have some more descriptive metadata that gives us hints, in which context the data was created:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "908b0f87",
+            "id": "a0b8e2d4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(f'Data object {obj.name} was created on {obj.create_time}')\n",
-                "print(f'Data object {obj.name} full path in iRODS is {obj.path}')\n",
-                "print(f'The data object was created on {obj.create_time}')\n",
-                "print(f'The data object was last modified on {obj.modify_time}')\n",
-                "print(f'The data object was uploaded by and is owned by {obj.owner_name}')"
+                "print(coll_metadata)\n",
+                "print(obj_metadata)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "7f721760",
+            "metadata": {},
+            "source": [
+                "## Finding data by their metadata"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "007b5097",
+            "id": "59518813",
             "metadata": {},
             "source": [
-                "**Data objects also carry a `size` and a `checksum`**, with which you can check whether the data reached iRODS completely. Checksums are particularly useful. With the size you can only check whether the length of your local file matches the on in iRODS. However, you cannot see if the contents is really the same. E.g. the length of 'Hello' and 'Hallo' are the same, but they do differ. With a checksum you can detect this. A checksum is a digest of the contents of a file.\n",
+                "Metadata does not only help you to. keep an overview over your data, but can also be used to select and retrieve data. In iBridges you can use the user-defined metadata and some system metadata fields to search for data.\n",
                 "\n",
-                "**Note, both functions, `upload` and `download`, will always calculate and compare the checksums between your computer and iRODS**, to make sure that the data is tranferred correctly. "
+                "In our first example we list all collections and data objects in our iRODS home."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "73727623",
+            "id": "e6918fe7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print('Data object size', obj.size)\n",
-                "print('Data object checksum', obj.checksum)"
+                "from ibridges.search import search_data\n",
+                "result = search_data(session, path=session.home)\n",
+                "print(result)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c0d605fa",
+            "id": "31c88425",
             "metadata": {},
             "source": [
-                "The iRODS full path `obj.path` is the address with which you can get the full data object. Currently, this is the uploaded file and its system metadata\n",
+                "The output is a list of Python dictionaries, where each dictionary contains\n",
+                "\n",
+                "1) Collections: `'COLL_NAME': '/<ZONE>/home/<YOUR PATH>'}`\n",
+                "2) Data Objects: \n",
+                "    ```\n",
+                "    {'COLL_NAME': '/<ZONE>/home/<YOUR PATH>', \n",
+                "     'DATA_NAME': '<OBJECT NAME>', \n",
+                "     'D_DATA_CHECKSUM': '<CHECKSUM>'}\n",
+                "    ```\n",
                 "\n",
-                "<img src=\"img/DataObject2.png\" width=\"400\">"
+                "Now let's try to find data by its metadata. We will have to create a Python dictionary with the metadata keys and the metadata values as search criterion:"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "d3614078",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "5b054794",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Data object replicas"
+                "key_vals = {'prov:wasGeneratedBy': 'Christine'}\n",
+                "result = search_data(session, key_vals=key_vals)\n",
+                "print(result)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "98a206e8",
+            "id": "81d73352",
             "metadata": {},
             "source": [
-                "Usually when we upload a file to another computer we create one new item which can be found under the path that we used to upload the data. \n",
-                "\n",
-                "Some iRODS systems distribute the uploaded data to different storage systems. That means, that the file is stored on several storage systems, but you have one path under which you can find the data and address the data. This is called in iRODS a data object `relpica`. When you download data the system decides for you, which is the most advantageous replica to give to you in terms of speed and integrity.\n",
-                "\n",
-                "<img src=\"img/DataObject3.png\" width=\"400\">\n",
-                "\n",
-                "Let us inspect how many replicas of our file we have in iRODS:"
+                "If we do not want to specify the particular value of the key, we can use a *wildcard*. In iRODS the wildcard is `%`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f4ce4f52",
+            "id": "49a9f17e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges.data_operations import obj_replicas\n",
-                "obj_replicas(obj)"
+                "key_vals = {'prov:wasGeneratedBy': '%'}\n",
+                "result = search_data(session, key_vals=key_vals)\n",
+                "print(result)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9438ebba",
+            "id": "69a2e046",
             "metadata": {},
             "source": [
-                "In Yoda you might have to wait for some time until the data is replicated.\n",
+                "Now we also receive the data object that was generated by *Maarten*.\n",
                 "\n",
-                "The structure of the answer is a list, where each element of this list is structured like this:"
+                "And of course we can combine information about the path and the metadata. they will be connected with `and`. The following search will retrieve all data objects and collections wich are labeled with a metadata key *'prov:wasGeneratedBy'* and whose path has the prefix */nluu12p/home/research-test-christine/demo/*."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4b33598a",
+            "id": "e0d2fad9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "item = obj_replicas(obj)[0]\n",
-                "print('Relplica index:', item[0])\n",
-                "print('Storage system:', item[1])\n",
-                "print('Replica cecksum', item[2])\n",
-                "print('Replica size', item[3])\n",
-                "print('Replica status', item[4])"
+                "key_vals = {'prov:wasGeneratedBy': '%'}\n",
+                "result = search_data(session, path='/nluu12p/home/research-test-christine/%', key_vals=key_vals)\n",
+                "print(result)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0e94ef61",
+            "id": "14bc70b0",
             "metadata": {},
             "source": [
-                "The replica status tells you of this particular copy of the data is verified and ok. It should say `good`. In all other cases please send the whole replica information including the path to your iRODS help."
+                "## Retrieving data"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "946e355c",
+            "metadata": {},
+            "source": [
+                "Now that we have the search results in a list of Python dictionaries, we can use the information to create the full iRODS paths and continue working with them e.g. download them."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ff72b0ca",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ibridges.path import IrodsPath\n",
+                "\n",
+                "paths = [IrodsPath(session, r.get('COLL_NAME', '')).joinpath(r.get('DATA_NAME', '')) for r in result]\n",
+                "print(paths)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1143fc1f",
+            "id": "4072812e",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `ibridges-0.1.6/tutorials/03-iRODS-Paths.ipynb` & `ibridges-0.2.0/tutorials/05-Data-Sharing.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9532191001400561%*

 * *Differences: {"'cells'": "{1: {'id': 'ea97cc95', 'source': ['In this tutorial we will show you how to share "*

 * *            'your data with other users in the iRODS system. To see the effects it is helpful to '*

 * *            "team up with a colleague!!!']}, 2: {'id': 'd81b1269', 'source': ['## What are "*

 * *            "permissions']}, 3: {'id': '48815ec5', 'source': {insert: [(0, 'Permissions in iRODS "*

 * *            'are part of the data objects and collections. They give information and they allow '*

 * *            "other users o […]*

```diff
@@ -1,270 +1,339 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "b814e80d",
+            "id": "b34804ad",
             "metadata": {},
             "source": [
-                "# A word on local paths and iRODS paths"
+                "# Data sharing - iRODS permissions"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "18b446f3",
+            "id": "ea97cc95",
             "metadata": {},
             "source": [
-                "## Local paths on your computer and `pathlib`"
+                "In this tutorial we will show you how to share your data with other users in the iRODS system. To see the effects it is helpful to team up with a colleague!!!"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2fdd6100",
+            "id": "d81b1269",
             "metadata": {},
             "source": [
-                "You might have wondered in the previous tutorials why we do not simply note down the location of data like a string `/home/user/folder/datafile.txt`.\n",
+                "## What are permissions"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "48815ec5",
+            "metadata": {},
+            "source": [
+                "Permissions in iRODS are part of the data objects and collections. They give information and they allow other users of the same iRODS system to read and edit your data.\n",
                 "\n",
-                "- Operating systems use different standard locations. For example your user folder lies in different locations for Linux, MacOS and Windows\n",
-                "- The separator between parts of the path differs, Linux and MacOS use `/` while Windows uses `\\`.\n",
+                "<img src=\"img/DataObject6.png\" width=\"400\">\n",
                 "\n",
-                "To be sure we are in your home directory independent from the operating system, we use:"
+                "In iRODS there are four types of permissions:\n",
+                "\n",
+                "| Access | Meaning|\n",
+                "|:---:|:---|\n",
+                "|read| The user or the group can **read and download** the data.|\n",
+                "|write| The user or group can **modify data objects and upload data to collections**, but can not delete the data or collection.|\n",
+                "|own| The user or group can **share and delete** the data.|"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "dee1520f",
+            "metadata": {},
+            "source": [
+                "## Give access to data objects and collections"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dd8f03ec",
+            "id": "ed6a8a46",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "Path.expanduser(Path('~'))"
+                "from ibridges.interactive import interactive_auth\n",
+                "session = interactive_auth()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "96578ae7",
+            "id": "76f3ab74",
             "metadata": {},
             "source": [
-                "Another way to retrieve this location is:"
+                "Let us have a look at the permissions of our demo data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8b91ca62",
+            "id": "df8697e4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Path.home()"
+                "from ibridges.path import IrodsPath\n",
+                "\n",
+                "irods_coll_path = IrodsPath(session, '~').joinpath('demo')\n",
+                "coll = irods_coll_path.collection\n",
+                "obj = irods_coll_path.joinpath('demofile.txt').dataobject"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d05ac550",
+            "id": "785383c9",
             "metadata": {},
             "source": [
-                "Moreover, when we want to extend a path with a new subdirectory, we can conveniently use:"
+                "Like for the metadata we need to load the permissions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6cdf6780",
+            "id": "3b3fc2d5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "Path.home().joinpath('new_dir')"
+                "from ibridges.permissions import Permissions\n",
+                "coll_perm = Permissions(session, coll)\n",
+                "print(coll_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7f3afd10",
+            "id": "43e1409b",
             "metadata": {},
             "source": [
-                "The command will take care that the correct separator is used and it provides you with functions to test whether the location already exist, to create the location etc:"
+                "In a native iRODS instance you will see your own username who is labeled with `own`. In Yoda you will see three groups: *research-\\<group\\>*, *read-\\<group\\>* and the *\\<datamanager\\>* group. Every user in these groups has the respective permissions on the data.\n",
+                "\n",
+                "Now we will give your colleague explicit access. **Note that if your colleague is also in one of the respective Yoda groups, the highest permission (the most powerful) will apply.**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3f8f2645",
+            "id": "c70d6b13",
             "metadata": {},
             "outputs": [],
             "source": [
-                "path = Path.home().joinpath('new_dir')\n",
-                "print(f'{path} exists: {path.exists()}')\n",
-                "print(f'{path} has parts: {path.parts}')"
+                "coll_perm.set('write', '<username>')\n",
+                "print(coll_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "014692ed",
+            "id": "3d1dd8d4",
             "metadata": {},
             "source": [
-                "## iRODS paths and `IrodsPath`"
+                "You will see a new entry with your colleague's iRODS name and *modify object*. We can get the default permission names like that:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "795dea7b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "coll_perm.available_permissions"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d77ce9cc",
+            "id": "bbebfaca",
             "metadata": {},
             "source": [
-                "iRODS also uses `/` as the separator.\n",
-                "\n",
-                "To determine the default home location in iRODS is dependent on how the iRODS instance is setup. In a default iRODS instance you have a personal home collection:\n",
-                "`/<zonename>/home/<username>`\n",
-                "\n",
-                "On Yoda instances you have a group collection:\n",
-                "`/<yodazone>/home/research-<groupname>`\n",
+                "Note that some permission-types have synonyms:\n",
                 "\n",
-                "You can set this home collection in your `irods_environment.json`.\n",
-                "\n",
-                "iBridges offers the `IrodsPath` which has similar functions as the `pathlib.Path`. We will always need a valis iRODS session to create those paths:"
+                "+ read object: 'read', 'read object', 'read_object'\n",
+                "+ modify object: 'write', 'modify object', 'modify_object'"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "63a89479",
+            "metadata": {},
+            "source": [
+                "## Remove access"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b8713621",
+            "metadata": {},
+            "source": [
+                "To remove any permissions, we use the keyword *null*. Again, please note, if your colleague is still part of a group that has access to your data, this will have no effect."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "06846322",
+            "id": "7c804ff3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges.interactive import interactive_auth\n",
-                "session = interactive_auth()"
+                "coll_perm.set('null', '<username>')\n",
+                "print(coll_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "808df0e1",
+            "id": "0e3f3562",
             "metadata": {},
             "source": [
-                "Now we can retrieve our configured home collection:"
+                "iBridges also prohibits that you lock yourself out of your data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e1557bf6",
+            "id": "144c2d96",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges.path import IrodsPath\n",
-                "print(IrodsPath(session, '~'))\n",
-                "# or \n",
-                "print(IrodsPath(session, session.home))"
+                "coll_perm.set('write', session.username)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "19a4bf31",
+            "id": "f167ffae",
             "metadata": {},
             "source": [
-                "Here a list of some functionality:"
+                "All the above functionality can also be used for objects"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2b7df9dc",
+            "id": "b322bdb9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "irods_path = IrodsPath(session, session.home)\n",
-                "print(f'Extend {irods_path}:', irods_path.joinpath('new_collection'))\n",
-                "print(f'{irods_path} exists:', irods_path.exists())\n",
-                "print(f'{irods_path} is collection:', irods_path.collection_exists())\n",
-                "print(f'{irods_path} is data object:', irods_path.dataobject_exists())\n",
-                "print(f'{irods_path} has parts: {irods_path.parts}')"
+                "obj_perm = Permissions(session, obj)\n",
+                "print(obj_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "82ea884f",
+            "id": "b4cff4b3",
             "metadata": {},
             "source": [
-                "## Concatenating iRODS paths  and local paths"
+                "## Collections: Inheritance"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "fe0e20ed",
+            "id": "6a4e0119",
             "metadata": {},
             "source": [
-                "Assume we would like to create a counter part collection to our local path:"
+                "You might have noticed that collections carry a special permissions keyword *inheritance* which can be `True` or `False`. If inheritance is switched on all new data objects and subcollections will receive the same permissions as the parent collection.\n",
+                "\n",
+                "Below we create a new collection, ans give access to your colleague and switch the inheritance on:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a1dd79a2",
+            "id": "2073f3b5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "path"
+                "new_coll_path = IrodsPath(session, '~').joinpath('demo1')\n",
+                "coll = IrodsPath.create_collection(session, new_coll_path)\n",
+                "coll_perm = Permissions(session, coll)\n",
+                "coll_perm.set('write', '<username>')\n",
+                "coll_perm.set('inherit')\n",
+                "print(coll_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5d89637e",
+            "id": "8c462e8d",
             "metadata": {},
             "source": [
-                "We know that we would have to create `new_dir` in our iRODS home collection:"
+                "Now we create a new subcollection:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4aee24f6",
+            "id": "88b5fbd2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "name = path.name\n",
-                "new_irods_coll_path = irods_path.joinpath(name)\n",
-                "print(new_irods_coll_path)"
+                "subcoll = IrodsPath.create_collection(session, new_coll_path.joinpath('subcoll'))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c0482bab",
+            "id": "7e00c83f",
             "metadata": {},
             "source": [
-                "You see, that `path.name` gives us the name of the last part of the path. We join that name to the iRODS path and now we can create the new collection:"
+                "And inspect the permissions. They should be the same as the ones above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e590f4d7",
+            "id": "e38a779c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "coll = IrodsPath.create_collection(session, new_irods_coll_path)"
+                "subcoll_perm = Permissions(session, subcoll)\n",
+                "print(subcoll_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1da30ba5",
+            "id": "896e5f3d",
+            "metadata": {},
+            "source": [
+                "Now we will switch off the inheritance of the parent collection and create another subcollection:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f588a39c",
             "metadata": {},
+            "outputs": [],
+            "source": [
+                "coll_perm.set('noinherit')\n",
+                "print(coll_perm)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "5af70cf0",
+            "metadata": {},
+            "outputs": [],
             "source": [
-                "## Summary"
+                "subcoll = IrodsPath.create_collection(session, new_coll_path.joinpath('subcoll1'))\n",
+                "subcoll_perm = Permissions(session, subcoll)\n",
+                "print(subcoll_perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e7dc79ec",
+            "id": "8838c6bd",
             "metadata": {},
             "source": [
-                "To work with `pathlib` and `IrodsPath` is safer since it takes care of the correct concatenation of parts of the path according to the operating system and their specific setup."
+                "You will see now that you `own` *subcoll1*, that the inheritance of this collection is also `False` and that you colleague has no permissions on the new subcollection."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "20f547d9",
+            "id": "39fecb18",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `ibridges-0.1.6/tutorials/04-Metadata.ipynb` & `ibridges-0.2.0/tutorials/00-FirstSteps.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9345399962480442%*

 * *Differences: {"'cells'": "{0: {'id': '939d9be3', 'source': ['# iBridges First Steps']}, 1: {'id': '1c955adf', "*

 * *            "'source': ['This note book is for the impatient user. We will take you through the "*

 * *            "main functionality of the iBridges API.']}, 2: {'id': 'fffb6d7d', 'source': ['To "*

 * *            'follow the notebook you need a valid iRODS configuration file installed in your '*

 * *            '`.irods` directory. If you do not have that please follow our guide '*

 * *            "[here](01-Setup-and-connect. […]*

```diff
@@ -1,451 +1,754 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "f9e6811a",
+            "id": "939d9be3",
             "metadata": {},
             "source": [
-                "# User-defined metadata"
+                "# iBridges First Steps"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8564525b",
+            "id": "1c955adf",
             "metadata": {},
             "source": [
-                "Next to system metadata, iRODS allows you to create own metadata with data objects and collections.\n",
-                "\n",
-                "You can use that metadata to describe your data andlater search for this data; and it can help you keeping the overview of what was the input for an analysis and what is the outcome.\n",
-                "\n",
-                "<img src=\"img/DataObject5.png\" width=\"400\">\n",
-                "\n",
-                "Technically, iRODS offers metadata as key-value-units triple. Let's investigate this:"
+                "This note book is for the impatient user. We will take you through the main functionality of the iBridges API."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bde731e4",
+            "id": "fffb6d7d",
             "metadata": {},
             "source": [
-                "## Add metadata to data objects"
+                "To follow the notebook you need a valid iRODS configuration file installed in your `.irods` directory. If you do not have that please follow our guide [here](01-Setup-and-connect.ipynb)."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "784fdac1",
+            "id": "e02a7976",
             "metadata": {},
             "source": [
-                "As always: first we have to create an iRODS session:"
+                "## Create an iRODS session (connection to iRODS server)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "277459df",
+            "id": "b6fd51d6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges.interactive import interactive_auth\n",
                 "session = interactive_auth()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "81094d42",
+            "id": "26b76d89",
             "metadata": {},
             "source": [
-                "Now we can retrieve a data object and insect its metadata."
+                "The `interactive_auth` takes the default `.irods/irods_environment.json` to connect to the iRODS server. You can direct the authentication to a different file like this:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "69066865",
+            "id": "e6d1ccf2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges import get_dataobject\n",
-                "from ibridges.path import IrodsPath\n",
-                "from ibridges.meta import MetaData\n",
+                "from pathlib import Path\n",
+                "session = interactive_auth(irods_env_path=Path(\"~\").expanduser().joinpath(\".irods\", \"another_env_file.json\"))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0fb9577d",
+            "metadata": {},
+            "source": [
+                "### Checking some session parameters"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "fe178d2c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "print(session.username)\n",
+                "print(session.default_resc) # the resource to which data will be uploaded\n",
+                "print(session.zone) # default home for iRODS /zone/home/username\n",
+                "print(session.server_version)\n",
+                "print(session.home)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "1e484823",
+            "metadata": {},
+            "source": [
+                "## A word on iRODS paths"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0a2f1607",
+            "metadata": {},
+            "source": [
+                "On a local file name we have folders/directories and files. In iRODS we call them collections and data objects. In contrast to files, data objects carry system metadata and user defined metadata. Likewise for collections."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "37d5d770",
+            "metadata": {},
+            "source": [
+                "`iBridges` supports iRODS paths with an own module `IrodsPath`. In this module all paths will be relative to the `session.home` unless they start with `/`.\n",
                 "\n",
-                "irods_coll_path = IrodsPath(session, '~').joinpath('demo')\n",
-                "obj = get_dataobject(session, irods_coll_path.joinpath('demofile.txt'))\n",
+                "There are three ways to create an `IrodsPath` from your home."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "15201901",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ibridges import IrodsPath\n",
+                "home = IrodsPath(session, session.home)\n",
+                "home1 = IrodsPath(session, \"~\")\n",
+                "home2 = IrodsPath(session)\n",
                 "\n",
-                "obj_metadata = MetaData(obj)\n",
-                "print(obj_metadata)"
+                "print(home)\n",
+                "print(home1)\n",
+                "print(home2)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7d9a578b",
+            "id": "a6db47a6",
             "metadata": {},
             "source": [
-                "Most probably you will see no metadata in the above cell. **Note, that system metadata and user-defined metadata are two different entities in a data object!**\n",
-                "With the command `MetaData(obj)` we only retrieve the user-defined metadata.\n",
+                "`IrodsPaths` implement some functionalities comparable to their counterparts in `Pathlib`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ae669333",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# some stats\n",
+                "print(home)\n",
+                "print(home.exists())\n",
+                "print(home.dataobject_exists())\n",
+                "print(home.collection_exists())\n",
+                "print(home.parent)\n",
                 "\n",
-                "<img src=\"img/DataObject4.png\" width=\"400\">"
+                "# path manipulation\n",
+                "print(home.joinpath(\"sub_collection\"))\n",
+                "\n",
+                "# iRODS system metadata\n",
+                "print(f\"Size of {home}: {home.size}\") # size in bytes\n",
+                "\n",
+                "# iRODS operations\n",
+                "new_coll = IrodsPath.create_collection(session, home.joinpath(\"new_coll_name\"))\n",
+                "new_coll_path = IrodsPath(session, new_coll.path)\n",
+                "print(f\"Created: {new_coll_path}\")\n",
+                "new_coll_path = new_coll_path.rename(\"new_coll_name1\")\n",
+                "print(f\"Moved to: {new_coll_path}\")\n",
+                "new_coll_path.remove()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "9cddc08e",
+            "metadata": {},
+            "source": [
+                "For a full Tutorial please have a look [here](02-iRODS-paths.ipynb)."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b6716876",
+            "metadata": {},
+            "source": [
+                "## Working with data"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1fb67574",
+            "id": "236b368e",
             "metadata": {},
             "source": [
-                "Now we can add some own metadata. The metadata comes as key-value-units triple:"
+                "[Full Tutorial](03-Working-with-data.ipynb) and a tutorial for [Data Synchronisation](06-Data-sync.ipynb)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "79a1bb89",
+            "id": "f56d4204",
             "metadata": {},
             "outputs": [],
             "source": [
-                "obj_metadata.add('Key', 'Value', 'Units')\n",
-                "print(obj_metadata)"
+                "from pathlib import Path\n",
+                "from ibridges.util import obj_replicas\n",
+                "from ibridges import upload, download"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "6cd1bd28",
+            "metadata": {},
+            "source": [
+                "### Upload a file or folder"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "dafbeaff",
+            "id": "ec66ec0c",
             "metadata": {},
             "source": [
-                "Sometimes we do not really have `units`, so we can leave this part empty:"
+                "Create a local file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fb439f38",
+            "id": "08d96d6c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "obj_metadata.add('Author', 'Christine')\n",
-                "print(obj_metadata)"
+                "# create a local file\n",
+                "local_path = Path.expanduser(Path('~')).joinpath(\"demofile.txt\")\n",
+                "f = open(local_path, \"a\")\n",
+                "f.write(\"My content! Super important\")\n",
+                "f.close()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3bfbfa71",
+            "id": "9d9dee41",
             "metadata": {},
             "source": [
-                "We can also add a second author:"
+                "Determine the iRODS path the file should be uploaded to."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bb35166a",
+            "id": "043536c3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "obj_metadata.add('Author', 'Raoul')\n",
-                "print(obj_metadata)"
+                "irods_path = IrodsPath(session, session.home, \"new_coll\")\n",
+                "if not irods_path.collection_exists():\n",
+                "    coll = IrodsPath.create_collection(session, irods_path)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "116c0f10",
+            "id": "d0de939a",
+            "metadata": {},
+            "source": [
+                "We can first check that an upload would change with the `dry-run`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "45991a0a",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You see, that keys in **iRODS metadata keys can have different values**. That is different from python dictionaries where one key can only have one value. **How then to overwrite a value?**"
+                "# upload the file to our collection\n",
+                "from pprint import pprint\n",
+                "ops = upload(session, local_path, irods_path, dry_run=True, overwrite=True)\n",
+                "pprint(ops)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cf6d7f93",
+            "id": "e8f827d3",
             "metadata": {},
             "source": [
-                "## Overwrite metadata"
+                "The function will only show what really needs to be updated on iRODS based on checksums. Now we can really upload the file. We will use the `overwrite` flag to update all existing data in iRODS."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bb9768fe",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "upload(session, local_path, irods_path, overwrite=True)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "975d3b36",
+            "metadata": {},
+            "source": [
+                "The `ops` dictionary can also be used to log what has been uploaded."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cb5b7fef",
+            "id": "a0893c4b",
             "metadata": {},
             "source": [
-                "If youw wish to *overwrite* a value, you can first add the new metadata key-value-units triple as above and subsequently remove the old one, you need to specify the whole triple if the metadata contains a units part. As you see the follwing command will fail:"
+                "### Retrieve a  data object from iRODS and checking their status"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d0cbd9bf",
+            "id": "f6673452",
             "metadata": {},
             "outputs": [],
             "source": [
-                "obj_metadata.delete('Key', 'Value')"
+                "obj_path = irods_path.joinpath(\"demofile.txt\")\n",
+                "obj = obj_path.dataobject"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "77993416",
+            "id": "b8f0d6e4",
             "metadata": {},
             "source": [
-                "While this one will succeed:"
+                "Some system metadata of the object:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ce98d47c",
+            "id": "c8da0670",
             "metadata": {},
             "outputs": [],
             "source": [
-                "obj_metadata.delete('Key', 'Value', 'Units')"
+                "print('data object name\\t', obj.name)\n",
+                "print('data object path\\t', obj.path)\n",
+                "print('data object size\\t', obj.size)\n",
+                "print('data object checksum\\t', obj.checksum)\n",
+                "print('data replicas\\t', obj_replicas(obj))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e7f47a59",
+            "id": "6ed47426",
             "metadata": {},
             "source": [
-                "You can also set all existing values to **one** new value:"
+                "### Open a data object in read or write mode"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c9f0a95b",
+            "id": "93288ef0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(obj_metadata)\n",
-                "obj_metadata.set('Author', 'Maarten')\n",
-                "print(obj_metadata)"
+                "stream = obj.open('r')\n",
+                "text = stream.read().decode()\n",
+                "stream.close()\n",
+                "print(text)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c3f54857",
+            "id": "26bb46ff",
             "metadata": {},
             "source": [
-                "## Add metadata to collections"
+                "### Download a data object or collection"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "51438d57",
+            "id": "af5205a2",
             "metadata": {},
             "source": [
-                "The same functionality we saw above, we can use for collections:"
+                "Downloads work similar as the uploads: use the `dry_run` to see what will change and use the `overwrite` flag to update all already existing data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "65fb35a5",
+            "id": "e734843b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges import get_collection\n",
-                "coll = get_collection(session, irods_coll_path)\n",
-                "coll_metadata = MetaData(coll)\n",
-                "print(coll_metadata)"
+                "ipath = IrodsPath(session, irods_path)\n",
+                "print(ipath)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2af31459",
+            "id": "a54a1dd1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "coll_metadata.add('TypeOfCollection', 'Results')\n",
-                "print(coll_metadata)"
+                "from pathlib import Path\n",
+                "local_path = Path(\"~/Downloads\").expanduser()\n",
+                "print(\"Download folder exists\", local_path.is_dir())\n",
+                "download(session, ipath, local_path, overwrite=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d7eacaba",
+            "id": "5c1637df",
             "metadata": {},
             "source": [
-                "## Which metadata can help you keeping an overview?"
+                "## User defined metadata of data objects and collections"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cb48bb74",
+            "id": "5d3ad69d",
             "metadata": {},
             "source": [
-                "iRODS metadata can help you keeping an overview while youare working with data and maybe many files which have relations to each other. There are ontologies which define keywords and links between keywords like the **[prov-o Ontology](https://www.w3.org/TR/prov-o/#prov-o-at-a-glance)**.\n",
-                "\n",
-                "Let's see how we can annotate our test data, so that we know that it is test data."
+                "[Full Tutorial](04-Metadata.ipynb)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "928bf82c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# upload a file\n",
+                "local_path = Path(\"~\").expanduser().joinpath(\"demofile.txt\")\n",
+                "irods_path = IrodsPath(session, session.home, \"new_coll\")\n",
+                "if not irods_path.collection_exists():\n",
+                "    coll = IrodsPath.create_collection(session, irods_path)\n",
+                "upload(session, local_path, irods_path, overwrite = True)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "510e390a",
+            "metadata": {},
+            "source": [
+                "### Retrieve an iRODS object or collection and list its metadata"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "9ae7d602",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "obj = irods_path.joinpath(\"demofile.txt\").dataobject"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bbadefc7",
+            "id": "2e8f3c90",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from datetime import datetime\n",
-                "coll_metadata.add('prov:wasGeneratedBy', 'Christine')\n",
-                "coll_metadata.add('CollectionType', 'testcollection')\n",
-                "obj_metadata.add('prov:SoftwareAgent', 'iRODS jupyter Tutorial')\n",
-                "obj_metadata.add('prov:wasGeneratedBy', 'Maarten')\n",
-                "obj_metadata.add('DataType', 'testdata')"
+                "from ibridges.meta import MetaData\n",
+                "obj_meta = MetaData(obj)\n",
+                "print(obj_meta)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5be8180b",
+            "id": "42007e1e",
+            "metadata": {},
+            "source": [
+                "### View, add, set and delete metadata"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cfa7f559",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Now we have some more descriptive metadata that gives us hints, in which context the data was created:"
+                "obj_meta.add('NewKey', 'NewValue')\n",
+                "obj_meta.add('NewKey', 'AnotherValue')\n",
+                "print(obj_meta)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a0b8e2d4",
+            "id": "d8aa144a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(coll_metadata)\n",
-                "print(obj_metadata)"
+                "obj_meta.delete('NewKey', 'NewValue')\n",
+                "print(obj_meta)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7f721760",
+            "id": "f7b5cafa",
+            "metadata": {},
+            "source": [
+                "We can also set the meta data to a single key, value, units pair. This will remove any other entries with the same key."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "770cbec2",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Finding data by their metadata"
+                "obj_meta.set(\"NewKey\", \"YetAnotherValue\")\n",
+                "print(obj_meta)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "59518813",
+            "id": "2198d111-ee11-42e3-b24b-d774d95e7156",
             "metadata": {},
             "source": [
-                "Metadata does not only help you to. keep an overview over your data, but can also be used to select and retrieve data. In iBridges you can use the user-defined metadata and some system metadata fields to search for data.\n",
-                "\n",
-                "In our first example we list all collections and data objects in our iRODS home."
+                "### Accessing metadata \n",
+                "With the print function you can quickly inspect the metadata of an iRODS collection or object. If you want to extract and do something with the metadata, you can iterate over all metadata entries. We give a small example below where we assume that the metadata contains a key/name *AUTHOR*:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e6918fe7",
+            "id": "8debeb07",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for md in obj_meta:\n",
+                "    print(md.name, \"has value\", md.value)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "215251fc",
+            "metadata": {},
+            "source": [
+                "## Search for data"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "89009c88",
+            "metadata": {},
+            "source": [
+                "How can you retrieve the location of an iRODS collection or data object by its metadata or partial part? To this end we provide the function `search`"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "52cb2500",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges.search import search_data\n",
-                "result = search_data(session, path=session.home)\n",
+                "\n",
+                "#all collections and objects with \n",
+                "key_vals = {\"NEWKEY\": \"YetAnotherValue\"}\n",
+                "result = search_data(session, key_vals=key_vals)\n",
                 "print(result)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "31c88425",
+            "id": "9aca8830",
             "metadata": {},
             "source": [
-                "The output is a list of Python dictionaries, where each dictionary contains\n",
-                "\n",
-                "1) Collections: `'COLL_NAME': '/<ZONE>/home/<YOUR PATH>'}`\n",
-                "2) Data Objects: \n",
-                "    ```\n",
-                "    {'COLL_NAME': '/<ZONE>/home/<YOUR PATH>', \n",
-                "     'DATA_NAME': '<OBJECT NAME>', \n",
-                "     'D_DATA_CHECKSUM': '<CHECKSUM>'}\n",
-                "    ```\n",
+                "The result gives us the collection, the object name, and its checksum.\n",
                 "\n",
-                "Now let's try to find data by its metadata. We will have to create a Python dictionary with the metadata keys and the metadata values as search criterion:"
+                "The wildcard in iRODS searches is the `%`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5b054794",
+            "id": "6e750edb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "key_vals = {'prov:wasGeneratedBy': 'Christine'}\n",
-                "result = search_data(session, key_vals=key_vals)\n",
+                "result = search_data(session, path=session.home+\"/new_coll/%\")\n",
                 "print(result)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "81d73352",
+            "id": "30a2d4a6",
+            "metadata": {},
+            "source": [
+                "## Permissions"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e2dc3a91",
             "metadata": {},
             "source": [
-                "If we do not want to specify the particular value of the key, we can use a *wildcard*. In iRODS the wildcard is `%`."
+                "**Note: In Yoda 1.9 users cannot set permissions any longer.**\n",
+                "\n",
+                "[Full Tutorial](05-Data-Sharing.ipynb)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "fca96b65",
+            "metadata": {},
+            "source": [
+                "### Accessing the permissions of a data object or collection in iRODS\n",
+                "\n",
+                "Objects and collections have permissions attached to them. Permissions, which work like access levels, must be specified per user or group. The basic permissions are `own` (implies reading and writing), `modify object` (editing and reading), and `read object`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "49a9f17e",
+            "id": "1eb3a627",
             "metadata": {},
             "outputs": [],
             "source": [
-                "key_vals = {'prov:wasGeneratedBy': '%'}\n",
-                "result = search_data(session, key_vals=key_vals)\n",
-                "print(result)"
+                "from ibridges.permissions import Permissions\n",
+                "\n",
+                "# select a file to inspect and set permissions on\n",
+                "item_path = IrodsPath(session, session.home) # Path to collection or data object\n",
+                "collection = item_path.collection  # Get the collection, use item_path.dataobject for data objects\n",
+                "\n",
+                "# instantiate permissions with that object\n",
+                "perm = Permissions(session, collection)\n",
+                "print(f'Permissions for {item_path}:\\n')\n",
+                "print(perm)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "f2d1c093",
+            "metadata": {},
+            "source": [
+                "### Available permissions on your iRODS server"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "691dbaa1",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "perm.available_permissions"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "69a2e046",
+            "id": "b84f75ba",
             "metadata": {},
             "source": [
-                "Now we also receive the data object that was generated by *Maarten*.\n",
+                "### Adding permissions to a collection or data object"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4e2e1737",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "perm.set('modify object', '<username or group name>')\n",
+                "print(perm)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e5779c58",
+            "metadata": {},
+            "source": [
+                "Note that some permission-types have synonyms:\n",
                 "\n",
-                "And of course we can combine information about the path and the metadata. they will be connected with `and`. The following search will retrieve all data objects and collections wich are labeled with a metadata key *'prov:wasGeneratedBy'* and whose path has the prefix */nluu12p/home/research-test-christine/demo/*."
+                "+ read object: 'read', 'read object', 'read_object'\n",
+                "+ modify object: 'write', 'modify object', 'modify_object'"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "8c2ba10d",
+            "metadata": {},
+            "source": [
+                "### Removing permissions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e0d2fad9",
+            "id": "21bda746",
             "metadata": {},
             "outputs": [],
             "source": [
-                "key_vals = {'prov:wasGeneratedBy': '%'}\n",
-                "result = search_data(session, path='/nluu12p/home/research-test-christine/%', key_vals=key_vals)\n",
-                "print(result)"
+                "perm.set('null', '<username or group name>')\n",
+                "print(perm)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "14bc70b0",
+            "id": "4d52f16b",
             "metadata": {},
             "source": [
-                "## Retrieving data"
+                "### Inheritance"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "946e355c",
+            "id": "76942f18",
             "metadata": {},
             "source": [
-                "Now that we have the search results in a list of Python dictionaries, we can use the information to create the full iRODS paths and continue working with them e.g. download them."
+                "Collections have two special permissions level `inherit` and `noinherit`. From the point in time where inheritance in switched on, all newly added subcollections and data objects will inherit their initial permissions from the collection."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ff72b0ca",
+            "id": "60251c8a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges.path import IrodsPath\n",
+                "# Retrieve a collection from iRODS\n",
+                "coll_path = session.home\n",
+                "coll = session.irods_session.collections.get(item_path)\n",
+                "coll_perm = Permissions(session, coll)\n",
                 "\n",
-                "paths = [IrodsPath(session, r.get('COLL_NAME', '')).joinpath(r.get('DATA_NAME', '')) for r in result]\n",
-                "print(paths)"
+                "#Switch inheritance on\n",
+                "coll_perm.set('inherit')\n",
+                "print(coll_perm)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ec9bd025",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Switch inheritance off\n",
+                "coll_perm.set('noinherit')\n",
+                "print(coll_perm)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4072812e",
+            "id": "79a02f14",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `ibridges-0.1.6/tutorials/Data_sync.ipynb` & `ibridges-0.2.0/tutorials/06-Data-sync.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983940972222223%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from pprint import pprint\\n')]}}, 6: {'source': "*

 * *            '[\'source = IrodsPath(session, "~", "<your irods collection>")\\n\', \'target = '*

 * *            'Path(os.path.expanduser("~"), "<your local folder>")\']}, 7: {\'source\': '*

 * *            "['print(target, target.is_dir())\\n', 'print(source, source.collection_exists())']}, "*

 * *            "11: {'source': {insert: [(7, ')\\n'), (8, 'pprint(changes)')], delete: [7]}}}"}*

```diff
@@ -23,14 +23,15 @@
             "execution_count": null,
             "id": "de207d54",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "from pathlib import Path\n",
+                "from pprint import pprint\n",
                 "from ibridges.interactive import interactive_auth\n",
                 "from ibridges.path import IrodsPath\n",
                 "from ibridges.sync import sync_data"
             ]
         },
         {
             "cell_type": "markdown",
@@ -66,27 +67,27 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "39de2a38-2c35-48e8-9de4-cf426eaecefd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "target = IrodsPath(session, \"~\", \"<irods path>\")\n",
-                "source = Path(os.path.expanduser(\"~\"), \"<local path>\")"
+                "source = IrodsPath(session, \"~\", \"<your irods collection>\")\n",
+                "target = Path(os.path.expanduser(\"~\"), \"<your local folder>\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6b180cee-3753-4a1e-a10f-5cfc50fcb8b0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(target, target.collection_exists())\n",
-                "print(source, source.is_dir())"
+                "print(target, target.is_dir())\n",
+                "print(source, source.collection_exists())"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d20dd782",
             "metadata": {},
             "source": [
@@ -131,15 +132,16 @@
                 "changes = sync_data(\n",
                 "    session=session,\n",
                 "    source=source,\n",
                 "    target=target,\n",
                 "    max_level=max_level,      \n",
                 "    dry_run=dry_run,\n",
                 "    copy_empty_folders=copy_empty_folders\n",
-                ")"
+                ")\n",
+                "pprint(changes)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ec01f5ca",
             "metadata": {},
             "source": [
```

### Comparing `ibridges-0.1.6/tutorials/img/DataObject1.png` & `ibridges-0.2.0/tutorials/img/DataObject1.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/DataObject2.png` & `ibridges-0.2.0/tutorials/img/DataObject2.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/DataObject3.png` & `ibridges-0.2.0/tutorials/img/DataObject3.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/DataObject4.png` & `ibridges-0.2.0/tutorials/img/DataObject4.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/DataObject5.png` & `ibridges-0.2.0/tutorials/img/DataObject5.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/DataObject6.png` & `ibridges-0.2.0/tutorials/img/DataObject6.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/Save_json.png` & `ibridges-0.2.0/tutorials/img/Save_json.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.6/tutorials/img/Yoda_environment.png` & `ibridges-0.2.0/tutorials/img/Yoda_environment.png`

 * *Files identical despite different names*

