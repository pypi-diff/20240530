# Comparing `tmp/ropt-0.3.0.tar.gz` & `tmp/ropt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt-0.3.0.tar", last modified: Mon May  6 15:21:08 2024, max compression
+gzip compressed data, was "ropt-0.3.1.tar", last modified: Thu May 30 07:33:35 2024, max compression
```

## Comparing `ropt-0.3.0.tar` & `ropt-0.3.1.tar`

### file list

```diff
@@ -1,185 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.564519 ropt-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.528518 ropt-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.536518 ropt-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-06 15:21:02.000000 ropt-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 15:21:02.000000 ropt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-06 15:21:08.564519 ropt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-06 15:21:02.000000 ropt-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.536518 ropt-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.536518 ropt-0.3.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/enopt_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/enums.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/evaluator.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/function_transforms.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/optimization_steps.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/optimizer_plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/plan_config.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/realization_filters.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/reporting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/results.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/sampler_plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/usage/robust_optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/usage/running.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/de_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/de_nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/rosenbrock_deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/rosenbrock_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/examples/script_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/script_optimizer/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/script_optimizer/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 15:21:02.000000 ropt-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-06 15:21:02.000000 ropt-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:21:08.564519 ropt-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.532518 ropt-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/src/ropt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.544518 ropt-0.3.0/src/ropt/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/apps/_script_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.544518 ropt-0.3.0/src/ropt/config/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.544518 ropt-0.3.0/src/ropt/config/enopt/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_enopt_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_function_transform_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_gradient_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_linear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_nonlinear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_objective_functions_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_optimizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_realization_filter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_realizations_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_sampler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_variables_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/config/plan/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/plan/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/plan/_plan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25390 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_evaluator_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_ensemble_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/function_transform/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/function_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/function_transform/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/function_transform/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/optimization_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/reset_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/update_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/realization_filter/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/realization_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/realization_filter/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/realization_filter/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/sampler/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/sampler/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.556519 ropt-0.3.0/src/ropt/report/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.556519 ropt-0.3.0/src/ropt/results/
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_bound_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_function_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_function_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_gradient_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_gradient_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_maximize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_nonlinear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_result_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.560519 ropt-0.3.0/src/ropt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.564519 ropt-0.3.0/src/ropt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.564519 ropt-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25752 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_ensemble_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_failed_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_function_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    44245 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_realization_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_result_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_results_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_scipy_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_scipy_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.905211 ropt-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.869210 ropt-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.877210 ropt-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-30 07:33:28.000000 ropt-0.3.1/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-30 07:33:28.000000 ropt-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-30 07:33:28.000000 ropt-0.3.1/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-30 07:33:28.000000 ropt-0.3.1/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-30 07:33:28.000000 ropt-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 07:33:28.000000 ropt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-30 07:33:35.905211 ropt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-30 07:33:28.000000 ropt-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.877210 ropt-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.877210 ropt-0.3.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.881210 ropt-0.3.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/enopt_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/enums.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/evaluator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/function_transforms.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/optimization_steps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/optimizer_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/plan_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/realization_filters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/reporting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/results.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/sampler_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/reference/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.881210 ropt-0.3.1/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/usage/robust_optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-30 07:33:28.000000 ropt-0.3.1/docs/usage/running.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.881210 ropt-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-30 07:33:28.000000 ropt-0.3.1/examples/de_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-30 07:33:28.000000 ropt-0.3.1/examples/de_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-30 07:33:28.000000 ropt-0.3.1/examples/rosenbrock_deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-30 07:33:28.000000 ropt-0.3.1/examples/rosenbrock_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.881210 ropt-0.3.1/examples/script_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-30 07:33:28.000000 ropt-0.3.1/examples/script_optimizer/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-30 07:33:28.000000 ropt-0.3.1/examples/script_optimizer/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 07:33:28.000000 ropt-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-30 07:33:28.000000 ropt-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:33:35.905211 ropt-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.873211 ropt-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.881210 ropt-0.3.1/src/ropt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.885210 ropt-0.3.1/src/ropt/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/apps/_script_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.885210 ropt-0.3.1/src/ropt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.885210 ropt-0.3.1/src/ropt/config/enopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_enopt_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_function_transform_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_gradient_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_linear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_nonlinear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_objective_functions_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_optimizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_realization_filter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_realizations_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_sampler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/_variables_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/enopt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.889211 ropt-0.3.1/src/ropt/config/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/plan/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/plan/_plan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.889211 ropt-0.3.1/src/ropt/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25390 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_evaluator_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/evaluator/parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.889211 ropt-0.3.1/src/ropt/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/optimization/_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/optimization/_ensemble_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/optimization/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/optimization/_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/optimization/_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.889211 ropt-0.3.1/src/ropt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.889211 ropt-0.3.1/src/ropt/plugins/function_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/function_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/function_transform/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/function_transform/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.893211 ropt-0.3.1/src/ropt/plugins/optimization_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/reset_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimization_steps/update_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.893211 ropt-0.3.1/src/ropt/plugins/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimizer/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimizer/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/optimizer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.893211 ropt-0.3.1/src/ropt/plugins/realization_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/realization_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/realization_filter/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/realization_filter/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.893211 ropt-0.3.1/src/ropt/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/sampler/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/plugins/sampler/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.897210 ropt-0.3.1/src/ropt/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/report/_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/report/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/report/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.897210 ropt-0.3.1/src/ropt/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_bound_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_function_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_function_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_gradient_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_gradient_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_linear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_maximize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_nonlinear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_result_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/results/_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.897210 ropt-0.3.1/src/ropt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-30 07:33:28.000000 ropt-0.3.1/src/ropt/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.901210 ropt-0.3.1/src/ropt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 07:33:35.000000 ropt-0.3.1/src/ropt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:35.901210 ropt-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25752 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_ensemble_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_failed_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_function_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44245 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_realization_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_results_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_scipy_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_scipy_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-30 07:33:28.000000 ropt-0.3.1/tests/test_xarray.py
```

### Comparing `ropt-0.3.0/.github/workflows/build-docs.yml` & `ropt-0.3.1/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/.github/workflows/release.yml` & `ropt-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/.github/workflows/static-checks.yml` & `ropt-0.3.1/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/.github/workflows/tests.yml` & `ropt-0.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/LICENSE` & `ropt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/PKG-INFO` & `ropt-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.3.0
+Version: 0.3.1
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ropt-0.3.0/README.md` & `ropt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/docs/index.md` & `ropt-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/docs/reference/evaluator.md` & `ropt-0.3.1/docs/reference/evaluator.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/docs/reference/realization_filters.md` & `ropt-0.3.1/docs/reference/realization_filters.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/docs/reference/results.md` & `ropt-0.3.1/docs/reference/results.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/docs/usage/robust_optimization.md` & `ropt-0.3.1/docs/usage/robust_optimization.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/docs/usage/running.md` & `ropt-0.3.1/docs/usage/running.md`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/examples/de_linear.py` & `ropt-0.3.1/examples/de_linear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/examples/de_nonlinear.py` & `ropt-0.3.1/examples/de_nonlinear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/examples/rosenbrock_deterministic.py` & `ropt-0.3.1/examples/rosenbrock_deterministic.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/examples/rosenbrock_ensemble.py` & `ropt-0.3.1/examples/rosenbrock_ensemble.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/examples/script_optimizer/rosenbrock.py` & `ropt-0.3.1/examples/script_optimizer/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/examples/script_optimizer/run.py` & `ropt-0.3.1/examples/script_optimizer/run.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/mkdocs.yml` & `ropt-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/pyproject.toml` & `ropt-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/apps/_script_optimizer.py` & `ropt-0.3.1/src/ropt/apps/_script_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import os
 from collections import abc, defaultdict
 from dataclasses import dataclass, field
 from itertools import groupby
 from pathlib import Path
+from shutil import rmtree
 from string import Template
 from traceback import format_exception
 from typing import (
     Any,
     Callable,
     DefaultDict,
     Dict,
@@ -199,15 +200,19 @@
         variable_export_depth: int = 0,
         get_function_files: Callable[
             [EnOptConfig], Tuple[Tuple[str, ...], Tuple[str, ...]]
         ] = get_function_files,
         callbacks: Optional[Dict[EventType, Callable[..., None]]] = None,
         seed: Optional[int] = None,
         provider: Optional[ExecutionProvider] = None,
+        htex_kwargs: Optional[Dict[str, Any]] = None,
         max_threads: int = 4,
+        worker_restart: int = 0,
+        polling: float = 0.1,
+        max_submit: int = 500,
     ) -> None:
         """Initialize the optimizer.
 
         The directory where the jobs run is constructed from by nesting
         directories according the `job_labels` tuple. These directories are
         located in the directory where the optimizer runs, which can be set
         using the `work_dir` parameter of the `run()` method.
@@ -222,28 +227,36 @@
             job_labels:            Label formats to use in generating filenames
                                    reports
             variable_export_depth: The depth parameter for exporting variables
             get_function_files:    Callable to retrieve function file names
             callbacks:             Dictionary of callbacks for the optimizer
             seed:                  Seed for the random number generator
             provider:              The provider that executes the jobs
+            htex_kwargs:           Keyword arguments forwarded to the htex executor
             max_threads:           Maximum number of threads for local runs
+            worker_restart:        Restart the workers every `worker_restart` batch
+            polling:               How often should be polled for status
+            max_submit:            Maximum number of variables to submit simultaneously
         """
         self._plan = plan
         self._tasks = tasks
         self._work_dir = Path(work_dir).resolve()
         self._job_labels = job_labels
         self._variable_export_depth = variable_export_depth
         self._get_function_files = get_function_files
         self._callbacks = callbacks
         self._seed = seed
         self._provider = provider
+        self._htex_kwargs = htex_kwargs
         self._max_threads = max_threads
+        self._worker_restart = worker_restart
         self._status: Dict[int, Any] = {}
         self._optimal_result: Optional[FunctionResults] = None
+        self._polling = polling
+        self._max_submit = max_submit
 
         self._job_dir = self._work_dir if job_dir is None else Path(job_dir)
         if not self._job_dir.is_absolute():
             self._job_dir = self._work_dir / self._job_dir
 
     def _set_logger(self) -> None:
         self._logger = logging.getLogger("ScriptBasedOptimizer")
@@ -266,21 +279,41 @@
             msg = f"Realization name must be an integer: {realization}"
             raise ConfigError(msg)
 
         job_labels = tuple(
             label.format(batch=batch_id, realization=realization, job=job_idx)
             for label in self._job_labels
         )
-
         path = self._job_dir / Path(*job_labels)
-        Path.mkdir(path, parents=True, exist_ok=True)
+        objective_names, constraint_names = self._get_function_files(context.config)
+        objective_paths = tuple(path / name for name in objective_names)
+        constraint_paths = tuple(path / name for name in constraint_names)
+
+        var_path = path / "var-vector.npy"
+        if all(
+            path.exists() for path in (var_path, *objective_paths, *constraint_paths)
+        ) and np.allclose(np.load(var_path), variables):
+            return [
+                ScriptTask(
+                    future=None,
+                    objective_paths=objective_paths,
+                    constraint_paths=constraint_paths,
+                )
+            ]
+
+        if not self._tasks.items():
+            return []
+
+        rmtree(path, ignore_errors=True)
+        Path.mkdir(path, parents=True)
+        np.save(var_path, variables)
 
         assert context.config.variables.names is not None
         variables_to_json(
-            variables[job_idx],
+            variables,
             context.config.variables.names,
             path,
             depth=self._variable_export_depth,
         )
 
         tasks: List[ScriptTask] = []
         for task_name, script in self._tasks.items():
@@ -296,18 +329,16 @@
                         stdout=((path / task_name).with_suffix(".stdout"), "a"),
                         stderr=((path / task_name).with_suffix(".stderr"), "a"),
                     ),
                     job_labels=job_labels,
                     realization=realization,
                 ),
             )
-
-        objective_names, constraint_names = self._get_function_files(context.config)
-        tasks[-1].objective_paths = tuple(path / name for name in objective_names)
-        tasks[-1].constraint_paths = tuple(path / name for name in constraint_names)
+        tasks[-1].objective_paths = objective_paths
+        tasks[-1].constraint_paths = constraint_paths
 
         return tasks
 
     def _log_task(self, task: ScriptTask) -> None:
         if not task.logged:
             job_label = ", ".join(task.job_labels)
 
@@ -430,14 +461,18 @@
         try:
             self._set_logger()
             evaluator = ParslEvaluator(
                 self._workflow,
                 monitor=self._monitor,
                 provider=self._provider,
                 max_threads=self._max_threads,
+                worker_restart=self._worker_restart,
+                htex_kwargs=self._htex_kwargs,
+                polling=self._polling,
+                max_submit=self._max_submit,
             )
             optimizer = EnsembleOptimizer(evaluator)
             optimizer.add_observer(
                 EventType.FINISHED_OPTIMIZER_STEP,
                 self._handle_finished_optimizer,
             )
             if self._callbacks is not None:
```

### Comparing `ropt-0.3.0/src/ropt/config/enopt/__init__.py` & `ropt-0.3.1/src/ropt/config/enopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_enopt_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_function_transform_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_function_transform_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_gradient_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_gradient_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_linear_constraints_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_linear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_nonlinear_constraints_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_nonlinear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_objective_functions_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_objective_functions_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_optimizer_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_optimizer_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_realization_filter_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_realization_filter_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_realizations_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_realizations_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_sampler_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_sampler_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_utils.py` & `ropt-0.3.1/src/ropt/config/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Utilities for checking configuration values."""
+
 import sys
 from collections import Counter
 from enum import IntEnum
 from typing import Any, Optional, Tuple, Type, cast
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
@@ -10,45 +12,96 @@
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 
 def normalize(array: NDArray[np.float64]) -> NDArray[np.float64]:
+    """Normalize a vector.
+
+        Normalize the sum of the values to one.
+
+    Args:
+        array: The input array
+
+    Returns:
+        ValueError: The normalized array
+    """
     if array.sum() < np.finfo(np.float64).eps:
         msg = "the sum of weights is not positive"
         raise ValueError(msg)
     return immutable_array(array / array.sum())
 
 
 def immutable_array(
     array_like: ArrayLike,
     **kwargs: Any,  # noqa: ANN401
 ) -> NDArray[Any]:
+    """Make an immutable array.
+
+    Converts the input to an array and makes it immutable.`
+
+    Args:
+        array_like: The input
+        kwargs    : Additional keyword arguments for array conversion
+
+    Returns:
+        The immutable array.
+    """
     array = np.array(array_like, **kwargs)
     array.setflags(write=False)
     return array
 
 
 def broadcast_arrays(*args: Any) -> Tuple[NDArray[Any], ...]:  # noqa: ANN401
+    """Broadcast a set of arrays and makes them immutable.
+
+    Args:
+        args: The input arrays
+
+    Returns:
+        The broadcasted immutable arrays.
+    """
     results = np.broadcast_arrays(*args)
     return tuple(immutable_array(result) for result in results)
 
 
 def broadcast_1d_array(array: NDArray[Any], name: str, size: int) -> NDArray[Any]:
+    """Broadcast the input array to an 1D array of given size.
+
+    Args:
+        array: The input array
+        name:  The name of the array, used in an error message
+        size:  The size of the result
+
+    Returns:
+        An 1D array of the requested size.
+    """
     if size == 0:
         return immutable_array([], dtype=array.dtype)
     try:
         return np.broadcast_to(immutable_array(array), (size,))
     except ValueError as err:
         msg = f"{name} cannot be broadcasted to a length of {size}"
         raise ValueError(msg) from err
 
 
 def check_enum_values(value: NDArray[np.ubyte], enum_type: Type[IntEnum]) -> None:
+    """Check if an enum value is valid.
+
+    Given an array of byte integers, check of the values are within the range of
+    values of the given enum.
+
+    Args:
+        value:     The enum values
+        enum_type: The type to check
+
+    Raises:
+        ValueError: If the array contains an invalid value.
+    """
     min_enum = min(item.value for item in enum_type)
     max_enum = max(item.value for item in enum_type)
     if np.any(value < min_enum) or np.any(value > max_enum):
         msg = "invalid enumeration value"
         raise ValueError(msg)
```

### Comparing `ropt-0.3.0/src/ropt/config/enopt/_variables_config.py` & `ropt-0.3.1/src/ropt/config/enopt/_variables_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         scales:         Optional scales, used for scaling the variables
         indices:        Optional indices of variables to optimize.
         delimiters:     Delimiters used to construct names from tuples
     """
 
     names: Optional[UniqueNames] = None
     types: Optional[ArrayEnum] = None
-    initial_values: Array1D
+    initial_values: Array1D = np.array(0.0)
     lower_bounds: Array1D = np.array(-np.inf)
     upper_bounds: Array1D = np.array(np.inf)
     offsets: Optional[Array1D] = None
     scales: Optional[Array1D] = None
     indices: Optional[ArrayIndices] = None
     delimiters: str = Field(":", min_length=0)
```

### Comparing `ropt-0.3.0/src/ropt/config/enopt/constants.py` & `ropt-0.3.1/src/ropt/config/enopt/constants.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/plan/__init__.py` & `ropt-0.3.1/src/ropt/config/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/config/plan/_config.py` & `ropt-0.3.1/src/ropt/config/plan/_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, Literal, Optional, Set, Union
 
 from pydantic import BaseModel, ConfigDict, Field
 
+from ropt.config.utils import Array2D  # noqa: TCH001
+
 from ._plan_config import PlanConfig  # noqa: TCH001
 
 
 class TrackerStepConfig(BaseModel):
     """The configuration class for tracker steps.
 
     This configuration class is used within an optimization plan to specify a
@@ -145,12 +147,14 @@
     Info:
         This configuration class has its `extra` property set to `"allow"`, as
         it is expected that external code may parse additional fields for
         further configuration.
     """
 
     id: Optional[str] = None
+    variables: Optional[Array2D] = None
 
     model_config = ConfigDict(
         extra="allow",
         validate_default=True,
+        arbitrary_types_allowed=True,
     )
```

### Comparing `ropt-0.3.0/src/ropt/enums.py` & `ropt-0.3.1/src/ropt/enums.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/__init__.py` & `ropt-0.3.1/src/ropt/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/_concurrent.py` & `ropt-0.3.1/src/ropt/evaluator/_concurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     These task objects should contain the future that represents the task and
     return the results of the evaluation.
 
     It should implement two functions to retrieve the objective function values
     and optional constraint values.
     """
 
-    future: Any
+    future: Optional[Any]
 
     @abstractmethod
     def get_objectives(self) -> Optional[NDArray[np.float64]]:
         """Return the objectives calculated by the task.
 
         This method will only be called after the future is done, and if no
         exception was raised during the execution of the task.
@@ -67,66 +67,67 @@
     least the `done()`, `exception()`, and `result()` methods.
 
     To use a class derived from `ConcurrentEvaluator`, pass the object via the
     `evaluator` argument of the
     [`EnsembleOptimizer`][ropt.optimization.EnsembleOptimizer] constructor.
     """
 
-    def __init__(self, *, enable_cache: bool = True) -> None:
+    def __init__(
+        self, *, enable_cache: bool = True, polling: float = 0.1, max_submit: int = 500
+    ) -> None:
         """Initialize a concurrent evaluator object.
 
         Args:
-            enable_cache: Enable the caching mechanism.
+            enable_cache: Enable the caching mechanism
+            polling:      Time in seconds between checking job status
+            max_submit:   Maximum number of variables to submit simultaneously
         """
-        self.polling: float = 0.1
-        "The time in seconds between polling for evaluation status."
-
         self._batch_id = 0
+        self._polling = polling
+        self._max_submit = max_submit
         self._cache: Optional[_Cache] = _Cache() if enable_cache else None
 
     @abstractmethod
     def launch(
         self,
         batch_id: Any,  # noqa: ANN401
+        job_id: int,
         variables: NDArray[np.float64],
         context: EvaluatorContext,
-        active: Optional[NDArray[np.bool_]],
-    ) -> Dict[int, ConcurrentTask]:
-        """Launch the evaluations and return futures.
-
-        This method must implement the process of launching a batch of function
-        evaluations for a set of variable vectors passed via the `variables`
-        parameter. A unique batch ID is passed via the `batch_id`, which can be
-        optionally used.
+    ) -> Optional[ConcurrentTask]:
+        """Launch an evaluation and return futures.
+
+        This method must implement the process of launching a a single function
+        evaluation for a variable vector passed via the `variables` parameter. A
+        unique batch ID is passed via the `batch_id`, which can be optionally
+        used.
 
         This method should return a dictionary mapping the indices of the jobs
         to the tasks that will contain the result. The tasks are objects
         deriving from the [`ConcurrentTask`][ropt.evaluator.ConcurrentTask]
         class, containing the future object representing the launched task and
         its result. Under the hood, other tasks may be launched, but only those
         that contain results should be returned.
 
         This method is called by the `__call__` method, which implements the
         [`Evaluator`][ropt.evaluator.Evaluator] callback signature and can be
         passed by the [`EnsembleOptimizer`][ropt.optimization.EnsembleOptimizer]
         object.
 
         The `context` argument with optional information is passed from the
-        `__call__` method unchanged. The `active` document passes a boolean
-        vector indicating which realizations are active. It not `None` it should
-        take precedence over the corresponding field in the `context` variable.
+        `__call__` method unchanged.
 
         Args:
             batch_id:  The ID of the batch of evaluations to run.
+            job_id:    The ID of the job launched for the variables
             variables: The matrix of variables to evaluate.
             context:   Evaluator context.
-            active:    Optional active realizations.
 
         Returns:
-            A dictionary mapping the indices of launched evaluations to tasks.
+            The last future or `None` if no tasks were launched.
         """
 
     def monitor(self) -> None:  # noqa: B027
         """Monitor the states of the running evaluations.
 
         This method is called regularly in the polling loop that checks the
         futures until all results are collected. If the status of the
@@ -153,27 +154,41 @@
         """
         objective_results, constraint_results = _init_results(variables, context)
 
         active = self._try_cache(
             variables, context, objective_results, constraint_results
         )
 
-        tasks = self.launch(self._batch_id, variables, context, active)
-        tasks = tasks.copy()  # Use a shallow copy so we can safely modify the dict.
-        while tasks:
-            # We are modifying the dict while iterating, use a copy of the keys:
-            for idx in list(tasks.keys()):
-                if tasks[idx].future.done():
-                    if tasks[idx].future.exception() is None:
+        var_idx = 0
+        tasks: Dict[int, ConcurrentTask] = {}
+
+        # Keep submitting and monitoring until all variables and tasks are done:
+        while var_idx < variables.shape[0] or len(tasks) > 0:
+            # Add more tasks up to a maximum of max_submit:
+            for _ in range(self._max_submit - len(tasks)):
+                if var_idx < variables.shape[0]:
+                    if active is None or active[var_idx]:
+                        task = self.launch(
+                            self._batch_id, var_idx, variables[var_idx], context
+                        )
+                        if task is not None:
+                            tasks[var_idx] = task
+                    var_idx += 1
+
+            # Monitor the current tasks:
+            for idx in list(tasks.keys()):  # tasks changes size, hence list()
+                future = tasks[idx].future
+                if future is None or future.done():
+                    if future is None or future.exception() is None:
                         objective_results[idx, :] = tasks[idx].get_objectives()
                         if constraint_results is not None:
                             constraint_results[idx, :] = tasks[idx].get_constraints()
                     del tasks[idx]
             self.monitor()
-            time.sleep(self.polling)
+            time.sleep(self._polling)
 
         result = EvaluatorResult(
             objectives=objective_results,
             constraints=constraint_results,
             batch_id=self._batch_id,
         )
```

### Comparing `ropt-0.3.0/src/ropt/evaluator/_ensemble_evaluator.py` & `ropt-0.3.1/src/ropt/evaluator/_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/_evaluator.py` & `ropt-0.3.1/src/ropt/evaluator/_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/_evaluator_results.py` & `ropt-0.3.1/src/ropt/evaluator/_evaluator_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/_function.py` & `ropt-0.3.1/src/ropt/evaluator/_function.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/_gradient.py` & `ropt-0.3.1/src/ropt/evaluator/_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/_utils.py` & `ropt-0.3.1/src/ropt/evaluator/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/evaluator/parsl.py` & `ropt-0.3.1/src/ropt/evaluator/parsl.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [`parsl`](https://parsl-project.org/) library for parallel programming. This
 evaluator makes it possible to efficiently run `ropt` optimizations on a wide
 range of compute resources.
 """
 
 from dataclasses import dataclass
 from enum import Enum
+from time import sleep
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import parsl
 from numpy.typing import NDArray
 from parsl.config import Config
 from parsl.dataflow.futures import AppFuture
@@ -45,15 +46,15 @@
 
     Attributes:
         future:    The future of the task
         state:     The last sampled state
         exception: Any exception that may have occurred,  None otherwise
     """
 
-    future: AppFuture
+    future: Optional[AppFuture]
     state: State = State.UNKNOWN
     exception: Optional[BaseException] = None
 
 
 class ParslEvaluator(ConcurrentEvaluator):
     """A function evaluator based on the parsl library."""
 
@@ -61,104 +62,134 @@
 
     def __init__(  # noqa: PLR0913
         self,
         workflow: Callable[..., Any],
         *,
         monitor: Optional[Callable[..., Any]] = None,
         provider: Optional[ExecutionProvider] = None,
+        htex_kwargs: Optional[Dict[str, Any]] = None,
         max_threads: int = 4,
         retries: int = 0,
+        worker_restart: int = 0,
         enable_cache: bool = True,
+        polling: float = 0.1,
+        max_submit: int = 500,
     ) -> None:
         """Create a parsl evaluator object.
 
         Args:
-            provider:     Parsl execution provider to use. By default `LocalProvider`
-            workflow:     Callback to start a single workflow run
-            monitor:      Monitor function
-            max_threads:  Maximum number of threads for local execution. Defaults to 4
-            retries:      Number of retries upon failure of a task. Defaults to 0
-            enable_cache: If `True` enable function value caching.
+            provider:       Parsl execution provider to use. By default `LocalProvider`
+            workflow:       Callback to start a single workflow run
+            monitor:        Monitor function
+            htex_kwargs:    Keyword arguments forwarded to the htex executor
+            max_threads:    Maximum number of threads for local execution. Defaults to 4
+            retries:        Number of retries upon failure of a task. Defaults to 0
+            worker_restart: Restart the workers every `worker_restart` batch.
+            enable_cache:   If `True` enable function value caching.
+            polling:        Time in seconds between checking job status
+            max_submit:   Maximum number of variables to submit simultaneously
         """
-        super().__init__(enable_cache=enable_cache)
+        super().__init__(
+            enable_cache=enable_cache, polling=polling, max_submit=max_submit
+        )
 
         self._batch_id: int
         self._variables: NDArray[np.float64]
         self._jobs: Dict[int, List[Task]] = {}
         self._workflow = workflow
         self._monitor = monitor
+        self._executor: Union[ThreadPoolExecutor, HighThroughputExecutor]
+
+        parsl.clear()
 
-        executor: Union[ThreadPoolExecutor, HighThroughputExecutor]
         if provider is None or isinstance(provider, LocalProvider):
-            executor = ThreadPoolExecutor(
+            self._executor = ThreadPoolExecutor(
                 label="local_threads", max_threads=max_threads
             )
+            self._worker_restart = 0
+            self._htex_kwargs = {}
         else:
-            executor = HighThroughputExecutor(
-                label="high_throughput_executor", provider=provider, max_workers=1
+            if htex_kwargs is None:
+                htex_kwargs = {}
+            htex_kwargs.setdefault("max_workers_per_node", 1)
+            htex_kwargs.setdefault("heartbeat_period", 30)
+            self._executor = HighThroughputExecutor(
+                label="high_throughput_executor", provider=provider, **htex_kwargs
             )
+            self._worker_restart = worker_restart
+            self._htex_kwargs = htex_kwargs
 
-        parsl.clear()
         parsl.load(
             Config(
-                executors=[executor],
+                executors=[self._executor],
                 strategy="htex_auto_scale",
                 retries=retries,
                 run_dir=self._RUN_INFO_DIR,
             ),
         )
 
     def launch(
         self,
         batch_id: int,
+        job_id: int,
         variables: NDArray[np.float64],
         context: EvaluatorContext,
-        active: Optional[NDArray[np.bool_]],
-    ) -> Dict[int, ConcurrentTask]:
+    ) -> Optional[ConcurrentTask]:
         """Launch the parsl task.
 
         See the [ropt.evaluator.ConcurrentEvaluator][] abstract base class.
 
         # noqa
         """
+        if (
+            self._worker_restart > 0
+            and batch_id > 0
+            and job_id == 0
+            and batch_id % self._worker_restart == 0
+        ):
+            assert isinstance(self._executor, HighThroughputExecutor)
+            while self._executor.connected_workers > 0:
+                self._executor.scale_in(self._executor.connected_workers)
+                sleep(self._htex_kwargs["heartbeat_period"])
+        if job_id == 0:
+            self._jobs = {}
         self._batch_id = batch_id
-        self._variables = variables
-        self._jobs = {
-            job_idx: self._workflow(batch_id, job_idx, variables, context)
-            for job_idx in range(variables.shape[0])
-            if active is None or active[job_idx]
-        }
-        return {idx: futures[-1] for idx, futures in self._jobs.items()}
+        job: List[Task] = self._workflow(batch_id, job_id, variables, context)
+        if job:
+            self._jobs[job_id] = job
+            return job[-1]
+        return None
 
-    def monitor(self) -> None:
+    def monitor(self) -> None:  # noqa: C901
         """Monitor the tasks of all jobs.
 
         See the [ropt.evaluator.ConcurrentEvaluator][] abstract base class.
 
         # noqa
         """
         changed = False
         for job in self._jobs.values():
             for task in job:
-                # Make sure task.exception is update from the future:
-                if task.future.done() and task.exception is None:
-                    task.exception = task.future.exception()
-
-                # Default is not running:
-                state: State = State.PENDING
-
-                # Set the state:
-                if task.exception is not None:
-                    state = State.FAILED
-                elif task.future.done():
-                    state = State.SUCCESS
-                elif task.future.running():
-                    state = State.RUNNING
-                elif task.future.task_status() == "launched":
-                    state = State.LAUNCHED
-
-                # If the state changed, remember:
-                if state != task.state:
-                    task.state = state
-                    changed = True
+                if task.future is not None:
+                    # Update task.exception from the future:
+                    if task.future.done() and task.exception is None:
+                        task.exception = task.future.exception()
+
+                    # Default is not running:
+                    state: State = State.PENDING
+
+                    # Set the state:
+                    if task.exception is not None:
+                        state = State.FAILED
+                    elif task.future.done():
+                        state = State.SUCCESS
+                    elif task.future.running():
+                        state = State.RUNNING
+                    elif task.future.task_status() == "launched":
+                        state = State.LAUNCHED
+
+                    # If the state changed, remember:
+                    if state != task.state:
+                        task.state = state
+                        changed = True
         if self._monitor is not None and changed:
             self._monitor(self._batch_id, self._jobs)
```

### Comparing `ropt-0.3.0/src/ropt/events.py` & `ropt-0.3.1/src/ropt/events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/exceptions.py` & `ropt-0.3.1/src/ropt/exceptions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/optimization/_bases.py` & `ropt-0.3.1/src/ropt/optimization/_bases.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/optimization/_ensemble_optimizer.py` & `ropt-0.3.1/src/ropt/optimization/_ensemble_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/optimization/_events.py` & `ropt-0.3.1/src/ropt/optimization/_events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/optimization/_optimizer.py` & `ropt-0.3.1/src/ropt/optimization/_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,18 +217,27 @@
     ) -> NDArray[np.float64]:
         assert gradients is not None
         weighted_objective_gradient = (
             gradients.weighted_objective.copy()
             if variable_indices is None
             else gradients.weighted_objective[variable_indices]
         )
+        constraint_gradients = (
+            None
+            if gradients.constraints is None
+            else (
+                gradients.constraints.copy()
+                if variable_indices is None
+                else gradients.constraints[:, variable_indices]
+            )
+        )
         return (
             np.expand_dims(weighted_objective_gradient, axis=0)
-            if gradients.constraints is None
-            else np.vstack((weighted_objective_gradient, gradients.constraints))
+            if constraint_gradients is None
+            else np.vstack((weighted_objective_gradient, constraint_gradients))
         )
 
     def _get_constraint_scales(self, config: EnOptConfig) -> NDArray[np.float64]:
         assert config.nonlinear_constraints is not None
         scales = self._function_evaluator.constraint_auto_scales
         if scales is None:
             return config.nonlinear_constraints.scales
```

### Comparing `ropt-0.3.0/src/ropt/optimization/_plan.py` & `ropt-0.3.1/src/ropt/optimization/_plan.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/__init__.py` & `ropt-0.3.1/src/ropt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/_manager.py` & `ropt-0.3.1/src/ropt/plugins/_manager.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/function_transform/default.py` & `ropt-0.3.1/src/ropt/plugins/function_transform/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/function_transform/protocol.py` & `ropt-0.3.1/src/ropt/plugins/function_transform/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/_utils.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/default.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/enopt_config.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/evaluator.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,18 @@
             self._private_context.evaluator,
             self._private_context.result_id_iter,
             self._private_context.rng,
             self._private_context.plugin_manager,
         )
 
         if variables is None:
-            variables = self._private_plan.enopt_config.variables.initial_values
+            if self._private_config.variables is None:
+                variables = self._private_plan.enopt_config.variables.initial_values
+            else:
+                variables = self._private_config.variables
 
         exit_code = OptimizerExitCode.EVALUATION_STEP_FINISHED
         try:
             results = ensemble_evaluator.calculate(
                 variables, compute_functions=True, compute_gradients=False
             )
         except OptimizationAborted as exc:
```

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/label.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/label.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/optimizer.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/protocol.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/reset_tracker.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/reset_tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/restart.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/restart.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/tracker.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimization_steps/update_config.py` & `ropt-0.3.1/src/ropt/plugins/optimization_steps/update_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimizer/__init__.py` & `ropt-0.3.1/src/ropt/plugins/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimizer/protocol.py` & `ropt-0.3.1/src/ropt/plugins/optimizer/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimizer/scipy.py` & `ropt-0.3.1/src/ropt/plugins/optimizer/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/optimizer/utils.py` & `ropt-0.3.1/src/ropt/plugins/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/protocol.py` & `ropt-0.3.1/src/ropt/plugins/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/realization_filter/__init__.py` & `ropt-0.3.1/src/ropt/plugins/realization_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/realization_filter/default.py` & `ropt-0.3.1/src/ropt/plugins/realization_filter/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/realization_filter/protocol.py` & `ropt-0.3.1/src/ropt/plugins/realization_filter/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/sampler/__init__.py` & `ropt-0.3.1/src/ropt/plugins/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/sampler/protocol.py` & `ropt-0.3.1/src/ropt/plugins/sampler/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/plugins/sampler/scipy.py` & `ropt-0.3.1/src/ropt/plugins/sampler/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/report/__init__.py` & `ropt-0.3.1/src/ropt/report/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/report/_data_frame.py` & `ropt-0.3.1/src/ropt/report/_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/report/_table.py` & `ropt-0.3.1/src/ropt/report/_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/report/_utils.py` & `ropt-0.3.1/src/ropt/report/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/__init__.py` & `ropt-0.3.1/src/ropt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_bound_constraints.py` & `ropt-0.3.1/src/ropt/results/_bound_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_function_evaluations.py` & `ropt-0.3.1/src/ropt/results/_function_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_function_results.py` & `ropt-0.3.1/src/ropt/results/_function_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_functions.py` & `ropt-0.3.1/src/ropt/results/_functions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_gradient_evaluations.py` & `ropt-0.3.1/src/ropt/results/_gradient_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_gradient_results.py` & `ropt-0.3.1/src/ropt/results/_gradient_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_gradients.py` & `ropt-0.3.1/src/ropt/results/_gradients.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_linear_constraints.py` & `ropt-0.3.1/src/ropt/results/_linear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_maximize.py` & `ropt-0.3.1/src/ropt/results/_maximize.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_nonlinear_constraints.py` & `ropt-0.3.1/src/ropt/results/_nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_pandas.py` & `ropt-0.3.1/src/ropt/results/_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_realizations.py` & `ropt-0.3.1/src/ropt/results/_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_result_field.py` & `ropt-0.3.1/src/ropt/results/_result_field.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_results.py` & `ropt-0.3.1/src/ropt/results/_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_utils.py` & `ropt-0.3.1/src/ropt/results/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/results/_xarray.py` & `ropt-0.3.1/src/ropt/results/_xarray.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/utils/_misc.py` & `ropt-0.3.1/src/ropt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt/utils/scaling.py` & `ropt-0.3.1/src/ropt/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/src/ropt.egg-info/PKG-INFO` & `ropt-0.3.1/src/ropt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.3.0
+Version: 0.3.1
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ropt-0.3.0/src/ropt.egg-info/SOURCES.txt` & `ropt-0.3.1/src/ropt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 src/ropt/config/enopt/_linear_constraints_config.py
 src/ropt/config/enopt/_nonlinear_constraints_config.py
 src/ropt/config/enopt/_objective_functions_config.py
 src/ropt/config/enopt/_optimizer_config.py
 src/ropt/config/enopt/_realization_filter_config.py
 src/ropt/config/enopt/_realizations_config.py
 src/ropt/config/enopt/_sampler_config.py
-src/ropt/config/enopt/_utils.py
 src/ropt/config/enopt/_variables_config.py
 src/ropt/config/enopt/constants.py
 src/ropt/config/plan/__init__.py
 src/ropt/config/plan/_config.py
 src/ropt/config/plan/_plan_config.py
 src/ropt/evaluator/__init__.py
 src/ropt/evaluator/_concurrent.py
```

### Comparing `ropt-0.3.0/tests/conftest.py` & `ropt-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_concurrent.py` & `ropt-0.3.1/tests/test_concurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,46 +54,44 @@
         return cast(NDArray[np.float64], self.future.result())
 
 
 class ConcurrentTestEvaluator(ConcurrentEvaluator):
     def __init__(
         self, functions: Tuple[Callable[..., Any], ...], fail_index: int = -1
     ) -> None:
-        super().__init__(enable_cache=True)
+        super().__init__(enable_cache=True, polling=0.0)
 
         self._executor = ThreadPoolExecutor(max_workers=4)
         self._functions = functions
         self._fail_index = fail_index
         self._tasks: Dict[int, ConcurrentTask]
-        self.polling = 0.0
 
     def launch(
         self,
         batch_id: int,  # noqa: ARG002
+        job_id: int,
         variables: NDArray[np.float64],
         context: EvaluatorContext,  # noqa: ARG002
-        active: Optional[NDArray[np.bool_]],
-    ) -> Dict[int, ConcurrentTask]:
-        self._tasks = {
-            idx: TaskTestEvaluator(
-                future=self._executor.submit(
-                    _run_functions,
-                    self._functions,
-                    variables[idx, :],
-                    self._fail_index == idx,
-                ),
-            )
-            for idx in range(variables.shape[0])
-            if active is None or active[idx]
-        }
-        return self._tasks
+    ) -> Optional[ConcurrentTask]:
+        if job_id == 0:
+            self._tasks = {}
+        task = TaskTestEvaluator(
+            future=self._executor.submit(
+                _run_functions,
+                self._functions,
+                variables,
+                self._fail_index == job_id,
+            ),
+        )
+        self._tasks[job_id] = task
+        return task
 
     def monitor(self) -> None:
         for idx, task in self._tasks.items():
-            if task.future.exception() is not None:
+            if task.future is not None and task.future.exception() is not None:
                 print(f"error in evaluation {idx}")  # noqa: T201
 
     def disable_functions(self) -> None:
         self._functions = (lambda _0, _1: 0.0, lambda _0, _1: 0.0)
 
 
 def test_concurrent(enopt_config: Any, test_functions: Any) -> None:
```

### Comparing `ropt-0.3.0/tests/test_config.py` & `ropt-0.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_ensemble_gradient.py` & `ropt-0.3.1/tests/test_ensemble_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_examples.py` & `ropt-0.3.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_failed_realizations.py` & `ropt-0.3.1/tests/test_failed_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_function_transforms.py` & `ropt-0.3.1/tests/test_function_transforms.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_netcdf.py` & `ropt-0.3.1/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_optimizer.py` & `ropt-0.3.1/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_pandas.py` & `ropt-0.3.1/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_parsl.py` & `ropt-0.3.1/tests/test_parsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ropt.evaluator.parsl import ParslEvaluator, State, Task
 from ropt.optimization import EnsembleOptimizer
 
 
 @dataclass
 class ParslTestTask(Task):
     def get_objectives(self) -> Optional[NDArray[np.float64]]:
+        assert self.future is not None
         result = self.future.result()
         if result is None:
             return None
         return cast(NDArray[np.float64], result)
 
 
 @pytest.fixture(name="enopt_config")
@@ -69,15 +70,15 @@
     variables: NDArray[np.float64],
     context: EvaluatorContext,  # noqa: ARG001
     functions: Tuple[Callable[..., Any], ...],
     fail_index: int = -1,
 ) -> List[ParslTestTask]:
     return [
         ParslTestTask(
-            future=_run_functions(functions, variables[idx, :], fail=idx == fail_index)
+            future=_run_functions(functions, variables, fail=idx == fail_index)
         ),
     ]
 
 
 def parsl_monitor(batch_id: int, jobs: Dict[int, List[ParslTestTask]]) -> None:
     for job_idx, tasks in jobs.items():
         for task_idx, task in enumerate(tasks):
```

### Comparing `ropt-0.3.0/tests/test_realization_filters.py` & `ropt-0.3.1/tests/test_realization_filters.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_result_table.py` & `ropt-0.3.1/tests/test_result_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_results.py` & `ropt-0.3.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_results_data_frame.py` & `ropt-0.3.1/tests/test_results_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_samplers.py` & `ropt-0.3.1/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_scipy_optimizers.py` & `ropt-0.3.1/tests/test_scipy_optimizers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_scipy_samplers.py` & `ropt-0.3.1/tests/test_scipy_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.3.0/tests/test_xarray.py` & `ropt-0.3.1/tests/test_xarray.py`

 * *Files identical despite different names*

