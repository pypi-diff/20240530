# Comparing `tmp/kbcstorage-0.9.0.tar.gz` & `tmp/kbcstorage-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbcstorage-0.9.0.tar", last modified: Thu May  9 12:29:58 2024, max compression
+gzip compressed data, was "kbcstorage-0.9.1.tar", last modified: Thu May 30 17:55:19 2024, max compression
```

## Comparing `kbcstorage-0.9.0.tar` & `kbcstorage-0.9.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.env.template
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.764406 kbcstorage-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.764406 kbcstorage-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.768406 kbcstorage-0.9.0/kbcstorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/configurations_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24013 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/tables_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/kbcstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.768406 kbcstorage-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/base_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.772406 kbcstorage-0.9.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_workspaces_abs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/branches_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/bucket_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/component_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/configuration_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/job_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/table_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/token_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/triggers_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/workspace_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.690804 kbcstorage-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.678804 kbcstorage-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.678804 kbcstorage-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-30 17:55:19.690804 kbcstorage-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.682804 kbcstorage-0.9.1/kbcstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/configurations_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24013 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/tables_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/kbcstorage/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.686804 kbcstorage-0.9.1/kbcstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-30 17:55:19.000000 kbcstorage-0.9.1/kbcstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-30 17:55:19.000000 kbcstorage-0.9.1/kbcstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:55:19.000000 kbcstorage-0.9.1/kbcstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 17:55:19.000000 kbcstorage-0.9.1/kbcstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 17:55:19.000000 kbcstorage-0.9.1/kbcstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:55:19.690804 kbcstorage-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.682804 kbcstorage-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/base_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.686804 kbcstorage-0.9.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/functional/test_workspaces_abs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:19.686804 kbcstorage-0.9.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/branches_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/bucket_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/component_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/configuration_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/job_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/table_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/token_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/triggers_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-30 17:55:14.000000 kbcstorage-0.9.1/tests/mocks/workspace_responses.py
```

### Comparing `kbcstorage-0.9.0/.github/workflows/push.yml` & `kbcstorage-0.9.1/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/LICENSE` & `kbcstorage-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/PKG-INFO` & `kbcstorage-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbcstorage
-Version: 0.9.0
+Version: 0.9.1
 Summary: Client for Keboola Storage API
 Author-email: Keboola <developers@keboola.com>
 License: MIT License
         
         Copyright (c) Keboola :(){:|:&};: s.r.o.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `kbcstorage-0.9.0/README.md` & `kbcstorage-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/base.py` & `kbcstorage-0.9.1/kbcstorage/base.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/branches.py` & `kbcstorage-0.9.1/kbcstorage/branches.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/buckets.py` & `kbcstorage-0.9.1/kbcstorage/buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/client.py` & `kbcstorage-0.9.1/kbcstorage/client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/components.py` & `kbcstorage-0.9.1/kbcstorage/components.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/configurations.py` & `kbcstorage-0.9.1/kbcstorage/configurations.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/configurations_metadata.py` & `kbcstorage-0.9.1/kbcstorage/configurations_metadata.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/files.py` & `kbcstorage-0.9.1/kbcstorage/files.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/jobs.py` & `kbcstorage-0.9.1/kbcstorage/jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/tables.py` & `kbcstorage-0.9.1/kbcstorage/tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/tables_metadata.py` & `kbcstorage-0.9.1/kbcstorage/tables_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         if not isinstance(metadata_id, str) or metadata_id == '':
             raise ValueError("Invalid metadata_id '{}'.".format(metadata_id))
 
         url = '{}/{}/metadata/{}'.format(self.base_url, table_id, metadata_id)
 
         self._delete(url)
 
-    def create(self, table_id, provider, metadata, columns_metadata):
+    def create(self, table_id, provider, metadata, columns_metadata=None):
         """
         Post metadata to a table.
 
         Args:
             table_id (str): Table id
             provider (str): Provider of the metadata
             metadata (list): List of metadata dictionaries with 'key' and 'value'
@@ -82,26 +82,29 @@
         Raises:
             requests.HTTPError: If the API request fails.
             ValueError: If the table_id is not a string or is empty.
             ValueError: If the provider is not a string or is empty.
             ValueError: If the metadata is not a list.
             ValueError: If the columns_metadata is not a list
         """
+        if columns_metadata is None:
+            columns_metadata = []
         if not isinstance(table_id, str) or table_id == '':
             raise ValueError("Invalid table_id '{}'.".format(table_id))
         if not isinstance(provider, str) or provider == '':
             raise ValueError("Invalid provider '{}'.".format(provider))
         if not isinstance(metadata, list):
             raise ValueError("Invalid metadata '{}'.".format(metadata))
-        if not isinstance(columns_metadata, list):
+        if columns_metadata is not None and not isinstance(columns_metadata, list):
             raise ValueError("Invalid columns_metadata '{}'.".format(columns_metadata))
 
         url = '{}/{}/metadata'.format(self.base_url, table_id)
         headers = {
             'Content-Type': 'application/json',
         }
         data = {
             "provider": provider,
-            "metadata": metadata,
-            "columnsMetadata": columns_metadata
+            "metadata": metadata
         }
+        if columns_metadata:
+            data["columnsMetadata"] = columns_metadata
         return self._post(url, data=json.dumps(data), headers=headers)
```

### Comparing `kbcstorage-0.9.0/kbcstorage/tokens.py` & `kbcstorage-0.9.1/kbcstorage/tokens.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/triggers.py` & `kbcstorage-0.9.1/kbcstorage/triggers.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage/workspaces.py` & `kbcstorage-0.9.1/kbcstorage/workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/kbcstorage.egg-info/PKG-INFO` & `kbcstorage-0.9.1/kbcstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbcstorage
-Version: 0.9.0
+Version: 0.9.1
 Summary: Client for Keboola Storage API
 Author-email: Keboola <developers@keboola.com>
 License: MIT License
         
         Copyright (c) Keboola :(){:|:&};: s.r.o.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `kbcstorage-0.9.0/kbcstorage.egg-info/SOURCES.txt` & `kbcstorage-0.9.1/kbcstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/pyproject.toml` & `kbcstorage-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/base_test_case.py` & `kbcstorage-0.9.1/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_base.py` & `kbcstorage-0.9.1/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_buckets.py` & `kbcstorage-0.9.1/tests/functional/test_buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_client.py` & `kbcstorage-0.9.1/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_components.py` & `kbcstorage-0.9.1/tests/functional/test_components.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_configurations.py` & `kbcstorage-0.9.1/tests/functional/test_configurations.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_files.py` & `kbcstorage-0.9.1/tests/functional/test_files.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_tables.py` & `kbcstorage-0.9.1/tests/functional/test_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,26 @@
                         'value': 'success',
                         'columnName': 'col1'
                     }
                 ]
             ]
         )
 
+        with self.subTest("Test empty columns metadata"):
+            # test that empty [] is not actually put in the request
+            self.tables.metadata.create(
+                table_id=table_id,
+                provider='test',
+                metadata=[{
+                    'key': 'test_table_with_metadata',
+                    'value': 'success'
+                }],
+                columns_metadata=[]
+            )
+
         table_info = self.tables.detail(table_id)
         with self.subTest("Test metadata key in response"):
             self.assertIn('metadata', table_info)
         with self.subTest("Test metadata structure"):
             self.assertEqual(1, len(table_info['metadata']))
             self.assertIn('id', table_info['metadata'][0])
             self.assertEqual('test_table_with_metadata', table_info['metadata'][0]['key'])
```

### Comparing `kbcstorage-0.9.0/tests/functional/test_tokens.py` & `kbcstorage-0.9.1/tests/functional/test_tokens.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_triggers.py` & `kbcstorage-0.9.1/tests/functional/test_triggers.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_workspaces.py` & `kbcstorage-0.9.1/tests/functional/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/functional/test_workspaces_abs.py` & `kbcstorage-0.9.1/tests/functional/test_workspaces_abs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/bucket_responses.py` & `kbcstorage-0.9.1/tests/mocks/bucket_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/component_responses.py` & `kbcstorage-0.9.1/tests/mocks/component_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/configuration_responses.py` & `kbcstorage-0.9.1/tests/mocks/configuration_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/job_responses.py` & `kbcstorage-0.9.1/tests/mocks/job_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/table_responses.py` & `kbcstorage-0.9.1/tests/mocks/table_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_branches.py` & `kbcstorage-0.9.1/tests/mocks/test_branches.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_buckets.py` & `kbcstorage-0.9.1/tests/mocks/test_buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_client.py` & `kbcstorage-0.9.1/tests/mocks/test_client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_components.py` & `kbcstorage-0.9.1/tests/mocks/test_components.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_configurations.py` & `kbcstorage-0.9.1/tests/mocks/test_configurations.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_jobs.py` & `kbcstorage-0.9.1/tests/mocks/test_jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_tables.py` & `kbcstorage-0.9.1/tests/mocks/test_tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_tokens.py` & `kbcstorage-0.9.1/tests/mocks/test_tokens.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_triggers.py` & `kbcstorage-0.9.1/tests/mocks/test_triggers.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/test_workspaces.py` & `kbcstorage-0.9.1/tests/mocks/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/token_responses.py` & `kbcstorage-0.9.1/tests/mocks/token_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/triggers_responses.py` & `kbcstorage-0.9.1/tests/mocks/triggers_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.9.0/tests/mocks/workspace_responses.py` & `kbcstorage-0.9.1/tests/mocks/workspace_responses.py`

 * *Files identical despite different names*

