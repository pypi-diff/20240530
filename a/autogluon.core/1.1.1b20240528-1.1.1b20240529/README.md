# Comparing `tmp/autogluon.core-1.1.1b20240528.tar.gz` & `tmp/autogluon.core-1.1.1b20240529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-1.1.1b20240528.tar", last modified: Tue May 28 09:04:06 2024, max compression
+gzip compressed data, was "autogluon.core-1.1.1b20240529.tar", last modified: Wed May 29 09:04:23 2024, max compression
```

## Comparing `autogluon.core-1.1.1b20240528.tar` & `autogluon.core-1.1.1b20240529.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.913530 autogluon.core-1.1.1b20240528/
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-28 09:04:06.913530 autogluon.core-1.1.1b20240528/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:04:06.913530 autogluon.core-1.1.1b20240528/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.897529 autogluon.core-1.1.1b20240528/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.897529 autogluon.core-1.1.1b20240528/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.901529 autogluon.core-1.1.1b20240528/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.901529 autogluon.core-1.1.1b20240528/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.901529 autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.901529 autogluon.core-1.1.1b20240528/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.901529 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29424 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.901529 autogluon.core-1.1.1b20240528/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.905530 autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.905530 autogluon.core-1.1.1b20240528/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.905530 autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)   102328 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.905530 autogluon.core-1.1.1b20240528/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.905530 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67049 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    45241 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.905530 autogluon.core-1.1.1b20240528/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.909530 autogluon.core-1.1.1b20240528/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.909530 autogluon.core-1.1.1b20240528/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-28 09:03:40.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.909530 autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.909530 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.909530 autogluon.core-1.1.1b20240528/src/autogluon/core/stacked_overfitting/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/stacked_overfitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.909530 autogluon.core-1.1.1b20240528/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   199164 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.913530 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36236 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.913530 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.913530 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    50705 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-28 09:03:41.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:06.897529 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:04:06.000000 autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.541357 autogluon.core-1.1.1b20240529/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-29 09:04:23.541357 autogluon.core-1.1.1b20240529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:04:23.541357 autogluon.core-1.1.1b20240529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.525357 autogluon.core-1.1.1b20240529/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.525357 autogluon.core-1.1.1b20240529/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.529357 autogluon.core-1.1.1b20240529/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.529357 autogluon.core-1.1.1b20240529/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.529357 autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.529357 autogluon.core-1.1.1b20240529/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.533357 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29424 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21399 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.533357 autogluon.core-1.1.1b20240529/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.533357 autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.533357 autogluon.core-1.1.1b20240529/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.533357 autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102328 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.533357 autogluon.core-1.1.1b20240529/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67049 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45241 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/stacked_overfitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/stacked_overfitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.537357 autogluon.core-1.1.1b20240529/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199164 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.541357 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36236 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.541357 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.541357 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50705 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-29 09:04:01.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:04:23.529357 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:04:23.000000 autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-1.1.1b20240528/PKG-INFO` & `autogluon.core-1.1.1b20240529/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.1.1b20240528
+Version: 1.1.1b20240529
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-1.1.1b20240528/setup.py` & `autogluon.core-1.1.1b20240529/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/_setup_utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/constants.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/data/cleaner.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/dataset.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/executors.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from autogluon.common import space as ag_space
 from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.utils.try_import import try_import_ray
 
 try_import_ray()  # try import ray before importing the remaining contents so we can give proper error messages
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import Callable, List, Optional, Union
 
 import ray
 from ray import air, tune
 from ray.tune import ExperimentAnalysis, PlacementGroupFactory
 from ray.tune.schedulers import TrialScheduler
 from ray.tune.search import SearchAlgorithm, Searcher
@@ -260,21 +261,25 @@
 
     original_path = os.getcwd()
     save_dir = os.path.normpath(save_dir)
     if tune_config_kwargs is None:
         tune_config_kwargs = dict()
     if run_config_kwargs is None:
         run_config_kwargs = dict()
+
+    # storage_path needs to be an absolute path starting in Ray 2.7+
+    #  https://github.com/ultralytics/ultralytics/issues/4980#issuecomment-1741684208
+    storage_path = str(Path(os.path.dirname(save_dir)).resolve())
     tuner = tune.Tuner(
         tune.with_resources(tune.with_parameters(trainable, **trainable_args), resources_per_trial),
         param_space=search_space,
         tune_config=tune.TuneConfig(
             num_samples=num_samples, search_alg=searcher, scheduler=scheduler, metric=metric, mode=mode, time_budget_s=time_budget_s, **tune_config_kwargs
         ),
-        run_config=air.RunConfig(name=os.path.basename(save_dir), storage_path=os.path.dirname(save_dir), verbose=verbose, **run_config_kwargs),
+        run_config=air.RunConfig(name=os.path.basename(save_dir), storage_path=storage_path, verbose=verbose, **run_config_kwargs),
         _tuner_kwargs={"trial_name_creator": _trial_name_creator, "trial_dirname_creator": _trial_dirname_creator},
     )
     results = tuner.fit()
 
     os.chdir(original_path)  # go back to the original directory to avoid relative path being broken
     return results._experiment_analysis
```

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/__init__.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/_utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/problem_type.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/stacked_overfitting/utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/stacked_overfitting/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2123,15 +2123,15 @@
         if model.fit_time is not None:
             logger.log(20, f"\t{round(model.fit_time, 2)}s\t = Training   runtime")
         if model.predict_time is not None:
             logger.log(20, f"\t{round(model.predict_time, 2)}s\t = Validation runtime")
         predict_n_time_per_row = self.get_model_attribute_full(model=model.name, attribute="predict_n_time_per_row")
         predict_n_size = self.get_model_attribute_full(model=model.name, attribute="predict_n_size", func=min)
         if predict_n_time_per_row is not None and predict_n_time_per_row != 0 and predict_n_size is not None:
-            logger.log(30, f"\t{round(1 / predict_n_time_per_row, 1)}\t = Inference  throughput (rows/s | {int(predict_n_size)} batch size)")
+            logger.log(15, f"\t{round(1 / predict_n_time_per_row, 1)}\t = Inference  throughput (rows/s | {int(predict_n_size)} batch size)")
         if model.predict_1_time is not None:
             fit_metadata = model.get_fit_metadata()
             predict_1_batch_size = fit_metadata.get("predict_1_batch_size", None)
             assert predict_1_batch_size is not None, "predict_1_batch_size cannot be None if predict_1_time is not None"
 
             if _is_refit:
                 predict_1_time = self.get_model_attribute(model=model.name, attribute="predict_1_child_time")
```

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/trainer/utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/decorators.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/files.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/plots.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/time.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon/core/utils/version_utils.py` & `autogluon.core-1.1.1b20240529/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.1.1b20240528
+Version: 1.1.1b20240529
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-1.1.1b20240528/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-1.1.1b20240529/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

