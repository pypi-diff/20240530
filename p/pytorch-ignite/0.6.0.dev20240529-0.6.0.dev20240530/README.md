# Comparing `tmp/pytorch_ignite-0.6.0.dev20240529.tar.gz` & `tmp/pytorch_ignite-0.6.0.dev20240530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_ignite-0.6.0.dev20240529.tar", last modified: Wed May 29 00:14:40 2024, max compression
+gzip compressed data, was "pytorch_ignite-0.6.0.dev20240530.tar", last modified: Thu May 30 00:14:29 2024, max compression
```

## Comparing `pytorch_ignite-0.6.0.dev20240529.tar` & `pytorch_ignite-0.6.0.dev20240530.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.465584 pytorch_ignite-0.6.0.dev20240529/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-29 00:14:40.465584 pytorch_ignite-0.6.0.dev20240529/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.437584 pytorch_ignite-0.6.0.dev20240529/ignite/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 00:12:15.000000 pytorch_ignite-0.6.0.dev20240529/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.437584 pytorch_ignite-0.6.0.dev20240529/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.437584 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.441584 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.441584 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.441584 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.445584 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.445584 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.445584 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.449584 pytorch_ignite-0.6.0.dev20240529/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.453584 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/fbresearch_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    68261 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.457584 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.457584 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/maximum_mean_discrepancy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/multilabel_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mutual_information.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.461584 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/recall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.461584 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/pearson_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:14:40.465584 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-29 00:14:40.000000 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-29 00:14:40.000000 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:14:40.000000 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:14:40.000000 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 00:14:40.000000 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 00:14:40.000000 pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-29 00:14:40.465584 pytorch_ignite-0.6.0.dev20240529/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-29 00:11:49.000000 pytorch_ignite-0.6.0.dev20240529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.433170 pytorch_ignite-0.6.0.dev20240530/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-30 00:14:29.433170 pytorch_ignite-0.6.0.dev20240530/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.409170 pytorch_ignite-0.6.0.dev20240530/ignite/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 00:12:09.000000 pytorch_ignite-0.6.0.dev20240530/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.409170 pytorch_ignite-0.6.0.dev20240530/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.409170 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.409170 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.413170 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.413170 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.417170 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.417170 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.417170 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.417170 pytorch_ignite-0.6.0.dev20240530/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.421170 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/fbresearch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68261 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.429170 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.429170 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/maximum_mean_discrepancy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/multilabel_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mutual_information.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.429170 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/recall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.433170 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/pearson_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:14:29.433170 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-05-30 00:14:29.000000 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-30 00:14:29.000000 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:14:29.000000 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:14:29.000000 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 00:14:29.000000 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 00:14:29.000000 pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-30 00:14:29.433170 pytorch_ignite-0.6.0.dev20240530/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-30 00:11:37.000000 pytorch_ignite-0.6.0.dev20240530/setup.py
```

### Comparing `pytorch_ignite-0.6.0.dev20240529/LICENSE` & `pytorch_ignite-0.6.0.dev20240530/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/PKG-INFO` & `pytorch_ignite-0.6.0.dev20240530/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.6.0.dev20240529
+Version: 0.6.0.dev20240530
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch_ignite-0.6.0.dev20240529/README.md` & `pytorch_ignite-0.6.0.dev20240530/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/base/mixins.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/engines/common.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/engines/common.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/engines/tbptt.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/base_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/clearml_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/lr_finder.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/mlflow_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/neptune_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/param_scheduler.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/time_profilers.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/tqdm_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/visdom_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/handlers/wandb_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/average_precision.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/cohen_kappa.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/gpu_info.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/_base.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/mean_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/r2_score.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/contrib/metrics/roc_auc.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/auto.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/base.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABCMeta, abstractmethod
 from numbers import Number
 from typing import Any, Callable, cast, List, Optional, Union
 
 import torch
 from packaging.version import Version
 
-_torch_version_le_112 = Version(torch.__version__) > Version("1.12.0")
+_torch_version_gt_112 = Version(torch.__version__) > Version("1.12.0")
 
 
 class ComputationModel(metaclass=ABCMeta):
     """Base class for distributed computation models and defines interface methods.
     This class is public and should be used for other custom derived distributed models.
     """
 
@@ -325,15 +325,15 @@
 
     def get_node_rank(self) -> int:
         return 0
 
     def device(self) -> torch.device:
         if torch.cuda.is_available():
             return torch.device("cuda")
-        if _torch_version_le_112 and torch.backends.mps.is_available():
+        if _torch_version_gt_112 and torch.backends.mps.is_available():
             return torch.device("mps")
         return torch.device("cpu")
 
     def backend(self) -> Optional[str]:
         return None
 
     def finalize(self) -> None:
```

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/horovod.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/native.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/comp_models/xla.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/launcher.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/distributed/utils.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/engine/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/engine/deterministic.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/engine/engine.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/engine/events.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/engine/utils.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/base_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/checkpoint.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/clearml_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/early_stopping.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/ema_handler.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/fbresearch_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/fbresearch_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/lr_finder.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/mlflow_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/neptune_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/param_scheduler.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/polyaxon_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/state_param_scheduler.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/stores.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/tensorboard_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/terminate_on_nan.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/time_limit.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/time_profilers.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/timing.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/tqdm_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/utils.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/visdom_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/handlers/wandb_logger.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/accumulation.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/accuracy.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/average_precision.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/classification_report.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/cohen_kappa.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/confusion_matrix.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/cosine_similarity.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/entropy.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/epoch_metric.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/fbeta.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/frequency.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/fid.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/inception_score.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gan/utils.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/gpu_info.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/js_divergence.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/js_divergence.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/kl_divergence.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/loss.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/maximum_mean_discrepancy.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/maximum_mean_discrepancy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mean_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mean_pairwise_distance.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mean_squared_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/metric.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/metrics_lambda.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/mutual_information.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/mutual_information.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/bleu.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/rouge.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/nlp/utils.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/precision.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/precision_recall_curve.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/psnr.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/recall.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/__init__.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/_base.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/canberra_metric.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/fractional_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/fractional_bias.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/geometric_mean_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/manhattan_distance.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/maximum_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/mean_absolute_relative_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/mean_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/mean_normalized_bias.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/median_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/median_absolute_percentage_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/median_relative_absolute_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/pearson_correlation.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/r2_score.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/regression/wave_hedges_distance.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/roc_auc.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/root_mean_squared_error.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/running_average.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/ssim.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/ignite/utils.py` & `pytorch_ignite-0.6.0.dev20240530/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/pyproject.toml` & `pytorch_ignite-0.6.0.dev20240530/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/PKG-INFO` & `pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.6.0.dev20240529
+Version: 0.6.0.dev20240530
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch_ignite-0.6.0.dev20240529/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch_ignite-0.6.0.dev20240530/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/setup.cfg` & `pytorch_ignite-0.6.0.dev20240530/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch_ignite-0.6.0.dev20240529/setup.py` & `pytorch_ignite-0.6.0.dev20240530/setup.py`

 * *Files identical despite different names*

