# Comparing `tmp/sapientml_core-0.5.5.tar.gz` & `tmp/sapientml_core-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapientml_core-0.5.5.tar", max compression
+gzip compressed data, was "sapientml_core-0.5.6.tar", max compression
```

## Comparing `sapientml_core-0.5.5.tar` & `sapientml_core-0.5.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0    11356 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/LICENSE
--rw-r--r--   0        0        0     1669 2024-05-23 05:03:54.793486 sapientml_core-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      717 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/__init__.py
--rw-r--r--   0        0        0      585 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/__init__.py
--rw-r--r--   0        0        0     2513 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/artifacts/label_order.json
--rw-r--r--   0        0        0      585 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/__init__.py
--rw-r--r--   0        0        0    31184 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/pipeline_template.py
--rw-r--r--   0        0        0     2626 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/predicate.py
--rw-r--r--   0        0        0     4438 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/preprocessing_label.py
--rw-r--r--   0        0        0    17616 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/template_based_adaptation.py
--rw-r--r--   0        0        0        0 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/__init__.py
--rw-r--r--   0        0        0     2993 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/label_util.py
--rw-r--r--   0        0        0     2762 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/pp_component_groups.py
--rw-r--r--   0        0        0     2177 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/search_space.py
--rw-r--r--   0        0        0      899 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/enums.py
--rw-r--r--   0        0        0    17237 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/AutoEDA.py
--rw-r--r--   0        0        0    17606 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/AutoVisualization.py
--rw-r--r--   0        0        0    40509 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/code_miner.py
--rw-r--r--   0        0        0     1268 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/code_template.py
--rw-r--r--   0        0        0     3779 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/main.py
--rw-r--r--   0        0        0    20803 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/pipeline_explanation.py
--rw-r--r--   0        0        0      493 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/explain/templates/jupyter_content.json
--rw-r--r--   0        0        0    16874 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/generator.py
--rw-r--r--   0        0        0     1242 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/internal_path.py
--rw-r--r--   0        0        0    40076 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/meta_features.py
--rw-r--r--   0        0        0    23893 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/feature_importance.json
--rw-r--r--   0        0        0    59630 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/model_metafeatures_test.csv
--rw-r--r--   0        0        0     5658 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/mp_model_1.pkl
--rw-r--r--   0        0        0   223570 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/mp_model_2.pkl
--rw-r--r--   0        0        0    12634 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/pp_models.pkl
--rw-r--r--   0        0        0    17835 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/params.py
--rw-r--r--   0        0        0     1923 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/ps_macros.py
--rw-r--r--   0        0        0      585 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/seeding/__init__.py
--rw-r--r--   0        0        0     9591 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/seeding/predictor.py
--rw-r--r--   0        0        0     7667 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/component_description.json
--rw-r--r--   0        0        0      172 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/model_explanation.py.jinja
--rw-r--r--   0        0        0      683 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja
--rw-r--r--   0        0        0      281 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/classification_post_process.jinja
--rw-r--r--   0        0        0     4986 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja
--rw-r--r--   0        0        0    12287 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters.py.jinja
--rw-r--r--   0        0        0     3934 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja
--rw-r--r--   0        0        0     2551 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model.py.jinja
--rw-r--r--   0        0        0     1086 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_predict.py.jinja
--rw-r--r--   0        0        0     2540 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_test.py.jinja
--rw-r--r--   0        0        0     1797 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_train.py.jinja
--rw-r--r--   0        0        0      563 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/confusion_matrix.py.jinja
--rw-r--r--   0        0        0      285 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/drop_columns.py.jinja
--rw-r--r--   0        0        0     5098 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation.py.jinja
--rw-r--r--   0        0        0     4718 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation_test.py.jinja
--rw-r--r--   0        0        0     3848 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja
--rw-r--r--   0        0        0      662 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/inverse_target.py.jinja
--rw-r--r--   0        0        0     1082 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/permutation_importance.py.jinja
--rw-r--r--   0        0        0     2641 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/prediction_result.py.jinja
--rw-r--r--   0        0        0      398 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/preprocess_dataset.py.jinja
--rw-r--r--   0        0        0      728 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/shap.py.jinja
--rw-r--r--   0        0        0      285 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_predict.py.jinja
--rw-r--r--   0        0        0      396 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_test.py.jinja
--rw-r--r--   0        0        0      178 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_train.py.jinja
--rw-r--r--   0        0        0      287 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_validation.py.jinja
--rw-r--r--   0        0        0     1685 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_predict.py.jinja
--rw-r--r--   0        0        0     2472 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_test.py.jinja
--rw-r--r--   0        0        0     1426 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_train.py.jinja
--rw-r--r--   0        0        0     1676 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_validation.py.jinja
--rw-r--r--   0        0        0      953 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE.py.jinja
--rw-r--r--   0        0        0      495 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE_predict.jinja
--rw-r--r--   0        0        0      507 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE_train.jinja
--rw-r--r--   0        0        0      381 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/LabelEncoder.py.jinja
--rw-r--r--   0        0        0      217 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/LabelEncoder_predict.py.jinja
--rw-r--r--   0        0        0      360 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/LabelEncoder_train.py.jinja
--rw-r--r--   0        0        0      633 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing.py.jinja
--rw-r--r--   0        0        0      577 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja
--rw-r--r--   0        0        0      579 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja
--rw-r--r--   0        0        0      460 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/SMOTE.py.jinja
--rw-r--r--   0        0        0      562 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja
--rw-r--r--   0        0        0      384 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD_predict.py.jinja
--rw-r--r--   0        0        0      491 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD_train.py.jinja
--rw-r--r--   0        0        0     3280 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja
--rw-r--r--   0        0        0      763 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja
--rw-r--r--   0        0        0     2561 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja
--rw-r--r--   0        0        0      814 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja
--rw-r--r--   0        0        0      520 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja
--rw-r--r--   0        0        0      659 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja
--rw-r--r--   0        0        0     1031 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja
--rw-r--r--   0        0        0      620 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja
--rw-r--r--   0        0        0      770 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja
--rw-r--r--   0        0        0      794 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja
--rw-r--r--   0        0        0      425 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies_predict.py.jinja
--rw-r--r--   0        0        0      561 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja
--rw-r--r--   0        0        0      365 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/log.py.jinja
--rw-r--r--   0        0        0      266 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/log_predict.py.jinja
--rw-r--r--   0        0        0      156 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/log_train.py.jinja
--rw-r--r--   0        0        0     4623 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_results.py
--rw-r--r--   0        0        0     8573 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_runner.py
--rw-r--r--   0        0        0    32944 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/augmentation/mutator.py
--rw-r--r--   0        0        0     5241 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/ast_operation.py
--rw-r--r--   0        0        0    12596 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/dependent_api_extractor.py
--rw-r--r--   0        0        0     2762 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/determine_label_order.py
--rw-r--r--   0        0        0     7850 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/ast_info_collector.py
--rw-r--r--   0        0        0     8533 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/dataset_snapshot_extractor.py
--rw-r--r--   0        0        0     7987 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/determine_used_features.py
--rw-r--r--   0        0        0     1474 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/df_collector.py
--rw-r--r--   0        0        0     4791 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/static_analysis_of_columns.py
--rw-r--r--   0        0        0     7965 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/meta_feature_extractor.py
--rw-r--r--   0        0        0     6219 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/meta_feature_selector.py
--rw-r--r--   0        0        0    10682 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/meta_model_trainer.py
--rw-r--r--   0        0        0     5210 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/pp_model_trainer.py
--rw-r--r--   0        0        0      923 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/project.py
--rw-r--r--   0        0        0     4533 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/project_corpus.py
--rw-r--r--   0        0        0     5313 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/util/file_util.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 sapientml_core-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/LICENSE
+-rw-r--r--   0        0        0     1669 2024-05-30 02:24:40.001958 sapientml_core-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      717 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/__init__.py
+-rw-r--r--   0        0        0     2513 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/artifacts/label_order.json
+-rw-r--r--   0        0        0      585 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/generation/__init__.py
+-rw-r--r--   0        0        0    31184 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/generation/pipeline_template.py
+-rw-r--r--   0        0        0     2626 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/generation/predicate.py
+-rw-r--r--   0        0        0     4438 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/generation/preprocessing_label.py
+-rw-r--r--   0        0        0    17616 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/adaptation/generation/template_based_adaptation.py
+-rw-r--r--   0        0        0        0 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/design/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/design/label_util.py
+-rw-r--r--   0        0        0     2762 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/design/pp_component_groups.py
+-rw-r--r--   0        0        0     2177 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/design/search_space.py
+-rw-r--r--   0        0        0      899 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/enums.py
+-rw-r--r--   0        0        0    17237 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/AutoEDA.py
+-rw-r--r--   0        0        0    17606 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/AutoVisualization.py
+-rw-r--r--   0        0        0    40509 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/code_miner.py
+-rw-r--r--   0        0        0     1268 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/code_template.py
+-rw-r--r--   0        0        0     3779 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/main.py
+-rw-r--r--   0        0        0    20803 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/pipeline_explanation.py
+-rw-r--r--   0        0        0      493 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/explain/templates/jupyter_content.json
+-rw-r--r--   0        0        0    16874 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/generator.py
+-rw-r--r--   0        0        0     1242 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/internal_path.py
+-rw-r--r--   0        0        0    40076 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/meta_features.py
+-rw-r--r--   0        0        0    23893 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/models/feature_importance.json
+-rw-r--r--   0        0        0    59630 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/models/model_metafeatures_test.csv
+-rw-r--r--   0        0        0     5658 2024-05-30 02:24:26.037904 sapientml_core-0.5.6/sapientml_core/models/mp_model_1.pkl
+-rw-r--r--   0        0        0   223570 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/models/mp_model_2.pkl
+-rw-r--r--   0        0        0    12634 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/models/pp_models.pkl
+-rw-r--r--   0        0        0    17835 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/params.py
+-rw-r--r--   0        0        0     1923 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/ps_macros.py
+-rw-r--r--   0        0        0      585 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/seeding/__init__.py
+-rw-r--r--   0        0        0     9591 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/seeding/predictor.py
+-rw-r--r--   0        0        0     7667 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/explainability_templates/component_description.json
+-rw-r--r--   0        0        0      172 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/explainability_templates/model_explanation.py.jinja
+-rw-r--r--   0        0        0      683 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja
+-rw-r--r--   0        0        0      281 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/classification_post_process.jinja
+-rw-r--r--   0        0        0     4986 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja
+-rw-r--r--   0        0        0    12287 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/hyperparameters.py.jinja
+-rw-r--r--   0        0        0     3934 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja
+-rw-r--r--   0        0        0     2551 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/model.py.jinja
+-rw-r--r--   0        0        0     1086 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/model_predict.py.jinja
+-rw-r--r--   0        0        0     2540 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/model_test.py.jinja
+-rw-r--r--   0        0        0     1797 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/model_templates/model_train.py.jinja
+-rw-r--r--   0        0        0      563 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/confusion_matrix.py.jinja
+-rw-r--r--   0        0        0      285 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/drop_columns.py.jinja
+-rw-r--r--   0        0        0     5098 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/evaluation.py.jinja
+-rw-r--r--   0        0        0     4718 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/evaluation_test.py.jinja
+-rw-r--r--   0        0        0     3848 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja
+-rw-r--r--   0        0        0      662 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/inverse_target.py.jinja
+-rw-r--r--   0        0        0     1082 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/permutation_importance.py.jinja
+-rw-r--r--   0        0        0     2641 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/prediction_result.py.jinja
+-rw-r--r--   0        0        0      398 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/preprocess_dataset.py.jinja
+-rw-r--r--   0        0        0      728 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/shap.py.jinja
+-rw-r--r--   0        0        0      285 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/target_separation_predict.py.jinja
+-rw-r--r--   0        0        0      396 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/target_separation_test.py.jinja
+-rw-r--r--   0        0        0      178 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/target_separation_train.py.jinja
+-rw-r--r--   0        0        0      287 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/other_templates/target_separation_validation.py.jinja
+-rw-r--r--   0        0        0     1685 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/pipeline_predict.py.jinja
+-rw-r--r--   0        0        0     2472 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/pipeline_test.py.jinja
+-rw-r--r--   0        0        0     1426 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/pipeline_train.py.jinja
+-rw-r--r--   0        0        0     1676 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/pipeline_validation.py.jinja
+-rw-r--r--   0        0        0      953 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/DATE.py.jinja
+-rw-r--r--   0        0        0      495 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/DATE_predict.jinja
+-rw-r--r--   0        0        0      507 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/DATE_train.jinja
+-rw-r--r--   0        0        0      381 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/LabelEncoder.py.jinja
+-rw-r--r--   0        0        0      217 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/LabelEncoder_predict.py.jinja
+-rw-r--r--   0        0        0      360 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/LabelEncoder_train.py.jinja
+-rw-r--r--   0        0        0      633 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/Processing.py.jinja
+-rw-r--r--   0        0        0      577 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja
+-rw-r--r--   0        0        0      579 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja
+-rw-r--r--   0        0        0      460 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/SMOTE.py.jinja
+-rw-r--r--   0        0        0      562 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja
+-rw-r--r--   0        0        0      384 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/STANDARD_predict.py.jinja
+-rw-r--r--   0        0        0      491 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/STANDARD_train.py.jinja
+-rw-r--r--   0        0        0     3280 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja
+-rw-r--r--   0        0        0      763 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja
+-rw-r--r--   0        0        0     2561 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja
+-rw-r--r--   0        0        0      814 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja
+-rw-r--r--   0        0        0      520 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja
+-rw-r--r--   0        0        0      659 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja
+-rw-r--r--   0        0        0     1031 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja
+-rw-r--r--   0        0        0      620 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja
+-rw-r--r--   0        0        0      770 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja
+-rw-r--r--   0        0        0      794 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja
+-rw-r--r--   0        0        0      425 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/get_dummies_predict.py.jinja
+-rw-r--r--   0        0        0      561 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja
+-rw-r--r--   0        0        0      365 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/log.py.jinja
+-rw-r--r--   0        0        0      266 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/log_predict.py.jinja
+-rw-r--r--   0        0        0      156 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/log_train.py.jinja
+-rw-r--r--   0        0        0     4623 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/augmentation/mutation_results.py
+-rw-r--r--   0        0        0     8573 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/augmentation/mutation_runner.py
+-rw-r--r--   0        0        0    32944 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/augmentation/mutator.py
+-rw-r--r--   0        0        0     5241 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/dataflowmodel/ast_operation.py
+-rw-r--r--   0        0        0    12596 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/dataflowmodel/dependent_api_extractor.py
+-rw-r--r--   0        0        0     2762 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/dataflowmodel/determine_label_order.py
+-rw-r--r--   0        0        0     7850 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/denoising/ast_info_collector.py
+-rw-r--r--   0        0        0     8533 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/denoising/dataset_snapshot_extractor.py
+-rw-r--r--   0        0        0     7987 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/denoising/determine_used_features.py
+-rw-r--r--   0        0        0     1474 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/denoising/df_collector.py
+-rw-r--r--   0        0        0     4791 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/denoising/static_analysis_of_columns.py
+-rw-r--r--   0        0        0     7965 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/meta_feature_extractor.py
+-rw-r--r--   0        0        0     6219 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/meta_feature_selector.py
+-rw-r--r--   0        0        0    10682 2024-05-30 02:24:26.041904 sapientml_core-0.5.6/sapientml_core/training/meta_model_trainer.py
+-rw-r--r--   0        0        0     5210 2024-05-30 02:24:26.045904 sapientml_core-0.5.6/sapientml_core/training/pp_model_trainer.py
+-rw-r--r--   0        0        0      923 2024-05-30 02:24:26.045904 sapientml_core-0.5.6/sapientml_core/training/project.py
+-rw-r--r--   0        0        0     4533 2024-05-30 02:24:26.045904 sapientml_core-0.5.6/sapientml_core/training/project_corpus.py
+-rw-r--r--   0        0        0     5313 2024-05-30 02:24:26.045904 sapientml_core-0.5.6/sapientml_core/util/file_util.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 sapientml_core-0.5.6/PKG-INFO
```

### Comparing `sapientml_core-0.5.5/LICENSE` & `sapientml_core-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/pyproject.toml` & `sapientml_core-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "A SapientML plugin of SapientMLGenerator"
 license = "Apache-2.0"
 maintainers = [
   "Kosaku Kimura <kimura.kosaku@fujitsu.com>",
   "Akira Ura <ura.akira@fujitsu.com>",
 ]
 name = "sapientml-core"
-version = "0.5.5"
+version = "0.5.6"
 
 [tool.poetry.dependencies]
 catboost = ">=1.2.3"
 imbalanced-learn = ">=0.11,<0.13"
 ipykernel = "^6.25.1"
 japanize-matplotlib = "^1.1.3"
 jinja2 = "^3.1.2"
@@ -25,15 +25,15 @@
 python = ">=3.10,<3.13"
 sapientml = "*"
 sapientml-loaddata = "*"
 sapientml-preprocess = "*"
 scikit-learn = "1.3.2"
 scipy = "^1.11.1"
 seaborn = ">=0.12.2,<0.14.0"
-shap = ">=0.43,<0.45"
+shap = ">=0.43,<0.46"
 tqdm = "^4.66.1"
 xgboost = ">=1.7.6,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7,<25.0"
 flake8 = ">=6.1,<8.0"
 isort = "^5.12.0"
@@ -50,26 +50,26 @@
 [tool.poetry.plugins."sapientml.pipeline_generator"]
 sapientml = "sapientml_core:SapientMLGenerator"
 
 [tool.poetry.plugins."sapientml.config"]
 sapientml = "sapientml_core:SapientMLConfig"
 
 [tool.pysen]
-version = "0.5.5"
+version = "0.5.6"
 
 [tool.pysen-cli]
 settings_dir = ".pysen"
 
 [tool.pysen.lint]
 enable_black = true
 enable_flake8 = true
 enable_isort = true
 enable_mypy = false
 line_length = 120
-py_version = "0.5.5"
+py_version = "0.5.6"
 
 [tool.pysen.lint.source]
 includes = ["sapientml_core/", "tests/"]
 
 [tool.pytest.ini_options]
 addopts = "-s -x --cov=sapientml_core"
 testpaths = ["tests"]
```

### Comparing `sapientml_core-0.5.5/sapientml_core/__init__.py` & `sapientml_core-0.5.6/sapientml_core/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/__init__.py` & `sapientml_core-0.5.6/sapientml_core/adaptation/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/artifacts/label_order.json` & `sapientml_core-0.5.6/sapientml_core/adaptation/artifacts/label_order.json`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/generation/__init__.py` & `sapientml_core-0.5.6/sapientml_core/adaptation/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/generation/pipeline_template.py` & `sapientml_core-0.5.6/sapientml_core/adaptation/generation/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/generation/predicate.py` & `sapientml_core-0.5.6/sapientml_core/adaptation/generation/predicate.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/generation/preprocessing_label.py` & `sapientml_core-0.5.6/sapientml_core/adaptation/generation/preprocessing_label.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/adaptation/generation/template_based_adaptation.py` & `sapientml_core-0.5.6/sapientml_core/adaptation/generation/template_based_adaptation.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/design/label_util.py` & `sapientml_core-0.5.6/sapientml_core/design/label_util.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/design/pp_component_groups.py` & `sapientml_core-0.5.6/sapientml_core/design/pp_component_groups.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/design/search_space.py` & `sapientml_core-0.5.6/sapientml_core/design/search_space.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/enums.py` & `sapientml_core-0.5.6/sapientml_core/enums.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/explain/AutoEDA.py` & `sapientml_core-0.5.6/sapientml_core/explain/AutoEDA.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/explain/AutoVisualization.py` & `sapientml_core-0.5.6/sapientml_core/explain/AutoVisualization.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/explain/code_miner.py` & `sapientml_core-0.5.6/sapientml_core/explain/code_miner.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/explain/code_template.py` & `sapientml_core-0.5.6/sapientml_core/explain/code_template.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/explain/main.py` & `sapientml_core-0.5.6/sapientml_core/explain/main.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/explain/pipeline_explanation.py` & `sapientml_core-0.5.6/sapientml_core/explain/pipeline_explanation.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/generator.py` & `sapientml_core-0.5.6/sapientml_core/generator.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/internal_path.py` & `sapientml_core-0.5.6/sapientml_core/internal_path.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/meta_features.py` & `sapientml_core-0.5.6/sapientml_core/meta_features.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/models/feature_importance.json` & `sapientml_core-0.5.6/sapientml_core/models/feature_importance.json`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/models/model_metafeatures_test.csv` & `sapientml_core-0.5.6/sapientml_core/models/model_metafeatures_test.csv`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/models/mp_model_1.pkl` & `sapientml_core-0.5.6/sapientml_core/models/mp_model_1.pkl`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/models/mp_model_2.pkl` & `sapientml_core-0.5.6/sapientml_core/models/mp_model_2.pkl`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/models/pp_models.pkl` & `sapientml_core-0.5.6/sapientml_core/models/pp_models.pkl`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/params.py` & `sapientml_core-0.5.6/sapientml_core/params.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/ps_macros.py` & `sapientml_core-0.5.6/sapientml_core/ps_macros.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/seeding/__init__.py` & `sapientml_core-0.5.6/sapientml_core/seeding/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/seeding/predictor.py` & `sapientml_core-0.5.6/sapientml_core/seeding/predictor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/component_description.json` & `sapientml_core-0.5.6/sapientml_core/templates/explainability_templates/component_description.json`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/hyperparameters.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/model.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/model.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_predict.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/model_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_test.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/model_test.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/model_templates/model_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/confusion_matrix.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/confusion_matrix.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/evaluation.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation_test.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/evaluation_test.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/inverse_target.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/inverse_target.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/permutation_importance.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/permutation_importance.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/prediction_result.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/prediction_result.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/other_templates/shap.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/other_templates/shap.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/pipeline_predict.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/pipeline_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/pipeline_test.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/pipeline_test.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/pipeline_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/pipeline_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/pipeline_validation.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/pipeline_validation.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/DATE.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/Processing.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja` & `sapientml_core-0.5.6/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_results.py` & `sapientml_core-0.5.6/sapientml_core/training/augmentation/mutation_results.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_runner.py` & `sapientml_core-0.5.6/sapientml_core/training/augmentation/mutation_runner.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/augmentation/mutator.py` & `sapientml_core-0.5.6/sapientml_core/training/augmentation/mutator.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/ast_operation.py` & `sapientml_core-0.5.6/sapientml_core/training/dataflowmodel/ast_operation.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/dependent_api_extractor.py` & `sapientml_core-0.5.6/sapientml_core/training/dataflowmodel/dependent_api_extractor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/determine_label_order.py` & `sapientml_core-0.5.6/sapientml_core/training/dataflowmodel/determine_label_order.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/denoising/ast_info_collector.py` & `sapientml_core-0.5.6/sapientml_core/training/denoising/ast_info_collector.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/denoising/dataset_snapshot_extractor.py` & `sapientml_core-0.5.6/sapientml_core/training/denoising/dataset_snapshot_extractor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/denoising/determine_used_features.py` & `sapientml_core-0.5.6/sapientml_core/training/denoising/determine_used_features.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/denoising/df_collector.py` & `sapientml_core-0.5.6/sapientml_core/training/denoising/df_collector.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/denoising/static_analysis_of_columns.py` & `sapientml_core-0.5.6/sapientml_core/training/denoising/static_analysis_of_columns.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/meta_feature_extractor.py` & `sapientml_core-0.5.6/sapientml_core/training/meta_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/meta_feature_selector.py` & `sapientml_core-0.5.6/sapientml_core/training/meta_feature_selector.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/meta_model_trainer.py` & `sapientml_core-0.5.6/sapientml_core/training/meta_model_trainer.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/pp_model_trainer.py` & `sapientml_core-0.5.6/sapientml_core/training/pp_model_trainer.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/project.py` & `sapientml_core-0.5.6/sapientml_core/training/project.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/training/project_corpus.py` & `sapientml_core-0.5.6/sapientml_core/training/project_corpus.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/sapientml_core/util/file_util.py` & `sapientml_core-0.5.6/sapientml_core/util/file_util.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.5/PKG-INFO` & `sapientml_core-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapientml-core
-Version: 0.5.5
+Version: 0.5.6
 Summary: A SapientML plugin of SapientMLGenerator
 License: Apache-2.0
 Author: The SapientML Authors
 Maintainer: Kosaku Kimura
 Maintainer-email: kimura.kosaku@fujitsu.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,10 +26,10 @@
 Requires-Dist: optuna (>=3.2.0,<4.0.0)
 Requires-Dist: sapientml
 Requires-Dist: sapientml-loaddata
 Requires-Dist: sapientml-preprocess
 Requires-Dist: scikit-learn (==1.3.2)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.14.0)
-Requires-Dist: shap (>=0.43,<0.45)
+Requires-Dist: shap (>=0.43,<0.46)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: xgboost (>=1.7.6,<3.0.0)
```

