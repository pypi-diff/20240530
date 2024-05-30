# Comparing `tmp/crowdin-api-client-1.8.0.tar.gz` & `tmp/crowdin-api-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/crowdin-api-client-python/crowdin-api-client-python/dist/.tmp-jnrimcx8/crowdin-api-client-1.8.0.tar", last modified: Mon Jan 16 08:02:50 2023, max compression
+gzip compressed data, was "/home/runner/work/crowdin-api-client-python/crowdin-api-client-python/dist/.tmp-tmbnn4xh/crowdin-api-client-1.9.0.tar", last modified: Mon Feb 20 16:21:22 2023, max compression
```

## Comparing `crowdin-api-client-1.8.0.tar` & `crowdin-api-client-1.9.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/abstract/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/bundles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/bundles/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/bundles/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/bundles/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/dictionaries/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/dictionaries/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/distributions/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/distributions/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/distributions/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/groups/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/groups/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/groups/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/labels/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/labels/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/labels/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/labels/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/languages/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/languages/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/languages/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/languages/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/machine_translation_engines/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/machine_translation_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/machine_translation_engines/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/machine_translation_engines/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    21898 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_strings/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_strings/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_strings/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/source_strings/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/storages/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/storages/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_comments/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_comments/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_comments/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_comments/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_translations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_translations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_translations/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/string_translations/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_memory/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_memory/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_memory/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_memory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_status/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_status/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_status/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translations/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/translations/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/users/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/users/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/users/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/users/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/vendors/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/vendors/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/api_resources/workflows/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/crowdin_api/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/crowdin_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-01-16 08:02:50.000000 crowdin-api-client-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-01-16 08:02:34.000000 crowdin-api-client-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/abstract/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/bundles/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/bundles/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/bundles/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/dictionaries/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/dictionaries/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/distributions/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/distributions/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/distributions/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/groups/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/groups/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/groups/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/labels/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/labels/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/labels/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/languages/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/languages/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/languages/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/machine_translation_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/machine_translation_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/machine_translation_engines/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/machine_translation_engines/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21898 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_strings/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_strings/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_strings/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/source_strings/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/storages/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_comments/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_comments/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_comments/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_comments/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_translations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_translations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_translations/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/string_translations/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_memory/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_memory/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_memory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_status/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_status/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_status/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translations/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/translations/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/users/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/users/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/users/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/users/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/vendors/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/api_resources/workflows/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/crowdin_api/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/crowdin_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-20 16:21:22.000000 crowdin-api-client-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-02-20 16:21:07.000000 crowdin-api-client-1.9.0/setup.py
```

### Comparing `crowdin-api-client-1.8.0/LICENSE` & `crowdin-api-client-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/PKG-INFO` & `crowdin-api-client-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crowdin-api-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python client library for Crowdin API v2
 Home-page: https://github.com/crowdin/crowdin-api-client-python
 Author: Сrowdin
 Author-email: support@crowdin.com
 License: MIT
 Project-URL: Documentation, https://support.crowdin.com/api/v2/
 Project-URL: Source Code, https://github.com/crowdin/crowdin-api-client-python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<p align='center'><img src='https://support.crowdin.com/assets/logos/crowdin-dark-symbol.png' data-canonical-src='https://support.crowdin.com/assets/logos/crowdin-dark-symbol.png' width='150' height='150' align='center'/></p>](https://crowdin.com)
 
 # Crowdin Python client [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2Fcrowdin%2Fcrowdin-api-client-python&text=The%20Crowdin%20Python%20client%20is%20a%20lightweight%20interface%20to%20the%20Crowdin%20API)&nbsp;[![GitHub Repo stars](https://img.shields.io/github/stars/crowdin/crowdin-api-client-python?style=social&cacheSeconds=1800)](https://github.com/crowdin/crowdin-api-client-python/stargazers)
 
@@ -66,15 +66,16 @@
 class FirstCrowdinClient(CrowdinClient):
     TOKEN = "__token__"
     ORGANIZATION = "organizationName" # Optional, for Crowdin Enterprise only
     TIMEOUT = 60  # Optional, sets http request timeout.
     RETRY_DELAY = 0.1  # Optional, sets the delay between failed requests 
     MAX_RETRIES = 5  # Optional, sets the number of retries
     HEADERS = {"Some-Header": ""}  # Optional, sets additional http request headers
-    PAGE_SIZE = 25  # Optional, sets default page size 
+    PAGE_SIZE = 25  # Optional, sets default page size
+    EXTENDED_REQUEST_PARAMS = {"some-parameters": ""}  # Optional, sets additional parameters for request
 
 client = FirstCrowdinClient()
 
 # Create Project
 project_response = client.projects.add_project(name="New project", sourceLanguageId="en")
 
 # Get list of Projects
```

### Comparing `crowdin-api-client-1.8.0/README.md` & `crowdin-api-client-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 class FirstCrowdinClient(CrowdinClient):
     TOKEN = "__token__"
     ORGANIZATION = "organizationName" # Optional, for Crowdin Enterprise only
     TIMEOUT = 60  # Optional, sets http request timeout.
     RETRY_DELAY = 0.1  # Optional, sets the delay between failed requests 
     MAX_RETRIES = 5  # Optional, sets the number of retries
     HEADERS = {"Some-Header": ""}  # Optional, sets additional http request headers
-    PAGE_SIZE = 25  # Optional, sets default page size 
+    PAGE_SIZE = 25  # Optional, sets default page size
+    EXTENDED_REQUEST_PARAMS = {"some-parameters": ""}  # Optional, sets additional parameters for request
 
 client = FirstCrowdinClient()
 
 # Create Project
 project_response = client.projects.add_project(name="New project", sourceLanguageId="en")
 
 # Get list of Projects
```

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/__init__.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/abstract/resources.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/abstract/resources.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/bundles/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/bundles/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/dictionaries/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/dictionaries/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/distributions/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/distributions/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/glossaries/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/glossaries/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/groups/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/groups/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/labels/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/labels/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/languages/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/languages/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/machine_translation_engines/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/machine_translation_engines/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/projects/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/projects/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/reports/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/reports/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/screenshots/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/screenshots/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/source_files/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/source_files/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     cleanTagsAggressively: bool
     translateHiddenText: bool
     translateHyperlinkUrls: bool
     translateHiddenRowsAndColumns: bool
     importNotes: bool
     importHiddenSlides: bool
     contentSegmentation: bool
-    srxStorageId: bool
+    srxStorageId: int
 
 
 class OtherImportOptions(TypedDict):
     contentSegmentation: bool
     srxStorageId: int
```

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/source_strings/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/source_strings/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/storages/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/storages/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/string_comments/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/string_comments/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/string_translations/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/string_translations/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/tasks/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/tasks/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/teams/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/teams/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_memory/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_memory/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_status/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_status/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/translation_status/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/translation_status/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/translations/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/translations/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/users/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/users/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/users/types.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/users/types.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/vendors/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/vendors/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/enums.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/enums.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/webhooks/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/webhooks/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/api_resources/workflows/resource.py` & `crowdin-api-client-1.9.0/crowdin_api/api_resources/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/client.py` & `crowdin-api-client-1.9.0/crowdin_api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,41 +16,43 @@
     HTTP_PROTOCOL = "https"
     TOKEN = None
     ORGANIZATION = None
     BASE_URL = "api.crowdin.com/api/v2/"
     HEADERS = {}
     USER_AGENT = "crowdin-api-client-python"
     PAGE_SIZE = 25
-    HEADERS = {}
+    EXTENDED_REQUEST_PARAMS = None
 
     def __init__(
         self,
         # TODO: replace this with union type expressions
         # once we do not have to support <3.10 anymore
         organization: Optional[str] = None,
         token: Optional[str] = None,
         base_url: Optional[str] = None,
         user_agent: Optional[str] = None,
         page_size: Optional[int] = None,
         timeout: Optional[int] = None,
         retry_delay: Union[int, float, None] = None,
         max_retries: Optional[int] = None,
         http_protocol: Optional[str] = None,
-        headers: Optional[dict] = None
+        headers: Optional[dict] = None,
+        extended_request_params: Optional[dict] = None
     ):
         self.ORGANIZATION = organization or self.ORGANIZATION
         self.TOKEN = token or self.TOKEN
         self.BASE_URL = base_url or self.BASE_URL
         self.USER_AGENT = user_agent or self.USER_AGENT
         self.PAGE_SIZE = page_size or self.PAGE_SIZE
         self.TIMEOUT = timeout or self.TIMEOUT
         self.RETRY_DELAY = retry_delay or self.RETRY_DELAY
         self.MAX_RETRIES = max_retries or self.MAX_RETRIES
         self.HTTP_PROTOCOL = http_protocol or self.HTTP_PROTOCOL
         self.HEADERS = headers or self.HEADERS
+        self.EXTENDED_REQUEST_PARAMS = extended_request_params or self.EXTENDED_REQUEST_PARAMS
         self._api_requestor = None
 
         if self.ORGANIZATION is None:
             self._platform_type = PlatformType.BASIC
         else:
             self._platform_type = PlatformType.ENTERPRISE
 
@@ -78,14 +80,15 @@
 
     def get_api_requestor(self) -> APIRequester:
         if self._api_requestor is None:
             self._api_requestor = self.API_REQUESTER_CLASS(
                 base_url=self.url,
                 timeout=self.TIMEOUT,
                 default_headers=self.get_default_headers(),
+                extended_params=self.EXTENDED_REQUEST_PARAMS
             )
 
         return self._api_requestor
 
     @property
     def bundles(self) -> api_resources.BundlesResource:
         return api_resources.BundlesResource(
```

### Comparing `crowdin-api-client-1.8.0/crowdin_api/exceptions.py` & `crowdin-api-client-1.9.0/crowdin_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/parser.py` & `crowdin-api-client-1.9.0/crowdin_api/parser.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api/requester.py` & `crowdin-api-client-1.9.0/crowdin_api/requester.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,19 +44,23 @@
     def __init__(
         self,
         base_url: str,
         timeout: int = 80,
         retry_delay: Union[int, float] = 0.1,  # 100 ms
         max_retries: int = 5,
         default_headers: Optional[Dict] = None,
+        extended_params: Optional[Dict] = None,
     ):
         self.base_url = base_url
         self._session = requests.Session()
         self._retry_delay = retry_delay
         self._max_retries = max_retries
+        self._extended_params = {} if extended_params is None else extended_params
+        if not isinstance(self._extended_params, dict):
+            raise TypeError(f"extended_params must be dict, not {type(self._extended_params)}")
 
         headers = copy(self.default_headers)
         headers.update(default_headers or {})
         self.session.headers.update(headers)
         self._timeout = timeout
 
     @property
@@ -109,14 +113,15 @@
             request_data = file
             file_mime_type = mimetypes.MimeTypes().guess_type(file.name)[0]
             headers["Content-Type"] = file_mime_type or self.default_file_content_type
             headers["Crowdin-API-FileName"] = os.path.basename(file.name)
         else:
             request_data = dumps(self._clear_data(request_data))
 
+        kwargs = {**self._extended_params, **kwargs}
         result = self.session.request(
             method,
             urljoin(self.base_url, path),
             params=loads(dumps(self._clear_data(params or {}))),
             headers=headers,
             data=request_data,
             timeout=self._timeout,
```

### Comparing `crowdin-api-client-1.8.0/crowdin_api/status.py` & `crowdin-api-client-1.9.0/crowdin_api/status.py`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/crowdin_api_client.egg-info/PKG-INFO` & `crowdin-api-client-1.9.0/crowdin_api_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crowdin-api-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python client library for Crowdin API v2
 Home-page: https://github.com/crowdin/crowdin-api-client-python
 Author: Сrowdin
 Author-email: support@crowdin.com
 License: MIT
 Project-URL: Documentation, https://support.crowdin.com/api/v2/
 Project-URL: Source Code, https://github.com/crowdin/crowdin-api-client-python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<p align='center'><img src='https://support.crowdin.com/assets/logos/crowdin-dark-symbol.png' data-canonical-src='https://support.crowdin.com/assets/logos/crowdin-dark-symbol.png' width='150' height='150' align='center'/></p>](https://crowdin.com)
 
 # Crowdin Python client [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2Fcrowdin%2Fcrowdin-api-client-python&text=The%20Crowdin%20Python%20client%20is%20a%20lightweight%20interface%20to%20the%20Crowdin%20API)&nbsp;[![GitHub Repo stars](https://img.shields.io/github/stars/crowdin/crowdin-api-client-python?style=social&cacheSeconds=1800)](https://github.com/crowdin/crowdin-api-client-python/stargazers)
 
@@ -66,15 +66,16 @@
 class FirstCrowdinClient(CrowdinClient):
     TOKEN = "__token__"
     ORGANIZATION = "organizationName" # Optional, for Crowdin Enterprise only
     TIMEOUT = 60  # Optional, sets http request timeout.
     RETRY_DELAY = 0.1  # Optional, sets the delay between failed requests 
     MAX_RETRIES = 5  # Optional, sets the number of retries
     HEADERS = {"Some-Header": ""}  # Optional, sets additional http request headers
-    PAGE_SIZE = 25  # Optional, sets default page size 
+    PAGE_SIZE = 25  # Optional, sets default page size
+    EXTENDED_REQUEST_PARAMS = {"some-parameters": ""}  # Optional, sets additional parameters for request
 
 client = FirstCrowdinClient()
 
 # Create Project
 project_response = client.projects.add_project(name="New project", sourceLanguageId="en")
 
 # Get list of Projects
```

### Comparing `crowdin-api-client-1.8.0/crowdin_api_client.egg-info/SOURCES.txt` & `crowdin-api-client-1.9.0/crowdin_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/setup.cfg` & `crowdin-api-client-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `crowdin-api-client-1.8.0/setup.py` & `crowdin-api-client-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     long_description=README,
     long_description_content_type="text/markdown",
     author="Сrowdin",
     author_email="support@crowdin.com",
     url="https://github.com/crowdin/crowdin-api-client-python",
     packages=find_packages(exclude=["*tests*", "*fixtures.py"]),
     package_dir={"crowdin_api": "crowdin_api"},
-    python_requires=">=3.6.*",
+    python_requires=">=3.6",
     license="MIT",
     install_requires=[
         "requests>=2.25.1",
         "typing-extensions; python_version < '3.8.0'",
     ],
     classifiers=[
         "Programming Language :: Python",
```

