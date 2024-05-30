# Comparing `tmp/qase_api_client-1.0.0b1.tar.gz` & `tmp/qase_api_client-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_api_client-1.0.0b1.tar", last modified: Mon May  6 08:04:43 2024, max compression
+gzip compressed data, was "qase_api_client-1.0.0b2.tar", last modified: Mon May  6 12:24:42 2024, max compression
```

## Comparing `qase_api_client-1.0.0b1.tar` & `qase_api_client-1.0.0b2.tar`

### file list

```diff
@@ -1,343 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.632710 qase_api_client-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-05-06 08:04:43.632710 qase_api_client-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:04:43.636711 qase_api_client-1.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.576711 qase_api_client-1.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.576711 qase_api_client-1.0.0b1/src/qase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.580711 qase_api_client-1.0.0b1/src/qase/api_client_v1/
--rw-r--r--   0 runner    (1001) docker     (127)    13366 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.584710 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45480 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/authors_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   108186 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/cases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36034 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    56337 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    83017 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/defects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    59778 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/environments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60490 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/milestones_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    58885 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/plans_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    67980 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    81141 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/results_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77184 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60697 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/shared_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    61325 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/suites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api/system_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25803 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.608710 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachmentupload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/bulk200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/bulk200_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_group_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_create_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_fields_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/external_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/external_issue_issues_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/hash_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/hash_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/id_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/id_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_code_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_counts_defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_counts_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/qql_defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/qql_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/qql_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/resultcreate_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_public_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_public_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/search_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/search_response_all_of_result_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_content_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/system_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/system_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/system_field_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/tag_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_external_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_casebulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_casebulk_cases_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_caseexternal_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step_result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/src/qase/api_client_v1/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.632710 qase_api_client-1.0.0b1/src/qase_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-05-06 08:04:43.000000 qase_api_client-1.0.0b1/src/qase_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-06 08:04:43.000000 qase_api_client-1.0.0b1/src/qase_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:04:43.000000 qase_api_client-1.0.0b1/src/qase_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 08:04:43.000000 qase_api_client-1.0.0b1/src/qase_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:04:43.000000 qase_api_client-1.0.0b1/src/qase_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:04:43.632710 qase_api_client-1.0.0b1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachment_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_attachmentupload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_author.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_author_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_author_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_author_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_authors_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_bulk200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_bulk200_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_cases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configuration_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configuration_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configuration_group_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configuration_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configuration_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field_create_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_fields_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_custom_fields_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defect_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_defects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_environments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_external_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_external_issue_issues_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_hash_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_hash_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_id_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_id_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestone_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestone_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestone_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_milestones_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_detailed_all_of_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_code_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_counts_defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_counts_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_qql_defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_qql_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_qql_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_create_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_create_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_create_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_result_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_resultcreate_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_results_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_public_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_public_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_run_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_search_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_search_response_all_of_result_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_content_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_step_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_shared_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suite_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_suites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_system_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_system_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_system_field_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_system_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_tag_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_external_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_external_issues_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_case_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_casebulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_casebulk_cases_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_caseexternal_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-06 08:04:34.000000 qase_api_client-1.0.0b1/test/test_test_step_result_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.408233 qase_api_client-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-05-06 12:24:42.408233 qase_api_client-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:24:42.408233 qase_api_client-1.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.348232 qase_api_client-1.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.348232 qase_api_client-1.0.0b2/src/qase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.348232 qase_api_client-1.0.0b2/src/qase/api_client_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.352232 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45359 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24100 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/authors_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108138 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/cases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56301 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82977 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/defects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59746 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60458 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/milestones_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58853 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67944 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/results_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77144 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60665 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/shared_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61289 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/system_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.376232 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachmentupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue_issues_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/resultcreate_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk_cases_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_caseexternal_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.404233 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.404233 qase_api_client-1.0.0b2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachmentupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_authors_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_bulk200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_bulk200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_cases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_create_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_fields_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_fields_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_external_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_external_issue_issues_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_hash_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_hash_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_id_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestones_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_detailed_all_of_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_code_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_counts_defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_counts_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_qql_defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_qql_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_qql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_resultcreate_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_results_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_public_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_public_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_response_all_of_result_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_content_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_field_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_external_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_external_issues_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_casebulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_casebulk_cases_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_caseexternal_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step_result_create.py
```

### Comparing `qase_api_client-1.0.0b1/PKG-INFO` & `qase_api_client-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-api-client
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Qase TestOps API V1 client for Python
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python
 Keywords: OpenAPI,OpenAPI-Generator,Qase.io TestOps API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -42,48 +42,48 @@
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
-import qase.apiv1
+import qase.api_client_v1
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import qase.apiv1
+import qase.api_client_v1
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import qase.apiv1
-from qase.apiv1.rest import ApiException
+import qase.api_client_v1
+from qase.api_client_v1.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.qase.io/v1
 # See configuration.py for a list of all supported configuration parameters.
-configuration = src.qase.apiv1.Configuration(
+configuration = qase.api_client_v1.Configuration(
     host = "https://api.qase.io/v1"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
@@ -92,17 +92,17 @@
 configuration.api_key['TokenAuth'] = os.environ["API_KEY"]
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['TokenAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with qase.apiv1.ApiClient(configuration) as api_client:
+with qase.api_client_v1.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = qase.apiv1.AttachmentsApi(api_client)
+    api_instance = qase.api_client_v1.AttachmentsApi(api_client)
     hash = 'hash_example' # str | Hash.
 
     try:
         # Remove attachment by Hash
         api_response = api_instance.delete_attachment(hash)
         print("The response of AttachmentsApi->delete_attachment:\n")
         pprint(api_response)
```

### Comparing `qase_api_client-1.0.0b1/README.md` & `qase_api_client-1.0.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,48 +21,48 @@
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
-import qase.apiv1
+import qase.api_client_v1
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import qase.apiv1
+import qase.api_client_v1
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import qase.apiv1
-from qase.apiv1.rest import ApiException
+import qase.api_client_v1
+from qase.api_client_v1.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.qase.io/v1
 # See configuration.py for a list of all supported configuration parameters.
-configuration = src.qase.apiv1.Configuration(
+configuration = qase.api_client_v1.Configuration(
     host = "https://api.qase.io/v1"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
@@ -71,17 +71,17 @@
 configuration.api_key['TokenAuth'] = os.environ["API_KEY"]
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['TokenAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with qase.apiv1.ApiClient(configuration) as api_client:
+with qase.api_client_v1.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = qase.apiv1.AttachmentsApi(api_client)
+    api_instance = qase.api_client_v1.AttachmentsApi(api_client)
     hash = 'hash_example' # str | Hash.
 
     try:
         # Remove attachment by Hash
         api_response = api_instance.delete_attachment(hash)
         print("The response of AttachmentsApi->delete_attachment:\n")
         pprint(api_response)
```

### Comparing `qase_api_client-1.0.0b1/pyproject.toml` & `qase_api_client-1.0.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-api-client"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "Qase TestOps API V1 client for Python"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/__init__.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,178 +14,178 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
 
 # import apis into sdk package
-from src.qase.api_client_v1.api.attachments_api import AttachmentsApi
-from src.qase.api_client_v1.api.authors_api import AuthorsApi
-from src.qase.api_client_v1.api.cases_api import CasesApi
-from src.qase.api_client_v1.api.configurations_api import ConfigurationsApi
-from src.qase.api_client_v1.api.custom_fields_api import CustomFieldsApi
-from src.qase.api_client_v1.api.defects_api import DefectsApi
-from src.qase.api_client_v1.api.environments_api import EnvironmentsApi
-from src.qase.api_client_v1.api.milestones_api import MilestonesApi
-from src.qase.api_client_v1.api.plans_api import PlansApi
-from src.qase.api_client_v1.api.projects_api import ProjectsApi
-from src.qase.api_client_v1.api.results_api import ResultsApi
-from src.qase.api_client_v1.api.runs_api import RunsApi
-from src.qase.api_client_v1.api.search_api import SearchApi
-from src.qase.api_client_v1.api.shared_steps_api import SharedStepsApi
-from src.qase.api_client_v1.api.suites_api import SuitesApi
-from src.qase.api_client_v1.api.system_fields_api import SystemFieldsApi
+from qase.api_client_v1.api.attachments_api import AttachmentsApi
+from qase.api_client_v1.api.authors_api import AuthorsApi
+from qase.api_client_v1.api.cases_api import CasesApi
+from qase.api_client_v1.api.configurations_api import ConfigurationsApi
+from qase.api_client_v1.api.custom_fields_api import CustomFieldsApi
+from qase.api_client_v1.api.defects_api import DefectsApi
+from qase.api_client_v1.api.environments_api import EnvironmentsApi
+from qase.api_client_v1.api.milestones_api import MilestonesApi
+from qase.api_client_v1.api.plans_api import PlansApi
+from qase.api_client_v1.api.projects_api import ProjectsApi
+from qase.api_client_v1.api.results_api import ResultsApi
+from qase.api_client_v1.api.runs_api import RunsApi
+from qase.api_client_v1.api.search_api import SearchApi
+from qase.api_client_v1.api.shared_steps_api import SharedStepsApi
+from qase.api_client_v1.api.suites_api import SuitesApi
+from qase.api_client_v1.api.system_fields_api import SystemFieldsApi
 
 # import ApiClient
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.api_client import ApiClient
-from src.qase.api_client_v1.configuration import Configuration
-from src.qase.api_client_v1.exceptions import OpenApiException
-from src.qase.api_client_v1.exceptions import ApiTypeError
-from src.qase.api_client_v1.exceptions import ApiValueError
-from src.qase.api_client_v1.exceptions import ApiKeyError
-from src.qase.api_client_v1.exceptions import ApiAttributeError
-from src.qase.api_client_v1.exceptions import ApiException
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.api_client import ApiClient
+from qase.api_client_v1.configuration import Configuration
+from qase.api_client_v1.exceptions import OpenApiException
+from qase.api_client_v1.exceptions import ApiTypeError
+from qase.api_client_v1.exceptions import ApiValueError
+from qase.api_client_v1.exceptions import ApiKeyError
+from qase.api_client_v1.exceptions import ApiAttributeError
+from qase.api_client_v1.exceptions import ApiException
 
 # import models into sdk package
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.attachment_get import AttachmentGet
-from src.qase.api_client_v1.models.attachment_hash import AttachmentHash
-from src.qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
-from src.qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
-from src.qase.api_client_v1.models.attachment_response import AttachmentResponse
-from src.qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
-from src.qase.api_client_v1.models.attachmentupload import Attachmentupload
-from src.qase.api_client_v1.models.author import Author
-from src.qase.api_client_v1.models.author_list_response import AuthorListResponse
-from src.qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
-from src.qase.api_client_v1.models.author_response import AuthorResponse
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.bulk200_response import Bulk200Response
-from src.qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
-from src.qase.api_client_v1.models.configuration import Configuration
-from src.qase.api_client_v1.models.configuration_create import ConfigurationCreate
-from src.qase.api_client_v1.models.configuration_group import ConfigurationGroup
-from src.qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
-from src.qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
-from src.qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
-from src.qase.api_client_v1.models.custom_field import CustomField
-from src.qase.api_client_v1.models.custom_field_create import CustomFieldCreate
-from src.qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
-from src.qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
-from src.qase.api_client_v1.models.custom_field_response import CustomFieldResponse
-from src.qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.custom_fields_response import CustomFieldsResponse
-from src.qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
-from src.qase.api_client_v1.models.defect import Defect
-from src.qase.api_client_v1.models.defect_create import DefectCreate
-from src.qase.api_client_v1.models.defect_list_response import DefectListResponse
-from src.qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
-from src.qase.api_client_v1.models.defect_query import DefectQuery
-from src.qase.api_client_v1.models.defect_response import DefectResponse
-from src.qase.api_client_v1.models.defect_status import DefectStatus
-from src.qase.api_client_v1.models.defect_update import DefectUpdate
-from src.qase.api_client_v1.models.environment import Environment
-from src.qase.api_client_v1.models.environment_create import EnvironmentCreate
-from src.qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
-from src.qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
-from src.qase.api_client_v1.models.environment_response import EnvironmentResponse
-from src.qase.api_client_v1.models.environment_update import EnvironmentUpdate
-from src.qase.api_client_v1.models.external_issue import ExternalIssue
-from src.qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
-from src.qase.api_client_v1.models.hash_response import HashResponse
-from src.qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
-from src.qase.api_client_v1.models.milestone import Milestone
-from src.qase.api_client_v1.models.milestone_create import MilestoneCreate
-from src.qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
-from src.qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
-from src.qase.api_client_v1.models.milestone_response import MilestoneResponse
-from src.qase.api_client_v1.models.milestone_update import MilestoneUpdate
-from src.qase.api_client_v1.models.plan import Plan
-from src.qase.api_client_v1.models.plan_create import PlanCreate
-from src.qase.api_client_v1.models.plan_detailed import PlanDetailed
-from src.qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
-from src.qase.api_client_v1.models.plan_list_response import PlanListResponse
-from src.qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
-from src.qase.api_client_v1.models.plan_query import PlanQuery
-from src.qase.api_client_v1.models.plan_response import PlanResponse
-from src.qase.api_client_v1.models.plan_update import PlanUpdate
-from src.qase.api_client_v1.models.project import Project
-from src.qase.api_client_v1.models.project_access import ProjectAccess
-from src.qase.api_client_v1.models.project_code_response import ProjectCodeResponse
-from src.qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
-from src.qase.api_client_v1.models.project_counts import ProjectCounts
-from src.qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
-from src.qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
-from src.qase.api_client_v1.models.project_create import ProjectCreate
-from src.qase.api_client_v1.models.project_list_response import ProjectListResponse
-from src.qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
-from src.qase.api_client_v1.models.project_response import ProjectResponse
-from src.qase.api_client_v1.models.qql_defect import QqlDefect
-from src.qase.api_client_v1.models.qql_plan import QqlPlan
-from src.qase.api_client_v1.models.qql_test_case import QqlTestCase
-from src.qase.api_client_v1.models.requirement import Requirement
-from src.qase.api_client_v1.models.response import Response
-from src.qase.api_client_v1.models.result import Result
-from src.qase.api_client_v1.models.result_create import ResultCreate
-from src.qase.api_client_v1.models.result_create_bulk import ResultCreateBulk
-from src.qase.api_client_v1.models.result_create_case import ResultCreateCase
-from src.qase.api_client_v1.models.result_create_response import ResultCreateResponse
-from src.qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
-from src.qase.api_client_v1.models.result_list_response import ResultListResponse
-from src.qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
-from src.qase.api_client_v1.models.result_response import ResultResponse
-from src.qase.api_client_v1.models.result_update import ResultUpdate
-from src.qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
-from src.qase.api_client_v1.models.run import Run
-from src.qase.api_client_v1.models.run_create import RunCreate
-from src.qase.api_client_v1.models.run_environment import RunEnvironment
-from src.qase.api_client_v1.models.run_list_response import RunListResponse
-from src.qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
-from src.qase.api_client_v1.models.run_milestone import RunMilestone
-from src.qase.api_client_v1.models.run_public import RunPublic
-from src.qase.api_client_v1.models.run_public_response import RunPublicResponse
-from src.qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
-from src.qase.api_client_v1.models.run_response import RunResponse
-from src.qase.api_client_v1.models.run_stats import RunStats
-from src.qase.api_client_v1.models.search_response import SearchResponse
-from src.qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
-from src.qase.api_client_v1.models.search_response_all_of_result_entities import SearchResponseAllOfResultEntities
-from src.qase.api_client_v1.models.shared_step import SharedStep
-from src.qase.api_client_v1.models.shared_step_content import SharedStepContent
-from src.qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
-from src.qase.api_client_v1.models.shared_step_create import SharedStepCreate
-from src.qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
-from src.qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
-from src.qase.api_client_v1.models.shared_step_response import SharedStepResponse
-from src.qase.api_client_v1.models.shared_step_update import SharedStepUpdate
-from src.qase.api_client_v1.models.suite import Suite
-from src.qase.api_client_v1.models.suite_create import SuiteCreate
-from src.qase.api_client_v1.models.suite_delete import SuiteDelete
-from src.qase.api_client_v1.models.suite_list_response import SuiteListResponse
-from src.qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
-from src.qase.api_client_v1.models.suite_response import SuiteResponse
-from src.qase.api_client_v1.models.suite_update import SuiteUpdate
-from src.qase.api_client_v1.models.system_field import SystemField
-from src.qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
-from src.qase.api_client_v1.models.system_field_option import SystemFieldOption
-from src.qase.api_client_v1.models.tag_value import TagValue
-from src.qase.api_client_v1.models.test_case import TestCase
-from src.qase.api_client_v1.models.test_case_create import TestCaseCreate
-from src.qase.api_client_v1.models.test_case_external_issues import TestCaseExternalIssues
-from src.qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
-from src.qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
-from src.qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
-from src.qase.api_client_v1.models.test_case_params import TestCaseParams
-from src.qase.api_client_v1.models.test_case_query import TestCaseQuery
-from src.qase.api_client_v1.models.test_case_response import TestCaseResponse
-from src.qase.api_client_v1.models.test_case_update import TestCaseUpdate
-from src.qase.api_client_v1.models.test_casebulk import TestCasebulk
-from src.qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
-from src.qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
-from src.qase.api_client_v1.models.test_step import TestStep
-from src.qase.api_client_v1.models.test_step_create import TestStepCreate
-from src.qase.api_client_v1.models.test_step_result import TestStepResult
-from src.qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.attachment_get import AttachmentGet
+from qase.api_client_v1.models.attachment_hash import AttachmentHash
+from qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
+from qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
+from qase.api_client_v1.models.attachment_response import AttachmentResponse
+from qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
+from qase.api_client_v1.models.attachmentupload import Attachmentupload
+from qase.api_client_v1.models.author import Author
+from qase.api_client_v1.models.author_list_response import AuthorListResponse
+from qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
+from qase.api_client_v1.models.author_response import AuthorResponse
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.bulk200_response import Bulk200Response
+from qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
+from qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration_create import ConfigurationCreate
+from qase.api_client_v1.models.configuration_group import ConfigurationGroup
+from qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
+from qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
+from qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
+from qase.api_client_v1.models.custom_field import CustomField
+from qase.api_client_v1.models.custom_field_create import CustomFieldCreate
+from qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
+from qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
+from qase.api_client_v1.models.custom_field_response import CustomFieldResponse
+from qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.custom_fields_response import CustomFieldsResponse
+from qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
+from qase.api_client_v1.models.defect import Defect
+from qase.api_client_v1.models.defect_create import DefectCreate
+from qase.api_client_v1.models.defect_list_response import DefectListResponse
+from qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
+from qase.api_client_v1.models.defect_query import DefectQuery
+from qase.api_client_v1.models.defect_response import DefectResponse
+from qase.api_client_v1.models.defect_status import DefectStatus
+from qase.api_client_v1.models.defect_update import DefectUpdate
+from qase.api_client_v1.models.environment import Environment
+from qase.api_client_v1.models.environment_create import EnvironmentCreate
+from qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
+from qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
+from qase.api_client_v1.models.environment_response import EnvironmentResponse
+from qase.api_client_v1.models.environment_update import EnvironmentUpdate
+from qase.api_client_v1.models.external_issue import ExternalIssue
+from qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
+from qase.api_client_v1.models.hash_response import HashResponse
+from qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
+from qase.api_client_v1.models.milestone import Milestone
+from qase.api_client_v1.models.milestone_create import MilestoneCreate
+from qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
+from qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
+from qase.api_client_v1.models.milestone_response import MilestoneResponse
+from qase.api_client_v1.models.milestone_update import MilestoneUpdate
+from qase.api_client_v1.models.plan import Plan
+from qase.api_client_v1.models.plan_create import PlanCreate
+from qase.api_client_v1.models.plan_detailed import PlanDetailed
+from qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
+from qase.api_client_v1.models.plan_list_response import PlanListResponse
+from qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
+from qase.api_client_v1.models.plan_query import PlanQuery
+from qase.api_client_v1.models.plan_response import PlanResponse
+from qase.api_client_v1.models.plan_update import PlanUpdate
+from qase.api_client_v1.models.project import Project
+from qase.api_client_v1.models.project_access import ProjectAccess
+from qase.api_client_v1.models.project_code_response import ProjectCodeResponse
+from qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
+from qase.api_client_v1.models.project_counts import ProjectCounts
+from qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
+from qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
+from qase.api_client_v1.models.project_create import ProjectCreate
+from qase.api_client_v1.models.project_list_response import ProjectListResponse
+from qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
+from qase.api_client_v1.models.project_response import ProjectResponse
+from qase.api_client_v1.models.qql_defect import QqlDefect
+from qase.api_client_v1.models.qql_plan import QqlPlan
+from qase.api_client_v1.models.qql_test_case import QqlTestCase
+from qase.api_client_v1.models.requirement import Requirement
+from qase.api_client_v1.models.response import Response
+from qase.api_client_v1.models.result import Result
+from qase.api_client_v1.models.result_create import ResultCreate
+from qase.api_client_v1.models.result_create_bulk import ResultCreateBulk
+from qase.api_client_v1.models.result_create_case import ResultCreateCase
+from qase.api_client_v1.models.result_create_response import ResultCreateResponse
+from qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
+from qase.api_client_v1.models.result_list_response import ResultListResponse
+from qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
+from qase.api_client_v1.models.result_response import ResultResponse
+from qase.api_client_v1.models.result_update import ResultUpdate
+from qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
+from qase.api_client_v1.models.run import Run
+from qase.api_client_v1.models.run_create import RunCreate
+from qase.api_client_v1.models.run_environment import RunEnvironment
+from qase.api_client_v1.models.run_list_response import RunListResponse
+from qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
+from qase.api_client_v1.models.run_milestone import RunMilestone
+from qase.api_client_v1.models.run_public import RunPublic
+from qase.api_client_v1.models.run_public_response import RunPublicResponse
+from qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
+from qase.api_client_v1.models.run_response import RunResponse
+from qase.api_client_v1.models.run_stats import RunStats
+from qase.api_client_v1.models.search_response import SearchResponse
+from qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
+from qase.api_client_v1.models.search_response_all_of_result_entities import SearchResponseAllOfResultEntities
+from qase.api_client_v1.models.shared_step import SharedStep
+from qase.api_client_v1.models.shared_step_content import SharedStepContent
+from qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
+from qase.api_client_v1.models.shared_step_create import SharedStepCreate
+from qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
+from qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
+from qase.api_client_v1.models.shared_step_response import SharedStepResponse
+from qase.api_client_v1.models.shared_step_update import SharedStepUpdate
+from qase.api_client_v1.models.suite import Suite
+from qase.api_client_v1.models.suite_create import SuiteCreate
+from qase.api_client_v1.models.suite_delete import SuiteDelete
+from qase.api_client_v1.models.suite_list_response import SuiteListResponse
+from qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
+from qase.api_client_v1.models.suite_response import SuiteResponse
+from qase.api_client_v1.models.suite_update import SuiteUpdate
+from qase.api_client_v1.models.system_field import SystemField
+from qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
+from qase.api_client_v1.models.system_field_option import SystemFieldOption
+from qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.test_case import TestCase
+from qase.api_client_v1.models.test_case_create import TestCaseCreate
+from qase.api_client_v1.models.test_case_external_issues import TestCaseExternalIssues
+from qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
+from qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
+from qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
+from qase.api_client_v1.models.test_case_params import TestCaseParams
+from qase.api_client_v1.models.test_case_query import TestCaseQuery
+from qase.api_client_v1.models.test_case_response import TestCaseResponse
+from qase.api_client_v1.models.test_case_update import TestCaseUpdate
+from qase.api_client_v1.models.test_casebulk import TestCasebulk
+from qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
+from qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
+from qase.api_client_v1.models.test_step import TestStep
+from qase.api_client_v1.models.test_step_create import TestStepCreate
+from qase.api_client_v1.models.test_step_result import TestStepResult
+from qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/attachments_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/attachments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBytes, StrictStr
 from typing import List, Optional, Union
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
-from src.qase.api_client_v1.models.attachment_response import AttachmentResponse
-from src.qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
-from src.qase.api_client_v1.models.hash_response import HashResponse
-
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
+from qase.api_client_v1.models.attachment_response import AttachmentResponse
+from qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
+from qase.api_client_v1.models.hash_response import HashResponse
+
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class AttachmentsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -884,15 +884,15 @@
 
 
 
     @validate_call
     def upload_attachment(
         self,
         code: Annotated[str, Field(min_length=2, strict=True, max_length=10, description="Code of project, where to search entities.")],
-        file: Optional[List[Union[StrictBytes, StrictStr]]] = None,
+        file: Optional[List] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -961,15 +961,15 @@
         ).data
 
 
     @validate_call
     def upload_attachment_with_http_info(
         self,
         code: Annotated[str, Field(min_length=2, strict=True, max_length=10, description="Code of project, where to search entities.")],
-        file: Optional[List[Union[StrictBytes, StrictStr]]] = None,
+        file: Optional[List] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1038,15 +1038,15 @@
         )
 
 
     @validate_call
     def upload_attachment_without_preload_content(
         self,
         code: Annotated[str, Field(min_length=2, strict=True, max_length=10, description="Code of project, where to search entities.")],
-        file: Optional[List[Union[StrictBytes, StrictStr]]] = None,
+        file: Optional[List] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/authors_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/authors_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.author_list_response import AuthorListResponse
-from src.qase.api_client_v1.models.author_response import AuthorResponse
+from qase.api_client_v1.models.author_list_response import AuthorListResponse
+from qase.api_client_v1.models.author_response import AuthorResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class AuthorsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/cases_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/cases_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
 from typing import List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.bulk200_response import Bulk200Response
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.test_case_create import TestCaseCreate
-from src.qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
-from src.qase.api_client_v1.models.test_case_response import TestCaseResponse
-from src.qase.api_client_v1.models.test_case_update import TestCaseUpdate
-from src.qase.api_client_v1.models.test_casebulk import TestCasebulk
-from src.qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.bulk200_response import Bulk200Response
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.test_case_create import TestCaseCreate
+from qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
+from qase.api_client_v1.models.test_case_response import TestCaseResponse
+from qase.api_client_v1.models.test_case_update import TestCaseUpdate
+from qase.api_client_v1.models.test_casebulk import TestCasebulk
+from qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class CasesApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/configurations_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/configurations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.configuration_create import ConfigurationCreate
-from src.qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
-from src.qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
-from src.qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.configuration_create import ConfigurationCreate
+from qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
+from qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
+from qase.api_client_v1.models.id_response import IdResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class ConfigurationsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/custom_fields_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/custom_fields_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.custom_field_create import CustomFieldCreate
-from src.qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
-from src.qase.api_client_v1.models.custom_field_response import CustomFieldResponse
-from src.qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
-from src.qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.custom_field_create import CustomFieldCreate
+from qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
+from qase.api_client_v1.models.custom_field_response import CustomFieldResponse
+from qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
+from qase.api_client_v1.models.id_response import IdResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class CustomFieldsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/defects_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/defects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.defect_create import DefectCreate
-from src.qase.api_client_v1.models.defect_list_response import DefectListResponse
-from src.qase.api_client_v1.models.defect_response import DefectResponse
-from src.qase.api_client_v1.models.defect_status import DefectStatus
-from src.qase.api_client_v1.models.defect_update import DefectUpdate
-from src.qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.defect_create import DefectCreate
+from qase.api_client_v1.models.defect_list_response import DefectListResponse
+from qase.api_client_v1.models.defect_response import DefectResponse
+from qase.api_client_v1.models.defect_status import DefectStatus
+from qase.api_client_v1.models.defect_update import DefectUpdate
+from qase.api_client_v1.models.id_response import IdResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class DefectsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/environments_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/environments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.environment_create import EnvironmentCreate
-from src.qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
-from src.qase.api_client_v1.models.environment_response import EnvironmentResponse
-from src.qase.api_client_v1.models.environment_update import EnvironmentUpdate
-from src.qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.environment_create import EnvironmentCreate
+from qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
+from qase.api_client_v1.models.environment_response import EnvironmentResponse
+from qase.api_client_v1.models.environment_update import EnvironmentUpdate
+from qase.api_client_v1.models.id_response import IdResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class EnvironmentsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/milestones_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/milestones_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.milestone_create import MilestoneCreate
-from src.qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
-from src.qase.api_client_v1.models.milestone_response import MilestoneResponse
-from src.qase.api_client_v1.models.milestone_update import MilestoneUpdate
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.milestone_create import MilestoneCreate
+from qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
+from qase.api_client_v1.models.milestone_response import MilestoneResponse
+from qase.api_client_v1.models.milestone_update import MilestoneUpdate
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class MilestonesApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/plans_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/plans_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.plan_create import PlanCreate
-from src.qase.api_client_v1.models.plan_list_response import PlanListResponse
-from src.qase.api_client_v1.models.plan_response import PlanResponse
-from src.qase.api_client_v1.models.plan_update import PlanUpdate
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.plan_create import PlanCreate
+from qase.api_client_v1.models.plan_list_response import PlanListResponse
+from qase.api_client_v1.models.plan_response import PlanResponse
+from qase.api_client_v1.models.plan_update import PlanUpdate
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class PlansApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/projects_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.project_access import ProjectAccess
-from src.qase.api_client_v1.models.project_code_response import ProjectCodeResponse
-from src.qase.api_client_v1.models.project_create import ProjectCreate
-from src.qase.api_client_v1.models.project_list_response import ProjectListResponse
-from src.qase.api_client_v1.models.project_response import ProjectResponse
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.project_access import ProjectAccess
+from qase.api_client_v1.models.project_code_response import ProjectCodeResponse
+from qase.api_client_v1.models.project_create import ProjectCreate
+from qase.api_client_v1.models.project_list_response import ProjectListResponse
+from qase.api_client_v1.models.project_response import ProjectResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class ProjectsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/results_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/results_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.hash_response import HashResponse
-from src.qase.api_client_v1.models.result_create import ResultCreate
-from src.qase.api_client_v1.models.result_create_response import ResultCreateResponse
-from src.qase.api_client_v1.models.result_list_response import ResultListResponse
-from src.qase.api_client_v1.models.result_response import ResultResponse
-from src.qase.api_client_v1.models.result_update import ResultUpdate
-from src.qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.hash_response import HashResponse
+from qase.api_client_v1.models.result_create import ResultCreate
+from qase.api_client_v1.models.result_create_response import ResultCreateResponse
+from qase.api_client_v1.models.result_list_response import ResultListResponse
+from qase.api_client_v1.models.result_response import ResultResponse
+from qase.api_client_v1.models.result_update import ResultUpdate
+from qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class ResultsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/runs_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/runs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.run_create import RunCreate
-from src.qase.api_client_v1.models.run_list_response import RunListResponse
-from src.qase.api_client_v1.models.run_public import RunPublic
-from src.qase.api_client_v1.models.run_public_response import RunPublicResponse
-from src.qase.api_client_v1.models.run_response import RunResponse
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.run_create import RunCreate
+from qase.api_client_v1.models.run_list_response import RunListResponse
+from qase.api_client_v1.models.run_public import RunPublic
+from qase.api_client_v1.models.run_public_response import RunPublicResponse
+from qase.api_client_v1.models.run_response import RunResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class RunsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/search_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/search_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.search_response import SearchResponse
+from qase.api_client_v1.models.search_response import SearchResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class SearchApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/shared_steps_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/shared_steps_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.hash_response import HashResponse
-from src.qase.api_client_v1.models.shared_step_create import SharedStepCreate
-from src.qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
-from src.qase.api_client_v1.models.shared_step_response import SharedStepResponse
-from src.qase.api_client_v1.models.shared_step_update import SharedStepUpdate
+from qase.api_client_v1.models.hash_response import HashResponse
+from qase.api_client_v1.models.shared_step_create import SharedStepCreate
+from qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
+from qase.api_client_v1.models.shared_step_response import SharedStepResponse
+from qase.api_client_v1.models.shared_step_update import SharedStepUpdate
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class SharedStepsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/suites_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/suites_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 from typing import Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.suite_create import SuiteCreate
-from src.qase.api_client_v1.models.suite_delete import SuiteDelete
-from src.qase.api_client_v1.models.suite_list_response import SuiteListResponse
-from src.qase.api_client_v1.models.suite_response import SuiteResponse
-from src.qase.api_client_v1.models.suite_update import SuiteUpdate
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.suite_create import SuiteCreate
+from qase.api_client_v1.models.suite_delete import SuiteDelete
+from qase.api_client_v1.models.suite_list_response import SuiteListResponse
+from qase.api_client_v1.models.suite_response import SuiteResponse
+from qase.api_client_v1.models.suite_update import SuiteUpdate
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class SuitesApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api/system_fields_api.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/system_fields_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from src.qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
+from qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
 
-from src.qase.api_client_v1.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v1.api_response import ApiResponse
-from src.qase.api_client_v1.rest import RESTResponseType
+from qase.api_client_v1.api_client import ApiClient, RequestSerialized
+from qase.api_client_v1.api_response import ApiResponse
+from qase.api_client_v1.rest import RESTResponseType
 
 
 class SystemFieldsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api_client.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,30 +10,32 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import datetime
+from io import BytesIO
+
 from dateutil.parser import parse
 from enum import Enum
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 from typing import Tuple, Optional, List, Dict
 
-from src.qase.api_client_v1.configuration import Configuration
-from src.qase.api_client_v1.api_response import ApiResponse, T as ApiResponseT
-import src.qase.api_client_v1.models
-from src.qase.api_client_v1 import rest
-from src.qase.api_client_v1.exceptions import (
+from qase.api_client_v1.configuration import Configuration
+from qase.api_client_v1.api_response import ApiResponse, T as ApiResponseT
+import qase.api_client_v1.models
+from qase.api_client_v1 import rest
+from qase.api_client_v1.exceptions import (
     ApiValueError,
     ApiException,
     BadRequestException,
     UnauthorizedException,
     ForbiddenException,
     NotFoundException,
     ServiceException
@@ -417,15 +419,15 @@
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in data.items()}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
-                klass = getattr(src.qase.apiv1.models, klass)
+                klass = getattr(qase.api_client_v1.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
@@ -515,14 +517,19 @@
 
         if files:
             for k, v in files.items():
                 if not v:
                     continue
                 file_names = v if type(v) is list else [v]
                 for n in file_names:
+                    if isinstance(n, BytesIO):
+                        params.append(
+                            tuple([k, tuple([n.name, n.getvalue(), n.mime])]))
+                        continue
+
                     with open(n, 'rb') as f:
                         filename = os.path.basename(f.name)
                         filedata = f.read()
                         mimetype = (
                             mimetypes.guess_type(filename)[0]
                             or 'application/octet-stream'
                         )
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/api_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/api_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/configuration.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
           cookieAuth:         # name for the security scheme
             type: apiKey
             in: cookie
             name: JSESSIONID  # cookie name
 
     You can programmatically set the cookie:
 
-conf = src.qase.api_client_v1.Configuration(
+conf = qase.api_client_v1.Configuration(
     api_key={'cookieAuth': 'abc123'}
     api_key_prefix={'cookieAuth': 'JSESSIONID'}
 )
 
     The following cookie will be added to the HTTP request:
        Cookie: JSESSIONID abc123
     """
@@ -126,15 +126,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("src.qase.api_client_v1")
+        self.logger["package_logger"] = logging.getLogger("qase.api_client_v1")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/exceptions.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/__init__.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,149 +11,149 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.attachment_get import AttachmentGet
-from src.qase.api_client_v1.models.attachment_hash import AttachmentHash
-from src.qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
-from src.qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
-from src.qase.api_client_v1.models.attachment_response import AttachmentResponse
-from src.qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
-from src.qase.api_client_v1.models.attachmentupload import Attachmentupload
-from src.qase.api_client_v1.models.author import Author
-from src.qase.api_client_v1.models.author_list_response import AuthorListResponse
-from src.qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
-from src.qase.api_client_v1.models.author_response import AuthorResponse
-from src.qase.api_client_v1.models.base_response import BaseResponse
-from src.qase.api_client_v1.models.bulk200_response import Bulk200Response
-from src.qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
-from src.qase.api_client_v1.models.configuration import Configuration
-from src.qase.api_client_v1.models.configuration_create import ConfigurationCreate
-from src.qase.api_client_v1.models.configuration_group import ConfigurationGroup
-from src.qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
-from src.qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
-from src.qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
-from src.qase.api_client_v1.models.custom_field import CustomField
-from src.qase.api_client_v1.models.custom_field_create import CustomFieldCreate
-from src.qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
-from src.qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
-from src.qase.api_client_v1.models.custom_field_response import CustomFieldResponse
-from src.qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.custom_fields_response import CustomFieldsResponse
-from src.qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
-from src.qase.api_client_v1.models.defect import Defect
-from src.qase.api_client_v1.models.defect_create import DefectCreate
-from src.qase.api_client_v1.models.defect_list_response import DefectListResponse
-from src.qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
-from src.qase.api_client_v1.models.defect_query import DefectQuery
-from src.qase.api_client_v1.models.defect_response import DefectResponse
-from src.qase.api_client_v1.models.defect_status import DefectStatus
-from src.qase.api_client_v1.models.defect_update import DefectUpdate
-from src.qase.api_client_v1.models.environment import Environment
-from src.qase.api_client_v1.models.environment_create import EnvironmentCreate
-from src.qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
-from src.qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
-from src.qase.api_client_v1.models.environment_response import EnvironmentResponse
-from src.qase.api_client_v1.models.environment_update import EnvironmentUpdate
-from src.qase.api_client_v1.models.external_issue import ExternalIssue
-from src.qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
-from src.qase.api_client_v1.models.hash_response import HashResponse
-from src.qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
-from src.qase.api_client_v1.models.id_response import IdResponse
-from src.qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
-from src.qase.api_client_v1.models.milestone import Milestone
-from src.qase.api_client_v1.models.milestone_create import MilestoneCreate
-from src.qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
-from src.qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
-from src.qase.api_client_v1.models.milestone_response import MilestoneResponse
-from src.qase.api_client_v1.models.milestone_update import MilestoneUpdate
-from src.qase.api_client_v1.models.plan import Plan
-from src.qase.api_client_v1.models.plan_create import PlanCreate
-from src.qase.api_client_v1.models.plan_detailed import PlanDetailed
-from src.qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
-from src.qase.api_client_v1.models.plan_list_response import PlanListResponse
-from src.qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
-from src.qase.api_client_v1.models.plan_query import PlanQuery
-from src.qase.api_client_v1.models.plan_response import PlanResponse
-from src.qase.api_client_v1.models.plan_update import PlanUpdate
-from src.qase.api_client_v1.models.project import Project
-from src.qase.api_client_v1.models.project_access import ProjectAccess
-from src.qase.api_client_v1.models.project_code_response import ProjectCodeResponse
-from src.qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
-from src.qase.api_client_v1.models.project_counts import ProjectCounts
-from src.qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
-from src.qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
-from src.qase.api_client_v1.models.project_create import ProjectCreate
-from src.qase.api_client_v1.models.project_list_response import ProjectListResponse
-from src.qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
-from src.qase.api_client_v1.models.project_response import ProjectResponse
-from src.qase.api_client_v1.models.qql_defect import QqlDefect
-from src.qase.api_client_v1.models.qql_plan import QqlPlan
-from src.qase.api_client_v1.models.qql_test_case import QqlTestCase
-from src.qase.api_client_v1.models.requirement import Requirement
-from src.qase.api_client_v1.models.response import Response
-from src.qase.api_client_v1.models.result import Result
-from src.qase.api_client_v1.models.result_create import ResultCreate
-from src.qase.api_client_v1.models.result_create_bulk import ResultCreateBulk
-from src.qase.api_client_v1.models.result_create_case import ResultCreateCase
-from src.qase.api_client_v1.models.result_create_response import ResultCreateResponse
-from src.qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
-from src.qase.api_client_v1.models.result_list_response import ResultListResponse
-from src.qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
-from src.qase.api_client_v1.models.result_response import ResultResponse
-from src.qase.api_client_v1.models.result_update import ResultUpdate
-from src.qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
-from src.qase.api_client_v1.models.run import Run
-from src.qase.api_client_v1.models.run_create import RunCreate
-from src.qase.api_client_v1.models.run_environment import RunEnvironment
-from src.qase.api_client_v1.models.run_list_response import RunListResponse
-from src.qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
-from src.qase.api_client_v1.models.run_milestone import RunMilestone
-from src.qase.api_client_v1.models.run_public import RunPublic
-from src.qase.api_client_v1.models.run_public_response import RunPublicResponse
-from src.qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
-from src.qase.api_client_v1.models.run_response import RunResponse
-from src.qase.api_client_v1.models.run_stats import RunStats
-from src.qase.api_client_v1.models.search_response import SearchResponse
-from src.qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
-from src.qase.api_client_v1.models.search_response_all_of_result_entities import SearchResponseAllOfResultEntities
-from src.qase.api_client_v1.models.shared_step import SharedStep
-from src.qase.api_client_v1.models.shared_step_content import SharedStepContent
-from src.qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
-from src.qase.api_client_v1.models.shared_step_create import SharedStepCreate
-from src.qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
-from src.qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
-from src.qase.api_client_v1.models.shared_step_response import SharedStepResponse
-from src.qase.api_client_v1.models.shared_step_update import SharedStepUpdate
-from src.qase.api_client_v1.models.suite import Suite
-from src.qase.api_client_v1.models.suite_create import SuiteCreate
-from src.qase.api_client_v1.models.suite_delete import SuiteDelete
-from src.qase.api_client_v1.models.suite_list_response import SuiteListResponse
-from src.qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
-from src.qase.api_client_v1.models.suite_response import SuiteResponse
-from src.qase.api_client_v1.models.suite_update import SuiteUpdate
-from src.qase.api_client_v1.models.system_field import SystemField
-from src.qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
-from src.qase.api_client_v1.models.system_field_option import SystemFieldOption
-from src.qase.api_client_v1.models.tag_value import TagValue
-from src.qase.api_client_v1.models.test_case import TestCase
-from src.qase.api_client_v1.models.test_case_create import TestCaseCreate
-from src.qase.api_client_v1.models.test_case_external_issues import TestCaseExternalIssues
-from src.qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
-from src.qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
-from src.qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
-from src.qase.api_client_v1.models.test_case_params import TestCaseParams
-from src.qase.api_client_v1.models.test_case_query import TestCaseQuery
-from src.qase.api_client_v1.models.test_case_response import TestCaseResponse
-from src.qase.api_client_v1.models.test_case_update import TestCaseUpdate
-from src.qase.api_client_v1.models.test_casebulk import TestCasebulk
-from src.qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
-from src.qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
-from src.qase.api_client_v1.models.test_step import TestStep
-from src.qase.api_client_v1.models.test_step_create import TestStepCreate
-from src.qase.api_client_v1.models.test_step_result import TestStepResult
-from src.qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.attachment_get import AttachmentGet
+from qase.api_client_v1.models.attachment_hash import AttachmentHash
+from qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
+from qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
+from qase.api_client_v1.models.attachment_response import AttachmentResponse
+from qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
+from qase.api_client_v1.models.attachmentupload import Attachmentupload
+from qase.api_client_v1.models.author import Author
+from qase.api_client_v1.models.author_list_response import AuthorListResponse
+from qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
+from qase.api_client_v1.models.author_response import AuthorResponse
+from qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.bulk200_response import Bulk200Response
+from qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
+from qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration_create import ConfigurationCreate
+from qase.api_client_v1.models.configuration_group import ConfigurationGroup
+from qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
+from qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
+from qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
+from qase.api_client_v1.models.custom_field import CustomField
+from qase.api_client_v1.models.custom_field_create import CustomFieldCreate
+from qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
+from qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
+from qase.api_client_v1.models.custom_field_response import CustomFieldResponse
+from qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.custom_fields_response import CustomFieldsResponse
+from qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
+from qase.api_client_v1.models.defect import Defect
+from qase.api_client_v1.models.defect_create import DefectCreate
+from qase.api_client_v1.models.defect_list_response import DefectListResponse
+from qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
+from qase.api_client_v1.models.defect_query import DefectQuery
+from qase.api_client_v1.models.defect_response import DefectResponse
+from qase.api_client_v1.models.defect_status import DefectStatus
+from qase.api_client_v1.models.defect_update import DefectUpdate
+from qase.api_client_v1.models.environment import Environment
+from qase.api_client_v1.models.environment_create import EnvironmentCreate
+from qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
+from qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
+from qase.api_client_v1.models.environment_response import EnvironmentResponse
+from qase.api_client_v1.models.environment_update import EnvironmentUpdate
+from qase.api_client_v1.models.external_issue import ExternalIssue
+from qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
+from qase.api_client_v1.models.hash_response import HashResponse
+from qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
+from qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
+from qase.api_client_v1.models.milestone import Milestone
+from qase.api_client_v1.models.milestone_create import MilestoneCreate
+from qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
+from qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
+from qase.api_client_v1.models.milestone_response import MilestoneResponse
+from qase.api_client_v1.models.milestone_update import MilestoneUpdate
+from qase.api_client_v1.models.plan import Plan
+from qase.api_client_v1.models.plan_create import PlanCreate
+from qase.api_client_v1.models.plan_detailed import PlanDetailed
+from qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
+from qase.api_client_v1.models.plan_list_response import PlanListResponse
+from qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
+from qase.api_client_v1.models.plan_query import PlanQuery
+from qase.api_client_v1.models.plan_response import PlanResponse
+from qase.api_client_v1.models.plan_update import PlanUpdate
+from qase.api_client_v1.models.project import Project
+from qase.api_client_v1.models.project_access import ProjectAccess
+from qase.api_client_v1.models.project_code_response import ProjectCodeResponse
+from qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
+from qase.api_client_v1.models.project_counts import ProjectCounts
+from qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
+from qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
+from qase.api_client_v1.models.project_create import ProjectCreate
+from qase.api_client_v1.models.project_list_response import ProjectListResponse
+from qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
+from qase.api_client_v1.models.project_response import ProjectResponse
+from qase.api_client_v1.models.qql_defect import QqlDefect
+from qase.api_client_v1.models.qql_plan import QqlPlan
+from qase.api_client_v1.models.qql_test_case import QqlTestCase
+from qase.api_client_v1.models.requirement import Requirement
+from qase.api_client_v1.models.response import Response
+from qase.api_client_v1.models.result import Result
+from qase.api_client_v1.models.result_create import ResultCreate
+from qase.api_client_v1.models.result_create_bulk import ResultCreateBulk
+from qase.api_client_v1.models.result_create_case import ResultCreateCase
+from qase.api_client_v1.models.result_create_response import ResultCreateResponse
+from qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
+from qase.api_client_v1.models.result_list_response import ResultListResponse
+from qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
+from qase.api_client_v1.models.result_response import ResultResponse
+from qase.api_client_v1.models.result_update import ResultUpdate
+from qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
+from qase.api_client_v1.models.run import Run
+from qase.api_client_v1.models.run_create import RunCreate
+from qase.api_client_v1.models.run_environment import RunEnvironment
+from qase.api_client_v1.models.run_list_response import RunListResponse
+from qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
+from qase.api_client_v1.models.run_milestone import RunMilestone
+from qase.api_client_v1.models.run_public import RunPublic
+from qase.api_client_v1.models.run_public_response import RunPublicResponse
+from qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
+from qase.api_client_v1.models.run_response import RunResponse
+from qase.api_client_v1.models.run_stats import RunStats
+from qase.api_client_v1.models.search_response import SearchResponse
+from qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
+from qase.api_client_v1.models.search_response_all_of_result_entities import SearchResponseAllOfResultEntities
+from qase.api_client_v1.models.shared_step import SharedStep
+from qase.api_client_v1.models.shared_step_content import SharedStepContent
+from qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
+from qase.api_client_v1.models.shared_step_create import SharedStepCreate
+from qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
+from qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
+from qase.api_client_v1.models.shared_step_response import SharedStepResponse
+from qase.api_client_v1.models.shared_step_update import SharedStepUpdate
+from qase.api_client_v1.models.suite import Suite
+from qase.api_client_v1.models.suite_create import SuiteCreate
+from qase.api_client_v1.models.suite_delete import SuiteDelete
+from qase.api_client_v1.models.suite_list_response import SuiteListResponse
+from qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
+from qase.api_client_v1.models.suite_response import SuiteResponse
+from qase.api_client_v1.models.suite_update import SuiteUpdate
+from qase.api_client_v1.models.system_field import SystemField
+from qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
+from qase.api_client_v1.models.system_field_option import SystemFieldOption
+from qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.test_case import TestCase
+from qase.api_client_v1.models.test_case_create import TestCaseCreate
+from qase.api_client_v1.models.test_case_external_issues import TestCaseExternalIssues
+from qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
+from qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
+from qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
+from qase.api_client_v1.models.test_case_params import TestCaseParams
+from qase.api_client_v1.models.test_case_query import TestCaseQuery
+from qase.api_client_v1.models.test_case_response import TestCaseResponse
+from qase.api_client_v1.models.test_case_update import TestCaseUpdate
+from qase.api_client_v1.models.test_casebulk import TestCasebulk
+from qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
+from qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
+from qase.api_client_v1.models.test_step import TestStep
+from qase.api_client_v1.models.test_step_create import TestStepCreate
+from qase.api_client_v1.models.test_step_result import TestStepResult
+from qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_get.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_get.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_hash.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_hash.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
+from qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AttachmentListResponse(BaseModel):
     """
     AttachmentListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment_get import AttachmentGet
+from qase.api_client_v1.models.attachment_get import AttachmentGet
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AttachmentListResponseAllOfResult(BaseModel):
     """
     AttachmentListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment_get import AttachmentGet
+from qase.api_client_v1.models.attachment_get import AttachmentGet
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AttachmentResponse(BaseModel):
     """
     AttachmentResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachment_uploads_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_uploads_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachmentupload import Attachmentupload
+from qase.api_client_v1.models.attachmentupload import Attachmentupload
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AttachmentUploadsResponse(BaseModel):
     """
     AttachmentUploadsResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/attachmentupload.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachmentupload.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
+from qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AuthorListResponse(BaseModel):
     """
     AuthorListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response_all_of_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.author import Author
+from qase.api_client_v1.models.author import Author
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AuthorListResponseAllOfResult(BaseModel):
     """
     AuthorListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/author_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.author import Author
+from qase.api_client_v1.models.author import Author
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AuthorResponse(BaseModel):
     """
     AuthorResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/base_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/base_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/bulk200_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
+from qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Bulk200Response(BaseModel):
     """
     Bulk200Response
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/bulk200_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_group.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration import Configuration
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ConfigurationGroup(BaseModel):
     """
     ConfigurationGroup
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_group_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
+from qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ConfigurationListResponse(BaseModel):
     """
     ConfigurationListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.configuration_group import ConfigurationGroup
+from qase.api_client_v1.models.configuration_group import ConfigurationGroup
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ConfigurationListResponseAllOfResult(BaseModel):
     """
     ConfigurationListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
+from qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CustomFieldCreate(BaseModel):
     """
     CustomFieldCreate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_create_value_inner.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create_value_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
+from qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CustomFieldListResponse(BaseModel):
     """
     CustomFieldListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.custom_field import CustomField
+from qase.api_client_v1.models.custom_field import CustomField
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CustomFieldResponse(BaseModel):
     """
     CustomFieldResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
+from qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CustomFieldUpdate(BaseModel):
     """
     CustomFieldUpdate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_field_value.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_value.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_fields_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
+from qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CustomFieldsResponse(BaseModel):
     """
     CustomFieldsResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.custom_field import CustomField
+from qase.api_client_v1.models.custom_field import CustomField
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CustomFieldsResponseAllOfResult(BaseModel):
     """
     CustomFieldsResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.tag_value import TagValue
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Defect(BaseModel):
     """
     Defect
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
+from qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DefectListResponse(BaseModel):
     """
     DefectListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.defect import Defect
+from qase.api_client_v1.models.defect import Defect
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DefectListResponseAllOfResult(BaseModel):
     """
     DefectListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_query.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.tag_value import TagValue
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DefectQuery(BaseModel):
     """
     DefectQuery
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.defect import Defect
+from qase.api_client_v1.models.defect import Defect
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DefectResponse(BaseModel):
     """
     DefectResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_status.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_status.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/defect_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
+from qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class EnvironmentListResponse(BaseModel):
     """
     EnvironmentListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response_all_of_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.environment import Environment
+from qase.api_client_v1.models.environment import Environment
 from typing import Optional, Set
 from typing_extensions import Self
 
 class EnvironmentListResponseAllOfResult(BaseModel):
     """
     EnvironmentListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.environment import Environment
+from qase.api_client_v1.models.environment import Environment
 from typing import Optional, Set
 from typing_extensions import Self
 
 class EnvironmentResponse(BaseModel):
     """
     EnvironmentResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/environment_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/external_issue.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
+from qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ExternalIssue(BaseModel):
     """
     ExternalIssue
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/external_issue_issues_inner.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/hash_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
+from qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class HashResponse(BaseModel):
     """
     HashResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/hash_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/id_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
+from qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class IdResponse(BaseModel):
     """
     IdResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/id_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
+from qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class MilestoneListResponse(BaseModel):
     """
     MilestoneListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.milestone import Milestone
+from qase.api_client_v1.models.milestone import Milestone
 from typing import Optional, Set
 from typing_extensions import Self
 
 class MilestoneListResponseAllOfResult(BaseModel):
     """
     MilestoneListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.milestone import Milestone
+from qase.api_client_v1.models.milestone import Milestone
 from typing import Optional, Set
 from typing_extensions import Self
 
 class MilestoneResponse(BaseModel):
     """
     MilestoneResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/milestone_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_detailed.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from src.qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
+from qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PlanDetailed(BaseModel):
     """
     PlanDetailed
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
+from qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PlanListResponse(BaseModel):
+class RunListResponse(BaseModel):
     """
-    PlanListResponse
+    RunListResponse
     """ # noqa: E501
     status: Optional[StrictBool] = None
-    result: Optional[PlanListResponseAllOfResult] = None
+    result: Optional[RunListResponseAllOfResult] = None
     __properties: ClassVar[List[str]] = ["status", "result"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PlanListResponse from a JSON string"""
+        """Create an instance of RunListResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,21 +74,21 @@
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict['result'] = self.result.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PlanListResponse from a dict"""
+        """Create an instance of RunListResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status"),
-            "result": PlanListResponseAllOfResult.from_dict(obj["result"]) if obj.get("result") is not None else None
+            "result": RunListResponseAllOfResult.from_dict(obj["result"]) if obj.get("result") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.plan import Plan
+from qase.api_client_v1.models.plan import Plan
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PlanListResponseAllOfResult(BaseModel):
     """
     PlanListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_query.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.plan_detailed import PlanDetailed
+from qase.api_client_v1.models.plan_detailed import PlanDetailed
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PlanResponse(BaseModel):
     """
     PlanResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/plan_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.project_counts import ProjectCounts
+from qase.api_client_v1.models.project_counts import ProjectCounts
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Project(BaseModel):
     """
     Project
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_access.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_access.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_code_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
+from qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ProjectCodeResponse(BaseModel):
     """
     ProjectCodeResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_code_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_counts.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
-from src.qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
+from qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
+from qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ProjectCounts(BaseModel):
     """
     ProjectCounts
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_counts_defects.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_defects.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_counts_runs.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_runs.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
+from qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ProjectListResponse(BaseModel):
     """
     ProjectListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response_all_of_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.project import Project
+from qase.api_client_v1.models.project import Project
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ProjectListResponseAllOfResult(BaseModel):
     """
     ProjectListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/project_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.project import Project
+from qase.api_client_v1.models.project import Project
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ProjectResponse(BaseModel):
     """
     ProjectResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/qql_defect.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_defect.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.tag_value import TagValue
 from typing import Optional, Set
 from typing_extensions import Self
 
 class QqlDefect(BaseModel):
     """
     QqlDefect
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/qql_plan.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_plan.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/qql_test_case.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.tag_value import TagValue
-from src.qase.api_client_v1.models.test_case_params import TestCaseParams
-from src.qase.api_client_v1.models.test_step import TestStep
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.test_case_params import TestCaseParams
+from qase.api_client_v1.models.test_step import TestStep
 from typing import Optional, Set
 from typing_extensions import Self
 
 class QqlTestCase(BaseModel):
     """
     QqlTestCase
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/requirement.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/requirement.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.test_step_result import TestStepResult
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.test_step_result import TestStepResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Result(BaseModel):
     """
     Result
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.result_create_case import ResultCreateCase
-from src.qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
+from qase.api_client_v1.models.result_create_case import ResultCreateCase
+from qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultCreate(BaseModel):
     """
     ResultCreate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_bulk.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.result_create import ResultCreate
+from qase.api_client_v1.models.result_create import ResultCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultCreateBulk(BaseModel):
     """
     ResultCreateBulk
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_case.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
+from qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultCreateResponse(BaseModel):
     """
     ResultCreateResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_create_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
+from qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultListResponse(BaseModel):
     """
     ResultListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.result import Result
+from qase.api_client_v1.models.result import Result
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultListResponseAllOfResult(BaseModel):
     """
     ResultListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.result import Result
+from qase.api_client_v1.models.result import Result
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultResponse(BaseModel):
     """
     ResultResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/result_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
+from qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultUpdate(BaseModel):
     """
     ResultUpdate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/resultcreate_bulk.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/resultcreate_bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.result_create import ResultCreate
+from qase.api_client_v1.models.result_create import ResultCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultcreateBulk(BaseModel):
     """
     ResultcreateBulk
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.run_environment import RunEnvironment
-from src.qase.api_client_v1.models.run_milestone import RunMilestone
-from src.qase.api_client_v1.models.run_stats import RunStats
-from src.qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.run_environment import RunEnvironment
+from qase.api_client_v1.models.run_milestone import RunMilestone
+from qase.api_client_v1.models.run_stats import RunStats
+from qase.api_client_v1.models.tag_value import TagValue
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Run(BaseModel):
     """
     Run
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_environment.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_environment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
+from qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RunListResponse(BaseModel):
+class SharedStepListResponse(BaseModel):
     """
-    RunListResponse
+    SharedStepListResponse
     """ # noqa: E501
     status: Optional[StrictBool] = None
-    result: Optional[RunListResponseAllOfResult] = None
+    result: Optional[SharedStepListResponseAllOfResult] = None
     __properties: ClassVar[List[str]] = ["status", "result"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RunListResponse from a JSON string"""
+        """Create an instance of SharedStepListResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,21 +74,21 @@
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict['result'] = self.result.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RunListResponse from a dict"""
+        """Create an instance of SharedStepListResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status"),
-            "result": RunListResponseAllOfResult.from_dict(obj["result"]) if obj.get("result") is not None else None
+            "result": SharedStepListResponseAllOfResult.from_dict(obj["result"]) if obj.get("result") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response_all_of_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.run import Run
+from qase.api_client_v1.models.run import Run
 from typing import Optional, Set
 from typing_extensions import Self
 
 class RunListResponseAllOfResult(BaseModel):
     """
     RunListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_milestone.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_milestone.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_public.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_public_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
+from qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class RunPublicResponse(BaseModel):
     """
     RunPublicResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_public_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.run import Run
+from qase.api_client_v1.models.run import Run
 from typing import Optional, Set
 from typing_extensions import Self
 
 class RunResponse(BaseModel):
     """
     RunResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/run_stats.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_stats.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/search_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
+from qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SearchResponse(BaseModel):
     """
     SearchResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/search_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
-from src.qase.api_client_v1.models.search_response_all_of_result_entities import SearchResponseAllOfResultEntities
+from qase.api_client_v1.models.search_response_all_of_result_entities import SearchResponseAllOfResultEntities
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SearchResponseAllOfResult(BaseModel):
     """
     SearchResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/search_response_all_of_result_entities.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 
 from __future__ import annotations
 import json
 import pprint
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Any, List, Optional
-from src.qase.api_client_v1.models.defect_query import DefectQuery
-from src.qase.api_client_v1.models.plan_query import PlanQuery
-from src.qase.api_client_v1.models.requirement import Requirement
-from src.qase.api_client_v1.models.result import Result
-from src.qase.api_client_v1.models.run import Run
-from src.qase.api_client_v1.models.test_case_query import TestCaseQuery
+from qase.api_client_v1.models.defect_query import DefectQuery
+from qase.api_client_v1.models.plan_query import PlanQuery
+from qase.api_client_v1.models.requirement import Requirement
+from qase.api_client_v1.models.result import Result
+from qase.api_client_v1.models.run import Run
+from qase.api_client_v1.models.test_case_query import TestCaseQuery
 from pydantic import StrictStr, Field
 from typing import Union, List, Optional, Dict
 from typing_extensions import Literal, Self
 
 SEARCHRESPONSEALLOFRESULTENTITIES_ONE_OF_SCHEMAS = ["DefectQuery", "PlanQuery", "Requirement", "Result", "Run", "TestCaseQuery"]
 
 class SearchResponseAllOfResultEntities(BaseModel):
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.shared_step_content import SharedStepContent
+from qase.api_client_v1.models.shared_step_content import SharedStepContent
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SharedStep(BaseModel):
     """
     SharedStep
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_content.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment_hash import AttachmentHash
+from qase.api_client_v1.models.attachment_hash import AttachmentHash
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SharedStepContent(BaseModel):
     """
     SharedStepContent
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_content_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
+from qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SharedStepCreate(BaseModel):
     """
     SharedStepCreate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
+from qase.api_client_v1.models.shared_step import SharedStep
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SharedStepListResponse(BaseModel):
+class SharedStepResponse(BaseModel):
     """
-    SharedStepListResponse
+    SharedStepResponse
     """ # noqa: E501
     status: Optional[StrictBool] = None
-    result: Optional[SharedStepListResponseAllOfResult] = None
+    result: Optional[SharedStep] = None
     __properties: ClassVar[List[str]] = ["status", "result"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SharedStepListResponse from a JSON string"""
+        """Create an instance of SharedStepResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,21 +74,21 @@
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict['result'] = self.result.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SharedStepListResponse from a dict"""
+        """Create an instance of SharedStepResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status"),
-            "result": SharedStepListResponseAllOfResult.from_dict(obj["result"]) if obj.get("result") is not None else None
+            "result": SharedStep.from_dict(obj["result"]) if obj.get("result") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.shared_step import SharedStep
+from qase.api_client_v1.models.shared_step import SharedStep
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SharedStepListResponseAllOfResult(BaseModel):
     """
     SharedStepListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.shared_step import SharedStep
+from qase.api_client_v1.models.suite import Suite
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SharedStepResponse(BaseModel):
+class SuiteResponse(BaseModel):
     """
-    SharedStepResponse
+    SuiteResponse
     """ # noqa: E501
     status: Optional[StrictBool] = None
-    result: Optional[SharedStep] = None
+    result: Optional[Suite] = None
     __properties: ClassVar[List[str]] = ["status", "result"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SharedStepResponse from a JSON string"""
+        """Create an instance of SuiteResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,21 +74,21 @@
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict['result'] = self.result.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SharedStepResponse from a dict"""
+        """Create an instance of SuiteResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status"),
-            "result": SharedStep.from_dict(obj["result"]) if obj.get("result") is not None else None
+            "result": Suite.from_dict(obj["result"]) if obj.get("result") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/shared_step_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
+from qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SharedStepUpdate(BaseModel):
     """
     SharedStepUpdate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_delete.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_delete.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
+from qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SuiteListResponse(BaseModel):
     """
     SuiteListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.suite import Suite
+from qase.api_client_v1.models.suite import Suite
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SuiteListResponseAllOfResult(BaseModel):
     """
     SuiteListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.suite import Suite
+from qase.api_client_v1.models.test_case import TestCase
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SuiteResponse(BaseModel):
+class TestCaseResponse(BaseModel):
     """
-    SuiteResponse
+    TestCaseResponse
     """ # noqa: E501
     status: Optional[StrictBool] = None
-    result: Optional[Suite] = None
+    result: Optional[TestCase] = None
     __properties: ClassVar[List[str]] = ["status", "result"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SuiteResponse from a JSON string"""
+        """Create an instance of TestCaseResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,21 +74,21 @@
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict['result'] = self.result.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SuiteResponse from a dict"""
+        """Create an instance of TestCaseResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status"),
-            "result": Suite.from_dict(obj["result"]) if obj.get("result") is not None else None
+            "result": TestCase.from_dict(obj["result"]) if obj.get("result") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/suite_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/system_field.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.system_field_option import SystemFieldOption
+from qase.api_client_v1.models.system_field_option import SystemFieldOption
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SystemField(BaseModel):
     """
     SystemField
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/system_field_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.system_field import SystemField
+from qase.api_client_v1.models.system_field import SystemField
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SystemFieldListResponse(BaseModel):
     """
     SystemFieldListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/system_field_option.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_option.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/tag_value.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/tag_value.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.external_issue import ExternalIssue
-from src.qase.api_client_v1.models.tag_value import TagValue
-from src.qase.api_client_v1.models.test_case_params import TestCaseParams
-from src.qase.api_client_v1.models.test_step import TestStep
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.external_issue import ExternalIssue
+from qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.test_case_params import TestCaseParams
+from qase.api_client_v1.models.test_step import TestStep
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCase(BaseModel):
     """
     TestCase
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.test_step_create import TestStepCreate
+from qase.api_client_v1.models.test_step_create import TestStepCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseCreate(BaseModel):
     """
     TestCaseCreate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_external_issues.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
-from src.qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
+from qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseExternalIssues(BaseModel):
     """
     TestCaseExternalIssues
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_list_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
+from qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseListResponse(BaseModel):
     """
     TestCaseListResponse
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.test_case import TestCase
+from qase.api_client_v1.models.test_case import TestCase
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseListResponseAllOfResult(BaseModel):
     """
     TestCaseListResponseAllOfResult
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_params.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_params.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_query.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
-from src.qase.api_client_v1.models.tag_value import TagValue
-from src.qase.api_client_v1.models.test_case_params import TestCaseParams
-from src.qase.api_client_v1.models.test_step import TestStep
+from qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.test_case_params import TestCaseParams
+from qase.api_client_v1.models.test_step import TestStep
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseQuery(BaseModel):
     """
     TestCaseQuery
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_response.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool
-from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.test_case import TestCase
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TestCaseResponse(BaseModel):
+class TestCasebulk(BaseModel):
     """
-    TestCaseResponse
+    TestCasebulk
     """ # noqa: E501
-    status: Optional[StrictBool] = None
-    result: Optional[TestCase] = None
-    __properties: ClassVar[List[str]] = ["status", "result"]
+    cases: List[TestCasebulkCasesInner]
+    __properties: ClassVar[List[str]] = ["cases"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TestCaseResponse from a JSON string"""
+        """Create an instance of TestCasebulk from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,28 +66,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of result
-        if self.result:
-            _dict['result'] = self.result.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in cases (list)
+        _items = []
+        if self.cases:
+            for _item in self.cases:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['cases'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TestCaseResponse from a dict"""
+        """Create an instance of TestCasebulk from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status"),
-            "result": TestCase.from_dict(obj["result"]) if obj.get("result") is not None else None
+            "cases": [TestCasebulkCasesInner.from_dict(_item) for _item in obj["cases"]] if obj.get("cases") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_case_update.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.test_step_create import TestStepCreate
+from qase.api_client_v1.models.test_step_create import TestStepCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseUpdate(BaseModel):
     """
     TestCaseUpdate
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_casebulk.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
-from typing import Any, ClassVar, Dict, List
-from src.qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from typing import Any, ClassVar, Dict, List, Optional
+from qase.api_client_v1.models.attachment import Attachment
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TestCasebulk(BaseModel):
+class TestStepResult(BaseModel):
     """
-    TestCasebulk
+    TestStepResult
     """ # noqa: E501
-    cases: List[TestCasebulkCasesInner]
-    __properties: ClassVar[List[str]] = ["cases"]
+    status: Optional[StrictInt] = None
+    position: Optional[StrictInt] = None
+    attachments: Optional[List[Attachment]] = None
+    steps: Optional[List[Dict[str, Any]]] = Field(default=None, description="Nested steps results will be here. The same structure is used for them for them.")
+    __properties: ClassVar[List[str]] = ["status", "position", "attachments", "steps"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TestCasebulk from a JSON string"""
+        """Create an instance of TestStepResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,31 +69,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in cases (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in attachments (list)
         _items = []
-        if self.cases:
-            for _item in self.cases:
+        if self.attachments:
+            for _item in self.attachments:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['cases'] = _items
+            _dict['attachments'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TestCasebulk from a dict"""
+        """Create an instance of TestStepResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "cases": [TestCasebulkCasesInner.from_dict(_item) for _item in obj["cases"]] if obj.get("cases") is not None else None
+            "status": obj.get("status"),
+            "position": obj.get("position"),
+            "attachments": [Attachment.from_dict(_item) for _item in obj["attachments"]] if obj.get("attachments") is not None else None,
+            "steps": obj.get("steps")
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_casebulk_cases_inner.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk_cases_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from src.qase.api_client_v1.models.test_step_create import TestStepCreate
+from qase.api_client_v1.models.test_step_create import TestStepCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCasebulkCasesInner(BaseModel):
     """
     TestCasebulkCasesInner
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_caseexternal_issues.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_caseexternal_issues.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
-from src.qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
+from qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestCaseexternalIssues(BaseModel):
     """
     TestCaseexternalIssues
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.attachment import Attachment
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TestStep(BaseModel):
     """
     TestStep
     """ # noqa: E501
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step_result.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from src.qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TestStepResult(BaseModel):
+class PlanListResponse(BaseModel):
     """
-    TestStepResult
+    PlanListResponse
     """ # noqa: E501
-    status: Optional[StrictInt] = None
-    position: Optional[StrictInt] = None
-    attachments: Optional[List[Attachment]] = None
-    steps: Optional[List[Dict[str, Any]]] = Field(default=None, description="Nested steps results will be here. The same structure is used for them for them.")
-    __properties: ClassVar[List[str]] = ["status", "position", "attachments", "steps"]
+    status: Optional[StrictBool] = None
+    result: Optional[PlanListResponseAllOfResult] = None
+    __properties: ClassVar[List[str]] = ["status", "result"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TestStepResult from a JSON string"""
+        """Create an instance of PlanListResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,34 +67,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in attachments (list)
-        _items = []
-        if self.attachments:
-            for _item in self.attachments:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['attachments'] = _items
+        # override the default output from pydantic by calling `to_dict()` of result
+        if self.result:
+            _dict['result'] = self.result.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TestStepResult from a dict"""
+        """Create an instance of PlanListResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status"),
-            "position": obj.get("position"),
-            "attachments": [Attachment.from_dict(_item) for _item in obj["attachments"]] if obj.get("attachments") is not None else None,
-            "steps": obj.get("steps")
+            "result": PlanListResponseAllOfResult.from_dict(obj["result"]) if obj.get("result") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/models/test_step_result_create.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/src/qase/api_client_v1/rest.py` & `qase_api_client-1.0.0b2/src/qase/api_client_v1/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import io
 import json
 import re
 import ssl
 
 import urllib3
 
-from src.qase.api_client_v1.exceptions import ApiException, ApiValueError
+from qase.api_client_v1.exceptions import ApiException, ApiValueError
 
 SUPPORTED_SOCKS_PROXIES = {"socks5", "socks5h", "socks4", "socks4a"}
 RESTResponseType = urllib3.HTTPResponse
 
 
 def is_socks_proxy_url(url):
     if url is None:
```

### Comparing `qase_api_client-1.0.0b1/src/qase_api_client.egg-info/PKG-INFO` & `qase_api_client-1.0.0b2/src/qase_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-api-client
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Qase TestOps API V1 client for Python
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python
 Keywords: OpenAPI,OpenAPI-Generator,Qase.io TestOps API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -42,48 +42,48 @@
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
-import qase.apiv1
+import qase.api_client_v1
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import qase.apiv1
+import qase.api_client_v1
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import qase.apiv1
-from qase.apiv1.rest import ApiException
+import qase.api_client_v1
+from qase.api_client_v1.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.qase.io/v1
 # See configuration.py for a list of all supported configuration parameters.
-configuration = src.qase.apiv1.Configuration(
+configuration = qase.api_client_v1.Configuration(
     host = "https://api.qase.io/v1"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
@@ -92,17 +92,17 @@
 configuration.api_key['TokenAuth'] = os.environ["API_KEY"]
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['TokenAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with qase.apiv1.ApiClient(configuration) as api_client:
+with qase.api_client_v1.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = qase.apiv1.AttachmentsApi(api_client)
+    api_instance = qase.api_client_v1.AttachmentsApi(api_client)
     hash = 'hash_example' # str | Hash.
 
     try:
         # Remove attachment by Hash
         api_response = api_instance.delete_attachment(hash)
         print("The response of AttachmentsApi->delete_attachment:\n")
         pprint(api_response)
```

### Comparing `qase_api_client-1.0.0b1/src/qase_api_client.egg-info/SOURCES.txt` & `qase_api_client-1.0.0b2/src/qase_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b1/test/test_attachment.py` & `qase_api_client-1.0.0b2/test/test_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment import Attachment
+from qase.api_client_v1.models.attachment import Attachment
 
 class TestAttachment(unittest.TestCase):
     """Attachment unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachment_get.py` & `qase_api_client-1.0.0b2/test/test_attachment_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment_get import AttachmentGet
+from qase.api_client_v1.models.attachment_get import AttachmentGet
 
 class TestAttachmentGet(unittest.TestCase):
     """AttachmentGet unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachment_hash.py` & `qase_api_client-1.0.0b2/test/test_attachment_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment_hash import AttachmentHash
+from qase.api_client_v1.models.attachment_hash import AttachmentHash
 
 class TestAttachmentHash(unittest.TestCase):
     """AttachmentHash unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachment_list_response.py` & `qase_api_client-1.0.0b2/test/test_attachment_list_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
+from qase.api_client_v1.models.attachment_list_response import AttachmentListResponse
 
 class TestAttachmentListResponse(unittest.TestCase):
     """AttachmentListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `AttachmentListResponse`
         """
         model = AttachmentListResponse()
         if include_optional:
             return AttachmentListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.attachment_list_response_all_of_result.AttachmentListResponse_allOf_result(
+                result = qase.api_client_v1.models.attachment_list_response_all_of_result.AttachmentListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.attachment_get.AttachmentGet(
+                        qase.api_client_v1.models.attachment_get.AttachmentGet(
                             hash = '', 
                             file = '', 
                             mime = '', 
                             size = 56, 
                             extension = '', 
                             full_path = '', 
                             url = '', )
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachment_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_attachment_list_response_all_of_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
+from qase.api_client_v1.models.attachment_list_response_all_of_result import AttachmentListResponseAllOfResult
 
 class TestAttachmentListResponseAllOfResult(unittest.TestCase):
     """AttachmentListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = AttachmentListResponseAllOfResult()
         if include_optional:
             return AttachmentListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.attachment_get.AttachmentGet(
+                    qase.api_client_v1.models.attachment_get.AttachmentGet(
                         hash = '', 
                         file = '', 
                         mime = '', 
                         size = 56, 
                         extension = '', 
                         full_path = '', 
                         url = '', )
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachment_response.py` & `qase_api_client-1.0.0b2/test/test_attachment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment_response import AttachmentResponse
+from qase.api_client_v1.models.attachment_response import AttachmentResponse
 
 class TestAttachmentResponse(unittest.TestCase):
     """AttachmentResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `AttachmentResponse`
         """
         model = AttachmentResponse()
         if include_optional:
             return AttachmentResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.attachment_get.AttachmentGet(
+                result = qase.api_client_v1.models.attachment_get.AttachmentGet(
                     hash = '', 
                     file = '', 
                     mime = '', 
                     size = 56, 
                     extension = '', 
                     full_path = '', 
                     url = '', )
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachment_uploads_response.py` & `qase_api_client-1.0.0b2/test/test_attachment_uploads_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
+from qase.api_client_v1.models.attachment_uploads_response import AttachmentUploadsResponse
 
 class TestAttachmentUploadsResponse(unittest.TestCase):
     """AttachmentUploadsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,15 +34,15 @@
         # uncomment below to create an instance of `AttachmentUploadsResponse`
         """
         model = AttachmentUploadsResponse()
         if include_optional:
             return AttachmentUploadsResponse(
                 status = True,
                 result = [
-                    src.qase.api_client_v1.models.attachmentupload.Attachmentupload(
+                    qase.api_client_v1.models.attachmentupload.Attachmentupload(
                         hash = '', 
                         filename = '', 
                         mime = '', 
                         extension = '', 
                         url = '', 
                         team = '', )
                     ]
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachments_api.py` & `qase_api_client-1.0.0b2/test/test_attachments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.attachments_api import AttachmentsApi
+from qase.api_client_v1.api.attachments_api import AttachmentsApi
 
 
 class TestAttachmentsApi(unittest.TestCase):
     """AttachmentsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = AttachmentsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_attachmentupload.py` & `qase_api_client-1.0.0b2/test/test_attachmentupload.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.attachmentupload import Attachmentupload
+from qase.api_client_v1.models.attachmentupload import Attachmentupload
 
 class TestAttachmentupload(unittest.TestCase):
     """Attachmentupload unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_author.py` & `qase_api_client-1.0.0b2/test/test_author.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.author import Author
+from qase.api_client_v1.models.author import Author
 
 class TestAuthor(unittest.TestCase):
     """Author unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_author_list_response.py` & `qase_api_client-1.0.0b2/test/test_author_list_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.author_list_response import AuthorListResponse
+from qase.api_client_v1.models.author_list_response import AuthorListResponse
 
 class TestAuthorListResponse(unittest.TestCase):
     """AuthorListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `AuthorListResponse`
         """
         model = AuthorListResponse()
         if include_optional:
             return AuthorListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.author_list_response_all_of_result.AuthorListResponse_allOf_result(
+                result = qase.api_client_v1.models.author_list_response_all_of_result.AuthorListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.author.Author(
+                        qase.api_client_v1.models.author.Author(
                             id = 56, 
                             entity_type = '', 
                             email = '', 
                             name = '', 
                             is_active = True, )
                         ], )
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_author_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_author_list_response_all_of_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
+from qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
 
 class TestAuthorListResponseAllOfResult(unittest.TestCase):
     """AuthorListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = AuthorListResponseAllOfResult()
         if include_optional:
             return AuthorListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.author.Author(
+                    qase.api_client_v1.models.author.Author(
                         id = 56, 
                         entity_type = '', 
                         email = '', 
                         name = '', 
                         is_active = True, )
                     ]
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_author_response.py` & `qase_api_client-1.0.0b2/test/test_author_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.author_response import AuthorResponse
+from qase.api_client_v1.models.author_response import AuthorResponse
 
 class TestAuthorResponse(unittest.TestCase):
     """AuthorResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `AuthorResponse`
         """
         model = AuthorResponse()
         if include_optional:
             return AuthorResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.author.Author(
+                result = qase.api_client_v1.models.author.Author(
                     id = 56, 
                     entity_type = '', 
                     email = '', 
                     name = '', 
                     is_active = True, )
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_authors_api.py` & `qase_api_client-1.0.0b2/test/test_authors_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.authors_api import AuthorsApi
+from qase.api_client_v1.api.authors_api import AuthorsApi
 
 
 class TestAuthorsApi(unittest.TestCase):
     """AuthorsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = AuthorsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_base_response.py` & `qase_api_client-1.0.0b2/test/test_base_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.base_response import BaseResponse
+from qase.api_client_v1.models.base_response import BaseResponse
 
 class TestBaseResponse(unittest.TestCase):
     """BaseResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_bulk200_response.py` & `qase_api_client-1.0.0b2/test/test_bulk200_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.bulk200_response import Bulk200Response
+from qase.api_client_v1.models.bulk200_response import Bulk200Response
 
 class TestBulk200Response(unittest.TestCase):
     """Bulk200Response unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `Bulk200Response`
         """
         model = Bulk200Response()
         if include_optional:
             return Bulk200Response(
                 status = True,
-                result = src.qase.api_client_v1.models.bulk_200_response_all_of_result.bulk_200_response_allOf_result(
+                result = qase.api_client_v1.models.bulk_200_response_all_of_result.bulk_200_response_allOf_result(
                     ids = [
                         56
                         ], )
             )
         else:
             return Bulk200Response(
         )
```

### Comparing `qase_api_client-1.0.0b1/test/test_bulk200_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_bulk200_response_all_of_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
+from qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
 
 class TestBulk200ResponseAllOfResult(unittest.TestCase):
     """Bulk200ResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_cases_api.py` & `qase_api_client-1.0.0b2/test/test_cases_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.cases_api import CasesApi
+from qase.api_client_v1.api.cases_api import CasesApi
 
 
 class TestCasesApi(unittest.TestCase):
     """CasesApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = CasesApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_configuration.py` & `qase_api_client-1.0.0b2/test/test_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration import Configuration
 
 class TestConfiguration(unittest.TestCase):
     """Configuration unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_configuration_create.py` & `qase_api_client-1.0.0b2/test/test_configuration_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.configuration_create import ConfigurationCreate
+from qase.api_client_v1.models.configuration_create import ConfigurationCreate
 
 class TestConfigurationCreate(unittest.TestCase):
     """ConfigurationCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_configuration_group.py` & `qase_api_client-1.0.0b2/test/test_configuration_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.configuration_group import ConfigurationGroup
+from qase.api_client_v1.models.configuration_group import ConfigurationGroup
 
 class TestConfigurationGroup(unittest.TestCase):
     """ConfigurationGroup unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -35,15 +35,15 @@
         """
         model = ConfigurationGroup()
         if include_optional:
             return ConfigurationGroup(
                 id = 56,
                 title = '',
                 configurations = [
-                    src.qase.api_client_v1.models.configuration.Configuration(
+                    qase.api_client_v1.models.configuration.Configuration(
                         id = 56, 
                         title = '', )
                     ]
             )
         else:
             return ConfigurationGroup(
         )
```

### Comparing `qase_api_client-1.0.0b1/test/test_configuration_group_create.py` & `qase_api_client-1.0.0b2/test/test_configuration_group_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
+from qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
 
 class TestConfigurationGroupCreate(unittest.TestCase):
     """ConfigurationGroupCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_configuration_list_response.py` & `qase_api_client-1.0.0b2/test/test_configuration_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
+from qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
 
 class TestConfigurationListResponse(unittest.TestCase):
     """ConfigurationListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,24 +33,24 @@
             optional params are included """
         # uncomment below to create an instance of `ConfigurationListResponse`
         """
         model = ConfigurationListResponse()
         if include_optional:
             return ConfigurationListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.configuration_list_response_all_of_result.ConfigurationListResponse_allOf_result(
+                result = qase.api_client_v1.models.configuration_list_response_all_of_result.ConfigurationListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.configuration_group.ConfigurationGroup(
+                        qase.api_client_v1.models.configuration_group.ConfigurationGroup(
                             id = 56, 
                             title = '', 
                             configurations = [
-                                src.qase.api_client_v1.models.configuration.Configuration(
+                                qase.api_client_v1.models.configuration.Configuration(
                                     id = 56, 
                                     title = '', )
                                 ], )
                         ], )
             )
         else:
             return ConfigurationListResponse(
```

### Comparing `qase_api_client-1.0.0b1/test/test_configuration_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_configuration_list_response_all_of_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
+from qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
 
 class TestConfigurationListResponseAllOfResult(unittest.TestCase):
     """ConfigurationListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,19 +36,19 @@
         model = ConfigurationListResponseAllOfResult()
         if include_optional:
             return ConfigurationListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.configuration_group.ConfigurationGroup(
+                    qase.api_client_v1.models.configuration_group.ConfigurationGroup(
                         id = 56, 
                         title = '', 
                         configurations = [
-                            src.qase.api_client_v1.models.configuration.Configuration(
+                            qase.api_client_v1.models.configuration.Configuration(
                                 id = 56, 
                                 title = '', )
                             ], )
                     ]
             )
         else:
             return ConfigurationListResponseAllOfResult(
```

### Comparing `qase_api_client-1.0.0b1/test/test_configurations_api.py` & `qase_api_client-1.0.0b2/test/test_configurations_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.configurations_api import ConfigurationsApi
+from qase.api_client_v1.api.configurations_api import ConfigurationsApi
 
 
 class TestConfigurationsApi(unittest.TestCase):
     """ConfigurationsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = ConfigurationsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field.py` & `qase_api_client-1.0.0b2/test/test_custom_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field import CustomField
+from qase.api_client_v1.models.custom_field import CustomField
 
 class TestCustomField(unittest.TestCase):
     """CustomField unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field_create.py` & `qase_api_client-1.0.0b2/test/test_custom_field_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field_create import CustomFieldCreate
+from qase.api_client_v1.models.custom_field_create import CustomFieldCreate
 
 class TestCustomFieldCreate(unittest.TestCase):
     """CustomFieldCreate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,15 +34,15 @@
         # uncomment below to create an instance of `CustomFieldCreate`
         """
         model = CustomFieldCreate()
         if include_optional:
             return CustomFieldCreate(
                 title = '',
                 value = [
-                    src.qase.api_client_v1.models.custom_field_create_value_inner.CustomFieldCreate_value_inner(
+                    qase.api_client_v1.models.custom_field_create_value_inner.CustomFieldCreate_value_inner(
                         id = 56, 
                         title = '', )
                     ],
                 entity = 0,
                 type = 0,
                 placeholder = '',
                 default_value = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field_create_value_inner.py` & `qase_api_client-1.0.0b2/test/test_custom_field_create_value_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
+from qase.api_client_v1.models.custom_field_create_value_inner import CustomFieldCreateValueInner
 
 class TestCustomFieldCreateValueInner(unittest.TestCase):
     """CustomFieldCreateValueInner unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field_list_response.py` & `qase_api_client-1.0.0b2/test/test_custom_field_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
+from qase.api_client_v1.models.custom_field_list_response import CustomFieldListResponse
 
 class TestCustomFieldListResponse(unittest.TestCase):
     """CustomFieldListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `CustomFieldListResponse`
         """
         model = CustomFieldListResponse()
         if include_optional:
             return CustomFieldListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.custom_fields_response_all_of_result.CustomFieldsResponse_allOf_result(
+                result = qase.api_client_v1.models.custom_fields_response_all_of_result.CustomFieldsResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.custom_field.CustomField(
+                        qase.api_client_v1.models.custom_field.CustomField(
                             id = 56, 
                             title = '', 
                             entity = '', 
                             type = '', 
                             placeholder = '', 
                             default_value = '', 
                             value = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field_response.py` & `qase_api_client-1.0.0b2/test/test_custom_field_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field_response import CustomFieldResponse
+from qase.api_client_v1.models.custom_field_response import CustomFieldResponse
 
 class TestCustomFieldResponse(unittest.TestCase):
     """CustomFieldResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `CustomFieldResponse`
         """
         model = CustomFieldResponse()
         if include_optional:
             return CustomFieldResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.custom_field.CustomField(
+                result = qase.api_client_v1.models.custom_field.CustomField(
                     id = 56, 
                     title = '', 
                     entity = '', 
                     type = '', 
                     placeholder = '', 
                     default_value = '', 
                     value = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field_update.py` & `qase_api_client-1.0.0b2/test/test_custom_field_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
+from qase.api_client_v1.models.custom_field_update import CustomFieldUpdate
 
 class TestCustomFieldUpdate(unittest.TestCase):
     """CustomFieldUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,15 +34,15 @@
         # uncomment below to create an instance of `CustomFieldUpdate`
         """
         model = CustomFieldUpdate()
         if include_optional:
             return CustomFieldUpdate(
                 title = '',
                 value = [
-                    src.qase.api_client_v1.models.custom_field_create_value_inner.CustomFieldCreate_value_inner(
+                    qase.api_client_v1.models.custom_field_create_value_inner.CustomFieldCreate_value_inner(
                         id = 56, 
                         title = '', )
                     ],
                 replace_values = {
                     'key' : ''
                     },
                 placeholder = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_field_value.py` & `qase_api_client-1.0.0b2/test/test_custom_field_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_field_value import CustomFieldValue
+from qase.api_client_v1.models.custom_field_value import CustomFieldValue
 
 class TestCustomFieldValue(unittest.TestCase):
     """CustomFieldValue unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_fields_api.py` & `qase_api_client-1.0.0b2/test/test_custom_fields_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.custom_fields_api import CustomFieldsApi
+from qase.api_client_v1.api.custom_fields_api import CustomFieldsApi
 
 
 class TestCustomFieldsApi(unittest.TestCase):
     """CustomFieldsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = CustomFieldsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_fields_response.py` & `qase_api_client-1.0.0b2/test/test_custom_fields_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_fields_response import CustomFieldsResponse
+from qase.api_client_v1.models.custom_fields_response import CustomFieldsResponse
 
 class TestCustomFieldsResponse(unittest.TestCase):
     """CustomFieldsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `CustomFieldsResponse`
         """
         model = CustomFieldsResponse()
         if include_optional:
             return CustomFieldsResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.custom_fields_response_all_of_result.CustomFieldsResponse_allOf_result(
+                result = qase.api_client_v1.models.custom_fields_response_all_of_result.CustomFieldsResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.custom_field.CustomField(
+                        qase.api_client_v1.models.custom_field.CustomField(
                             id = 56, 
                             title = '', 
                             entity = '', 
                             type = '', 
                             placeholder = '', 
                             default_value = '', 
                             value = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_custom_fields_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_custom_fields_response_all_of_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
+from qase.api_client_v1.models.custom_fields_response_all_of_result import CustomFieldsResponseAllOfResult
 
 class TestCustomFieldsResponseAllOfResult(unittest.TestCase):
     """CustomFieldsResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = CustomFieldsResponseAllOfResult()
         if include_optional:
             return CustomFieldsResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.custom_field.CustomField(
+                    qase.api_client_v1.models.custom_field.CustomField(
                         id = 56, 
                         title = '', 
                         entity = '', 
                         type = '', 
                         placeholder = '', 
                         default_value = '', 
                         value = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect.py` & `qase_api_client-1.0.0b2/test/test_defect.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect import Defect
+from qase.api_client_v1.models.defect import Defect
 
 class TestDefect(unittest.TestCase):
     """Defect unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -39,31 +39,31 @@
                 id = 56,
                 title = '',
                 actual_result = '',
                 severity = '',
                 status = '',
                 milestone_id = 56,
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 resolved_at = '2021-12-30T19:23:59Z',
                 member_id = 56,
                 author_id = 56,
                 external_data = '',
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z',
                 created = '2021-12-30 19:23:59',
                 updated = '2021-12-30 19:23:59'
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_create.py` & `qase_api_client-1.0.0b2/test/test_defect_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_create import DefectCreate
+from qase.api_client_v1.models.defect_create import DefectCreate
 
 class TestDefectCreate(unittest.TestCase):
     """DefectCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_list_response.py` & `qase_api_client-1.0.0b2/test/test_defect_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,80 +11,74 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_list_response import DefectListResponse
+from qase.api_client_v1.models.defect_response import DefectResponse
 
-class TestDefectListResponse(unittest.TestCase):
-    """DefectListResponse unit test stubs"""
+class TestDefectResponse(unittest.TestCase):
+    """DefectResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> DefectListResponse:
-        """Test DefectListResponse
+    def make_instance(self, include_optional) -> DefectResponse:
+        """Test DefectResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `DefectListResponse`
+        # uncomment below to create an instance of `DefectResponse`
         """
-        model = DefectListResponse()
+        model = DefectResponse()
         if include_optional:
-            return DefectListResponse(
+            return DefectResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.defect_list_response_all_of_result.DefectListResponse_allOf_result(
-                    total = 56, 
-                    filtered = 56, 
-                    count = 56, 
-                    entities = [
-                        src.qase.api_client_v1.models.defect.Defect(
+                result = qase.api_client_v1.models.defect.Defect(
+                    id = 56, 
+                    title = '', 
+                    actual_result = '', 
+                    severity = '', 
+                    status = '', 
+                    milestone_id = 56, 
+                    custom_fields = [
+                        qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                             id = 56, 
+                            value = '', )
+                        ], 
+                    attachments = [
+                        qase.api_client_v1.models.attachment.Attachment(
+                            size = 56, 
+                            mime = '', 
+                            filename = '', 
+                            url = '', )
+                        ], 
+                    resolved_at = '2021-12-30T19:23:59Z', 
+                    member_id = 56, 
+                    author_id = 56, 
+                    external_data = '', 
+                    tags = [
+                        qase.api_client_v1.models.tag_value.TagValue(
                             title = '', 
-                            actual_result = '', 
-                            severity = '', 
-                            status = '', 
-                            milestone_id = 56, 
-                            custom_fields = [
-                                src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
-                                    id = 56, 
-                                    value = '', )
-                                ], 
-                            attachments = [
-                                src.qase.api_client_v1.models.attachment.Attachment(
-                                    size = 56, 
-                                    mime = '', 
-                                    filename = '', 
-                                    url = '', )
-                                ], 
-                            resolved_at = '2021-12-30T19:23:59Z', 
-                            member_id = 56, 
-                            author_id = 56, 
-                            external_data = '', 
-                            tags = [
-                                src.qase.api_client_v1.models.tag_value.TagValue(
-                                    title = '', 
-                                    internal_id = 56, )
-                                ], 
-                            created_at = '2021-12-30T19:23:59Z', 
-                            updated_at = '2021-12-30T19:23:59Z', 
-                            created = '2021-12-30 19:23:59', 
-                            updated = '2021-12-30 19:23:59', )
-                        ], )
+                            internal_id = 56, )
+                        ], 
+                    created_at = '2021-12-30T19:23:59Z', 
+                    updated_at = '2021-12-30T19:23:59Z', 
+                    created = '2021-12-30 19:23:59', 
+                    updated = '2021-12-30 19:23:59', )
             )
         else:
-            return DefectListResponse(
+            return DefectResponse(
         )
         """
 
-    def testDefectListResponse(self):
-        """Test DefectListResponse"""
+    def testDefectResponse(self):
+        """Test DefectResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_defect_list_response_all_of_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
+from qase.api_client_v1.models.defect_list_response_all_of_result import DefectListResponseAllOfResult
 
 class TestDefectListResponseAllOfResult(unittest.TestCase):
     """DefectListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,39 +36,39 @@
         model = DefectListResponseAllOfResult()
         if include_optional:
             return DefectListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.defect.Defect(
+                    qase.api_client_v1.models.defect.Defect(
                         id = 56, 
                         title = '', 
                         actual_result = '', 
                         severity = '', 
                         status = '', 
                         milestone_id = 56, 
                         custom_fields = [
-                            src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                            qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                                 id = 56, 
                                 value = '', )
                             ], 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
+                            qase.api_client_v1.models.attachment.Attachment(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', )
                             ], 
                         resolved_at = '2021-12-30T19:23:59Z', 
                         member_id = 56, 
                         author_id = 56, 
                         external_data = '', 
                         tags = [
-                            src.qase.api_client_v1.models.tag_value.TagValue(
+                            qase.api_client_v1.models.tag_value.TagValue(
                                 title = '', 
                                 internal_id = 56, )
                             ], 
                         created_at = '2021-12-30T19:23:59Z', 
                         updated_at = '2021-12-30T19:23:59Z', 
                         created = '2021-12-30 19:23:59', 
                         updated = '2021-12-30 19:23:59', )
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_query.py` & `qase_api_client-1.0.0b2/test/test_defect_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_query import DefectQuery
+from qase.api_client_v1.models.defect_query import DefectQuery
 
 class TestDefectQuery(unittest.TestCase):
     """DefectQuery unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -39,31 +39,31 @@
                 id = 56,
                 title = '',
                 actual_result = '',
                 severity = '',
                 status = '',
                 milestone_id = 56,
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 resolved = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 member_id = 56,
                 author_id = 56,
                 external_data = '',
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z'
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_response.py` & `qase_api_client-1.0.0b2/test/test_defect_list_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,74 +11,80 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_response import DefectResponse
+from qase.api_client_v1.models.defect_list_response import DefectListResponse
 
-class TestDefectResponse(unittest.TestCase):
-    """DefectResponse unit test stubs"""
+class TestDefectListResponse(unittest.TestCase):
+    """DefectListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> DefectResponse:
-        """Test DefectResponse
+    def make_instance(self, include_optional) -> DefectListResponse:
+        """Test DefectListResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `DefectResponse`
+        # uncomment below to create an instance of `DefectListResponse`
         """
-        model = DefectResponse()
+        model = DefectListResponse()
         if include_optional:
-            return DefectResponse(
+            return DefectListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.defect.Defect(
-                    id = 56, 
-                    title = '', 
-                    actual_result = '', 
-                    severity = '', 
-                    status = '', 
-                    milestone_id = 56, 
-                    custom_fields = [
-                        src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                result = qase.api_client_v1.models.defect_list_response_all_of_result.DefectListResponse_allOf_result(
+                    total = 56, 
+                    filtered = 56, 
+                    count = 56, 
+                    entities = [
+                        qase.api_client_v1.models.defect.Defect(
                             id = 56, 
-                            value = '', )
-                        ], 
-                    attachments = [
-                        src.qase.api_client_v1.models.attachment.Attachment(
-                            size = 56, 
-                            mime = '', 
-                            filename = '', 
-                            url = '', )
-                        ], 
-                    resolved_at = '2021-12-30T19:23:59Z', 
-                    member_id = 56, 
-                    author_id = 56, 
-                    external_data = '', 
-                    tags = [
-                        src.qase.api_client_v1.models.tag_value.TagValue(
                             title = '', 
-                            internal_id = 56, )
-                        ], 
-                    created_at = '2021-12-30T19:23:59Z', 
-                    updated_at = '2021-12-30T19:23:59Z', 
-                    created = '2021-12-30 19:23:59', 
-                    updated = '2021-12-30 19:23:59', )
+                            actual_result = '', 
+                            severity = '', 
+                            status = '', 
+                            milestone_id = 56, 
+                            custom_fields = [
+                                qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                                    id = 56, 
+                                    value = '', )
+                                ], 
+                            attachments = [
+                                qase.api_client_v1.models.attachment.Attachment(
+                                    size = 56, 
+                                    mime = '', 
+                                    filename = '', 
+                                    url = '', )
+                                ], 
+                            resolved_at = '2021-12-30T19:23:59Z', 
+                            member_id = 56, 
+                            author_id = 56, 
+                            external_data = '', 
+                            tags = [
+                                qase.api_client_v1.models.tag_value.TagValue(
+                                    title = '', 
+                                    internal_id = 56, )
+                                ], 
+                            created_at = '2021-12-30T19:23:59Z', 
+                            updated_at = '2021-12-30T19:23:59Z', 
+                            created = '2021-12-30 19:23:59', 
+                            updated = '2021-12-30 19:23:59', )
+                        ], )
             )
         else:
-            return DefectResponse(
+            return DefectListResponse(
         )
         """
 
-    def testDefectResponse(self):
-        """Test DefectResponse"""
+    def testDefectListResponse(self):
+        """Test DefectListResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_status.py` & `qase_api_client-1.0.0b2/test/test_defect_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_status import DefectStatus
+from qase.api_client_v1.models.defect_status import DefectStatus
 
 class TestDefectStatus(unittest.TestCase):
     """DefectStatus unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_defect_update.py` & `qase_api_client-1.0.0b2/test/test_defect_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.defect_update import DefectUpdate
+from qase.api_client_v1.models.defect_update import DefectUpdate
 
 class TestDefectUpdate(unittest.TestCase):
     """DefectUpdate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_defects_api.py` & `qase_api_client-1.0.0b2/test/test_defects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.defects_api import DefectsApi
+from qase.api_client_v1.api.defects_api import DefectsApi
 
 
 class TestDefectsApi(unittest.TestCase):
     """DefectsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = DefectsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_environment.py` & `qase_api_client-1.0.0b2/test/test_environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.environment import Environment
+from qase.api_client_v1.models.environment import Environment
 
 class TestEnvironment(unittest.TestCase):
     """Environment unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_environment_create.py` & `qase_api_client-1.0.0b2/test/test_environment_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.environment_create import EnvironmentCreate
+from qase.api_client_v1.models.environment_create import EnvironmentCreate
 
 class TestEnvironmentCreate(unittest.TestCase):
     """EnvironmentCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_environment_list_response.py` & `qase_api_client-1.0.0b2/test/test_environment_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
+from qase.api_client_v1.models.environment_list_response import EnvironmentListResponse
 
 class TestEnvironmentListResponse(unittest.TestCase):
     """EnvironmentListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `EnvironmentListResponse`
         """
         model = EnvironmentListResponse()
         if include_optional:
             return EnvironmentListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.environment_list_response_all_of_result.EnvironmentListResponse_allOf_result(
+                result = qase.api_client_v1.models.environment_list_response_all_of_result.EnvironmentListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.environment.Environment(
+                        qase.api_client_v1.models.environment.Environment(
                             id = 56, 
                             title = '', 
                             description = '', 
                             slug = '', 
                             host = '', )
                         ], )
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_environment_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_environment_list_response_all_of_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
+from qase.api_client_v1.models.environment_list_response_all_of_result import EnvironmentListResponseAllOfResult
 
 class TestEnvironmentListResponseAllOfResult(unittest.TestCase):
     """EnvironmentListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = EnvironmentListResponseAllOfResult()
         if include_optional:
             return EnvironmentListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.environment.Environment(
+                    qase.api_client_v1.models.environment.Environment(
                         id = 56, 
                         title = '', 
                         description = '', 
                         slug = '', 
                         host = '', )
                     ]
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_environment_response.py` & `qase_api_client-1.0.0b2/test/test_environment_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.environment_response import EnvironmentResponse
+from qase.api_client_v1.models.environment_response import EnvironmentResponse
 
 class TestEnvironmentResponse(unittest.TestCase):
     """EnvironmentResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `EnvironmentResponse`
         """
         model = EnvironmentResponse()
         if include_optional:
             return EnvironmentResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.environment.Environment(
+                result = qase.api_client_v1.models.environment.Environment(
                     id = 56, 
                     title = '', 
                     description = '', 
                     slug = '', 
                     host = '', )
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_environment_update.py` & `qase_api_client-1.0.0b2/test/test_environment_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.environment_update import EnvironmentUpdate
+from qase.api_client_v1.models.environment_update import EnvironmentUpdate
 
 class TestEnvironmentUpdate(unittest.TestCase):
     """EnvironmentUpdate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_environments_api.py` & `qase_api_client-1.0.0b2/test/test_environments_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.environments_api import EnvironmentsApi
+from qase.api_client_v1.api.environments_api import EnvironmentsApi
 
 
 class TestEnvironmentsApi(unittest.TestCase):
     """EnvironmentsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = EnvironmentsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_external_issue.py` & `qase_api_client-1.0.0b2/test/test_external_issue.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.external_issue import ExternalIssue
+from qase.api_client_v1.models.external_issue import ExternalIssue
 
 class TestExternalIssue(unittest.TestCase):
     """ExternalIssue unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,15 +34,15 @@
         # uncomment below to create an instance of `ExternalIssue`
         """
         model = ExternalIssue()
         if include_optional:
             return ExternalIssue(
                 type = '',
                 issues = [
-                    src.qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
+                    qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
                         id = '', 
                         link = '', )
                     ]
             )
         else:
             return ExternalIssue(
         )
```

### Comparing `qase_api_client-1.0.0b1/test/test_external_issue_issues_inner.py` & `qase_api_client-1.0.0b2/test/test_external_issue_issues_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
+from qase.api_client_v1.models.external_issue_issues_inner import ExternalIssueIssuesInner
 
 class TestExternalIssueIssuesInner(unittest.TestCase):
     """ExternalIssueIssuesInner unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_hash_response.py` & `qase_api_client-1.0.0b2/test/test_hash_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.hash_response import HashResponse
+from qase.api_client_v1.models.hash_response import HashResponse
 
 class TestHashResponse(unittest.TestCase):
     """HashResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `HashResponse`
         """
         model = HashResponse()
         if include_optional:
             return HashResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.hash_response_all_of_result.HashResponse_allOf_result(
+                result = qase.api_client_v1.models.hash_response_all_of_result.HashResponse_allOf_result(
                     hash = '', )
             )
         else:
             return HashResponse(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_hash_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_hash_response_all_of_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
+from qase.api_client_v1.models.hash_response_all_of_result import HashResponseAllOfResult
 
 class TestHashResponseAllOfResult(unittest.TestCase):
     """HashResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_id_response.py` & `qase_api_client-1.0.0b2/test/test_id_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.id_response import IdResponse
+from qase.api_client_v1.models.id_response import IdResponse
 
 class TestIdResponse(unittest.TestCase):
     """IdResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `IdResponse`
         """
         model = IdResponse()
         if include_optional:
             return IdResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.id_response_all_of_result.IdResponse_allOf_result(
+                result = qase.api_client_v1.models.id_response_all_of_result.IdResponse_allOf_result(
                     id = 56, )
             )
         else:
             return IdResponse(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_id_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_id_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
+from qase.api_client_v1.models.id_response_all_of_result import IdResponseAllOfResult
 
 class TestIdResponseAllOfResult(unittest.TestCase):
     """IdResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestone.py` & `qase_api_client-1.0.0b2/test/test_milestone.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.milestone import Milestone
+from qase.api_client_v1.models.milestone import Milestone
 
 class TestMilestone(unittest.TestCase):
     """Milestone unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestone_create.py` & `qase_api_client-1.0.0b2/test/test_milestone_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.milestone_create import MilestoneCreate
+from qase.api_client_v1.models.milestone_create import MilestoneCreate
 
 class TestMilestoneCreate(unittest.TestCase):
     """MilestoneCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestone_list_response.py` & `qase_api_client-1.0.0b2/test/test_milestone_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
+from qase.api_client_v1.models.milestone_list_response import MilestoneListResponse
 
 class TestMilestoneListResponse(unittest.TestCase):
     """MilestoneListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `MilestoneListResponse`
         """
         model = MilestoneListResponse()
         if include_optional:
             return MilestoneListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.milestone_list_response_all_of_result.MilestoneListResponse_allOf_result(
+                result = qase.api_client_v1.models.milestone_list_response_all_of_result.MilestoneListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.milestone.Milestone(
+                        qase.api_client_v1.models.milestone.Milestone(
                             id = 56, 
                             title = '', 
                             description = '', 
                             status = 'completed', 
                             due_date = '2021-12-30T19:23:59Z', 
                             created = '2021-12-30 19:23:59', 
                             updated = '2021-12-30 19:23:59',
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestone_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_milestone_list_response_all_of_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
+from qase.api_client_v1.models.milestone_list_response_all_of_result import MilestoneListResponseAllOfResult
 
 class TestMilestoneListResponseAllOfResult(unittest.TestCase):
     """MilestoneListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = MilestoneListResponseAllOfResult()
         if include_optional:
             return MilestoneListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.milestone.Milestone(
+                    qase.api_client_v1.models.milestone.Milestone(
                         id = 56, 
                         title = '', 
                         description = '', 
                         status = 'completed', 
                         due_date = '2021-12-30T19:23:59Z', 
                         created = '2021-12-30 19:23:59', 
                         updated = '2021-12-30 19:23:59',
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestone_response.py` & `qase_api_client-1.0.0b2/test/test_milestone_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.milestone_response import MilestoneResponse
+from qase.api_client_v1.models.milestone_response import MilestoneResponse
 
 class TestMilestoneResponse(unittest.TestCase):
     """MilestoneResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `MilestoneResponse`
         """
         model = MilestoneResponse()
         if include_optional:
             return MilestoneResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.milestone.Milestone(
+                result = qase.api_client_v1.models.milestone.Milestone(
                     id = 56, 
                     title = '', 
                     description = '', 
                     status = 'completed', 
                     due_date = '2021-12-30T19:23:59Z', 
                     created = '2021-12-30 19:23:59', 
                     updated = '2021-12-30 19:23:59',
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestone_update.py` & `qase_api_client-1.0.0b2/test/test_milestone_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.milestone_update import MilestoneUpdate
+from qase.api_client_v1.models.milestone_update import MilestoneUpdate
 
 class TestMilestoneUpdate(unittest.TestCase):
     """MilestoneUpdate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_milestones_api.py` & `qase_api_client-1.0.0b2/test/test_milestones_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.milestones_api import MilestonesApi
+from qase.api_client_v1.api.milestones_api import MilestonesApi
 
 
 class TestMilestonesApi(unittest.TestCase):
     """MilestonesApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = MilestonesApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan.py` & `qase_api_client-1.0.0b2/test/test_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan import Plan
+from qase.api_client_v1.models.plan import Plan
 
 class TestPlan(unittest.TestCase):
     """Plan unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_create.py` & `qase_api_client-1.0.0b2/test/test_plan_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_create import PlanCreate
+from qase.api_client_v1.models.plan_create import PlanCreate
 
 class TestPlanCreate(unittest.TestCase):
     """PlanCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_detailed.py` & `qase_api_client-1.0.0b2/test/test_plan_detailed.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_detailed import PlanDetailed
+from qase.api_client_v1.models.plan_detailed import PlanDetailed
 
 class TestPlanDetailed(unittest.TestCase):
     """PlanDetailed unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -42,15 +42,15 @@
                 cases_count = 56,
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z',
                 created = '2021-12-30 19:23:59',
                 updated = '2021-12-30 19:23:59',
                 average_time = 1.337,
                 cases = [
-                    src.qase.api_client_v1.models.plan_detailed_all_of_cases.PlanDetailed_allOf_cases(
+                    qase.api_client_v1.models.plan_detailed_all_of_cases.PlanDetailed_allOf_cases(
                         case_id = 56, 
                         assignee_id = 56, )
                     ]
             )
         else:
             return PlanDetailed(
         )
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_detailed_all_of_cases.py` & `qase_api_client-1.0.0b2/test/test_plan_detailed_all_of_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
+from qase.api_client_v1.models.plan_detailed_all_of_cases import PlanDetailedAllOfCases
 
 class TestPlanDetailedAllOfCases(unittest.TestCase):
     """PlanDetailedAllOfCases unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_list_response.py` & `qase_api_client-1.0.0b2/test/test_plan_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_list_response import PlanListResponse
+from qase.api_client_v1.models.plan_list_response import PlanListResponse
 
 class TestPlanListResponse(unittest.TestCase):
     """PlanListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `PlanListResponse`
         """
         model = PlanListResponse()
         if include_optional:
             return PlanListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.plan_list_response_all_of_result.PlanListResponse_allOf_result(
+                result = qase.api_client_v1.models.plan_list_response_all_of_result.PlanListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.plan.Plan(
+                        qase.api_client_v1.models.plan.Plan(
                             id = 56, 
                             title = '', 
                             description = '', 
                             cases_count = 56, 
                             created_at = '2021-12-30T19:23:59Z', 
                             updated_at = '2021-12-30T19:23:59Z', 
                             created = '2021-12-30 19:23:59',
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_plan_list_response_all_of_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
+from qase.api_client_v1.models.plan_list_response_all_of_result import PlanListResponseAllOfResult
 
 class TestPlanListResponseAllOfResult(unittest.TestCase):
     """PlanListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = PlanListResponseAllOfResult()
         if include_optional:
             return PlanListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.plan.Plan(
+                    qase.api_client_v1.models.plan.Plan(
                         id = 56, 
                         title = '', 
                         description = '', 
                         cases_count = 56, 
                         created_at = '2021-12-30T19:23:59Z', 
                         updated_at = '2021-12-30T19:23:59Z', 
                         created = '2021-12-30 19:23:59',
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_query.py` & `qase_api_client-1.0.0b2/test/test_plan_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_query import PlanQuery
+from qase.api_client_v1.models.plan_query import PlanQuery
 
 class TestPlanQuery(unittest.TestCase):
     """PlanQuery unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_response.py` & `qase_api_client-1.0.0b2/test/test_plan_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_response import PlanResponse
+from qase.api_client_v1.models.plan_response import PlanResponse
 
 class TestPlanResponse(unittest.TestCase):
     """PlanResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_plan_update.py` & `qase_api_client-1.0.0b2/test/test_plan_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.plan_update import PlanUpdate
+from qase.api_client_v1.models.plan_update import PlanUpdate
 
 class TestPlanUpdate(unittest.TestCase):
     """PlanUpdate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_plans_api.py` & `qase_api_client-1.0.0b2/test/test_plans_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.plans_api import PlansApi
+from qase.api_client_v1.api.plans_api import PlansApi
 
 
 class TestPlansApi(unittest.TestCase):
     """PlansApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = PlansApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_project.py` & `qase_api_client-1.0.0b2/test/test_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project import Project
+from qase.api_client_v1.models.project import Project
 
 class TestProject(unittest.TestCase):
     """Project unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,22 +34,22 @@
         # uncomment below to create an instance of `Project`
         """
         model = Project()
         if include_optional:
             return Project(
                 title = '',
                 code = '',
-                counts = src.qase.api_client_v1.models.project_counts.Project_counts(
+                counts = qase.api_client_v1.models.project_counts.Project_counts(
                     cases = 56, 
                     suites = 56, 
                     milestones = 56, 
-                    runs = src.qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
+                    runs = qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
                         total = 56, 
                         active = 56, ), 
-                    defects = src.qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
+                    defects = qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
                         total = 56, 
                         open = 56, ), )
             )
         else:
             return Project(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_access.py` & `qase_api_client-1.0.0b2/test/test_project_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_access import ProjectAccess
+from qase.api_client_v1.models.project_access import ProjectAccess
 
 class TestProjectAccess(unittest.TestCase):
     """ProjectAccess unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_code_response.py` & `qase_api_client-1.0.0b2/test/test_project_code_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_code_response import ProjectCodeResponse
+from qase.api_client_v1.models.project_code_response import ProjectCodeResponse
 
 class TestProjectCodeResponse(unittest.TestCase):
     """ProjectCodeResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `ProjectCodeResponse`
         """
         model = ProjectCodeResponse()
         if include_optional:
             return ProjectCodeResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.project_code_response_all_of_result.ProjectCodeResponse_allOf_result(
+                result = qase.api_client_v1.models.project_code_response_all_of_result.ProjectCodeResponse_allOf_result(
                     code = '', )
             )
         else:
             return ProjectCodeResponse(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_code_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_project_code_response_all_of_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
+from qase.api_client_v1.models.project_code_response_all_of_result import ProjectCodeResponseAllOfResult
 
 class TestProjectCodeResponseAllOfResult(unittest.TestCase):
     """ProjectCodeResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_counts.py` & `qase_api_client-1.0.0b2/test/test_project_counts.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_counts import ProjectCounts
+from qase.api_client_v1.models.project_counts import ProjectCounts
 
 class TestProjectCounts(unittest.TestCase):
     """ProjectCounts unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -35,18 +35,18 @@
         """
         model = ProjectCounts()
         if include_optional:
             return ProjectCounts(
                 cases = 56,
                 suites = 56,
                 milestones = 56,
-                runs = src.qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
+                runs = qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
                     total = 56, 
                     active = 56, ),
-                defects = src.qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
+                defects = qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
                     total = 56, 
                     open = 56, )
             )
         else:
             return ProjectCounts(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_counts_defects.py` & `qase_api_client-1.0.0b2/test/test_project_counts_defects.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
+from qase.api_client_v1.models.project_counts_defects import ProjectCountsDefects
 
 class TestProjectCountsDefects(unittest.TestCase):
     """ProjectCountsDefects unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_counts_runs.py` & `qase_api_client-1.0.0b2/test/test_project_counts_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
+from qase.api_client_v1.models.project_counts_runs import ProjectCountsRuns
 
 class TestProjectCountsRuns(unittest.TestCase):
     """ProjectCountsRuns unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_create.py` & `qase_api_client-1.0.0b2/test/test_project_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_create import ProjectCreate
+from qase.api_client_v1.models.project_create import ProjectCreate
 
 class TestProjectCreate(unittest.TestCase):
     """ProjectCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_list_response.py` & `qase_api_client-1.0.0b2/test/test_project_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_list_response import ProjectListResponse
+from qase.api_client_v1.models.project_list_response import ProjectListResponse
 
 class TestProjectListResponse(unittest.TestCase):
     """ProjectListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,30 +33,30 @@
             optional params are included """
         # uncomment below to create an instance of `ProjectListResponse`
         """
         model = ProjectListResponse()
         if include_optional:
             return ProjectListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.project_list_response_all_of_result.ProjectListResponse_allOf_result(
+                result = qase.api_client_v1.models.project_list_response_all_of_result.ProjectListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.project.Project(
+                        qase.api_client_v1.models.project.Project(
                             title = '', 
                             code = '', 
-                            counts = src.qase.api_client_v1.models.project_counts.Project_counts(
+                            counts = qase.api_client_v1.models.project_counts.Project_counts(
                                 cases = 56, 
                                 suites = 56, 
                                 milestones = 56, 
-                                runs = src.qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
+                                runs = qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
                                     total = 56, 
                                     active = 56, ), 
-                                defects = src.qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
+                                defects = qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
                                     total = 56, 
                                     open = 56, ), ), )
                         ], )
             )
         else:
             return ProjectListResponse(
         )
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_project_list_response_all_of_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
+from qase.api_client_v1.models.project_list_response_all_of_result import ProjectListResponseAllOfResult
 
 class TestProjectListResponseAllOfResult(unittest.TestCase):
     """ProjectListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,25 +36,25 @@
         model = ProjectListResponseAllOfResult()
         if include_optional:
             return ProjectListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.project.Project(
+                    qase.api_client_v1.models.project.Project(
                         title = '', 
                         code = '', 
-                        counts = src.qase.api_client_v1.models.project_counts.Project_counts(
+                        counts = qase.api_client_v1.models.project_counts.Project_counts(
                             cases = 56, 
                             suites = 56, 
                             milestones = 56, 
-                            runs = src.qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
+                            runs = qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
                                 total = 56, 
                                 active = 56, ), 
-                            defects = src.qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
+                            defects = qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
                                 total = 56, 
                                 open = 56, ), ), )
                     ]
             )
         else:
             return ProjectListResponseAllOfResult(
         )
```

### Comparing `qase_api_client-1.0.0b1/test/test_project_response.py` & `qase_api_client-1.0.0b2/test/test_project_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.project_response import ProjectResponse
+from qase.api_client_v1.models.project_response import ProjectResponse
 
 class TestProjectResponse(unittest.TestCase):
     """ProjectResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,25 +33,25 @@
             optional params are included """
         # uncomment below to create an instance of `ProjectResponse`
         """
         model = ProjectResponse()
         if include_optional:
             return ProjectResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.project.Project(
+                result = qase.api_client_v1.models.project.Project(
                     title = '', 
                     code = '', 
-                    counts = src.qase.api_client_v1.models.project_counts.Project_counts(
+                    counts = qase.api_client_v1.models.project_counts.Project_counts(
                         cases = 56, 
                         suites = 56, 
                         milestones = 56, 
-                        runs = src.qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
+                        runs = qase.api_client_v1.models.project_counts_runs.Project_counts_runs(
                             total = 56, 
                             active = 56, ), 
-                        defects = src.qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
+                        defects = qase.api_client_v1.models.project_counts_defects.Project_counts_defects(
                             total = 56, 
                             open = 56, ), ), )
             )
         else:
             return ProjectResponse(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_projects_api.py` & `qase_api_client-1.0.0b2/test/test_projects_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.projects_api import ProjectsApi
+from qase.api_client_v1.api.projects_api import ProjectsApi
 
 
 class TestProjectsApi(unittest.TestCase):
     """ProjectsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = ProjectsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_qql_defect.py` & `qase_api_client-1.0.0b2/test/test_qql_defect.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.qql_defect import QqlDefect
+from qase.api_client_v1.models.qql_defect import QqlDefect
 
 class TestQqlDefect(unittest.TestCase):
     """QqlDefect unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -39,31 +39,31 @@
                 id = 56,
                 title = '',
                 actual_result = '',
                 severity = '',
                 status = '',
                 milestone_id = 56,
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 resolved = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 member_id = 56,
                 author_id = 56,
                 external_data = '',
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z'
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_qql_plan.py` & `qase_api_client-1.0.0b2/test/test_qql_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.qql_plan import QqlPlan
+from qase.api_client_v1.models.qql_plan import QqlPlan
 
 class TestQqlPlan(unittest.TestCase):
     """QqlPlan unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_qql_test_case.py` & `qase_api_client-1.0.0b2/test/test_qql_test_case.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.qql_test_case import QqlTestCase
+from qase.api_client_v1.models.qql_test_case import QqlTestCase
 
 class TestQqlTestCase(unittest.TestCase):
     """QqlTestCase unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -49,49 +49,49 @@
                 is_flaky = 56,
                 behavior = 56,
                 automation = 56,
                 status = 56,
                 milestone_id = 56,
                 suite_id = 56,
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 steps_type = '',
                 steps = [
-                    src.qase.api_client_v1.models.test_step.TestStep(
+                    qase.api_client_v1.models.test_step.TestStep(
                         hash = '', 
                         shared_step_hash = '', 
                         shared_step_nested_hash = '', 
                         position = 56, 
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
+                            qase.api_client_v1.models.attachment.Attachment(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', )
                             ], 
                         steps = [
                             None
                             ], )
                     ],
                 params = None,
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 member_id = 56,
                 author_id = 56,
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z'
```

### Comparing `qase_api_client-1.0.0b1/test/test_requirement.py` & `qase_api_client-1.0.0b2/test/test_requirement.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.requirement import Requirement
+from qase.api_client_v1.models.requirement import Requirement
 
 class TestRequirement(unittest.TestCase):
     """Requirement unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_response.py` & `qase_api_client-1.0.0b2/test/test_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.response import Response
+from qase.api_client_v1.models.response import Response
 
 class TestResponse(unittest.TestCase):
     """Response unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_result.py` & `qase_api_client-1.0.0b2/test/test_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result import Result
+from qase.api_client_v1.models.result import Result
 
 class TestResult(unittest.TestCase):
     """Result unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -38,34 +38,34 @@
             return Result(
                 hash = '',
                 comment = '',
                 stacktrace = '',
                 run_id = 56,
                 case_id = 56,
                 steps = [
-                    src.qase.api_client_v1.models.test_step_result.TestStepResult(
+                    qase.api_client_v1.models.test_step_result.TestStepResult(
                         status = 56, 
                         position = 56, 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
+                            qase.api_client_v1.models.attachment.Attachment(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', )
                             ], 
                         steps = [
                             None
                             ], )
                     ],
                 status = '',
                 is_api_result = True,
                 time_spent_ms = 56,
                 end_time = '2021-12-30T19:23:59Z',
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ]
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_create.py` & `qase_api_client-1.0.0b2/test/test_result_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_create import ResultCreate
+from qase.api_client_v1.models.result_create import ResultCreate
 
 class TestResultCreate(unittest.TestCase):
     """ResultCreate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `ResultCreate`
         """
         model = ResultCreate()
         if include_optional:
             return ResultCreate(
                 case_id = 56,
-                case = src.qase.api_client_v1.models.result_create_case.ResultCreate_case(
+                case = qase.api_client_v1.models.result_create_case.ResultCreate_case(
                     title = '', 
                     suite_title = '', 
                     description = '', 
                     preconditions = '', 
                     postconditions = '', 
                     layer = '', 
                     severity = '', 
@@ -56,15 +56,15 @@
                     ],
                 stacktrace = '',
                 comment = '',
                 param = {
                     'key' : ''
                     },
                 steps = [
-                    src.qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
+                    qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
                         position = 56, 
                         status = 'passed', 
                         comment = '', 
                         attachments = [
                             ''
                             ], 
                         action = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_create_bulk.py` & `qase_api_client-1.0.0b2/test/test_result_create_bulk.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_create_bulk import ResultCreateBulk
+from qase.api_client_v1.models.result_create_bulk import ResultCreateBulk
 
 class TestResultCreateBulk(unittest.TestCase):
     """ResultCreateBulk unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,17 +33,17 @@
             optional params are included """
         # uncomment below to create an instance of `ResultCreateBulk`
         """
         model = ResultCreateBulk()
         if include_optional:
             return ResultCreateBulk(
                 results = [
-                    src.qase.api_client_v1.models.result_create.ResultCreate(
+                    qase.api_client_v1.models.result_create.ResultCreate(
                         case_id = 56, 
-                        case = src.qase.api_client_v1.models.result_create_case.ResultCreate_case(
+                        case = qase.api_client_v1.models.result_create_case.ResultCreate_case(
                             title = '', 
                             suite_title = '', 
                             description = '', 
                             preconditions = '', 
                             postconditions = '', 
                             layer = '', 
                             severity = '', 
@@ -58,31 +58,31 @@
                             ], 
                         stacktrace = '', 
                         comment = '', 
                         param = {
                             'key' : ''
                             }, 
                         steps = [
-                            src.qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
+                            qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
                                 position = 56, 
                                 status = 'passed', 
                                 comment = '', 
                                 action = '', 
                                 expected_result = '', 
                                 data = '', )
                             ], 
                         author_id = 56, )
                     ]
             )
         else:
             return ResultCreateBulk(
                 results = [
-                    src.qase.api_client_v1.models.result_create.ResultCreate(
+                    qase.api_client_v1.models.result_create.ResultCreate(
                         case_id = 56, 
-                        case = src.qase.api_client_v1.models.result_create_case.ResultCreate_case(
+                        case = qase.api_client_v1.models.result_create_case.ResultCreate_case(
                             title = '', 
                             suite_title = '', 
                             description = '', 
                             preconditions = '', 
                             postconditions = '', 
                             layer = '', 
                             severity = '', 
@@ -97,15 +97,15 @@
                             ], 
                         stacktrace = '', 
                         comment = '', 
                         param = {
                             'key' : ''
                             }, 
                         steps = [
-                            src.qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
+                            qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
                                 position = 56, 
                                 status = 'passed', 
                                 comment = '', 
                                 action = '', 
                                 expected_result = '', 
                                 data = '', )
                             ],
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_create_case.py` & `qase_api_client-1.0.0b2/test/test_result_create_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_create_case import ResultCreateCase
+from qase.api_client_v1.models.result_create_case import ResultCreateCase
 
 class TestResultCreateCase(unittest.TestCase):
     """ResultCreateCase unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_create_response.py` & `qase_api_client-1.0.0b2/test/test_result_create_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_create_response import ResultCreateResponse
+from qase.api_client_v1.models.result_create_response import ResultCreateResponse
 
 class TestResultCreateResponse(unittest.TestCase):
     """ResultCreateResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `ResultCreateResponse`
         """
         model = ResultCreateResponse()
         if include_optional:
             return ResultCreateResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.result_create_response_all_of_result.ResultCreateResponse_allOf_result(
+                result = qase.api_client_v1.models.result_create_response_all_of_result.ResultCreateResponse_allOf_result(
                     case_id = 56, 
                     hash = '', )
             )
         else:
             return ResultCreateResponse(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_create_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_result_create_response_all_of_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
+from qase.api_client_v1.models.result_create_response_all_of_result import ResultCreateResponseAllOfResult
 
 class TestResultCreateResponseAllOfResult(unittest.TestCase):
     """ResultCreateResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_list_response.py` & `qase_api_client-1.0.0b2/test/test_result_list_response_all_of_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,77 +11,75 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_list_response import ResultListResponse
+from qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
 
-class TestResultListResponse(unittest.TestCase):
-    """ResultListResponse unit test stubs"""
+class TestResultListResponseAllOfResult(unittest.TestCase):
+    """ResultListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ResultListResponse:
-        """Test ResultListResponse
+    def make_instance(self, include_optional) -> ResultListResponseAllOfResult:
+        """Test ResultListResponseAllOfResult
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ResultListResponse`
+        # uncomment below to create an instance of `ResultListResponseAllOfResult`
         """
-        model = ResultListResponse()
+        model = ResultListResponseAllOfResult()
         if include_optional:
-            return ResultListResponse(
-                status = True,
-                result = src.qase.api_client_v1.models.result_list_response_all_of_result.ResultListResponse_allOf_result(
-                    total = 56, 
-                    filtered = 56, 
-                    count = 56, 
-                    entities = [
-                        src.qase.api_client_v1.models.result.Result(
-                            hash = '', 
-                            comment = '', 
-                            stacktrace = '', 
-                            run_id = 56, 
-                            case_id = 56, 
-                            steps = [
-                                src.qase.api_client_v1.models.test_step_result.TestStepResult(
-                                    status = 56, 
-                                    position = 56, 
-                                    attachments = [
-                                        src.qase.api_client_v1.models.attachment.Attachment(
-                                            size = 56, 
-                                            mime = '', 
-                                            filename = '', 
-                                            url = '', )
-                                        ], )
-                                ], 
-                            status = '', 
-                            is_api_result = True, 
-                            time_spent_ms = 56, 
-                            end_time = '2021-12-30T19:23:59Z', 
-                            attachments = [
-                                src.qase.api_client_v1.models.attachment.Attachment(
-                                    size = 56, 
-                                    mime = '', 
-                                    filename = '', 
-                                    url = '', )
-                                ], )
-                        ], )
+            return ResultListResponseAllOfResult(
+                total = 56,
+                filtered = 56,
+                count = 56,
+                entities = [
+                    qase.api_client_v1.models.result.Result(
+                        hash = '', 
+                        comment = '', 
+                        stacktrace = '', 
+                        run_id = 56, 
+                        case_id = 56, 
+                        steps = [
+                            qase.api_client_v1.models.test_step_result.TestStepResult(
+                                status = 56, 
+                                position = 56, 
+                                attachments = [
+                                    qase.api_client_v1.models.attachment.Attachment(
+                                        size = 56, 
+                                        mime = '', 
+                                        filename = '', 
+                                        url = '', )
+                                    ], )
+                            ], 
+                        status = '', 
+                        is_api_result = True, 
+                        time_spent_ms = 56, 
+                        end_time = '2021-12-30T19:23:59Z', 
+                        attachments = [
+                            qase.api_client_v1.models.attachment.Attachment(
+                                size = 56, 
+                                mime = '', 
+                                filename = '', 
+                                url = '', )
+                            ], )
+                    ]
             )
         else:
-            return ResultListResponse(
+            return ResultListResponseAllOfResult(
         )
         """
 
-    def testResultListResponse(self):
-        """Test ResultListResponse"""
+    def testResultListResponseAllOfResult(self):
+        """Test ResultListResponseAllOfResult"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_result_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,75 +11,77 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_list_response_all_of_result import ResultListResponseAllOfResult
+from qase.api_client_v1.models.result_list_response import ResultListResponse
 
-class TestResultListResponseAllOfResult(unittest.TestCase):
-    """ResultListResponseAllOfResult unit test stubs"""
+class TestResultListResponse(unittest.TestCase):
+    """ResultListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ResultListResponseAllOfResult:
-        """Test ResultListResponseAllOfResult
+    def make_instance(self, include_optional) -> ResultListResponse:
+        """Test ResultListResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ResultListResponseAllOfResult`
+        # uncomment below to create an instance of `ResultListResponse`
         """
-        model = ResultListResponseAllOfResult()
+        model = ResultListResponse()
         if include_optional:
-            return ResultListResponseAllOfResult(
-                total = 56,
-                filtered = 56,
-                count = 56,
-                entities = [
-                    src.qase.api_client_v1.models.result.Result(
-                        hash = '', 
-                        comment = '', 
-                        stacktrace = '', 
-                        run_id = 56, 
-                        case_id = 56, 
-                        steps = [
-                            src.qase.api_client_v1.models.test_step_result.TestStepResult(
-                                status = 56, 
-                                position = 56, 
-                                attachments = [
-                                    src.qase.api_client_v1.models.attachment.Attachment(
-                                        size = 56, 
-                                        mime = '', 
-                                        filename = '', 
-                                        url = '', )
-                                    ], )
-                            ], 
-                        status = '', 
-                        is_api_result = True, 
-                        time_spent_ms = 56, 
-                        end_time = '2021-12-30T19:23:59Z', 
-                        attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
-                                size = 56, 
-                                mime = '', 
-                                filename = '', 
-                                url = '', )
-                            ], )
-                    ]
+            return ResultListResponse(
+                status = True,
+                result = qase.api_client_v1.models.result_list_response_all_of_result.ResultListResponse_allOf_result(
+                    total = 56, 
+                    filtered = 56, 
+                    count = 56, 
+                    entities = [
+                        qase.api_client_v1.models.result.Result(
+                            hash = '', 
+                            comment = '', 
+                            stacktrace = '', 
+                            run_id = 56, 
+                            case_id = 56, 
+                            steps = [
+                                qase.api_client_v1.models.test_step_result.TestStepResult(
+                                    status = 56, 
+                                    position = 56, 
+                                    attachments = [
+                                        qase.api_client_v1.models.attachment.Attachment(
+                                            size = 56, 
+                                            mime = '', 
+                                            filename = '', 
+                                            url = '', )
+                                        ], )
+                                ], 
+                            status = '', 
+                            is_api_result = True, 
+                            time_spent_ms = 56, 
+                            end_time = '2021-12-30T19:23:59Z', 
+                            attachments = [
+                                qase.api_client_v1.models.attachment.Attachment(
+                                    size = 56, 
+                                    mime = '', 
+                                    filename = '', 
+                                    url = '', )
+                                ], )
+                        ], )
             )
         else:
-            return ResultListResponseAllOfResult(
+            return ResultListResponse(
         )
         """
 
-    def testResultListResponseAllOfResult(self):
-        """Test ResultListResponseAllOfResult"""
+    def testResultListResponse(self):
+        """Test ResultListResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_response.py` & `qase_api_client-1.0.0b2/test/test_result_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_response import ResultResponse
+from qase.api_client_v1.models.result_response import ResultResponse
 
 class TestResultResponse(unittest.TestCase):
     """ResultResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,38 +33,38 @@
             optional params are included """
         # uncomment below to create an instance of `ResultResponse`
         """
         model = ResultResponse()
         if include_optional:
             return ResultResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.result.Result(
+                result = qase.api_client_v1.models.result.Result(
                     hash = '', 
                     comment = '', 
                     stacktrace = '', 
                     run_id = 56, 
                     case_id = 56, 
                     steps = [
-                        src.qase.api_client_v1.models.test_step_result.TestStepResult(
+                        qase.api_client_v1.models.test_step_result.TestStepResult(
                             status = 56, 
                             position = 56, 
                             attachments = [
-                                src.qase.api_client_v1.models.attachment.Attachment(
+                                qase.api_client_v1.models.attachment.Attachment(
                                     size = 56, 
                                     mime = '', 
                                     filename = '', 
                                     url = '', )
                                 ], )
                         ], 
                     status = '', 
                     is_api_result = True, 
                     time_spent_ms = 56, 
                     end_time = '2021-12-30T19:23:59Z', 
                     attachments = [
-                        src.qase.api_client_v1.models.attachment.Attachment(
+                        qase.api_client_v1.models.attachment.Attachment(
                             size = 56, 
                             mime = '', 
                             filename = '', 
                             url = '', )
                         ], )
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_result_update.py` & `qase_api_client-1.0.0b2/test/test_result_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.result_update import ResultUpdate
+from qase.api_client_v1.models.result_update import ResultUpdate
 
 class TestResultUpdate(unittest.TestCase):
     """ResultUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -41,15 +41,15 @@
                 defect = True,
                 attachments = [
                     ''
                     ],
                 stacktrace = '',
                 comment = '',
                 steps = [
-                    src.qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
+                    qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
                         position = 56, 
                         status = 'passed', 
                         comment = '', 
                         attachments = [
                             ''
                             ], 
                         action = '',
```

### Comparing `qase_api_client-1.0.0b1/test/test_resultcreate_bulk.py` & `qase_api_client-1.0.0b2/test/test_resultcreate_bulk.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
+from qase.api_client_v1.models.resultcreate_bulk import ResultcreateBulk
 
 class TestResultcreateBulk(unittest.TestCase):
     """ResultcreateBulk unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,17 +33,17 @@
             optional params are included """
         # uncomment below to create an instance of `ResultcreateBulk`
         """
         model = ResultcreateBulk()
         if include_optional:
             return ResultcreateBulk(
                 results = [
-                    src.qase.api_client_v1.models.result_create.ResultCreate(
+                    qase.api_client_v1.models.result_create.ResultCreate(
                         case_id = 56, 
-                        case = src.qase.api_client_v1.models.result_create_case.ResultCreate_case(
+                        case = qase.api_client_v1.models.result_create_case.ResultCreate_case(
                             title = '', 
                             suite_title = '', 
                             description = '', 
                             preconditions = '', 
                             postconditions = '', 
                             layer = '', 
                             severity = '', 
@@ -58,31 +58,31 @@
                             ], 
                         stacktrace = '', 
                         comment = '', 
                         param = {
                             'key' : ''
                             }, 
                         steps = [
-                            src.qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
+                            qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
                                 position = 56, 
                                 status = 'passed', 
                                 comment = '', 
                                 action = '', 
                                 expected_result = '', 
                                 data = '', )
                             ], 
                         author_id = 56, )
                     ]
             )
         else:
             return ResultcreateBulk(
                 results = [
-                    src.qase.api_client_v1.models.result_create.ResultCreate(
+                    qase.api_client_v1.models.result_create.ResultCreate(
                         case_id = 56, 
-                        case = src.qase.api_client_v1.models.result_create_case.ResultCreate_case(
+                        case = qase.api_client_v1.models.result_create_case.ResultCreate_case(
                             title = '', 
                             suite_title = '', 
                             description = '', 
                             preconditions = '', 
                             postconditions = '', 
                             layer = '', 
                             severity = '', 
@@ -97,15 +97,15 @@
                             ], 
                         stacktrace = '', 
                         comment = '', 
                         param = {
                             'key' : ''
                             }, 
                         steps = [
-                            src.qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
+                            qase.api_client_v1.models.test_step_result_create.TestStepResultCreate(
                                 position = 56, 
                                 status = 'passed', 
                                 comment = '', 
                                 action = '', 
                                 expected_result = '', 
                                 data = '', )
                             ],
```

### Comparing `qase_api_client-1.0.0b1/test/test_results_api.py` & `qase_api_client-1.0.0b2/test/test_results_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.results_api import ResultsApi
+from qase.api_client_v1.api.results_api import ResultsApi
 
 
 class TestResultsApi(unittest.TestCase):
     """ResultsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = ResultsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_run.py` & `qase_api_client-1.0.0b2/test/test_run.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run import Run
+from qase.api_client_v1.models.run import Run
 
 class TestRun(unittest.TestCase):
     """Run unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -40,43 +40,43 @@
                 title = '',
                 description = '',
                 status = 56,
                 status_text = '',
                 start_time = '2021-12-30T19:23:59Z',
                 end_time = '2021-12-30T19:23:59Z',
                 public = True,
-                stats = src.qase.api_client_v1.models.run_stats.Run_stats(
+                stats = qase.api_client_v1.models.run_stats.Run_stats(
                     total = 56, 
                     statuses = {
                         'key' : 56
                         }, 
                     untested = 56, 
                     passed = 56, 
                     failed = 56, 
                     blocked = 56, 
                     skipped = 56, 
                     retest = 56, 
                     in_progress = 56, 
                     invalid = 56, ),
                 time_spent = 56,
-                environment = src.qase.api_client_v1.models.run_environment.Run_environment(
+                environment = qase.api_client_v1.models.run_environment.Run_environment(
                     title = '', 
                     description = '', 
                     slug = '', 
                     host = '', ),
-                milestone = src.qase.api_client_v1.models.run_milestone.Run_milestone(
+                milestone = qase.api_client_v1.models.run_milestone.Run_milestone(
                     title = '', 
                     description = '', ),
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 cases = [
                     56
                     ]
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_create.py` & `qase_api_client-1.0.0b2/test/test_run_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_create import RunCreate
+from qase.api_client_v1.models.run_create import RunCreate
 
 class TestRunCreate(unittest.TestCase):
     """RunCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_environment.py` & `qase_api_client-1.0.0b2/test/test_run_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_environment import RunEnvironment
+from qase.api_client_v1.models.run_environment import RunEnvironment
 
 class TestRunEnvironment(unittest.TestCase):
     """RunEnvironment unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_list_response.py` & `qase_api_client-1.0.0b2/test/test_run_list_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_list_response import RunListResponse
+from qase.api_client_v1.models.run_list_response import RunListResponse
 
 class TestRunListResponse(unittest.TestCase):
     """RunListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,57 +33,57 @@
             optional params are included """
         # uncomment below to create an instance of `RunListResponse`
         """
         model = RunListResponse()
         if include_optional:
             return RunListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.run_list_response_all_of_result.RunListResponse_allOf_result(
+                result = qase.api_client_v1.models.run_list_response_all_of_result.RunListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.run.Run(
+                        qase.api_client_v1.models.run.Run(
                             id = 56, 
                             title = '', 
                             description = '', 
                             status = 56, 
                             status_text = '', 
                             start_time = '2021-12-30T19:23:59Z', 
                             end_time = '2021-12-30T19:23:59Z', 
                             public = True, 
-                            stats = src.qase.api_client_v1.models.run_stats.Run_stats(
+                            stats = qase.api_client_v1.models.run_stats.Run_stats(
                                 total = 56, 
                                 statuses = {
                                     'key' : 56
                                     }, 
                                 untested = 56, 
                                 passed = 56, 
                                 failed = 56, 
                                 blocked = 56, 
                                 skipped = 56, 
                                 retest = 56, 
                                 in_progress = 56, 
                                 invalid = 56, ), 
                             time_spent = 56, 
-                            environment = src.qase.api_client_v1.models.run_environment.Run_environment(
+                            environment = qase.api_client_v1.models.run_environment.Run_environment(
                                 title = '', 
                                 description = '', 
                                 slug = '', 
                                 host = '', ), 
-                            milestone = src.qase.api_client_v1.models.run_milestone.Run_milestone(
+                            milestone = qase.api_client_v1.models.run_milestone.Run_milestone(
                                 title = '', 
                                 description = '', ), 
                             custom_fields = [
-                                src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                                qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                                     id = 56, 
                                     value = '', )
                                 ], 
                             tags = [
-                                src.qase.api_client_v1.models.tag_value.TagValue(
+                                qase.api_client_v1.models.tag_value.TagValue(
                                     title = '', 
                                     internal_id = 56, )
                                 ], 
                             cases = [
                                 56
                                 ], )
                         ], )
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_run_list_response_all_of_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
+from qase.api_client_v1.models.run_list_response_all_of_result import RunListResponseAllOfResult
 
 class TestRunListResponseAllOfResult(unittest.TestCase):
     """RunListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,52 +36,52 @@
         model = RunListResponseAllOfResult()
         if include_optional:
             return RunListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.run.Run(
+                    qase.api_client_v1.models.run.Run(
                         id = 56, 
                         title = '', 
                         description = '', 
                         status = 56, 
                         status_text = '', 
                         start_time = '2021-12-30T19:23:59Z', 
                         end_time = '2021-12-30T19:23:59Z', 
                         public = True, 
-                        stats = src.qase.api_client_v1.models.run_stats.Run_stats(
+                        stats = qase.api_client_v1.models.run_stats.Run_stats(
                             total = 56, 
                             statuses = {
                                 'key' : 56
                                 }, 
                             untested = 56, 
                             passed = 56, 
                             failed = 56, 
                             blocked = 56, 
                             skipped = 56, 
                             retest = 56, 
                             in_progress = 56, 
                             invalid = 56, ), 
                         time_spent = 56, 
-                        environment = src.qase.api_client_v1.models.run_environment.Run_environment(
+                        environment = qase.api_client_v1.models.run_environment.Run_environment(
                             title = '', 
                             description = '', 
                             slug = '', 
                             host = '', ), 
-                        milestone = src.qase.api_client_v1.models.run_milestone.Run_milestone(
+                        milestone = qase.api_client_v1.models.run_milestone.Run_milestone(
                             title = '', 
                             description = '', ), 
                         custom_fields = [
-                            src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                            qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                                 id = 56, 
                                 value = '', )
                             ], 
                         tags = [
-                            src.qase.api_client_v1.models.tag_value.TagValue(
+                            qase.api_client_v1.models.tag_value.TagValue(
                                 title = '', 
                                 internal_id = 56, )
                             ], 
                         cases = [
                             56
                             ], )
                     ]
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_milestone.py` & `qase_api_client-1.0.0b2/test/test_run_milestone.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_milestone import RunMilestone
+from qase.api_client_v1.models.run_milestone import RunMilestone
 
 class TestRunMilestone(unittest.TestCase):
     """RunMilestone unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_public.py` & `qase_api_client-1.0.0b2/test/test_run_public.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_public import RunPublic
+from qase.api_client_v1.models.run_public import RunPublic
 
 class TestRunPublic(unittest.TestCase):
     """RunPublic unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_public_response.py` & `qase_api_client-1.0.0b2/test/test_run_public_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_public_response import RunPublicResponse
+from qase.api_client_v1.models.run_public_response import RunPublicResponse
 
 class TestRunPublicResponse(unittest.TestCase):
     """RunPublicResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `RunPublicResponse`
         """
         model = RunPublicResponse()
         if include_optional:
             return RunPublicResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.run_public_response_all_of_result.RunPublicResponse_allOf_result(
+                result = qase.api_client_v1.models.run_public_response_all_of_result.RunPublicResponse_allOf_result(
                     url = '', )
             )
         else:
             return RunPublicResponse(
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_public_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_run_public_response_all_of_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
+from qase.api_client_v1.models.run_public_response_all_of_result import RunPublicResponseAllOfResult
 
 class TestRunPublicResponseAllOfResult(unittest.TestCase):
     """RunPublicResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_response.py` & `qase_api_client-1.0.0b2/test/test_run_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_response import RunResponse
+from qase.api_client_v1.models.run_response import RunResponse
 
 class TestRunResponse(unittest.TestCase):
     """RunResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,52 +33,52 @@
             optional params are included """
         # uncomment below to create an instance of `RunResponse`
         """
         model = RunResponse()
         if include_optional:
             return RunResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.run.Run(
+                result = qase.api_client_v1.models.run.Run(
                     id = 56, 
                     title = '', 
                     description = '', 
                     status = 56, 
                     status_text = '', 
                     start_time = '2021-12-30T19:23:59Z', 
                     end_time = '2021-12-30T19:23:59Z', 
                     public = True, 
-                    stats = src.qase.api_client_v1.models.run_stats.Run_stats(
+                    stats = qase.api_client_v1.models.run_stats.Run_stats(
                         total = 56, 
                         statuses = {
                             'key' : 56
                             }, 
                         untested = 56, 
                         passed = 56, 
                         failed = 56, 
                         blocked = 56, 
                         skipped = 56, 
                         retest = 56, 
                         in_progress = 56, 
                         invalid = 56, ), 
                     time_spent = 56, 
-                    environment = src.qase.api_client_v1.models.run_environment.Run_environment(
+                    environment = qase.api_client_v1.models.run_environment.Run_environment(
                         title = '', 
                         description = '', 
                         slug = '', 
                         host = '', ), 
-                    milestone = src.qase.api_client_v1.models.run_milestone.Run_milestone(
+                    milestone = qase.api_client_v1.models.run_milestone.Run_milestone(
                         title = '', 
                         description = '', ), 
                     custom_fields = [
-                        src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                        qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                             id = 56, 
                             value = '', )
                         ], 
                     tags = [
-                        src.qase.api_client_v1.models.tag_value.TagValue(
+                        qase.api_client_v1.models.tag_value.TagValue(
                             title = '', 
                             internal_id = 56, )
                         ], 
                     cases = [
                         56
                         ], )
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_run_stats.py` & `qase_api_client-1.0.0b2/test/test_run_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.run_stats import RunStats
+from qase.api_client_v1.models.run_stats import RunStats
 
 class TestRunStats(unittest.TestCase):
     """RunStats unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_runs_api.py` & `qase_api_client-1.0.0b2/test/test_runs_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.runs_api import RunsApi
+from qase.api_client_v1.api.runs_api import RunsApi
 
 
 class TestRunsApi(unittest.TestCase):
     """RunsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = RunsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_search_api.py` & `qase_api_client-1.0.0b2/test/test_search_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.search_api import SearchApi
+from qase.api_client_v1.api.search_api import SearchApi
 
 
 class TestSearchApi(unittest.TestCase):
     """SearchApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = SearchApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_search_response.py` & `qase_api_client-1.0.0b2/test/test_search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.search_response import SearchResponse
+from qase.api_client_v1.models.search_response import SearchResponse
 
 class TestSearchResponse(unittest.TestCase):
     """SearchResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `SearchResponse`
         """
         model = SearchResponse()
         if include_optional:
             return SearchResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.search_response_all_of_result.SearchResponse_allOf_result(
+                result = qase.api_client_v1.models.search_response_all_of_result.SearchResponse_allOf_result(
                     entities = [
                         null
                         ], 
                     total = 56, )
             )
         else:
             return SearchResponse(
```

### Comparing `qase_api_client-1.0.0b1/test/test_search_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_search_response_all_of_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
+from qase.api_client_v1.models.search_response_all_of_result import SearchResponseAllOfResult
 
 class TestSearchResponseAllOfResult(unittest.TestCase):
     """SearchResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step.py` & `qase_api_client-1.0.0b2/test/test_shared_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step import SharedStep
+from qase.api_client_v1.models.shared_step import SharedStep
 
 class TestSharedStep(unittest.TestCase):
     """SharedStep unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -37,21 +37,21 @@
         if include_optional:
             return SharedStep(
                 hash = '',
                 title = '',
                 action = '',
                 expected_result = '',
                 steps = [
-                    src.qase.api_client_v1.models.shared_step_content.SharedStepContent(
+                    qase.api_client_v1.models.shared_step_content.SharedStepContent(
                         data = '', 
                         hash = '', 
                         action = '', 
                         expected_result = '', 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment_hash.AttachmentHash(
+                            qase.api_client_v1.models.attachment_hash.AttachmentHash(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', 
                                 hash = '', )
                             ], )
                     ],
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_content.py` & `qase_api_client-1.0.0b2/test/test_shared_step_content.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_content import SharedStepContent
+from qase.api_client_v1.models.shared_step_content import SharedStepContent
 
 class TestSharedStepContent(unittest.TestCase):
     """SharedStepContent unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -37,15 +37,15 @@
         if include_optional:
             return SharedStepContent(
                 data = '',
                 hash = '',
                 action = '',
                 expected_result = '',
                 attachments = [
-                    src.qase.api_client_v1.models.attachment_hash.AttachmentHash(
+                    qase.api_client_v1.models.attachment_hash.AttachmentHash(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', 
                         hash = '', )
                     ]
             )
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_content_create.py` & `qase_api_client-1.0.0b2/test/test_shared_step_content_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
+from qase.api_client_v1.models.shared_step_content_create import SharedStepContentCreate
 
 class TestSharedStepContentCreate(unittest.TestCase):
     """SharedStepContentCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_create.py` & `qase_api_client-1.0.0b2/test/test_shared_step_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_create import SharedStepCreate
+from qase.api_client_v1.models.shared_step_create import SharedStepCreate
 
 class TestSharedStepCreate(unittest.TestCase):
     """SharedStepCreate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -37,15 +37,15 @@
         if include_optional:
             return SharedStepCreate(
                 title = '',
                 action = '',
                 expected_result = '',
                 data = '',
                 steps = [
-                    src.qase.api_client_v1.models.shared_step_content_create.SharedStepContentCreate(
+                    qase.api_client_v1.models.shared_step_content_create.SharedStepContentCreate(
                         hash = '', 
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         attachments = [
                             ''
                             ], )
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_list_response.py` & `qase_api_client-1.0.0b2/test/test_shared_step_list_response_all_of_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,77 +11,75 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
+from qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
 
-class TestSharedStepListResponse(unittest.TestCase):
-    """SharedStepListResponse unit test stubs"""
+class TestSharedStepListResponseAllOfResult(unittest.TestCase):
+    """SharedStepListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SharedStepListResponse:
-        """Test SharedStepListResponse
+    def make_instance(self, include_optional) -> SharedStepListResponseAllOfResult:
+        """Test SharedStepListResponseAllOfResult
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SharedStepListResponse`
+        # uncomment below to create an instance of `SharedStepListResponseAllOfResult`
         """
-        model = SharedStepListResponse()
+        model = SharedStepListResponseAllOfResult()
         if include_optional:
-            return SharedStepListResponse(
-                status = True,
-                result = src.qase.api_client_v1.models.shared_step_list_response_all_of_result.SharedStepListResponse_allOf_result(
-                    total = 56, 
-                    filtered = 56, 
-                    count = 56, 
-                    entities = [
-                        src.qase.api_client_v1.models.shared_step.SharedStep(
-                            hash = '', 
-                            title = '', 
-                            action = '', 
-                            expected_result = '', 
-                            steps = [
-                                src.qase.api_client_v1.models.shared_step_content.SharedStepContent(
-                                    data = '', 
-                                    hash = '', 
-                                    action = '', 
-                                    expected_result = '', 
-                                    attachments = [
-                                        src.qase.api_client_v1.models.attachment_hash.AttachmentHash(
-                                            size = 56, 
-                                            mime = '', 
-                                            filename = '', 
-                                            url = '', 
-                                            hash = '', )
-                                        ], )
-                                ], 
-                            data = '', 
-                            cases = [
-                                56
-                                ], 
-                            cases_count = 56, 
-                            created = '2021-12-30 19:23:59', 
-                            updated = '2021-12-30 19:23:59', 
-                            created_at = '2021-12-30T19:23:59Z', 
-                            updated_at = '2021-12-30T19:23:59Z', )
-                        ], )
+            return SharedStepListResponseAllOfResult(
+                total = 56,
+                filtered = 56,
+                count = 56,
+                entities = [
+                    qase.api_client_v1.models.shared_step.SharedStep(
+                        hash = '', 
+                        title = '', 
+                        action = '', 
+                        expected_result = '', 
+                        steps = [
+                            qase.api_client_v1.models.shared_step_content.SharedStepContent(
+                                data = '', 
+                                hash = '', 
+                                action = '', 
+                                expected_result = '', 
+                                attachments = [
+                                    qase.api_client_v1.models.attachment_hash.AttachmentHash(
+                                        size = 56, 
+                                        mime = '', 
+                                        filename = '', 
+                                        url = '', 
+                                        hash = '', )
+                                    ], )
+                            ], 
+                        data = '', 
+                        cases = [
+                            56
+                            ], 
+                        cases_count = 56, 
+                        created = '2021-12-30 19:23:59', 
+                        updated = '2021-12-30 19:23:59', 
+                        created_at = '2021-12-30T19:23:59Z', 
+                        updated_at = '2021-12-30T19:23:59Z', )
+                    ]
             )
         else:
-            return SharedStepListResponse(
+            return SharedStepListResponseAllOfResult(
         )
         """
 
-    def testSharedStepListResponse(self):
-        """Test SharedStepListResponse"""
+    def testSharedStepListResponseAllOfResult(self):
+        """Test SharedStepListResponseAllOfResult"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_shared_step_list_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,75 +11,77 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_list_response_all_of_result import SharedStepListResponseAllOfResult
+from qase.api_client_v1.models.shared_step_list_response import SharedStepListResponse
 
-class TestSharedStepListResponseAllOfResult(unittest.TestCase):
-    """SharedStepListResponseAllOfResult unit test stubs"""
+class TestSharedStepListResponse(unittest.TestCase):
+    """SharedStepListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SharedStepListResponseAllOfResult:
-        """Test SharedStepListResponseAllOfResult
+    def make_instance(self, include_optional) -> SharedStepListResponse:
+        """Test SharedStepListResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SharedStepListResponseAllOfResult`
+        # uncomment below to create an instance of `SharedStepListResponse`
         """
-        model = SharedStepListResponseAllOfResult()
+        model = SharedStepListResponse()
         if include_optional:
-            return SharedStepListResponseAllOfResult(
-                total = 56,
-                filtered = 56,
-                count = 56,
-                entities = [
-                    src.qase.api_client_v1.models.shared_step.SharedStep(
-                        hash = '', 
-                        title = '', 
-                        action = '', 
-                        expected_result = '', 
-                        steps = [
-                            src.qase.api_client_v1.models.shared_step_content.SharedStepContent(
-                                data = '', 
-                                hash = '', 
-                                action = '', 
-                                expected_result = '', 
-                                attachments = [
-                                    src.qase.api_client_v1.models.attachment_hash.AttachmentHash(
-                                        size = 56, 
-                                        mime = '', 
-                                        filename = '', 
-                                        url = '', 
-                                        hash = '', )
-                                    ], )
-                            ], 
-                        data = '', 
-                        cases = [
-                            56
-                            ], 
-                        cases_count = 56, 
-                        created = '2021-12-30 19:23:59', 
-                        updated = '2021-12-30 19:23:59', 
-                        created_at = '2021-12-30T19:23:59Z', 
-                        updated_at = '2021-12-30T19:23:59Z', )
-                    ]
+            return SharedStepListResponse(
+                status = True,
+                result = qase.api_client_v1.models.shared_step_list_response_all_of_result.SharedStepListResponse_allOf_result(
+                    total = 56, 
+                    filtered = 56, 
+                    count = 56, 
+                    entities = [
+                        qase.api_client_v1.models.shared_step.SharedStep(
+                            hash = '', 
+                            title = '', 
+                            action = '', 
+                            expected_result = '', 
+                            steps = [
+                                qase.api_client_v1.models.shared_step_content.SharedStepContent(
+                                    data = '', 
+                                    hash = '', 
+                                    action = '', 
+                                    expected_result = '', 
+                                    attachments = [
+                                        qase.api_client_v1.models.attachment_hash.AttachmentHash(
+                                            size = 56, 
+                                            mime = '', 
+                                            filename = '', 
+                                            url = '', 
+                                            hash = '', )
+                                        ], )
+                                ], 
+                            data = '', 
+                            cases = [
+                                56
+                                ], 
+                            cases_count = 56, 
+                            created = '2021-12-30 19:23:59', 
+                            updated = '2021-12-30 19:23:59', 
+                            created_at = '2021-12-30T19:23:59Z', 
+                            updated_at = '2021-12-30T19:23:59Z', )
+                        ], )
             )
         else:
-            return SharedStepListResponseAllOfResult(
+            return SharedStepListResponse(
         )
         """
 
-    def testSharedStepListResponseAllOfResult(self):
-        """Test SharedStepListResponseAllOfResult"""
+    def testSharedStepListResponse(self):
+        """Test SharedStepListResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_response.py` & `qase_api_client-1.0.0b2/test/test_shared_step_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_response import SharedStepResponse
+from qase.api_client_v1.models.shared_step_response import SharedStepResponse
 
 class TestSharedStepResponse(unittest.TestCase):
     """SharedStepResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,27 +33,27 @@
             optional params are included """
         # uncomment below to create an instance of `SharedStepResponse`
         """
         model = SharedStepResponse()
         if include_optional:
             return SharedStepResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.shared_step.SharedStep(
+                result = qase.api_client_v1.models.shared_step.SharedStep(
                     hash = '', 
                     title = '', 
                     action = '', 
                     expected_result = '', 
                     steps = [
-                        src.qase.api_client_v1.models.shared_step_content.SharedStepContent(
+                        qase.api_client_v1.models.shared_step_content.SharedStepContent(
                             data = '', 
                             hash = '', 
                             action = '', 
                             expected_result = '', 
                             attachments = [
-                                src.qase.api_client_v1.models.attachment_hash.AttachmentHash(
+                                qase.api_client_v1.models.attachment_hash.AttachmentHash(
                                     size = 56, 
                                     mime = '', 
                                     filename = '', 
                                     url = '', 
                                     hash = '', )
                                 ], )
                         ],
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_step_update.py` & `qase_api_client-1.0.0b2/test/test_shared_step_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.shared_step_update import SharedStepUpdate
+from qase.api_client_v1.models.shared_step_update import SharedStepUpdate
 
 class TestSharedStepUpdate(unittest.TestCase):
     """SharedStepUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -37,15 +37,15 @@
         if include_optional:
             return SharedStepUpdate(
                 title = '',
                 action = '',
                 expected_result = '',
                 data = '',
                 steps = [
-                    src.qase.api_client_v1.models.shared_step_content_create.SharedStepContentCreate(
+                    qase.api_client_v1.models.shared_step_content_create.SharedStepContentCreate(
                         hash = '', 
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         attachments = [
                             ''
                             ], )
```

### Comparing `qase_api_client-1.0.0b1/test/test_shared_steps_api.py` & `qase_api_client-1.0.0b2/test/test_shared_steps_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.shared_steps_api import SharedStepsApi
+from qase.api_client_v1.api.shared_steps_api import SharedStepsApi
 
 
 class TestSharedStepsApi(unittest.TestCase):
     """SharedStepsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = SharedStepsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite.py` & `qase_api_client-1.0.0b2/test/test_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite import Suite
+from qase.api_client_v1.models.suite import Suite
 
 class TestSuite(unittest.TestCase):
     """Suite unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite_create.py` & `qase_api_client-1.0.0b2/test/test_suite_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite_create import SuiteCreate
+from qase.api_client_v1.models.suite_create import SuiteCreate
 
 class TestSuiteCreate(unittest.TestCase):
     """SuiteCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite_delete.py` & `qase_api_client-1.0.0b2/test/test_suite_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite_delete import SuiteDelete
+from qase.api_client_v1.models.suite_delete import SuiteDelete
 
 class TestSuiteDelete(unittest.TestCase):
     """SuiteDelete unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite_list_response.py` & `qase_api_client-1.0.0b2/test/test_suite_list_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite_list_response import SuiteListResponse
+from qase.api_client_v1.models.suite_list_response import SuiteListResponse
 
 class TestSuiteListResponse(unittest.TestCase):
     """SuiteListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `SuiteListResponse`
         """
         model = SuiteListResponse()
         if include_optional:
             return SuiteListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.suite_list_response_all_of_result.SuiteListResponse_allOf_result(
+                result = qase.api_client_v1.models.suite_list_response_all_of_result.SuiteListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.suite.Suite(
+                        qase.api_client_v1.models.suite.Suite(
                             id = 56, 
                             title = '', 
                             description = '', 
                             preconditions = '', 
                             position = 56, 
                             cases_count = 56, 
                             parent_id = 56,
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_suite_list_response_all_of_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
+from qase.api_client_v1.models.suite_list_response_all_of_result import SuiteListResponseAllOfResult
 
 class TestSuiteListResponseAllOfResult(unittest.TestCase):
     """SuiteListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = SuiteListResponseAllOfResult()
         if include_optional:
             return SuiteListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.suite.Suite(
+                    qase.api_client_v1.models.suite.Suite(
                         id = 56, 
                         title = '', 
                         description = '', 
                         preconditions = '', 
                         position = 56, 
                         cases_count = 56, 
                         parent_id = 56,
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite_response.py` & `qase_api_client-1.0.0b2/test/test_suite_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite_response import SuiteResponse
+from qase.api_client_v1.models.suite_response import SuiteResponse
 
 class TestSuiteResponse(unittest.TestCase):
     """SuiteResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `SuiteResponse`
         """
         model = SuiteResponse()
         if include_optional:
             return SuiteResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.suite.Suite(
+                result = qase.api_client_v1.models.suite.Suite(
                     id = 56, 
                     title = '', 
                     description = '', 
                     preconditions = '', 
                     position = 56, 
                     cases_count = 56, 
                     parent_id = 56,
```

### Comparing `qase_api_client-1.0.0b1/test/test_suite_update.py` & `qase_api_client-1.0.0b2/test/test_suite_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.suite_update import SuiteUpdate
+from qase.api_client_v1.models.suite_update import SuiteUpdate
 
 class TestSuiteUpdate(unittest.TestCase):
     """SuiteUpdate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_suites_api.py` & `qase_api_client-1.0.0b2/test/test_suites_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.suites_api import SuitesApi
+from qase.api_client_v1.api.suites_api import SuitesApi
 
 
 class TestSuitesApi(unittest.TestCase):
     """SuitesApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = SuitesApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_system_field.py` & `qase_api_client-1.0.0b2/test/test_system_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.system_field import SystemField
+from qase.api_client_v1.models.system_field import SystemField
 
 class TestSystemField(unittest.TestCase):
     """SystemField unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -39,15 +39,15 @@
                 title = '',
                 slug = '',
                 default_value = '',
                 is_required = True,
                 entity = 56,
                 type = 56,
                 options = [
-                    src.qase.api_client_v1.models.system_field_option.SystemFieldOption(
+                    qase.api_client_v1.models.system_field_option.SystemFieldOption(
                         id = 56, 
                         title = '', 
                         slug = '', 
                         color = '', 
                         icon = '', 
                         is_default = True, 
                         read_only = True, )
```

### Comparing `qase_api_client-1.0.0b1/test/test_system_field_list_response.py` & `qase_api_client-1.0.0b2/test/test_system_field_list_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
+from qase.api_client_v1.models.system_field_list_response import SystemFieldListResponse
 
 class TestSystemFieldListResponse(unittest.TestCase):
     """SystemFieldListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,23 +34,23 @@
         # uncomment below to create an instance of `SystemFieldListResponse`
         """
         model = SystemFieldListResponse()
         if include_optional:
             return SystemFieldListResponse(
                 status = True,
                 result = [
-                    src.qase.api_client_v1.models.system_field.SystemField(
+                    qase.api_client_v1.models.system_field.SystemField(
                         title = '', 
                         slug = '', 
                         default_value = '', 
                         is_required = True, 
                         entity = 56, 
                         type = 56, 
                         options = [
-                            src.qase.api_client_v1.models.system_field_option.SystemFieldOption(
+                            qase.api_client_v1.models.system_field_option.SystemFieldOption(
                                 id = 56, 
                                 title = '', 
                                 slug = '', 
                                 color = '', 
                                 icon = '', 
                                 is_default = True, 
                                 read_only = True, )
```

### Comparing `qase_api_client-1.0.0b1/test/test_system_field_option.py` & `qase_api_client-1.0.0b2/test/test_system_field_option.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.system_field_option import SystemFieldOption
+from qase.api_client_v1.models.system_field_option import SystemFieldOption
 
 class TestSystemFieldOption(unittest.TestCase):
     """SystemFieldOption unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_system_fields_api.py` & `qase_api_client-1.0.0b2/test/test_system_fields_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.api.system_fields_api import SystemFieldsApi
+from qase.api_client_v1.api.system_fields_api import SystemFieldsApi
 
 
 class TestSystemFieldsApi(unittest.TestCase):
     """SystemFieldsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = SystemFieldsApi()
```

### Comparing `qase_api_client-1.0.0b1/test/test_tag_value.py` & `qase_api_client-1.0.0b2/test/test_tag_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.tag_value import TagValue
+from qase.api_client_v1.models.tag_value import TagValue
 
 class TestTagValue(unittest.TestCase):
     """TagValue unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case.py` & `qase_api_client-1.0.0b2/test/test_test_case.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case import TestCase
+from qase.api_client_v1.models.test_case import TestCase
 
 class TestTestCase(unittest.TestCase):
     """TestCase unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -49,64 +49,64 @@
                 is_flaky = 56,
                 behavior = 56,
                 automation = 56,
                 status = 56,
                 milestone_id = 56,
                 suite_id = 56,
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 steps_type = '',
                 steps = [
-                    src.qase.api_client_v1.models.test_step.TestStep(
+                    qase.api_client_v1.models.test_step.TestStep(
                         hash = '', 
                         shared_step_hash = '', 
                         shared_step_nested_hash = '', 
                         position = 56, 
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
+                            qase.api_client_v1.models.attachment.Attachment(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', )
                             ], 
                         steps = [
                             None
                             ], )
                     ],
                 params = None,
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 member_id = 56,
                 author_id = 56,
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z',
                 deleted = '2021-12-30T19:23:59.000000Z',
                 created = '2021-12-30T19:23:59.000000Z',
                 updated = '2021-12-30T19:23:59.000000Z',
                 external_issues = [
-                    src.qase.api_client_v1.models.external_issue.ExternalIssue(
+                    qase.api_client_v1.models.external_issue.ExternalIssue(
                         type = '', 
                         issues = [
-                            src.qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
+                            qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
                                 id = '', 
                                 link = '', )
                             ], )
                     ]
             )
         else:
             return TestCase(
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_create.py` & `qase_api_client-1.0.0b2/test/test_test_case_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_create import TestCaseCreate
+from qase.api_client_v1.models.test_case_create import TestCaseCreate
 
 class TestTestCaseCreate(unittest.TestCase):
     """TestCaseCreate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -51,15 +51,15 @@
                 milestone_id = 56,
                 automation = 56,
                 status = 56,
                 attachments = [
                     ''
                     ],
                 steps = [
-                    src.qase.api_client_v1.models.test_step_create.TestStepCreate(
+                    qase.api_client_v1.models.test_step_create.TestStepCreate(
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         position = 56, 
                         attachments = [
                             ''
                             ],
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_external_issues.py` & `qase_api_client-1.0.0b2/test/test_test_case_external_issues.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_external_issues import TestCaseExternalIssues
+from qase.api_client_v1.models.test_case_external_issues import TestCaseExternalIssues
 
 class TestTestCaseExternalIssues(unittest.TestCase):
     """TestCaseExternalIssues unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,26 +34,26 @@
         # uncomment below to create an instance of `TestCaseExternalIssues`
         """
         model = TestCaseExternalIssues()
         if include_optional:
             return TestCaseExternalIssues(
                 type = 'jira-cloud',
                 links = [
-                    src.qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
+                    qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
                         case_id = 56, 
                         external_issues = [
                             ''
                             ], )
                     ]
             )
         else:
             return TestCaseExternalIssues(
                 type = 'jira-cloud',
                 links = [
-                    src.qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
+                    qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
                         case_id = 56, 
                         external_issues = [
                             ''
                             ], )
                     ],
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_external_issues_links_inner.py` & `qase_api_client-1.0.0b2/test/test_test_case_external_issues_links_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
+from qase.api_client_v1.models.test_case_external_issues_links_inner import TestCaseExternalIssuesLinksInner
 
 class TestTestCaseExternalIssuesLinksInner(unittest.TestCase):
     """TestCaseExternalIssuesLinksInner unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_list_response.py` & `qase_api_client-1.0.0b2/test/test_test_case_list_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
+from qase.api_client_v1.models.test_case_list_response import TestCaseListResponse
 
 class TestTestCaseListResponse(unittest.TestCase):
     """TestCaseListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,20 +33,20 @@
             optional params are included """
         # uncomment below to create an instance of `TestCaseListResponse`
         """
         model = TestCaseListResponse()
         if include_optional:
             return TestCaseListResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.test_case_list_response_all_of_result.TestCaseListResponse_allOf_result(
+                result = qase.api_client_v1.models.test_case_list_response_all_of_result.TestCaseListResponse_allOf_result(
                     total = 56, 
                     filtered = 56, 
                     count = 56, 
                     entities = [
-                        src.qase.api_client_v1.models.test_case.TestCase(
+                        qase.api_client_v1.models.test_case.TestCase(
                             id = 56, 
                             position = 56, 
                             title = '', 
                             description = '', 
                             preconditions = '', 
                             postconditions = '', 
                             severity = 56, 
@@ -56,54 +56,54 @@
                             is_flaky = 56, 
                             behavior = 56, 
                             automation = 56, 
                             status = 56, 
                             milestone_id = 56, 
                             suite_id = 56, 
                             custom_fields = [
-                                src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                                qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                                     id = 56, 
                                     value = '', )
                                 ], 
                             attachments = [
-                                src.qase.api_client_v1.models.attachment.Attachment(
+                                qase.api_client_v1.models.attachment.Attachment(
                                     size = 56, 
                                     mime = '', 
                                     filename = '', 
                                     url = '', )
                                 ], 
                             steps_type = '', 
                             steps = [
-                                src.qase.api_client_v1.models.test_step.TestStep(
+                                qase.api_client_v1.models.test_step.TestStep(
                                     hash = '', 
                                     shared_step_hash = '', 
                                     shared_step_nested_hash = '', 
                                     position = 56, 
                                     action = '', 
                                     expected_result = '', 
                                     data = '', )
                                 ], 
                             params = null, 
                             tags = [
-                                src.qase.api_client_v1.models.tag_value.TagValue(
+                                qase.api_client_v1.models.tag_value.TagValue(
                                     title = '', 
                                     internal_id = 56, )
                                 ], 
                             member_id = 56, 
                             author_id = 56, 
                             created_at = '2021-12-30T19:23:59Z', 
                             updated_at = '2021-12-30T19:23:59Z', 
                             deleted = '2021-12-30T19:23:59.000000Z', 
                             created = '2021-12-30T19:23:59.000000Z', 
                             updated = '2021-12-30T19:23:59.000000Z', 
                             external_issues = [
-                                src.qase.api_client_v1.models.external_issue.ExternalIssue(
+                                qase.api_client_v1.models.external_issue.ExternalIssue(
                                     type = '', 
                                     issues = [
-                                        src.qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
+                                        qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
                                             id = '', 
                                             link = '', )
                                         ], )
                                 ], )
                         ], )
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_list_response_all_of_result.py` & `qase_api_client-1.0.0b2/test/test_test_case_list_response_all_of_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
+from qase.api_client_v1.models.test_case_list_response_all_of_result import TestCaseListResponseAllOfResult
 
 class TestTestCaseListResponseAllOfResult(unittest.TestCase):
     """TestCaseListResponseAllOfResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -36,15 +36,15 @@
         model = TestCaseListResponseAllOfResult()
         if include_optional:
             return TestCaseListResponseAllOfResult(
                 total = 56,
                 filtered = 56,
                 count = 56,
                 entities = [
-                    src.qase.api_client_v1.models.test_case.TestCase(
+                    qase.api_client_v1.models.test_case.TestCase(
                         id = 56, 
                         position = 56, 
                         title = '', 
                         description = '', 
                         preconditions = '', 
                         postconditions = '', 
                         severity = 56, 
@@ -54,54 +54,54 @@
                         is_flaky = 56, 
                         behavior = 56, 
                         automation = 56, 
                         status = 56, 
                         milestone_id = 56, 
                         suite_id = 56, 
                         custom_fields = [
-                            src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                            qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                                 id = 56, 
                                 value = '', )
                             ], 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
+                            qase.api_client_v1.models.attachment.Attachment(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', )
                             ], 
                         steps_type = '', 
                         steps = [
-                            src.qase.api_client_v1.models.test_step.TestStep(
+                            qase.api_client_v1.models.test_step.TestStep(
                                 hash = '', 
                                 shared_step_hash = '', 
                                 shared_step_nested_hash = '', 
                                 position = 56, 
                                 action = '', 
                                 expected_result = '', 
                                 data = '', )
                             ], 
                         params = null, 
                         tags = [
-                            src.qase.api_client_v1.models.tag_value.TagValue(
+                            qase.api_client_v1.models.tag_value.TagValue(
                                 title = '', 
                                 internal_id = 56, )
                             ], 
                         member_id = 56, 
                         author_id = 56, 
                         created_at = '2021-12-30T19:23:59Z', 
                         updated_at = '2021-12-30T19:23:59Z', 
                         deleted = '2021-12-30T19:23:59.000000Z', 
                         created = '2021-12-30T19:23:59.000000Z', 
                         updated = '2021-12-30T19:23:59.000000Z', 
                         external_issues = [
-                            src.qase.api_client_v1.models.external_issue.ExternalIssue(
+                            qase.api_client_v1.models.external_issue.ExternalIssue(
                                 type = '', 
                                 issues = [
-                                    src.qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
+                                    qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
                                         id = '', 
                                         link = '', )
                                     ], )
                             ], )
                     ]
             )
         else:
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_params.py` & `qase_api_client-1.0.0b2/test/test_test_case_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_params import TestCaseParams
+from qase.api_client_v1.models.test_case_params import TestCaseParams
 
 class TestTestCaseParams(unittest.TestCase):
     """TestCaseParams unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_query.py` & `qase_api_client-1.0.0b2/test/test_test_case_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_query import TestCaseQuery
+from qase.api_client_v1.models.test_case_query import TestCaseQuery
 
 class TestTestCaseQuery(unittest.TestCase):
     """TestCaseQuery unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -49,49 +49,49 @@
                 is_flaky = 56,
                 behavior = 56,
                 automation = 56,
                 status = 56,
                 milestone_id = 56,
                 suite_id = 56,
                 custom_fields = [
-                    src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                    qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                         id = 56, 
                         value = '', )
                     ],
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 steps_type = '',
                 steps = [
-                    src.qase.api_client_v1.models.test_step.TestStep(
+                    qase.api_client_v1.models.test_step.TestStep(
                         hash = '', 
                         shared_step_hash = '', 
                         shared_step_nested_hash = '', 
                         position = 56, 
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         attachments = [
-                            src.qase.api_client_v1.models.attachment.Attachment(
+                            qase.api_client_v1.models.attachment.Attachment(
                                 size = 56, 
                                 mime = '', 
                                 filename = '', 
                                 url = '', )
                             ], 
                         steps = [
                             None
                             ], )
                     ],
                 params = None,
                 tags = [
-                    src.qase.api_client_v1.models.tag_value.TagValue(
+                    qase.api_client_v1.models.tag_value.TagValue(
                         title = '', 
                         internal_id = 56, )
                     ],
                 member_id = 56,
                 author_id = 56,
                 created_at = '2021-12-30T19:23:59Z',
                 updated_at = '2021-12-30T19:23:59Z'
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_response.py` & `qase_api_client-1.0.0b2/test/test_test_case_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_response import TestCaseResponse
+from qase.api_client_v1.models.test_case_response import TestCaseResponse
 
 class TestTestCaseResponse(unittest.TestCase):
     """TestCaseResponse unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -33,15 +33,15 @@
             optional params are included """
         # uncomment below to create an instance of `TestCaseResponse`
         """
         model = TestCaseResponse()
         if include_optional:
             return TestCaseResponse(
                 status = True,
-                result = src.qase.api_client_v1.models.test_case.TestCase(
+                result = qase.api_client_v1.models.test_case.TestCase(
                     id = 56, 
                     position = 56, 
                     title = '', 
                     description = '', 
                     preconditions = '', 
                     postconditions = '', 
                     severity = 56, 
@@ -51,54 +51,54 @@
                     is_flaky = 56, 
                     behavior = 56, 
                     automation = 56, 
                     status = 56, 
                     milestone_id = 56, 
                     suite_id = 56, 
                     custom_fields = [
-                        src.qase.api_client_v1.models.custom_field_value.CustomFieldValue(
+                        qase.api_client_v1.models.custom_field_value.CustomFieldValue(
                             id = 56, 
                             value = '', )
                         ], 
                     attachments = [
-                        src.qase.api_client_v1.models.attachment.Attachment(
+                        qase.api_client_v1.models.attachment.Attachment(
                             size = 56, 
                             mime = '', 
                             filename = '', 
                             url = '', )
                         ], 
                     steps_type = '', 
                     steps = [
-                        src.qase.api_client_v1.models.test_step.TestStep(
+                        qase.api_client_v1.models.test_step.TestStep(
                             hash = '', 
                             shared_step_hash = '', 
                             shared_step_nested_hash = '', 
                             position = 56, 
                             action = '', 
                             expected_result = '', 
                             data = '', )
                         ], 
                     params = null, 
                     tags = [
-                        src.qase.api_client_v1.models.tag_value.TagValue(
+                        qase.api_client_v1.models.tag_value.TagValue(
                             title = '', 
                             internal_id = 56, )
                         ], 
                     member_id = 56, 
                     author_id = 56, 
                     created_at = '2021-12-30T19:23:59Z', 
                     updated_at = '2021-12-30T19:23:59Z', 
                     deleted = '2021-12-30T19:23:59.000000Z', 
                     created = '2021-12-30T19:23:59.000000Z', 
                     updated = '2021-12-30T19:23:59.000000Z', 
                     external_issues = [
-                        src.qase.api_client_v1.models.external_issue.ExternalIssue(
+                        qase.api_client_v1.models.external_issue.ExternalIssue(
                             type = '', 
                             issues = [
-                                src.qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
+                                qase.api_client_v1.models.external_issue_issues_inner.ExternalIssue_issues_inner(
                                     id = '', 
                                     link = '', )
                                 ], )
                         ], )
             )
         else:
             return TestCaseResponse(
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_case_update.py` & `qase_api_client-1.0.0b2/test/test_test_case_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_case_update import TestCaseUpdate
+from qase.api_client_v1.models.test_case_update import TestCaseUpdate
 
 class TestTestCaseUpdate(unittest.TestCase):
     """TestCaseUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -50,15 +50,15 @@
                 milestone_id = 56,
                 automation = 56,
                 status = 56,
                 attachments = [
                     ''
                     ],
                 steps = [
-                    src.qase.api_client_v1.models.test_step_create.TestStepCreate(
+                    qase.api_client_v1.models.test_step_create.TestStepCreate(
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         position = 56, 
                         attachments = [
                             ''
                             ],
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_casebulk.py` & `qase_api_client-1.0.0b2/test/test_test_casebulk.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_casebulk import TestCasebulk
+from qase.api_client_v1.models.test_casebulk import TestCasebulk
 
 class TestTestCasebulk(unittest.TestCase):
     """TestCasebulk unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_casebulk_cases_inner.py` & `qase_api_client-1.0.0b2/test/test_test_casebulk_cases_inner.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
+from qase.api_client_v1.models.test_casebulk_cases_inner import TestCasebulkCasesInner
 
 class TestTestCasebulkCasesInner(unittest.TestCase):
     """TestCasebulkCasesInner unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -51,15 +51,15 @@
                 milestone_id = 56,
                 automation = 56,
                 status = 56,
                 attachments = [
                     ''
                     ],
                 steps = [
-                    src.qase.api_client_v1.models.test_step_create.TestStepCreate(
+                    qase.api_client_v1.models.test_step_create.TestStepCreate(
                         action = '', 
                         expected_result = '', 
                         data = '', 
                         position = 56, 
                         attachments = [
                             ''
                             ], )
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_caseexternal_issues.py` & `qase_api_client-1.0.0b2/test/test_test_caseexternal_issues.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
+from qase.api_client_v1.models.test_caseexternal_issues import TestCaseexternalIssues
 
 class TestTestCaseexternalIssues(unittest.TestCase):
     """TestCaseexternalIssues unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -34,26 +34,26 @@
         # uncomment below to create an instance of `TestCaseexternalIssues`
         """
         model = TestCaseexternalIssues()
         if include_optional:
             return TestCaseexternalIssues(
                 type = 'jira-cloud',
                 links = [
-                    src.qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
+                    qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
                         case_id = 56, 
                         external_issues = [
                             ''
                             ], )
                     ]
             )
         else:
             return TestCaseexternalIssues(
                 type = 'jira-cloud',
                 links = [
-                    src.qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
+                    qase.api_client_v1.models.test_case_external_issues_links_inner.TestCaseExternalIssues_links_inner(
                         case_id = 56, 
                         external_issues = [
                             ''
                             ], )
                     ],
         )
         """
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_step.py` & `qase_api_client-1.0.0b2/test/test_test_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_step import TestStep
+from qase.api_client_v1.models.test_step import TestStep
 
 class TestTestStep(unittest.TestCase):
     """TestStep unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -40,15 +40,15 @@
                 shared_step_hash = '',
                 shared_step_nested_hash = '',
                 position = 56,
                 action = '',
                 expected_result = '',
                 data = '',
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 steps = [
                     None
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_step_create.py` & `qase_api_client-1.0.0b2/test/test_test_step_result_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,51 +11,54 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_step_create import TestStepCreate
+from qase.api_client_v1.models.test_step_result_create import TestStepResultCreate
 
-class TestTestStepCreate(unittest.TestCase):
-    """TestStepCreate unit test stubs"""
+class TestTestStepResultCreate(unittest.TestCase):
+    """TestStepResultCreate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TestStepCreate:
-        """Test TestStepCreate
+    def make_instance(self, include_optional) -> TestStepResultCreate:
+        """Test TestStepResultCreate
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TestStepCreate`
+        # uncomment below to create an instance of `TestStepResultCreate`
         """
-        model = TestStepCreate()
+        model = TestStepResultCreate()
         if include_optional:
-            return TestStepCreate(
-                action = '',
-                expected_result = '',
-                data = '',
+            return TestStepResultCreate(
                 position = 56,
+                status = 'passed',
+                comment = '',
                 attachments = [
                     ''
                     ],
+                action = '',
+                expected_result = '',
+                data = '',
                 steps = [
                     None
                     ]
             )
         else:
-            return TestStepCreate(
+            return TestStepResultCreate(
+                status = 'passed',
         )
         """
 
-    def testTestStepCreate(self):
-        """Test TestStepCreate"""
+    def testTestStepResultCreate(self):
+        """Test TestStepResultCreate"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qase_api_client-1.0.0b1/test/test_test_step_result.py` & `qase_api_client-1.0.0b2/test/test_test_step_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v1.models.test_step_result import TestStepResult
+from qase.api_client_v1.models.test_step_result import TestStepResult
 
 class TestTestStepResult(unittest.TestCase):
     """TestStepResult unit test stubs"""
 
     def setUp(self):
         pass
 
@@ -35,15 +35,15 @@
         """
         model = TestStepResult()
         if include_optional:
             return TestStepResult(
                 status = 56,
                 position = 56,
                 attachments = [
-                    src.qase.api_client_v1.models.attachment.Attachment(
+                    qase.api_client_v1.models.attachment.Attachment(
                         size = 56, 
                         mime = '', 
                         filename = '', 
                         url = '', )
                     ],
                 steps = [
                     None
```

