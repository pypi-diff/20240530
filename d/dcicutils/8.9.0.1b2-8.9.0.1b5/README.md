# Comparing `tmp/dcicutils-8.9.0.1b2.tar.gz` & `tmp/dcicutils-8.9.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.9.0.1b2.tar", max compression
+gzip compressed data, was "dcicutils-8.9.0.1b5.tar", max compression
```

## Comparing `dcicutils-8.9.0.1b2.tar` & `dcicutils-8.9.0.1b5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1102 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/README.rst
--rw-r--r--   0        0        0        0 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3295 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    18487 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11127 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7626 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/data_utils.py
--rw-r--r--   0        0        0    13499 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    73123 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10916 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0     1583 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/http_utils.py
--rw-r--r--   0        0        0    11502 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-05-30 11:56:06.301033 dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/log_utils.py
--rw-r--r--   0        0        0   107690 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    11062 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    45217 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    19468 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10604 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    29777 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    64030 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     4741 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/task_utils.py
--rw-r--r--   0        0        0     2997 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     3265 2024-05-30 11:56:06.305034 dcicutils-8.9.0.1b2/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4756 2024-05-30 11:56:06.309034 dcicutils-8.9.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 dcicutils-8.9.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/README.rst
+-rw-r--r--   0        0        0        0 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3295 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    18487 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11127 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7626 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    13499 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-05-30 20:10:04.257772 dcicutils-8.9.0.1b5/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    73123 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10916 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0     1583 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/http_utils.py
+-rw-r--r--   0        0        0    11502 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   109423 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    11062 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    45217 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    19468 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10604 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    29777 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-05-30 20:10:04.261772 dcicutils-8.9.0.1b5/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    64160 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     4741 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     2997 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     3265 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4756 2024-05-30 20:10:04.265772 dcicutils-8.9.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 dcicutils-8.9.0.1b5/PKG-INFO
```

### Comparing `dcicutils-8.9.0.1b2/LICENSE.txt` & `dcicutils-8.9.0.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/README.rst` & `dcicutils-8.9.0.1b5/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/base.py` & `dcicutils-8.9.0.1b5/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/beanstalk_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/bundle_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/captured_output.py` & `dcicutils-8.9.0.1b5/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/cloudformation_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/codebuild_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/command_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/common.py` & `dcicutils-8.9.0.1b5/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/contribution_scripts.py` & `dcicutils-8.9.0.1b5/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/contribution_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/creds_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/data_readers.py` & `dcicutils-8.9.0.1b5/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/data_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/datetime_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/deployment_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/diff_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/docker_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/ecr_scripts.py` & `dcicutils-8.9.0.1b5/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/ecr_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/ecs_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/env_base.py` & `dcicutils-8.9.0.1b5/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/env_manager.py` & `dcicutils-8.9.0.1b5/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/env_scripts.py` & `dcicutils-8.9.0.1b5/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/env_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/env_utils_legacy.py` & `dcicutils-8.9.0.1b5/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/es_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/exceptions.py` & `dcicutils-8.9.0.1b5/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/ff_mocks.py` & `dcicutils-8.9.0.1b5/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/ff_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/file_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/function_cache_decorator.py` & `dcicutils-8.9.0.1b5/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/glacier_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/http_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/http_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/jh_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/kibana/dashboards.json` & `dcicutils-8.9.0.1b5/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/kibana/readme.md` & `dcicutils-8.9.0.1b5/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/lang_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.9.0.1b5/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/license_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/log_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/misc_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This file contains functions that might be generally useful.
 """
 
 from collections import namedtuple
 import appdirs
+from copy import deepcopy
 import contextlib
 import datetime
 import functools
 import hashlib
 import inspect
 import io
 import json
@@ -2195,36 +2196,66 @@
     for pair in x:
         merged[pair['Key']] = pair['Value']
     for pair in y:
         merged[pair['Key']] = pair['Value']
     return [key_value_dict(k, v) for k, v in merged.items()]
 
 
-def merge_objects(target: Union[dict, List[Any]], source: Union[dict, List[Any]], full: bool = False) -> dict:
-    """
-    Merges the given source dictionary or list into the target dictionary or list.
-    This MAY well change the given target (dictionary or list) IN PLACE.
-    The the full argument is True then any target lists longer than the
-    source be will be filled out with the last element(s) of the source.
+def merge_objects(target: Union[dict, List[Any]], source: Union[dict, List[Any]],
+                  full: bool = False,  # deprecated
+                  expand_lists: Optional[bool] = None,
+                  primitive_lists: bool = False,
+                  copy: bool = False, _recursing: bool = False) -> Union[dict, List[Any]]:
+    """
+    Merges the given source dictionary or list into the target dictionary or list and returns the
+    result. This MAY well change the given target (dictionary or list) IN PLACE ... UNLESS the copy
+    argument is True, then the given target will not change as a local copy is made (and returned).
+
+    If the expand_lists argument is True then any target lists longer than the
+    source be will be filled out with the last element(s) of the source; the full
+    argument (is deprecated and) is a synomym for this. The default is False.
+
+    If the primitive_lists argument is True then lists of primitives (i.e. lists in which
+    NONE of its elements are dictionaries, lists, or tuples) will themselves be treated
+    like primitives, meaning the whole of a source list will replace the corresponding
+    target; otherwise they  will be merged normally, meaning each element of a source list
+    will be merged, recursively, into the corresponding target list. The default is False.
     """
+    def is_primitive_list(value: Any) -> bool:  # noqa
+        if not isinstance(value, list):
+            return False
+        for item in value:
+            if isinstance(item, (dict, list, tuple)):
+                return False
+        return True
+
     if target is None:
         return source
+    if expand_lists not in (True, False):
+        expand_lists = full is True
+    if (copy is True) and (_recursing is not True):
+        target = deepcopy(target)
     if isinstance(target, dict) and isinstance(source, dict) and source:
         for key, value in source.items():
-            target[key] = merge_objects(target[key], value, full) if key in target else value
+            if ((primitive_lists is True) and
+                (key in target) and is_primitive_list(target[key]) and is_primitive_list(value)):  # noqa
+                target[key] = value
+            else:
+                target[key] = merge_objects(target[key], value,
+                                            expand_lists=expand_lists, _recursing=True) if key in target else value
     elif isinstance(target, list) and isinstance(source, list) and source:
         for i in range(max(len(source), len(target))):
             if i < len(target):
                 if i < len(source):
-                    target[i] = merge_objects(target[i], source[i], full)
-                elif full:
-                    target[i] = merge_objects(target[i], source[len(source) - 1], full)
+                    target[i] = merge_objects(target[i], source[i], expand_lists=expand_lists, _recursing=True)
+                elif expand_lists is True:
+                    target[i] = merge_objects(target[i], source[len(source) - 1], expand_lists=expand_lists)
             else:
                 target.append(source[i])
-    elif source:
+    elif source not in (None, {}, []):
         target = source
     return target
 
 
 def load_json_from_file_expanding_environment_variables(file: str) -> Union[dict, list]:
     def expand_envronment_variables(data):  # noqa
         if isinstance(data, dict):
```

### Comparing `dcicutils-8.9.0.1b2/dcicutils/obfuscation_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/opensearch_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/portal_object_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/portal_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/progress_bar.py` & `dcicutils-8.9.0.1b5/dcicutils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/project_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/qa_checkers.py` & `dcicutils-8.9.0.1b5/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/qa_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/redis_tools.py` & `dcicutils-8.9.0.1b5/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/redis_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/s3_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/schema_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.9.0.1b5/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.9.0.1b5/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.9.0.1b5/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/secrets_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/sheet_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/snapshot_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/structured_data.py` & `dcicutils-8.9.0.1b5/dcicutils/structured_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self._warnings = {}
         self._errors = {}
         self._resolved_refs = set()
         self._validated = False
         self._nrows = 0
         self._autoadd_properties = autoadd if isinstance(autoadd, dict) and autoadd else None
         self._norefs = True if norefs is True else False
-        self._merge = True if merge is True else False
+        self._merge = True if merge is True else False  # New merge functionality (2024-05-25)
         self._debug_sleep = None
         if debug_sleep:
             try:
                 self._debug_sleep = float(debug_sleep)
             except Exception:
                 self._debug_sleep = None
         self.load_file(file) if file else None
@@ -343,24 +343,24 @@
     def _load_json_file(self, file: str) -> None:
         with open(file) as f:
             data = json.load(f)
             if ((schema_name_inferred_from_file_name := Schema.type_name(file)) and
                 (self._portal.get_schema(schema_name_inferred_from_file_name) is not None)):  # noqa
                 # If the JSON file name looks like a schema name then assume it
                 # contains an object or an array of object of that schema type.
-                if self._merge:
+                if self._merge:  # New merge functionality (2024-05-25)
                     data = self._merge_with_existing_portal_object(data, schema_name_inferred_from_file_name)
                 self._add(Schema.type_name(file), data)
             elif isinstance(data, dict):
                 # Otherwise if the JSON file name does not look like a schema name then
                 # assume it a dictionary where each property is the name of a schema, and
                 # which (each property) contains a list of object of that schema type.
                 for schema_name in data:
                     item = data[schema_name]
-                    if self._merge:
+                    if self._merge:  # New merge functionality (2024-05-25)
                         item = self._merge_with_existing_portal_object(item, schema_name)
                     self._add(schema_name, item)
 
     def _load_reader(self, reader: RowReader, type_name: str) -> None:
         schema = None
         noschema = False
         structured_row_template = None
@@ -376,16 +376,15 @@
                     type_name = schema_name
                 structured_row_template = _StructuredRowTemplate(reader.header, schema)
             structured_row = structured_row_template.create_row()
             for column_name, value in row.items():
                 structured_row_template.set_value(structured_row, column_name, value, reader.file, reader.row_number)
                 if self._autoadd_properties:
                     self._add_properties(structured_row, self._autoadd_properties, schema)
-            # New merge functionality (2024-05-25).
-            if self._merge:
+            if self._merge:  # New merge functionality (2024-05-25)
                 structured_row = self._merge_with_existing_portal_object(structured_row, schema_name)
             if (prune_error := self._prune_structured_row(structured_row)) is not None:
                 self._note_error({"src": create_dict(type=schema_name, row=reader.row_number),
                                   "error": prune_error}, "validation")
             else:
                 self._add(type_name, structured_row)  # TODO: why type_name and not schema_name?
             if self._progress:
@@ -433,15 +432,15 @@
         Given a Portal object (presumably/in-practice from the given metadata), if there is
         an existing Portal item, identified by the identifying properties for the given object,
         then merges the given object into the existing one and returns the result; otherwise
         just returns the given object. Note that the given object may be CHANGED in place.
         """
         for identifying_path in self._portal.get_identifying_paths(portal_object, portal_type):
             if existing_portal_object := self._portal.get_metadata(identifying_path, raw=True, raise_exception=False):
-                return merge_objects(existing_portal_object, portal_object)
+                return merge_objects(existing_portal_object, portal_object, primitive_lists=True)
         return portal_object
 
     def _is_ref_lookup_specified_type(ref_lookup_flags: int) -> bool:
         return (ref_lookup_flags &
                 Portal.LOOKUP_SPECIFIED_TYPE) == Portal.LOOKUP_SPECIFIED_TYPE
 
     def _is_ref_lookup_root(ref_lookup_flags: int) -> bool:
```

### Comparing `dcicutils-8.9.0.1b2/dcicutils/submitr/progress_constants.py` & `dcicutils-8.9.0.1b5/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.9.0.1b5/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/task_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/tmpfile_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/trace_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/validation_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/variant_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/dcicutils/zip_utils.py` & `dcicutils-8.9.0.1b5/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.9.0.1b2/pyproject.toml` & `dcicutils-8.9.0.1b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.9.0.1b2"  # TODO: To become 8.10.0
+version = "8.9.0.1b5"  # TODO: To become 8.10.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.9.0.1b2/PKG-INFO` & `dcicutils-8.9.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.9.0.1b2
+Version: 8.9.0.1b5
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
```

