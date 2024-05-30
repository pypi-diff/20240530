# Comparing `tmp/nuclia-2.0.9.tar.gz` & `tmp/nuclia-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-2.0.9.tar", last modified: Wed Mar 20 07:37:03 2024, max compression
+gzip compressed data, was "nuclia-2.1.0.tar", last modified: Fri May 17 10:40:24 2024, max compression
```

## Comparing `nuclia-2.0.9.tar` & `nuclia-2.1.0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.067428 nuclia-2.0.9/
--rw-r--r--   0 ebr        (501) staff       (20)       59 2024-03-20 07:37:02.000000 nuclia-2.0.9/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)        7 2024-03-20 07:37:02.000000 nuclia-2.0.9/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)     3647 2024-03-20 07:37:02.000000 nuclia-2.0.9/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2024-03-20 07:37:02.000000 nuclia-2.0.9/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2024-03-20 07:37:02.000000 nuclia-2.0.9/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      270 2024-03-20 07:37:02.000000 nuclia-2.0.9/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2053 2024-03-20 07:37:03.067598 nuclia-2.0.9/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      967 2024-03-20 07:37:02.000000 nuclia-2.0.9/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2024-03-20 07:37:02.000000 nuclia-2.0.9/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2024-03-20 07:37:02.000000 nuclia-2.0.9/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.037974 nuclia-2.0.9/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      871 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/01-README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1894 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/02-auth.md
--rw-r--r--   0 ebr        (501) staff       (20)     5530 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/03-kb.md
--rw-r--r--   0 ebr        (501) staff       (20)     3285 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/04-upload.md
--rw-r--r--   0 ebr        (501) staff       (20)     2357 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/05-search.md
--rw-r--r--   0 ebr        (501) staff       (20)     1234 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/06-read.md
--rw-r--r--   0 ebr        (501) staff       (20)     3247 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/07-nua.md
--rw-r--r--   0 ebr        (501) staff       (20)     1987 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/08-import-export.md
--rw-r--r--   0 ebr        (501) staff       (20)     2072 2024-03-20 07:37:02.000000 nuclia-2.0.9/docs/09-manage.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.039909 nuclia-2.0.9/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      645 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.046312 nuclia-2.0.9/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1522 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     8077 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)     1021 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     8242 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      521 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.047912 nuclia-2.0.9/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)    14202 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)    16530 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)    10083 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/nua_responses.py
--rw-r--r--   0 ebr        (501) staff       (20)      472 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/lib/utils.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.057603 nuclia-2.0.9/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      822 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      647 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     1966 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/agent.py
--rw-r--r--   0 ebr        (501) staff       (20)    20954 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     9654 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/export_import.py
--rw-r--r--   0 ebr        (501) staff       (20)     6035 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     4648 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      462 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/logs.py
--rw-r--r--   0 ebr        (501) staff       (20)      369 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1288 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/nucliadb.py
--rw-r--r--   0 ebr        (501) staff       (20)     4896 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)     2196 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     6870 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     7361 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)    19774 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      342 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.058622 nuclia-2.0.9/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.059278 nuclia-2.0.9/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       74 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1527 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/fixtures.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.062492 nuclia-2.0.9/nuclia/tests/test_kb/
--rw-r--r--   0 ebr        (501) staff       (20)      741 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)     1019 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_export_import.py
--rw-r--r--   0 ebr        (501) staff       (20)      879 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_labels.py
--rw-r--r--   0 ebr        (501) staff       (20)      269 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_logs.py
--rw-r--r--   0 ebr        (501) staff       (20)      996 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_resource.py
--rw-r--r--   0 ebr        (501) staff       (20)      990 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_kb/test_search.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.064166 nuclia-2.0.9/nuclia/tests/test_manage/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      289 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/test_account.py
--rw-r--r--   0 ebr        (501) staff       (20)      540 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     1015 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_manage/test_kb.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.065611 nuclia-2.0.9/nuclia/tests/test_nua/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nua/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      334 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nua/test_agent.py
--rw-r--r--   0 ebr        (501) staff       (20)     1108 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nua/test_predict.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.066275 nuclia-2.0.9/nuclia/tests/test_nucliadb/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nucliadb/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1235 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/test_nucliadb/test_crud.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.067059 nuclia-2.0.9/nuclia/tests/unit/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/unit/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      980 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia/tests/unit/test_export_import.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-03-20 07:37:03.044915 nuclia-2.0.9/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2053 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1948 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      137 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2024-03-20 07:37:02.000000 nuclia-2.0.9/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      137 2024-03-20 07:37:02.000000 nuclia-2.0.9/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2024-03-20 07:37:03.068421 nuclia-2.0.9/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2024-03-20 07:37:02.000000 nuclia-2.0.9/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)      211 2024-03-20 07:37:02.000000 nuclia-2.0.9/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.100597 nuclia-2.1.0/
+-rw-r--r--   0 ebr        (501) staff       (20)       75 2024-05-17 10:40:23.000000 nuclia-2.1.0/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-17 10:40:23.000000 nuclia-2.1.0/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)     3946 2024-05-17 10:40:23.000000 nuclia-2.1.0/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2024-05-17 10:40:23.000000 nuclia-2.1.0/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2024-05-17 10:40:23.000000 nuclia-2.1.0/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      270 2024-05-17 10:40:23.000000 nuclia-2.1.0/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2070 2024-05-17 10:40:24.100454 nuclia-2.1.0/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      967 2024-05-17 10:40:23.000000 nuclia-2.1.0/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2024-05-17 10:40:23.000000 nuclia-2.1.0/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2024-05-17 10:40:23.000000 nuclia-2.1.0/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.081286 nuclia-2.1.0/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      871 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/01-README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1894 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/02-auth.md
+-rw-r--r--   0 ebr        (501) staff       (20)     5534 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/03-kb.md
+-rw-r--r--   0 ebr        (501) staff       (20)     3285 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/04-upload.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2357 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/05-search.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1234 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/06-read.md
+-rw-r--r--   0 ebr        (501) staff       (20)     3247 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/07-nua.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1987 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/08-import-export.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2072 2024-05-17 10:40:23.000000 nuclia-2.1.0/docs/09-manage.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.083322 nuclia-2.1.0/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      698 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.086130 nuclia-2.1.0/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1522 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8077 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1021 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8242 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      565 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.087875 nuclia-2.1.0/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)    15010 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)    19017 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)    11215 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ebr        (501) staff       (20)      589 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/lib/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/py.typed
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.093608 nuclia-2.1.0/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      822 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      647 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1966 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/agent.py
+-rw-r--r--   0 ebr        (501) staff       (20)    20954 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9654 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)    11245 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     4648 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      462 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/logs.py
+-rw-r--r--   0 ebr        (501) staff       (20)      369 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1288 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/nucliadb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8137 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2196 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6886 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)    10421 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)    19774 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      342 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.094440 nuclia-2.1.0/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.094704 nuclia-2.1.0/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       74 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1527 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/fixtures.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.096238 nuclia-2.1.0/nuclia/tests/test_kb/
+-rw-r--r--   0 ebr        (501) staff       (20)      741 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_kb/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1019 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_kb/test_export_import.py
+-rw-r--r--   0 ebr        (501) staff       (20)      879 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_kb/test_labels.py
+-rw-r--r--   0 ebr        (501) staff       (20)      269 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_kb/test_logs.py
+-rw-r--r--   0 ebr        (501) staff       (20)      996 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_kb/test_resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1935 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_kb/test_search.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.097180 nuclia-2.1.0/nuclia/tests/test_manage/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_manage/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      289 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_manage/test_account.py
+-rw-r--r--   0 ebr        (501) staff       (20)      540 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_manage/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1015 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_manage/test_kb.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.098430 nuclia-2.1.0/nuclia/tests/test_nua/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_nua/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      334 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_nua/test_agent.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1931 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_nua/test_predict.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.098914 nuclia-2.1.0/nuclia/tests/test_nucliadb/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_nucliadb/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1235 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/test_nucliadb/test_crud.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.099478 nuclia-2.1.0/nuclia/tests/unit/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/unit/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      980 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia/tests/unit/test_export_import.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-17 10:40:24.099906 nuclia-2.1.0/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2070 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1964 2024-05-17 10:40:24.000000 nuclia-2.1.0/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       46 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      160 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-17 10:40:23.000000 nuclia-2.1.0/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      159 2024-05-17 10:40:23.000000 nuclia-2.1.0/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2024-05-17 10:40:24.101117 nuclia-2.1.0/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2024-05-17 10:40:23.000000 nuclia-2.1.0/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)      228 2024-05-17 10:40:23.000000 nuclia-2.1.0/test-requirements.txt
```

### Comparing `nuclia-2.0.9/CHANGELOG.md` & `nuclia-2.1.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,92 @@
 # Changelog
 
-## 2.0.9 (2024-03-20)
+## 2.1.0 (2024-05-17)
 
+- Integrate new /ask endpoint
 
-- Chat needs a timeout.
+## 2.0.12 (2024-05-16)
 
+- Add generative stream on NUA API
+- Support security groups on search endpoints raw queries
 
-## 2.0.8 (2024-03-18)
+## 2.0.11 (2024-03-27)
 
+- Handle nucliadb back pressure with backoff
 
-- Support CSS selector when uploading links
+## 2.0.10 (2024-03-26)
 
+- Support summarize resources on a KB and Async KB management
 
-## 2.0.7 (2024-03-18)
+## 2.0.9 (2024-03-20)
 
+- Chat needs a timeout.
 
-- Fix bug on export creating folders.
+## 2.0.8 (2024-03-18)
 
+- Support CSS selector when uploading links
 
-## 2.0.6 (2024-03-15)
+## 2.0.7 (2024-03-18)
 
+- Fix bug on export creating folders.
+
+## 2.0.6 (2024-03-15)
 
 - Add async export/import.
 - Add Query endpoint.
 
-
 ## 2.0.5 (2024-03-08)
 
-
 - Fix dependencies.
 
-
 ## 2.0.4 (2024-02-29)
 
-
 - Allow to download Knowledge Box logs
 
-
 ## 2.0.3 (2024-02-26)
 
-
 - Fix upload chunk size
 - Support async
 
-
 ## 2.0.2 (2024-02-23)
 
-
 - Check errors when getting remote files
 - Increase uploads chunk size to work with both s3 and gcs
 
-
 ## 2.0.1 (2024-02-21)
 
-
 - Delete and update resources by slug natively with nucliadb-sdk
-- Support `all`, `any`, `none` and `not_all` operators in `filters` parameter 
-
+- Support `all`, `any`, `none` and `not_all` operators in `filters` parameter
 
 ## 2.0.0 (2024-02-18)
 
-
 - Support AsyncIO Auth and Predict
 
-
 ## 1.2.4 (2024-01-18)
 
-
 - Allow to set remote files field at creation
 
-
 ## 1.2.3 (2024-01-16)
 
-
 - Support resources summarization
 
-
 ## 1.2.2 (2024-01-11)
 
-
 - Update Nuclia dependencies to get the new AWS region.
 
-
 ## 1.2.1 (2024-01-08)
 
-
 - Improve prompt generation
 
-
 ## 1.2.0 (2023-12-21)
 
 ** BREAKING CHANGE **
 
 - Use the new regional endpoints
 
-
 ## 1.1.22 (2023-12-15)
 
 - Fix context format and add test
 
 ## 1.1.21 (2023-12-11)
 
 - Support the new regional endpoints.
```

### Comparing `nuclia-2.0.9/LICENSE` & `nuclia-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/README.md` & `nuclia-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/01-README.md` & `nuclia-2.1.0/docs/01-README.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/02-auth.md` & `nuclia-2.1.0/docs/02-auth.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/03-kb.md` & `nuclia-2.1.0/docs/03-kb.md`

 * *Files 0% similar despite different names*

```diff
@@ -188,9 +188,9 @@
   nuclia kb logs get --type=SEARCH --month=2024-02
   ```
 
 - SDK:
   ```python
   from nuclia import sdk
   kb = sdk.NucliaKB()
-  kb.logs(type="FEEDBACK", month="2024-02")
+  kb.logs.get(type="FEEDBACK", month="2024-02")
   ```
```

### Comparing `nuclia-2.0.9/docs/04-upload.md` & `nuclia-2.1.0/docs/04-upload.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/05-search.md` & `nuclia-2.1.0/docs/05-search.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/06-read.md` & `nuclia-2.1.0/docs/06-read.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/07-nua.md` & `nuclia-2.1.0/docs/07-nua.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/08-import-export.md` & `nuclia-2.1.0/docs/08-import-export.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/docs/09-manage.md` & `nuclia-2.1.0/docs/09-manage.md`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/cli/run.py` & `nuclia-2.1.0/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/cli/utils.py` & `nuclia-2.1.0/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/config.py` & `nuclia-2.1.0/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/data.py` & `nuclia-2.1.0/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/decorators.py` & `nuclia-2.1.0/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/exceptions.py` & `nuclia-2.1.0/nuclia/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,7 +24,11 @@
 
 class AlreadyConsumed(Exception):
     pass
 
 
 class GettingRemoteFileError(Exception):
     pass
+
+
+class RateLimitError(Exception):
+    pass
```

### Comparing `nuclia-2.0.9/nuclia/lib/kb.py` & `nuclia-2.1.0/nuclia/lib/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import base64
 import csv
 import os
 from enum import Enum
 from typing import Dict, Optional
 
 import aiofiles
+import backoff
 import httpx
 import requests
-from nucliadb_models.search import ChatRequest
+from nucliadb_models.search import AskRequest, SummarizeRequest
 from nucliadb_sdk import NucliaDB, NucliaDBAsync, Region
 from tqdm import tqdm
 
+from nuclia.exceptions import RateLimitError
 from nuclia.lib.utils import handle_http_errors
 
 RESOURCE_PATH = "/resource/{rid}"
 RESOURCE_PATH_BY_SLUG = "/slug/{slug}"
 SEARCH_PATH = "/search"
 CREATE_RESOURCE_PATH = "/resources"
 CREATE_VECTORSET = "/vectorset/{vectorset}"
 VECTORSETS = "/vectorsets"
 COUNTER = "/counters"
 SEARCH_URL = "/search"
 FIND_URL = "/find"
-CHAT_URL = "/chat"
+ASK_URL = "/ask"
+SUMMARIZE_URL = "/summarize"
 LABELS_URL = "/labelsets"
 ENTITIES_URL = "/entitiesgroups"
 DOWNLOAD_EXPORT_URL = "/export/{export_id}"
 DOWNLOAD_URL = "/{uri}"
 TUS_UPLOAD_RESOURCE_URL = "/resource/{rid}/file/{field}/tusupload"
 TUS_UPLOAD_URL = "/tusupload"
 ACTIVITY_LOG_URL = "/activity/download?type={type}&month={month}"
@@ -159,20 +162,20 @@
             )
             self.stream_session = requests.Session()
             self.stream_session.headers.update(self.reader_headers)
             self.writer_session = httpx.Client(
                 headers=self.writer_headers, base_url=url  # type: ignore
             )
 
-    def chat(self, request: ChatRequest):
+    def ask(self, request: AskRequest, timeout: int = 1000):
         if self.url is None or self.stream_session is None:
             raise Exception("KB not configured")
-        url = f"{self.url}{CHAT_URL}"
+        url = f"{self.url}{ASK_URL}"
         response: requests.Response = self.stream_session.post(
-            url, data=request.json(), stream=True
+            url, data=request.json(), stream=True, timeout=timeout
         )
         handle_http_errors(response)
         return response
 
     def download(self, uri: str) -> bytes:
         # uri has format
         # /kb/2a00d5b4-cfcc-48eb-85ac-d70bfd38b26d/resource/41d02aac4ade48098b23e38141807738/file/file/download/field
@@ -186,14 +189,17 @@
 
         new_uri = "/".join(uri_parts[3:])
         url = DOWNLOAD_URL.format(uri=new_uri)
         response: httpx.Response = self.reader_session.get(url)
         handle_http_errors(response)
         return response.content
 
+    @backoff.on_exception(
+        backoff.expo, RateLimitError, jitter=backoff.random_jitter, max_tries=5
+    )
     def start_tus_upload(
         self,
         size: int,
         filename: str,
         field: Optional[str] = None,
         rid: Optional[str] = None,
         md5: Optional[str] = None,
@@ -303,20 +309,20 @@
             self.reader_session = httpx.AsyncClient(
                 headers=self.reader_headers, base_url=url  # type: ignore
             )
             self.writer_session = httpx.AsyncClient(
                 headers=self.writer_headers, base_url=url  # type: ignore
             )
 
-    async def chat(self, request: ChatRequest, timeout: int = 1000):
+    async def ask(self, request: AskRequest, timeout: int = 1000):
         if self.url is None or self.reader_session is None:
             raise Exception("KB not configured")
-        url = f"{self.url}{CHAT_URL}"
+        url = f"{self.url}{ASK_URL}"
         req = self.reader_session.build_request(
-            "POST", url, json=request.dict(), timeout=1000
+            "POST", url, json=request.dict(), timeout=timeout
         )
         response = await self.reader_session.send(req, stream=True)
         handle_http_errors(response)
         return response
 
     async def download_export(self, export_id: str, path: str, chunk_size: int):
         if self.reader_session is None:
@@ -355,14 +361,17 @@
 
         new_uri = "/".join(uri_parts[3:])
         url = DOWNLOAD_URL.format(uri=new_uri)
         response = await self.reader_session.get(url)
         handle_http_errors(response)
         return response.content
 
+    @backoff.on_exception(
+        backoff.expo, RateLimitError, jitter=backoff.random_jitter, max_tries=5
+    )
     async def start_tus_upload(
         self,
         size: int,
         filename: str,
         field: Optional[str] = None,
         rid: Optional[str] = None,
         md5: Optional[str] = None,
@@ -403,7 +412,18 @@
         # upload url has all path, we should remove /kb/kbid/
         upload_url = "/" + "/".join(upload_url.split("/")[3:])
         response = await self.writer_session.patch(
             upload_url, headers=headers, content=data
         )
         handle_http_errors(response)
         return int(response.headers.get("Upload-Offset"))
+
+    async def summarize(self, request: SummarizeRequest, timeout: int = 1000):
+        if self.url is None or self.writer_session is None:
+            raise Exception("KB not configured")
+        url = f"{self.url}{SUMMARIZE_URL}"
+        assert self.reader_session
+        response = await self.reader_session.post(
+            url, json=request.dict(), timeout=timeout
+        )
+        handle_http_errors(response)
+        return response
```

### Comparing `nuclia-2.0.9/nuclia/lib/nua.py` & `nuclia-2.1.0/nuclia/lib/nua.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import base64
 from time import sleep
-from typing import Any, Dict, List, Optional, Type, TypeVar
+from typing import Any, AsyncIterator, Dict, Iterator, List, Optional, Type, TypeVar
 
 import aiofiles
+from deprecated import deprecated
 from httpx import AsyncClient, Client
 from nucliadb_protos.writer_pb2 import BrokerMessage
 from pydantic import BaseModel
 
 from nuclia import REGIONAL
 from nuclia.exceptions import NuaAPIException
 from nuclia.lib.nua_responses import (
     ChatModel,
     ChatResponse,
     ConfigSchema,
     Empty,
+    GenerativeChunk,
+    GenerativeResponse,
     LearningConfigurationCreation,
     LearningConfigurationUpdate,
     LinkUpload,
     ProcessRequestStatus,
     ProcessRequestStatusResults,
     PushPayload,
     PushResponseV2,
@@ -26,15 +29,14 @@
     Sentence,
     Source,
     StoredLearningConfiguration,
     SummarizedModel,
     SummarizeModel,
     SummarizeResource,
     Tokens,
-    UserPrompt,
 )
 
 SENTENCE_PREDICT = "/api/v1/predict/sentence"
 CHAT_PREDICT = "/api/v1/predict/chat"
 SUMMARIZE_PREDICT = "/api/v1/predict/summarize"
 TOKENS_PREDICT = "/api/v1/predict/tokens"
 QUERY_PREDICT = "/api/v1/predict/query"
@@ -45,57 +47,87 @@
 SCHEMA_KBID = "/api/v1/schema"
 CONFIG = "/api/v1/config"
 
 ConvertType = TypeVar("ConvertType", bound=BaseModel)
 
 
 class NuaClient:
-    def __init__(self, region: str, account: str, token: str):
+    def __init__(
+        self,
+        region: str,
+        account: str,
+        token: Optional[str] = None,
+        headers: Optional[Dict[str, str]] = None,
+    ):
         self.region = region
         self.account = account
         self.token = token
         if "http" in region:
             self.url = region.strip("/")
         else:
             self.url = REGIONAL.format(region=region).strip("/")
-        self.headers = {"X-STF-NUAKEY": f"Bearer {token}"}
+
+        if token is None and headers is not None:
+            self.headers = headers
+        else:
+            self.headers = {"X-STF-NUAKEY": f"Bearer {token}"}
+
+        self.stream_headers = self.headers.copy()
+        self.stream_headers["Accept"] = "application/x-ndjson"
         self.client = Client(headers=self.headers, base_url=self.url)
+        self.stream_client = Client(headers=self.stream_headers, base_url=self.url)
 
     def _request(
         self,
         method: str,
         url: str,
         output: Type[ConvertType],
-        json: Optional[Dict[Any, Any]] = None,
+        payload: Optional[Dict[Any, Any]] = None,
         timeout: int = 60,
     ) -> ConvertType:
-        resp = self.client.request(method, url, json=json, timeout=timeout)
+        resp = self.client.request(method, url, json=payload, timeout=timeout)
         if resp.status_code != 200:
             raise NuaAPIException(code=resp.status_code, detail=resp.content.decode())
 
         try:
             data = output.parse_obj(resp.json())
         except Exception:
             data = output.parse_raw(resp.content)
         return data
 
+    def _stream(
+        self,
+        method: str,
+        url: str,
+        payload: Optional[Dict[Any, Any]] = None,
+        timeout: int = 60,
+    ) -> Iterator[GenerativeChunk]:
+        with self.stream_client.stream(
+            method,
+            url,
+            json=payload,
+            timeout=timeout,
+        ) as response:
+            for json_body in response.iter_lines():
+                yield GenerativeChunk.parse_raw(json_body)  # type: ignore
+
     def add_config_predict(self, kbid: str, config: LearningConfigurationCreation):
         endpoint = f"{self.url}{CONFIG}/{kbid}"
         self._request(
-            "POST", endpoint, json=config.dict(exclude_none=True), output=Empty
+            "POST", endpoint, payload=config.dict(exclude_none=True), output=Empty
         )
 
     def del_config_predict(self, kbid: str):
         endpoint = f"{self.url}{CONFIG}/{kbid}"
         self._request("DELETE", endpoint, output=Empty)
 
     def update_config_predict(self, kbid: str, config: LearningConfigurationUpdate):
         endpoint = f"{self.url}{CONFIG}/{kbid}"
         self._request(
-            "POST", endpoint, json=config.dict(exclude_none=True), output=Empty
+            "POST", endpoint, payload=config.dict(exclude_none=True), output=Empty
         )
 
     def schema_predict(self, kbid: Optional[str] = None) -> ConfigSchema:
         endpoint = f"{self.url}{SCHEMA}"
         if kbid is not None:
             endpoint = f"{self.url}{SCHEMA_KBID}/{kbid}"
         return self._request("GET", endpoint, output=ConfigSchema)
@@ -130,64 +162,60 @@
             endpoint += f"&semantic_model={semantic_model}"
         if token_model:
             endpoint += f"&token_model={token_model}"
         if generative_model:
             endpoint += f"&generative_model={generative_model}"
         return self._request("GET", endpoint, output=QueryInfo)
 
-    def generate_predict(
-        self, text: str, model: Optional[str] = None, timeout: int = 300
+    def generate(
+        self, body: ChatModel, model: Optional[str] = None, timeout: int = 300
     ) -> ChatResponse:
         endpoint = f"{self.url}{CHAT_PREDICT}"
         if model:
             endpoint += f"?model={model}"
 
-        body = ChatModel(
-            question="",
-            retrieval=False,
-            user_id="Nuclia PY CLI",
-            user_prompt=UserPrompt(prompt=text),
-        )
         return self._request(
-            "POST", endpoint, json=body.dict(), output=ChatResponse, timeout=timeout
+            "POST", endpoint, payload=body.dict(), output=ChatResponse, timeout=timeout
         )
 
+    def generate_stream(
+        self, body: ChatModel, model: Optional[str] = None, timeout: int = 300
+    ) -> Iterator[GenerativeResponse]:
+        endpoint = f"{self.url}{CHAT_PREDICT}"
+        if model:
+            endpoint += f"?model={model}"
+
+        for gr in self._stream(
+            "POST",
+            endpoint,
+            payload=body.dict(),
+            timeout=timeout,
+        ):
+            yield gr.chunk
+
     def summarize(
         self, documents: Dict[str, str], model: Optional[str] = None, timeout: int = 300
     ) -> SummarizedModel:
         endpoint = f"{self.url}{SUMMARIZE_PREDICT}"
         if model:
             endpoint += f"?model={model}"
 
         body = SummarizeModel(
             resources={
                 key: SummarizeResource(fields={"field": document})
                 for key, document in documents.items()
             }
         )
         return self._request(
-            "POST", endpoint, json=body.dict(), output=SummarizedModel, timeout=timeout
-        )
-
-    def generate_retrieval(
-        self,
-        question: str,
-        context: List[str],
-        model: Optional[str] = None,
-    ) -> ChatResponse:
-        endpoint = f"{self.url}{CHAT_PREDICT}"
-        if model:
-            endpoint += f"?model={model}"
-        body = ChatModel(
-            question=question,
-            retrieval=True,
-            user_id="Nuclia PY CLI",
-            query_context=context,
+            "POST",
+            endpoint,
+            payload=body.dict(),
+            output=SummarizedModel,
+            timeout=timeout,
         )
-        return self._request("POST", endpoint, json=body.dict(), output=ChatResponse)
 
     def process_file(self, path: str, kbid: str = "default") -> PushResponseV2:
         filename = path.split("/")[-1]
         upload_endpoint = f"{self.url}{UPLOAD_PROCESS}"
 
         headers = self.headers.copy()
         headers["X-FILENAME"] = base64.b64encode(filename.encode()).decode()
@@ -199,15 +227,15 @@
         payload = PushPayload(
             uuid=None, source=Source.HTTP, kbid=RestrictedIDString(kbid)
         )
 
         payload.filefield[filename] = resp.content.decode()
         process_endpoint = f"{self.url}{PUSH_PROCESS}"
         return self._request(
-            "POST", process_endpoint, json=payload.dict(), output=PushResponseV2
+            "POST", process_endpoint, payload=payload.dict(), output=PushResponseV2
         )
 
     def process_link(
         self,
         url: str,
         kbid: Optional[str] = None,
         headers: Dict[str, str] = {},
@@ -219,15 +247,15 @@
         )
 
         payload.linkfield["link"] = LinkUpload(
             link=url, headers=headers, cookies=cookies, localstorage=localstorage
         )
         process_endpoint = f"{self.url}{PUSH_PROCESS}"
         return self._request(
-            "POST", process_endpoint, json=payload.dict(), output=PushResponseV2
+            "POST", process_endpoint, payload=payload.dict(), output=PushResponseV2
         )
 
     def wait_for_processing(
         self, response: PushResponseV2, timeout: int = 30
     ) -> Optional[BrokerMessage]:
         resp = self.processing_id_status(response.processing_id)
         count = timeout
@@ -249,61 +277,91 @@
 
     def processing_id_status(self, process_id: str) -> ProcessRequestStatus:
         activity_endpoint = f"{self.url}{STATUS_PROCESS}/{process_id}"
         return self._request("GET", activity_endpoint, ProcessRequestStatus)
 
 
 class AsyncNuaClient:
-    def __init__(self, region: str, account: str, token: str):
+    def __init__(
+        self,
+        region: str,
+        account: str,
+        token: Optional[str] = None,
+        headers: Optional[Dict[str, str]] = None,
+    ):
         self.region = region
         self.account = account
         self.token = token
         if "http" in region:
             self.url = region.strip("/")
         else:
             self.url = REGIONAL.format(region=region).strip("/")
-        self.headers = {"X-STF-NUAKEY": f"Bearer {token}"}
+        if token is None and headers is not None:
+            self.headers = headers
+        else:
+            self.headers = {"X-STF-NUAKEY": f"Bearer {token}"}
+
+        self.stream_headers = self.headers.copy()
+        self.stream_headers["Accept"] = "application/x-ndjson"
+
         self.client = AsyncClient(headers=self.headers, base_url=self.url)
+        self.stream_client = AsyncClient(headers=self.stream_headers, base_url=self.url)
 
     async def _request(
         self,
         method: str,
         url: str,
         output: Type[ConvertType],
-        json: Optional[Dict[Any, Any]] = None,
+        payload: Optional[Dict[Any, Any]] = None,
         timeout: int = 60,
     ) -> ConvertType:
-        resp = await self.client.request(method, url, json=json, timeout=timeout)
+        resp = await self.client.request(method, url, json=payload, timeout=timeout)
         if resp.status_code != 200:
             raise NuaAPIException(code=resp.status_code, detail=resp.content.decode())
 
         try:
-            data = output.parse_obj(resp.json())
+            data = output.parse_raw(resp.json())
         except Exception:
-            data = output()
+            data = output.parse_raw(resp.content)
         return data
 
+    async def _stream(
+        self,
+        method: str,
+        url: str,
+        payload: Optional[Dict[Any, Any]] = None,
+        timeout: int = 60,
+    ) -> AsyncIterator[GenerativeChunk]:
+        async with self.stream_client.stream(
+            method,
+            url,
+            json=payload,
+            timeout=timeout,
+        ) as response:
+            async for json_body in response.aiter_lines():
+                yield GenerativeChunk.parse_raw(json_body)  # type: ignore
+
     async def add_config_predict(
         self, kbid: str, config: LearningConfigurationCreation
     ):
         endpoint = f"{CONFIG}/{kbid}"
         await self._request(
-            "GET", endpoint, json=config.dict(exclude_none=True), output=Empty
+            "GET", endpoint, payload=config.dict(exclude_none=True), output=Empty
         )
 
     async def del_config_predict(self, kbid: str):
         endpoint = f"{self.url}{CONFIG}/{kbid}"
         await self._request("DELETE", endpoint, output=Empty)
 
     async def update_config_predict(
         self, kbid: str, config: LearningConfigurationUpdate
     ):
         endpoint = f"{CONFIG}/{kbid}"
         await self._request(
-            "POST", endpoint, json=config.dict(exclude_none=True), output=Empty
+            "POST", endpoint, payload=config.dict(exclude_none=True), output=Empty
         )
 
     async def schema_predict(self, kbid: Optional[str] = None) -> ConfigSchema:
         endpoint = f"{SCHEMA}"
         if kbid is not None:
             endpoint = f"{SCHEMA_KBID}/{kbid}"
         return await self._request("GET", endpoint, output=ConfigSchema)  # type: ignore
@@ -342,47 +400,71 @@
             endpoint += f"&semantic_model={semantic_model}"
         if token_model:
             endpoint += f"&token_model={token_model}"
         if generative_model:
             endpoint += f"&generative_model={generative_model}"
         return await self._request("GET", endpoint, output=QueryInfo)
 
+    @deprecated(version="2.1.0", reason="You should use generate function")
     async def generate_predict(
-        self, text: str, model: Optional[str] = None, timeout: int = 300
+        self, body: ChatModel, model: Optional[str] = None, timeout: int = 300
     ) -> ChatResponse:
         endpoint = f"{self.url}{CHAT_PREDICT}"
         if model:
             endpoint += f"?model={model}"
 
-        body = ChatModel(
-            question="",
-            retrieval=False,
-            user_id="Nuclia PY CLI",
-            user_prompt=UserPrompt(prompt=text),
+        return await self._request(
+            "POST", endpoint, payload=body.dict(), output=ChatResponse, timeout=timeout
         )
 
+    async def generate(
+        self, body: ChatModel, model: Optional[str] = None, timeout: int = 300
+    ) -> ChatResponse:
+        endpoint = f"{self.url}{CHAT_PREDICT}"
+        if model:
+            endpoint += f"?model={model}"
+
         return await self._request(
-            "POST", endpoint, json=body.dict(), output=ChatResponse, timeout=timeout
+            "POST", endpoint, payload=body.dict(), output=ChatResponse, timeout=timeout
         )
 
+    async def generate_stream(
+        self, body: ChatModel, model: Optional[str] = None, timeout: int = 300
+    ) -> AsyncIterator[GenerativeResponse]:
+        endpoint = f"{self.url}{CHAT_PREDICT}"
+        if model:
+            endpoint += f"?model={model}"
+
+        async for gr in self._stream(
+            "POST",
+            endpoint,
+            payload=body.dict(),
+            timeout=timeout,
+        ):
+            yield gr.chunk
+
     async def summarize(
         self, documents: Dict[str, str], model: Optional[str] = None, timeout: int = 300
     ) -> SummarizedModel:
         endpoint = f"{self.url}{SUMMARIZE_PREDICT}"
         if model:
             endpoint += f"?model={model}"
 
         body = SummarizeModel(
             resources={
                 key: SummarizeResource(fields={"field": document})
                 for key, document in documents.items()
             }
         )
         return await self._request(
-            "POST", endpoint, json=body.dict(), output=SummarizedModel, timeout=timeout
+            "POST",
+            endpoint,
+            payload=body.dict(),
+            output=SummarizedModel,
+            timeout=timeout,
         )
 
     async def generate_retrieval(
         self,
         question: str,
         context: List[str],
         model: Optional[str] = None,
@@ -393,15 +475,15 @@
         body = ChatModel(
             question=question,
             retrieval=True,
             user_id="Nuclia PY CLI",
             query_context=context,
         )
         return await self._request(
-            "POST", endpoint, json=body.dict(), output=ChatResponse
+            "POST", endpoint, payload=body.dict(), output=ChatResponse
         )
 
     async def process_link(
         self,
         url: str,
         kbid: Optional[str] = None,
         headers: Dict[str, str] = {},
@@ -413,15 +495,15 @@
         )
 
         payload.linkfield["link"] = LinkUpload(
             link=url, headers=headers, cookies=cookies, localstorage=localstorage
         )
         process_endpoint = f"{self.url}{PUSH_PROCESS}"
         return await self._request(
-            "POST", process_endpoint, json=payload.dict(), output=PushResponseV2
+            "POST", process_endpoint, payload=payload.dict(), output=PushResponseV2
         )
 
     async def process_file(
         self, path: str, kbid: Optional[str] = None
     ) -> PushResponseV2:
         filename = path.split("/")[-1]
         upload_endpoint = f"{self.url}{UPLOAD_PROCESS}"
@@ -436,15 +518,15 @@
         payload = PushPayload(
             uuid=None, source=Source.HTTP, kbid=RestrictedIDString(kbid)
         )
 
         payload.filefield[filename] = resp.content.decode()
         process_endpoint = f"{self.url}{PUSH_PROCESS}"
         return await self._request(
-            "POST", process_endpoint, json=payload.dict(), output=PushResponseV2
+            "POST", process_endpoint, payload=payload.dict(), output=PushResponseV2
         )
 
     async def wait_for_processing(
         self, response: PushResponseV2, timeout: int = 30
     ) -> Optional[BrokerMessage]:
         status = await self.processing_id_status(response.processing_id)
         count = timeout
```

### Comparing `nuclia-2.0.9/nuclia/lib/nua_responses.py` & `nuclia-2.1.0/nuclia/lib/nua_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, List, Literal, Optional, Union, cast
 
 from pydantic import BaseModel, ConstrainedStr, Field
 
 
 class GenerativeOption(BaseModel):
     name: str
     value: str
@@ -270,17 +270,17 @@
     account_seq: Optional[int] = None
     queue: Optional[ProcessingQueueType] = None
     # On Public api, uuid may be generated by the proxy, so we need to return it to the user
     uuid: Optional[str] = None
 
 
 class ProcessingStatusInfo(BaseModel):
-    last_delivered_seqid: Optional[
-        int
-    ] = None  # When none, means we already don't have information about this queue
+    last_delivered_seqid: Optional[int] = (
+        None  # When none, means we already don't have information about this queue
+    )
 
 
 class ProcessingStatus(BaseModel):
     shared: ProcessingStatusInfo
     account: Optional[ProcessingStatusInfo]
 
 
@@ -425,14 +425,62 @@
     def parse_raw(  # type: ignore
         cls,
         b: bytes,
     ):
         return ChatResponse(answer=b.decode())
 
 
+GenerativeResponseType = Literal["text", "meta", "citations", "status"]
+
+
+class TextGenerativeResponse(BaseModel):
+    type: Literal["text"] = "text"
+    text: str
+
+
+class MetaGenerativeResponse(BaseModel):
+    type: Literal["meta"] = "meta"
+    input_tokens: int
+    output_tokens: int
+    timings: dict[str, float]
+
+
+class CitationsGenerativeResponse(BaseModel):
+    type: Literal["citations"] = "citations"
+    citations: dict[str, Any]
+
+
+class StatusGenerativeResponse(BaseModel):
+    type: Literal["status"] = "status"
+    code: str
+    details: Optional[str] = None
+
+
+GenerativeResponse = Union[
+    TextGenerativeResponse,
+    MetaGenerativeResponse,
+    CitationsGenerativeResponse,
+    StatusGenerativeResponse,
+]
+
+
+class GenerativeChunk(BaseModel):
+    chunk: GenerativeResponse = Field(..., discriminator="type")
+
+
+class GenerativeFullResponse(BaseModel):
+    input_tokens: Optional[int] = None
+    output_tokens: Optional[int] = None
+    timings: Optional[dict[str, float]] = None
+    citations: Optional[dict[str, Any]] = None
+    code: Optional[str] = None
+    details: Optional[str] = None
+    text: str
+
+
 class StoredLearningConfiguration(BaseModel):
     resource_labelers_models: Optional[List[str]] = None
     paragraph_labelers_models: Optional[List[str]] = None
     intent_models: Optional[List[str]] = None
 
     semantic_model: str
     anonymization_model: str
```

### Comparing `nuclia-2.0.9/nuclia/sdk/__init__.py` & `nuclia-2.1.0/nuclia/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/accounts.py` & `nuclia-2.1.0/nuclia/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/agent.py` & `nuclia-2.1.0/nuclia/sdk/agent.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/auth.py` & `nuclia-2.1.0/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/export_import.py` & `nuclia-2.1.0/nuclia/sdk/export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/kbs.py` & `nuclia-2.1.0/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/nucliadb.py` & `nuclia-2.1.0/nuclia/sdk/nucliadb.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/process.py` & `nuclia-2.1.0/nuclia/sdk/process.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/sdk/resource.py` & `nuclia-2.1.0/nuclia/sdk/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "texts",
     "files",
     "usermetadata",
     "fieldmetadata",
     "title",
     "summary",
     "metadata",
+    "security",
 ]
 
 
 class NucliaResource:
     """
     Manage existing resource
```

### Comparing `nuclia-2.0.9/nuclia/sdk/search.py` & `nuclia-2.1.0/nuclia/sdk/search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-import base64
+import sys
+import warnings
 from dataclasses import dataclass
-from io import BytesIO
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from nucliadb_models.search import (
+    AskRequest,
+    AskResponseItem,
     ChatRequest,
     Filter,
     FindRequest,
     KnowledgeboxFindResults,
+    KnowledgeboxSearchResults,
     Relations,
     SearchOptions,
     SearchRequest,
+    SyncAskResponse,
 )
+from pydantic import ValidationError
 
 from nuclia.data import get_async_auth, get_auth
 from nuclia.decorators import kb, pretty
 from nuclia.lib.kb import AsyncNucliaDBClient, NucliaDBClient
 from nuclia.sdk.auth import AsyncNucliaAuth, NucliaAuth
 
 
 @dataclass
 class ChatAnswer:
     answer: bytes
     learning_id: str
     relations_result: Optional[Relations]
     find_result: Optional[KnowledgeboxFindResults]
+    citations: Optional[Dict[str, Any]]
+    timings: Optional[Dict[str, float]]
+    tokens: Optional[Dict[str, int]]
 
     def __str__(self):
         return self.answer.decode()
 
 
 class NucliaSearch:
     """
@@ -48,25 +56,33 @@
     @pretty
     def search(
         self,
         *,
         query: Union[str, SearchRequest] = "",
         filters: Optional[Union[List[str], List[Filter]]] = None,
         **kwargs,
-    ):
+    ) -> KnowledgeboxSearchResults:
         """
         Perform a search query.
 
         See https://docs.nuclia.dev/docs/api#tag/Search/operation/Search_Knowledge_Box_kb__kbid__search_post
         """
         ndb: AsyncNucliaDBClient = kwargs["ndb"]
         if isinstance(query, str):
             req = SearchRequest(query=query, filters=(filters or []))  # type: ignore
-        else:
+        elif isinstance(query, SearchRequest):
             req = query
+        elif isinstance(query, dict):
+            try:
+                req = SearchRequest.parse_obj(query)
+            except ValidationError as exc:
+                print(exc)
+                sys.exit(1)
+        else:
+            raise Exception("Invalid Query either str or SearchRequest")
 
         return ndb.ndb.search(req, kbid=ndb.kbid)
 
     @kb
     @pretty
     def find(
         self,
@@ -87,67 +103,76 @@
             req = FindRequest(
                 query=query,
                 highlight=highlight,
                 filters=filters or [],  # type: ignore
             )
         elif isinstance(query, FindRequest):
             req = query
+        elif isinstance(query, dict):
+            try:
+                req = FindRequest.parse_obj(query)
+            except ValidationError as exc:
+                print(exc)
+                sys.exit(1)
         else:
             raise Exception("Invalid Query either str or FindRequest")
 
         if relations:
             req.features.append(SearchOptions.RELATIONS)
 
         return ndb.ndb.find(req, kbid=ndb.kbid)
 
     @kb
     def chat(
         self,
         *,
-        query: Union[str, ChatRequest],
+        query: Union[str, dict, ChatRequest],
         filters: Optional[Union[List[str], List[Filter]]] = None,
         **kwargs,
     ):
         """
         Answer a question.
 
         See https://docs.nuclia.dev/docs/api#tag/Search/operation/Chat_Knowledge_Box_kb__kbid__chat_post
         """
         ndb: NucliaDBClient = kwargs["ndb"]
         if isinstance(query, str):
-            req = ChatRequest(
+            req = AskRequest(
                 query=query,
                 filters=filters or [],  # type: ignore
             )
+        elif isinstance(query, dict):
+            try:
+                req = AskRequest.parse_obj(query)
+            except ValidationError as exc:
+                print(exc)
+                sys.exit(1)
+        elif isinstance(query, ChatRequest):
+            # Convert ChatRequest to AskRequest
+            req = AskRequest.parse_obj(query.dict())
         else:
-            req = query
-        response = ndb.chat(req)
-        header = response.raw.read(4)
-        payload_size = int.from_bytes(header, byteorder="big", signed=False)
-        data = response.raw.read(payload_size)
-
-        find_result = KnowledgeboxFindResults.parse_raw(base64.b64decode(data))
+            raise ValueError("Invalid query type. Must be str, dict or ChatRequest.")
 
-        data = response.raw.read()
-        answer, relations_payload = data.split(b"_END_")
-
-        relations_payload = response.raw.read()
-
-        learning_id = response.headers.get("NUCLIA-LEARNING-ID")
-
-        relations_result = None
-        if len(relations_payload) > 0:
-            relations_result = Relations.parse_raw(base64.b64decode(relations_payload))
-
-        return ChatAnswer(
-            answer=answer,
-            learning_id=learning_id,
-            relations_result=relations_result,
-            find_result=find_result,
+        ask_response: SyncAskResponse = ndb.ndb.ask(kbid=ndb.kbid, content=req)
+        # Convert to ChatAnswer
+        result = ChatAnswer(
+            answer=ask_response.answer.encode(),
+            learning_id=ask_response.learning_id,
+            relations_result=ask_response.relations,
+            find_result=ask_response.retrieval_results,
+            citations=ask_response.citations,
+            timings=None,
+            tokens=None,
         )
+        if ask_response.metadata is not None:
+            if ask_response.metadata.timings is not None:
+                result.timings = ask_response.metadata.timings.dict()
+            if ask_response.metadata.tokens is not None:
+                result.tokens = ask_response.metadata.tokens.dict()
+        return result
 
 
 class AsyncNucliaSearch:
     """
     Perform search on a Knowledge Box.
 
     `find` and `search` accept the following parameters:
@@ -173,16 +198,24 @@
         Perform a search query.
 
         See https://docs.nuclia.dev/docs/api#tag/Search/operation/Search_Knowledge_Box_kb__kbid__search_post
         """
         ndb: NucliaDBClient = kwargs["ndb"]
         if isinstance(query, str):
             req = SearchRequest(query=query, filters=(filters or []))
-        else:
+        elif isinstance(query, SearchRequest):
             req = query
+        elif isinstance(query, dict):
+            try:
+                req = SearchRequest.parse_obj(query)
+            except ValidationError as exc:
+                print(exc)
+                sys.exit(1)
+        else:
+            raise Exception("Invalid Query either str or SearchRequest")
 
         return await ndb.ndb.search(req, kbid=ndb.kbid)
 
     @kb
     @pretty
     async def find(
         self,
@@ -200,61 +233,90 @@
         """
 
         ndb: AsyncNucliaDBClient = kwargs["ndb"]
         if isinstance(query, str) and highlight is not None:
             req = FindRequest(query=query, highlight=highlight, filters=(filters or []))
         elif isinstance(query, FindRequest):
             req = query
+        elif isinstance(query, dict):
+            try:
+                req = FindRequest.parse_obj(query)
+            except ValidationError as exc:
+                print(exc)
+                sys.exit(1)
         else:
             raise Exception("Invalid Query either str or FindRequest")
 
         if relations:
             req.features.append(SearchOptions.RELATIONS)
 
         return await ndb.ndb.find(req, kbid=ndb.kbid)
 
     @kb
     async def chat(
         self,
         *,
-        query: Union[str, ChatRequest],
+        query: Union[str, dict, ChatRequest],
         filters: Optional[List[str]] = None,
         timeout: int = 100,
         **kwargs,
     ):
         """
         Answer a question.
 
         See https://docs.nuclia.dev/docs/api#tag/Search/operation/Chat_Knowledge_Box_kb__kbid__chat_post
         """
-        ndb: AsyncNucliaDBClient = kwargs["ndb"]
+        ndb: NucliaDBClient = kwargs["ndb"]
         if isinstance(query, str):
-            req = ChatRequest(query=query, filters=(filters or []))
+            req = AskRequest(
+                query=query,
+                filters=filters or [],  # type: ignore
+            )
+        elif isinstance(query, dict):
+            try:
+                req = AskRequest.parse_obj(query)
+            except ValidationError as exc:
+                print(exc)
+                sys.exit(1)
+        elif isinstance(query, ChatRequest):
+            # Convert ChatRequest to AskRequest
+            req = AskRequest.parse_obj(query.dict())
         else:
-            req = query
-
-        content = b""
-        response = await ndb.chat(req, timeout=timeout)
-
-        content = await response.aread()
-        stream = BytesIO(content)
-        header = stream.read(4)
-        payload_size = int.from_bytes(header, byteorder="big", signed=False)
-        data = stream.read(payload_size)
-
-        find_result = KnowledgeboxFindResults.parse_raw(base64.b64decode(data))
-
-        data = stream.read()
-        answer, relations_payload = data.split(b"_END_")
-
-        learning_id = response.headers.get("NUCLIA-LEARNING-ID")
-
-        relations_result = None
-        if len(relations_payload) > 0:
-            relations_result = Relations.parse_raw(base64.b64decode(relations_payload))
-
-        return ChatAnswer(
-            answer=answer,
-            learning_id=learning_id,
-            relations_result=relations_result,
-            find_result=find_result,
+            raise ValueError("Invalid query type. Must be str, dict or ChatRequest.")
+        ask_stream_response = await ndb.ask(req, timeout=timeout)
+        # Parse the stream response and convert to ChatAnswer
+        result = ChatAnswer(
+            answer=b"",
+            learning_id=ask_stream_response.headers.get("NUCLIA-LEARNING-ID", ""),
+            relations_result=None,
+            find_result=None,
+            citations=None,
+            timings=None,
+            tokens=None,
         )
+        async for line in ask_stream_response.aiter_lines():
+            try:
+                ask_response_item = AskResponseItem.parse_raw(line).item
+            except Exception as e:
+                warnings.warn(f"Failed to parse AskResponseItem: {e}. item: {line}")
+                continue
+            if ask_response_item.type == "answer":
+                result.answer += ask_response_item.text.encode()
+            elif ask_response_item.type == "retrieval":
+                result.find_result = ask_response_item.results
+            elif ask_response_item.type == "relations":
+                result.relations_result = ask_response_item.relations
+            elif ask_response_item.type == "citations":
+                result.citations = ask_response_item.citations
+            elif ask_response_item.type == "metadata":
+                if ask_response_item.timings:
+                    result.timings = ask_response_item.timings.dict()
+                if ask_response_item.tokens:
+                    result.tokens = ask_response_item.tokens.dict()
+            elif ask_response_item.type == "status":
+                # Status is ignored
+                pass
+            else:  # pragma: no cover
+                warnings.warn(
+                    f"Unknown chat stream item type: {ask_response_item.type}"
+                )
+        return result
```

### Comparing `nuclia-2.0.9/nuclia/sdk/upload.py` & `nuclia-2.1.0/nuclia/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/fixtures.py` & `nuclia-2.1.0/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_kb/test_conversation.py` & `nuclia-2.1.0/nuclia/tests/test_kb/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_kb/test_export_import.py` & `nuclia-2.1.0/nuclia/tests/test_kb/test_export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_kb/test_labels.py` & `nuclia-2.1.0/nuclia/tests/test_kb/test_labels.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_kb/test_resource.py` & `nuclia-2.1.0/nuclia/tests/test_kb/test_resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_kb/test_search.py` & `nuclia-2.1.0/nuclia/tests/test_kb/test_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,25 +9,58 @@
     search = NucliaSearch()
     results = search.find(query="Who is hedy Lamarr?")
     assert len(results.resources.keys()) == 2
     titles = [r.title for r in results.resources.values()]
     assert "Lamarr Lesson plan.pdf" in titles
 
 
+def test_find_object(testing_config):
+    if IS_PROD:
+        assert True
+        return
+    search = NucliaSearch()
+    results = search.find(query={"query": "Who is hedy Lamarr?"})
+    assert len(results.resources.keys()) == 2
+    titles = [r.title for r in results.resources.values()]
+    assert "Lamarr Lesson plan.pdf" in titles
+
+
+def test_chat(testing_config):
+    if IS_PROD:
+        assert True
+        return
+    search = NucliaSearch()
+    results = search.chat(query="Who is hedy Lamarr?")
+    answer = results.answer.decode()
+    print("Chat answer: ", answer)
+    assert "Lamarr" in answer
+
+
 def test_search(testing_config):
     if IS_PROD:
         assert True
         return
     search = NucliaSearch()
     results = search.search(query="Who is hedy Lamarr?")
     assert len(results.resources.keys()) == 2
     titles = [r.title for r in results.resources.values()]
     assert "Lamarr Lesson plan.pdf" in titles
 
 
+def test_search_object(testing_config):
+    if IS_PROD:
+        assert True
+        return
+    search = NucliaSearch()
+    results = search.search(query={"query": "Who is hedy Lamarr?"})
+    assert len(results.resources.keys()) == 2
+    titles = [r.title for r in results.resources.values()]
+    assert "Lamarr Lesson plan.pdf" in titles
+
+
 def test_filters(testing_config):
     if IS_PROD:
         assert True
         return
     search = NucliaSearch()
     results = search.find(
         query="Who is hedy Lamarr?", filters=["/icon/application/pdf"]
```

### Comparing `nuclia-2.0.9/nuclia/tests/test_manage/test_auth.py` & `nuclia-2.1.0/nuclia/tests/test_manage/test_auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_manage/test_kb.py` & `nuclia-2.1.0/nuclia/tests/test_manage/test_kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/test_nucliadb/test_crud.py` & `nuclia-2.1.0/nuclia/tests/test_nucliadb/test_crud.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia/tests/unit/test_export_import.py` & `nuclia-2.1.0/nuclia/tests/unit/test_export_import.py`

 * *Files identical despite different names*

### Comparing `nuclia-2.0.9/nuclia.egg-info/SOURCES.txt` & `nuclia-2.1.0/nuclia.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 docs/08-import-export.md
 docs/09-manage.md
 nuclia/__init__.py
 nuclia/config.py
 nuclia/data.py
 nuclia/decorators.py
 nuclia/exceptions.py
+nuclia/py.typed
 nuclia.egg-info/PKG-INFO
 nuclia.egg-info/SOURCES.txt
 nuclia.egg-info/dependency_links.txt
 nuclia.egg-info/entry_points.txt
 nuclia.egg-info/requires.txt
 nuclia.egg-info/top_level.txt
 nuclia.egg-info/zip-safe
```

### Comparing `nuclia-2.0.9/setup.py` & `nuclia-2.1.0/setup.py`

 * *Files identical despite different names*

