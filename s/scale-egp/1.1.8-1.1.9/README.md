# Comparing `tmp/scale_egp-1.1.8.tar.gz` & `tmp/scale_egp-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_egp-1.1.8.tar", max compression
+gzip compressed data, was "scale_egp-1.1.9.tar", max compression
```

## Comparing `scale_egp-1.1.8.tar` & `scale_egp-1.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    17873 2024-05-22 22:08:13.394012 scale_egp-1.1.8/README.md
--rw-r--r--   0        0        0     1138 2024-05-22 22:08:13.394012 scale_egp-1.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/__init__.py
--rw-r--r--   0        0        0       74 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/__init__.py
--rw-r--r--   0        0        0     4791 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/cli_main.py
--rw-r--r--   0        0        0    18199 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/collections.py
--rw-r--r--   0        0        0     7857 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/formatter.py
--rw-r--r--   0        0        0     1469 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/model_instance_description.py
--rw-r--r--   0        0        0     1828 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/parser.py
--rw-r--r--   0        0        0    52384 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/vpc_setup_commands.py
--rw-r--r--   0        0        0     1733 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/__init__.py
--rw-r--r--   0        0        0    13096 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/client.py
--rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/__init__.py
--rw-r--r--   0        0        0     2914 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/application_specs.py
--rw-r--r--   0        0        0     3170 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/chunks.py
--rw-r--r--   0        0        0     5476 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/completions.py
--rw-r--r--   0        0        0     2500 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_configs.py
--rw-r--r--   0        0        0    25385 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_datasets.py
--rw-r--r--   0        0        0     8055 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/evaluations.py
--rw-r--r--   0        0        0     4918 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/fine_tuning.py
--rw-r--r--   0        0        0    25810 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/knowledge_bases.py
--rw-r--r--   0        0        0     2685 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/model_groups.py
--rw-r--r--   0        0        0     4798 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/model_templates.py
--rw-r--r--   0        0        0     7667 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/models.py
--rw-r--r--   0        0        0     1862 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/question_sets.py
--rw-r--r--   0        0        0     2588 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/questions.py
--rw-r--r--   0        0        0     1510 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/users.py
--rw-r--r--   0        0        0        0 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/constants/__init__.py
--rw-r--r--   0        0        0      762 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/constants/model_schemas.py
--rw-r--r--   0        0        0     9257 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/enums.py
--rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/__init__.py
--rw-r--r--   0        0        0     2712 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/fine_tuning_jobs.py
--rw-r--r--   0        0        0     2126 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/model_enums.py
--rw-r--r--   0        0        0     8545 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/model_vendor_configuration.py
--rw-r--r--   0        0        0      647 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/__init__.py
--rw-r--r--   0        0        0     4651 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/agents.py
--rw-r--r--   0        0        0      741 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/application_specs.py
--rw-r--r--   0        0        0     6125 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/chunks.py
--rw-r--r--   0        0        0     6750 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/completions.py
--rw-r--r--   0        0        0     1016 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/embeddings.py
--rw-r--r--   0        0        0     1019 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_configs.py
--rw-r--r--   0        0        0     3551 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_dataset_test_cases.py
--rw-r--r--   0        0        0     1686 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_datasets.py
--rw-r--r--   0        0        0     4837 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_test_case_results.py
--rw-r--r--   0        0        0     1398 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluations.py
--rw-r--r--   0        0        0     3401 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/fine_tuning.py
--rw-r--r--   0        0        0     1860 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_artifacts.py
--rw-r--r--   0        0        0     1559 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_chunks.py
--rw-r--r--   0        0        0    15686 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_uploads.py
--rw-r--r--   0        0        0     1863 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_bases.py
--rw-r--r--   0        0        0     1112 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/memory_strategy.py
--rw-r--r--   0        0        0     2478 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/message.py
--rw-r--r--   0        0        0     3557 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/model_templates.py
--rw-r--r--   0        0        0    14065 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/models.py
--rw-r--r--   0        0        0     1086 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/models_group.py
--rw-r--r--   0        0        0      891 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/question_sets.py
--rw-r--r--   0        0        0     5234 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/questions.py
--rw-r--r--   0        0        0      410 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/user_info.py
--rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/__init__.py
--rw-r--r--   0        0        0    11461 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/api_utils.py
--rw-r--r--   0        0        0     3639 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/model_utils.py
--rw-r--r--   0        0        0      107 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/strenum_compat.py
--rw-r--r--   0        0        0    18948 1970-01-01 00:00:00.000000 scale_egp-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    17873 2024-05-29 22:40:02.515356 scale_egp-1.1.9/README.md
+-rw-r--r--   0        0        0     1138 2024-05-29 22:40:02.515356 scale_egp-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/__init__.py
+-rw-r--r--   0        0        0       74 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/__init__.py
+-rw-r--r--   0        0        0     4791 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/cli_main.py
+-rw-r--r--   0        0        0    18199 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/collections.py
+-rw-r--r--   0        0        0     7857 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/formatter.py
+-rw-r--r--   0        0        0     1469 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/model_instance_description.py
+-rw-r--r--   0        0        0     1828 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/parser.py
+-rw-r--r--   0        0        0    52384 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/cli/vpc_setup_commands.py
+-rw-r--r--   0        0        0     1733 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/__init__.py
+-rw-r--r--   0        0        0    13096 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/client.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/__init__.py
+-rw-r--r--   0        0        0     2914 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/application_specs.py
+-rw-r--r--   0        0        0     3170 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/chunks.py
+-rw-r--r--   0        0        0     5476 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/completions.py
+-rw-r--r--   0        0        0     2500 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/evaluation_configs.py
+-rw-r--r--   0        0        0    25385 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/evaluation_datasets.py
+-rw-r--r--   0        0        0     8055 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/evaluations.py
+-rw-r--r--   0        0        0     4918 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/fine_tuning.py
+-rw-r--r--   0        0        0    25810 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/knowledge_bases.py
+-rw-r--r--   0        0        0     2685 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/model_groups.py
+-rw-r--r--   0        0        0     4798 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/sdk/collections/model_templates.py
+-rw-r--r--   0        0        0     7667 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/collections/models.py
+-rw-r--r--   0        0        0     1862 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/collections/question_sets.py
+-rw-r--r--   0        0        0     2588 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/collections/questions.py
+-rw-r--r--   0        0        0     1510 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/collections/users.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/constants/__init__.py
+-rw-r--r--   0        0        0      762 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/constants/model_schemas.py
+-rw-r--r--   0        0        0     9319 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/enums.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/models/__init__.py
+-rw-r--r--   0        0        0     2712 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/models/fine_tuning_jobs.py
+-rw-r--r--   0        0        0     2126 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/models/model_enums.py
+-rw-r--r--   0        0        0     8545 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/models/model_vendor_configuration.py
+-rw-r--r--   0        0        0      647 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/__init__.py
+-rw-r--r--   0        0        0     4651 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/agents.py
+-rw-r--r--   0        0        0      741 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/application_specs.py
+-rw-r--r--   0        0        0     6125 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/chunks.py
+-rw-r--r--   0        0        0     6750 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/completions.py
+-rw-r--r--   0        0        0     1016 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/embeddings.py
+-rw-r--r--   0        0        0     1019 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/evaluation_configs.py
+-rw-r--r--   0        0        0     3551 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/evaluation_dataset_test_cases.py
+-rw-r--r--   0        0        0     1686 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/evaluation_datasets.py
+-rw-r--r--   0        0        0     4837 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/evaluation_test_case_results.py
+-rw-r--r--   0        0        0     1398 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/evaluations.py
+-rw-r--r--   0        0        0     3417 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/fine_tuning.py
+-rw-r--r--   0        0        0     1860 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/knowledge_base_artifacts.py
+-rw-r--r--   0        0        0     1559 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/knowledge_base_chunks.py
+-rw-r--r--   0        0        0    15686 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/knowledge_base_uploads.py
+-rw-r--r--   0        0        0     1863 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/knowledge_bases.py
+-rw-r--r--   0        0        0     1112 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/memory_strategy.py
+-rw-r--r--   0        0        0     2478 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/message.py
+-rw-r--r--   0        0        0     3557 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/model_templates.py
+-rw-r--r--   0        0        0    14103 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/models.py
+-rw-r--r--   0        0        0     1086 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/models_group.py
+-rw-r--r--   0        0        0      891 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/question_sets.py
+-rw-r--r--   0        0        0     5234 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/questions.py
+-rw-r--r--   0        0        0      410 2024-05-29 22:40:02.519356 scale_egp-1.1.9/scale_egp/sdk/types/user_info.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/utils/__init__.py
+-rw-r--r--   0        0        0    11461 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/utils/api_utils.py
+-rw-r--r--   0        0        0     3639 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/utils/model_utils.py
+-rw-r--r--   0        0        0      107 2024-05-29 22:40:02.515356 scale_egp-1.1.9/scale_egp/utils/strenum_compat.py
+-rw-r--r--   0        0        0    18948 1970-01-01 00:00:00.000000 scale_egp-1.1.9/PKG-INFO
```

### Comparing `scale_egp-1.1.8/README.md` & `scale_egp-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/pyproject.toml` & `scale_egp-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scale-egp"
-version = "1.1.8"
+version = "1.1.9"
 description = "SDK for Scale SGP API"
 license = "Apache 2.0 modified with Commons Clause"
 authors = ["Scale SGP team"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/sgp-py/"
 repository = "https://github.com/scaleapi/egp-py"
 packages = [{include = "scale_egp"}]
```

### Comparing `scale_egp-1.1.8/scale_egp/cli/cli_main.py` & `scale_egp-1.1.9/scale_egp/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/cli/collections.py` & `scale_egp-1.1.9/scale_egp/cli/collections.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/cli/formatter.py` & `scale_egp-1.1.9/scale_egp/cli/formatter.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/cli/model_instance_description.py` & `scale_egp-1.1.9/scale_egp/cli/model_instance_description.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/cli/parser.py` & `scale_egp-1.1.9/scale_egp/cli/parser.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/cli/vpc_setup_commands.py` & `scale_egp-1.1.9/scale_egp/cli/vpc_setup_commands.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/exceptions.py` & `scale_egp-1.1.9/scale_egp/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/client.py` & `scale_egp-1.1.9/scale_egp/sdk/client.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/application_specs.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/chunks.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/completions.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_configs.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_datasets.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/evaluations.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/fine_tuning.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/knowledge_bases.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/model_groups.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/model_groups.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/model_templates.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/models.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/question_sets.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/questions.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/collections/users.py` & `scale_egp-1.1.9/scale_egp/sdk/collections/users.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/constants/model_schemas.py` & `scale_egp-1.1.9/scale_egp/sdk/constants/model_schemas.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/enums.py` & `scale_egp-1.1.9/scale_egp/sdk/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     Currently only human evaluations are supported.
 
     Attributes:
         HUMAN: Denotes that an evaluation is a human evaluation.
     """
 
     HUMAN = "human"
+    LLM_AUTO = "llm_auto"
+    LLM_BENCHMARK = "llm_benchmark"
 
 
 class QuestionType(str, Enum):
     """
     An enum representing the different types of questions.
 
     This is used to specify the type of a question.
```

### Comparing `scale_egp-1.1.8/scale_egp/sdk/models/fine_tuning_jobs.py` & `scale_egp-1.1.9/scale_egp/sdk/models/fine_tuning_jobs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/models/model_enums.py` & `scale_egp-1.1.9/scale_egp/sdk/models/model_enums.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/models/model_vendor_configuration.py` & `scale_egp-1.1.9/scale_egp/sdk/models/model_vendor_configuration.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/__init__.py` & `scale_egp-1.1.9/scale_egp/sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/agents.py` & `scale_egp-1.1.9/scale_egp/sdk/types/agents.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/application_specs.py` & `scale_egp-1.1.9/scale_egp/sdk/types/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/chunks.py` & `scale_egp-1.1.9/scale_egp/sdk/types/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/completions.py` & `scale_egp-1.1.9/scale_egp/sdk/types/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/embeddings.py` & `scale_egp-1.1.9/scale_egp/sdk/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_configs.py` & `scale_egp-1.1.9/scale_egp/sdk/types/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_dataset_test_cases.py` & `scale_egp-1.1.9/scale_egp/sdk/types/evaluation_dataset_test_cases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_datasets.py` & `scale_egp-1.1.9/scale_egp/sdk/types/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_test_case_results.py` & `scale_egp-1.1.9/scale_egp/sdk/types/evaluation_test_case_results.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/evaluations.py` & `scale_egp-1.1.9/scale_egp/sdk/types/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/fine_tuning.py` & `scale_egp-1.1.9/scale_egp/sdk/types/fine_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # !!!!! DO NOT EVER CHANGE THIS FILE MANUALLY -- AUTOGENERATED by orm2pydantic.py !!!!!
-# Generated on 2024-04-17 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
+# Generated from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
 # To regenerate this file, run:
 # scaleapi/packages/egp-api-backend/scripts/orm2pydantic.sh
 
 from scale_egp.utils.model_utils import BaseModel, Entity
 from pydantic import Field
 
 from datetime import (datetime)
 from scale_egp.sdk.models.fine_tuning_jobs import (FineTuningJobStatus, FineTuningJobVendorConfiguration, TrainingDatasetORMSchemaTypeEnum)
 from scale_egp.utils.model_utils import (BaseModel)
 from scale_egp.utils.strenum_compat import (StrEnum)
 from typing import (Optional)
-DataSource = StrEnum('DataSource', [('S3', 'S3'), ('SHARE_POINT', 'SharePoint'), ('LOCAL_FILE', 'LocalFile'), ('LOCAL_CHUNKS', 'LocalChunks'), ('GOOGLE_DRIVE', 'GoogleDrive'), ('AZURE_BLOB_STORAGE', 'AzureBlobStorage')])
+DataSource = StrEnum('DataSource', [('S3', 'S3'), ('SHARE_POINT', 'SharePoint'), ('LOCAL_FILE', 'LocalFile'), ('LOCAL_CHUNKS', 'LocalChunks'), ('GOOGLE_DRIVE', 'GoogleDrive'), ('AZURE_BLOB_STORAGE', 'AzureBlobStorage'), ('CONFLUENCE', 'Confluence')])
 class TrainingDatasetRequest(BaseModel):
     name: str = Field(..., description="The name of the dataset")
     schema_type: TrainingDatasetORMSchemaTypeEnum = Field(..., description="The schema type of the dataset, currently only GENERATION is supported")
     data_source: DataSource = Field(..., description="The data source of the dataset, used to determine how to parse the location")
     account_id: str = Field(..., description="The ID of the account that owns the given entity.", can_patch=False)
```

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_artifacts.py` & `scale_egp-1.1.9/scale_egp/sdk/types/knowledge_base_artifacts.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_chunks.py` & `scale_egp-1.1.9/scale_egp/sdk/types/knowledge_base_chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_uploads.py` & `scale_egp-1.1.9/scale_egp/sdk/types/knowledge_base_uploads.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_bases.py` & `scale_egp-1.1.9/scale_egp/sdk/types/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/memory_strategy.py` & `scale_egp-1.1.9/scale_egp/sdk/types/memory_strategy.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/message.py` & `scale_egp-1.1.9/scale_egp/sdk/types/message.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/model_templates.py` & `scale_egp-1.1.9/scale_egp/sdk/types/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/models.py` & `scale_egp-1.1.9/scale_egp/sdk/types/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         stop_sequences: List of up to 4 sequences where the API will stop generating further tokens.
             The returned text will not contain the stop sequence.
         max_tokens: The maximum number of tokens to generate in the completion. The token count
             of your prompt plus max_tokens cannot exceed the model's context length. If not,
             specified, max_tokens will be determined based on the model used.
         prompts: List of prompts to generate completions for.
     """
-    
+
     temperature: float = Field(
         default=0.2,
         ge=0.0,
         le=1.0,
     )
     stop_sequences: Optional[List[str]] = Field(
         default=None,
@@ -303,14 +303,15 @@
 
     Attributes:
         embeddings: List of text, embedding pairs.
     """
 
     # List of text, embedding pairs, eg: [("text to embed", [1.0, 1.05, 2.07, ...]), ...]
     embeddings: List[Tuple[str, List[float]]]
+    tokens_used: Optional[int] = Field(0)
 
 
 class RerankingRequest(BaseModelRequest):
     """
     Request schema for reranking models.
 
     Attributes:
```

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/models_group.py` & `scale_egp-1.1.9/scale_egp/sdk/types/models_group.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/question_sets.py` & `scale_egp-1.1.9/scale_egp/sdk/types/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/sdk/types/questions.py` & `scale_egp-1.1.9/scale_egp/sdk/types/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/utils/api_utils.py` & `scale_egp-1.1.9/scale_egp/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/scale_egp/utils/model_utils.py` & `scale_egp-1.1.9/scale_egp/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.8/PKG-INFO` & `scale_egp-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-egp
-Version: 1.1.8
+Version: 1.1.9
 Summary: SDK for Scale SGP API
 Home-page: https://scaleapi.github.io/sgp-py/
 License: Apache 2.0 modified with Commons Clause
 Author: Scale SGP team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

