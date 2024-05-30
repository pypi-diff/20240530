# Comparing `tmp/holobench-1.8.0.tar.gz` & `tmp/holobench-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holobench-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "holobench-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `holobench-1.8.0.tar` & `holobench-1.9.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3650 2024-02-05 11:00:04.623454 holobench-1.8.0/README.md
--rw-r--r--   0        0        0     1236 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/__init__.py
--rw-r--r--   0        0        0    18867 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/bench_cfg.py
--rw-r--r--   0        0        0     4088 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/bench_plot_server.py
--rw-r--r--   0        0        0    10528 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/bench_report.py
--rw-r--r--   0        0        0     6072 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/bench_runner.py
--rw-r--r--   0        0        0    32539 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/bencher.py
--rw-r--r--   0        0        0     1627 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/caching.py
--rw-r--r--   0        0        0        0 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/__init__.py
--rw-r--r--   0        0        0     6989 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/benchmark_data.py
--rw-r--r--   0        0        0     1952 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_all.py
--rw-r--r--   0        0        0     3684 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_categorical.py
--rw-r--r--   0        0        0     1916 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_custom_sweep.py
--rw-r--r--   0        0        0     1174 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_docs.py
--rw-r--r--   0        0        0     3425 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_float3D.py
--rw-r--r--   0        0        0     3811 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_float_cat.py
--rw-r--r--   0        0        0     4269 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_floats.py
--rw-r--r--   0        0        0     3697 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_floats2D.py
--rw-r--r--   0        0        0     3180 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_holosweep.py
--rw-r--r--   0        0        0     3228 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_holosweep_objects.py
--rw-r--r--   0        0        0     4540 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_holosweep_tap.py
--rw-r--r--   0        0        0     3477 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_image.py
--rw-r--r--   0        0        0     6896 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_levels.py
--rw-r--r--   0        0        0     2687 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_pareto.py
--rw-r--r--   0        0        0     4200 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_sample_cache.py
--rw-r--r--   0        0        0     4063 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_sample_cache_context.py
--rw-r--r--   0        0        0    11703 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_simple.py
--rw-r--r--   0        0        0     1248 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_simple_bool.py
--rw-r--r--   0        0        0     1760 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_simple_cat.py
--rw-r--r--   0        0        0     1323 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_simple_float.py
--rw-r--r--   0        0        0     1570 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_strings.py
--rw-r--r--   0        0        0     2159 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_time_event.py
--rw-r--r--   0        0        0     3742 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_video.py
--rw-r--r--   0        0        0     6806 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/example_workflow.py
--rw-r--r--   0        0        0      846 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_bokeh_plotly.py
--rw-r--r--   0        0        0     1052 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_hover_ex.py
--rw-r--r--   0        0        0     1815 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_hvplot_explorer.py
--rw-r--r--   0        0        0     2619 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_interactive.py
--rw-r--r--   0        0        0     1414 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_streamnd.py
--rw-r--r--   0        0        0     1030 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_streams.py
--rw-r--r--   0        0        0     1172 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_template.py
--rw-r--r--   0        0        0     1835 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_updates.py
--rw-r--r--   0        0        0     3118 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/experimental/example_vector.py
--rw-r--r--   0        0        0     5605 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/meta/example_meta.py
--rw-r--r--   0        0        0      693 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/meta/example_meta_cat.py
--rw-r--r--   0        0        0      650 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/meta/example_meta_float.py
--rw-r--r--   0        0        0     1488 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/meta/example_meta_levels.py
--rw-r--r--   0        0        0     2370 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/optuna/example_optuna.py
--rw-r--r--   0        0        0     3372 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/shelved/example_float2D_scatter.py
--rw-r--r--   0        0        0     2966 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/shelved/example_float3D_cone.py
--rw-r--r--   0        0        0     2461 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/example/shelved/example_kwargs.py
--rw-r--r--   0        0        0     5927 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/job.py
--rw-r--r--   0        0        0     5303 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/optuna_conversions.py
--rw-r--r--   0        0        0        0 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/plotting/__init__.py
--rw-r--r--   0        0        0     4688 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/plotting/plot_filter.py
--rw-r--r--   0        0        0     3124 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/plotting/plt_cnt_cfg.py
--rw-r--r--   0        0        0        0 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/__init__.py
--rw-r--r--   0        0        0     3444 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/bench_result.py
--rw-r--r--   0        0        0    16257 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/bench_result_base.py
--rw-r--r--   0        0        0        0 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/composable_container/__init__.py
--rw-r--r--   0        0        0     2323 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/composable_container/composable_container_base.py
--rw-r--r--   0        0        0     1221 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/composable_container/composable_container_panel.py
--rw-r--r--   0        0        0     2508 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/composable_container/composable_container_video.py
--rw-r--r--   0        0        0     1746 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/float_formatter.py
--rw-r--r--   0        0        0    22254 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/holoview_result.py
--rw-r--r--   0        0        0    13437 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/optuna_result.py
--rw-r--r--   0        0        0     1115 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/panel_result.py
--rw-r--r--   0        0        0     2132 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/plotly_result.py
--rw-r--r--   0        0        0     1146 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/video_result.py
--rw-r--r--   0        0        0     6977 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/results/video_summary.py
--rw-r--r--   0        0        0     5536 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/utils.py
--rw-r--r--   0        0        0     6393 2024-02-05 11:00:04.623454 holobench-1.8.0/bencher/variables/inputs.py
--rw-r--r--   0        0        0     7361 2024-02-05 11:00:04.627454 holobench-1.8.0/bencher/variables/parametrised_sweep.py
--rw-r--r--   0        0        0     6028 2024-02-05 11:00:04.627454 holobench-1.8.0/bencher/variables/results.py
--rw-r--r--   0        0        0     6559 2024-02-05 11:00:04.627454 holobench-1.8.0/bencher/variables/sweep_base.py
--rw-r--r--   0        0        0     2860 2024-02-05 11:00:04.627454 holobench-1.8.0/bencher/variables/time.py
--rw-r--r--   0        0        0     4409 2024-02-05 11:00:04.627454 holobench-1.8.0/bencher/video_writer.py
--rw-r--r--   0        0        0     1571 2024-02-05 11:00:04.627454 holobench-1.8.0/bencher/worker_job.py
--rw-r--r--   0        0        0     2722 2024-02-05 11:00:04.635454 holobench-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 holobench-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3650 2024-02-07 15:45:27.217096 holobench-1.9.0/README.md
+-rw-r--r--   0        0        0     1236 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/__init__.py
+-rw-r--r--   0        0        0    18867 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/bench_cfg.py
+-rw-r--r--   0        0        0     4088 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/bench_plot_server.py
+-rw-r--r--   0        0        0    10528 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/bench_report.py
+-rw-r--r--   0        0        0     6165 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/bench_runner.py
+-rw-r--r--   0        0        0    32906 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/bencher.py
+-rw-r--r--   0        0        0     1627 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/caching.py
+-rw-r--r--   0        0        0        0 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/__init__.py
+-rw-r--r--   0        0        0     6989 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/benchmark_data.py
+-rw-r--r--   0        0        0     1952 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_all.py
+-rw-r--r--   0        0        0     3684 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_categorical.py
+-rw-r--r--   0        0        0     1916 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_custom_sweep.py
+-rw-r--r--   0        0        0     1174 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_docs.py
+-rw-r--r--   0        0        0     3425 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_float3D.py
+-rw-r--r--   0        0        0     3811 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_float_cat.py
+-rw-r--r--   0        0        0     4269 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_floats.py
+-rw-r--r--   0        0        0     3697 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_floats2D.py
+-rw-r--r--   0        0        0     3180 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_holosweep.py
+-rw-r--r--   0        0        0     3228 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_holosweep_objects.py
+-rw-r--r--   0        0        0     4540 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_holosweep_tap.py
+-rw-r--r--   0        0        0     3856 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_image.py
+-rw-r--r--   0        0        0     6896 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_levels.py
+-rw-r--r--   0        0        0     2687 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_pareto.py
+-rw-r--r--   0        0        0     4200 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_sample_cache.py
+-rw-r--r--   0        0        0     4063 2024-02-07 15:45:27.217096 holobench-1.9.0/bencher/example/example_sample_cache_context.py
+-rw-r--r--   0        0        0    11703 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_simple.py
+-rw-r--r--   0        0        0     1248 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_simple_bool.py
+-rw-r--r--   0        0        0     1760 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_simple_cat.py
+-rw-r--r--   0        0        0     1323 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_simple_float.py
+-rw-r--r--   0        0        0     1570 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_strings.py
+-rw-r--r--   0        0        0     2159 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_time_event.py
+-rw-r--r--   0        0        0     3742 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_video.py
+-rw-r--r--   0        0        0     6806 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/example_workflow.py
+-rw-r--r--   0        0        0      846 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_bokeh_plotly.py
+-rw-r--r--   0        0        0     1052 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_hover_ex.py
+-rw-r--r--   0        0        0     1815 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_hvplot_explorer.py
+-rw-r--r--   0        0        0     2619 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_interactive.py
+-rw-r--r--   0        0        0     1414 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_streamnd.py
+-rw-r--r--   0        0        0     1030 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_streams.py
+-rw-r--r--   0        0        0     1172 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_template.py
+-rw-r--r--   0        0        0     1835 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_updates.py
+-rw-r--r--   0        0        0     3118 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/experimental/example_vector.py
+-rw-r--r--   0        0        0     5605 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/meta/example_meta.py
+-rw-r--r--   0        0        0      693 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/meta/example_meta_cat.py
+-rw-r--r--   0        0        0      650 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/meta/example_meta_float.py
+-rw-r--r--   0        0        0     1488 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/meta/example_meta_levels.py
+-rw-r--r--   0        0        0     2370 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/optuna/example_optuna.py
+-rw-r--r--   0        0        0     3372 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/shelved/example_float2D_scatter.py
+-rw-r--r--   0        0        0     2966 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/shelved/example_float3D_cone.py
+-rw-r--r--   0        0        0     2461 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/example/shelved/example_kwargs.py
+-rw-r--r--   0        0        0     5927 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/job.py
+-rw-r--r--   0        0        0     5303 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/optuna_conversions.py
+-rw-r--r--   0        0        0        0 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/plotting/__init__.py
+-rw-r--r--   0        0        0     4688 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/plotting/plot_filter.py
+-rw-r--r--   0        0        0     3124 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/plotting/plt_cnt_cfg.py
+-rw-r--r--   0        0        0        0 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/__init__.py
+-rw-r--r--   0        0        0     3444 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/bench_result.py
+-rw-r--r--   0        0        0    18545 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/bench_result_base.py
+-rw-r--r--   0        0        0        0 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/composable_container/__init__.py
+-rw-r--r--   0        0        0     2383 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/composable_container/composable_container_base.py
+-rw-r--r--   0        0        0     1221 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/composable_container/composable_container_panel.py
+-rw-r--r--   0        0        0     2508 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/composable_container/composable_container_video.py
+-rw-r--r--   0        0        0     1746 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/float_formatter.py
+-rw-r--r--   0        0        0    22297 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/holoview_result.py
+-rw-r--r--   0        0        0    13437 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/optuna_result.py
+-rw-r--r--   0        0        0     1403 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/panel_result.py
+-rw-r--r--   0        0        0     2132 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/plotly_result.py
+-rw-r--r--   0        0        0     1146 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/video_result.py
+-rw-r--r--   0        0        0     6977 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/results/video_summary.py
+-rw-r--r--   0        0        0     5595 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/utils.py
+-rw-r--r--   0        0        0     6571 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/variables/inputs.py
+-rw-r--r--   0        0        0     7361 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/variables/parametrised_sweep.py
+-rw-r--r--   0        0        0     6028 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/variables/results.py
+-rw-r--r--   0        0        0     6560 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/variables/sweep_base.py
+-rw-r--r--   0        0        0     2860 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/variables/time.py
+-rw-r--r--   0        0        0     4409 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/video_writer.py
+-rw-r--r--   0        0        0     1571 2024-02-07 15:45:27.221096 holobench-1.9.0/bencher/worker_job.py
+-rw-r--r--   0        0        0     2722 2024-02-07 15:45:27.233096 holobench-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 holobench-1.9.0/PKG-INFO
```

### Comparing `holobench-1.8.0/README.md` & `holobench-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/__init__.py` & `holobench-1.9.0/bencher/__init__.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/bench_cfg.py` & `holobench-1.9.0/bencher/bench_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/bench_plot_server.py` & `holobench-1.9.0/bencher/bench_plot_server.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/bench_report.py` & `holobench-1.9.0/bencher/bench_report.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/bench_runner.py` & `holobench-1.9.0/bencher/bench_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,25 +99,26 @@
 
         if level is not None:
             min_level = level
             max_level = level
         for r in range(1, repeats + 1):
             for lvl in range(min_level, max_level + 1):
                 if grouped:
-                    report_level = BenchReport(f"{self.name}_{run_cfg.run_tag}")
+                    report_level = BenchReport(f"{run_cfg.run_tag}_{self.name}")
 
                 for bch_fn in self.bench_fns:
                     run_lvl = deepcopy(run_cfg)
                     run_lvl.level = lvl
                     run_lvl.repeats = r
                     logging.info(f"Running {bch_fn} at level: {lvl} with repeats:{r}")
                     if grouped:
                         res = bch_fn(run_lvl, report_level)
                     else:
                         res = bch_fn(run_lvl, BenchReport())
+                        res.report.bench_name = f"{run_cfg.run_tag}_{res.report.bench_name}"
                         self.show_publish(res.report, show, publish, save, debug)
                     self.results.append(res)
                 if grouped:
                     self.show_publish(report_level, show, publish, save, debug)
         return self.results
 
     def show_publish(self, report, show, publish, save, debug):
```

### Comparing `holobench-1.8.0/bencher/bencher.py` & `holobench-1.9.0/bencher/bencher.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,16 +171,21 @@
         # Maybe put this in SweepCfg
         self.input_vars = None
         self.result_vars = None
         self.const_vars = None
         self.plot_callbacks = []
         self.plot = True
 
-    def add_plot_callback(self, callback: Callable[[BenchResult], pn.panel]) -> None:
-        self.plot_callbacks.append(callback)
+    def add_plot_callback(self, callback: Callable[[BenchResult], pn.panel], **kwargs) -> None:
+        """Add a plotting callback that will be called on any result produced when calling a sweep funciton.  You can pass additional arguments to the plotting function with kwargs.  e.g.  add_plot_callback(bch.BenchResult.to_video_grid,)
+
+        Args:
+            callback (Callable[[BenchResult], pn.panel]): _description_
+        """
+        self.plot_callbacks.append(partial(callback, **kwargs))
 
     def set_worker(self, worker: Callable, worker_input_cfg: ParametrizedSweep = None) -> None:
         """Set the benchmark worker function and optionally the type the worker expects
 
         Args:
             worker (Callable): The benchmark worker function
             worker_input_cfg (ParametrizedSweep, optional): The input type the worker expects. Defaults to None.
```

### Comparing `holobench-1.8.0/bencher/caching.py` & `holobench-1.9.0/bencher/caching.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/benchmark_data.py` & `holobench-1.9.0/bencher/example/benchmark_data.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_all.py` & `holobench-1.9.0/bencher/example/example_all.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_categorical.py` & `holobench-1.9.0/bencher/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_custom_sweep.py` & `holobench-1.9.0/bencher/example/example_custom_sweep.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_docs.py` & `holobench-1.9.0/bencher/example/example_docs.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_float3D.py` & `holobench-1.9.0/bencher/example/example_float3D.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_float_cat.py` & `holobench-1.9.0/bencher/example/example_float_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_floats.py` & `holobench-1.9.0/bencher/example/example_floats.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_floats2D.py` & `holobench-1.9.0/bencher/example/example_floats2D.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_holosweep.py` & `holobench-1.9.0/bencher/example/example_holosweep.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_holosweep_objects.py` & `holobench-1.9.0/bencher/example/example_holosweep_objects.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_holosweep_tap.py` & `holobench-1.9.0/bencher/example/example_holosweep_tap.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_image.py` & `holobench-1.9.0/bencher/example/example_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 class BenchPolygons(bch.ParametrizedSweep):
     sides = bch.IntSweep(default=3, bounds=(3, 7))
     radius = bch.FloatSweep(default=1, bounds=(0.2, 1))
     linewidth = bch.FloatSweep(default=1, bounds=(1, 10))
     linestyle = bch.StringSweep(["solid", "dashed", "dotted"])
     color = bch.StringSweep(["red", "green", "blue"])
     polygon = bch.ResultImage()
+    area = bch.ResultVar()
     # hmap = bch.ResultHmap()
 
     def __call__(self, **kwargs):
         self.update_params_from_kwargs(**kwargs)
         points = polygon_points(self.radius, self.sides)
         # self.hmap = hv.Curve(points)
         self.polygon = self.points_to_polygon_png(points, bch.gen_image_path("polygon"))
+        self.area = self.radius * self.sides
         return super().__call__()
 
     def points_to_polygon_png(self, points: list[float], filename: str):
         """Draw a closed polygon and save to png"""
         fig = plt.figure(frameon=False)
         ax = plt.Axes(fig, [0.0, 0.0, 1.0, 1.0], frameon=False)
         ax.set_axis_off()
@@ -48,25 +50,34 @@
 
         return filename
 
 
 def example_image(
     run_cfg: bch.BenchRunCfg = bch.BenchRunCfg(), report: bch.BenchReport = bch.BenchReport()
 ) -> bch.Bench:
+    run_cfg.use_cache = False
     bench = bch.Bench("polygons", BenchPolygons(), run_cfg=run_cfg, report=report)
 
+    bench.result_vars = ["polygon", "area"]
+
+    bench.add_plot_callback(bch.BenchResult.to_sweep_summary)
+    # bench.add_plot_callback(bch.BenchResult.to_auto, level=2)
+    bench.add_plot_callback(bch.BenchResult.to_panes, level=3)
+    # bench.add_plot_callback(bch.BenchResult.to_panes)
+
     sweep_vars = ["sides", "radius", "linewidth", "color"]
+
+    # sweep_vars = ["sides", "radius" ]
+
     for i in range(1, len(sweep_vars)):
         s = sweep_vars[:i]
         bench.plot_sweep(
             f"Polygons Sweeping {len(s)} Parameters",
             input_vars=s,
-            result_vars=[BenchPolygons.param.polygon],
         )
-
     return bench
 
 
 def example_image_vid(
     run_cfg: bch.BenchRunCfg = bch.BenchRunCfg(), report: bch.BenchReport = bch.BenchReport()
 ) -> bch.Bench:
     bench = BenchPolygons().to_bench(run_cfg, report)
@@ -93,10 +104,10 @@
     # def example_image_pairs()
 
     ex_run_cfg = bch.BenchRunCfg()
     ex_run_cfg.use_sample_cache = True
     # ex_run_cfg.debug = True
     # ex_run_cfg.repeats = 2
     ex_run_cfg.level = 4
-    example_image_vid(ex_run_cfg).report.show()
+    # example_image_vid(ex_run_cfg).report.show()
     # example_image_vid_sequential(ex_run_cfg).report.show()
-    # example_image(ex_run_cfg).report.show()
+    example_image(ex_run_cfg).report.show()
```

### Comparing `holobench-1.8.0/bencher/example/example_levels.py` & `holobench-1.9.0/bencher/example/example_levels.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_pareto.py` & `holobench-1.9.0/bencher/example/example_pareto.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_sample_cache.py` & `holobench-1.9.0/bencher/example/example_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_sample_cache_context.py` & `holobench-1.9.0/bencher/example/example_sample_cache_context.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_simple.py` & `holobench-1.9.0/bencher/example/example_simple.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_simple_bool.py` & `holobench-1.9.0/bencher/example/example_simple_bool.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_simple_cat.py` & `holobench-1.9.0/bencher/example/example_simple_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_simple_float.py` & `holobench-1.9.0/bencher/example/example_simple_float.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_strings.py` & `holobench-1.9.0/bencher/example/example_strings.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_time_event.py` & `holobench-1.9.0/bencher/example/example_time_event.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_video.py` & `holobench-1.9.0/bencher/example/example_video.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/example_workflow.py` & `holobench-1.9.0/bencher/example/example_workflow.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_bokeh_plotly.py` & `holobench-1.9.0/bencher/example/experimental/example_bokeh_plotly.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_hover_ex.py` & `holobench-1.9.0/bencher/example/experimental/example_hover_ex.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_hvplot_explorer.py` & `holobench-1.9.0/bencher/example/experimental/example_hvplot_explorer.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_interactive.py` & `holobench-1.9.0/bencher/example/experimental/example_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_streamnd.py` & `holobench-1.9.0/bencher/example/experimental/example_streamnd.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_streams.py` & `holobench-1.9.0/bencher/example/experimental/example_streams.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_template.py` & `holobench-1.9.0/bencher/example/experimental/example_template.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_updates.py` & `holobench-1.9.0/bencher/example/experimental/example_updates.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/experimental/example_vector.py` & `holobench-1.9.0/bencher/example/experimental/example_vector.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/meta/example_meta.py` & `holobench-1.9.0/bencher/example/meta/example_meta.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/meta/example_meta_cat.py` & `holobench-1.9.0/bencher/example/meta/example_meta_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/meta/example_meta_float.py` & `holobench-1.9.0/bencher/example/meta/example_meta_float.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/meta/example_meta_levels.py` & `holobench-1.9.0/bencher/example/meta/example_meta_levels.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/optuna/example_optuna.py` & `holobench-1.9.0/bencher/example/optuna/example_optuna.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/shelved/example_float2D_scatter.py` & `holobench-1.9.0/bencher/example/shelved/example_float2D_scatter.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/shelved/example_float3D_cone.py` & `holobench-1.9.0/bencher/example/shelved/example_float3D_cone.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/example/shelved/example_kwargs.py` & `holobench-1.9.0/bencher/example/shelved/example_kwargs.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/job.py` & `holobench-1.9.0/bencher/job.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/optuna_conversions.py` & `holobench-1.9.0/bencher/optuna_conversions.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/plotting/plot_filter.py` & `holobench-1.9.0/bencher/plotting/plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/plotting/plt_cnt_cfg.py` & `holobench-1.9.0/bencher/plotting/plt_cnt_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/bench_result.py` & `holobench-1.9.0/bencher/results/bench_result.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/bench_result_base.py` & `holobench-1.9.0/bencher/results/bench_result_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 import holoviews as hv
 from functools import partial
 import panel as pn
 
 from bencher.utils import int_to_col, color_tuple_to_css, callable_name
 
 from bencher.variables.parametrised_sweep import ParametrizedSweep
+from bencher.variables.inputs import with_level
+
 from bencher.variables.results import OptDir
 from copy import deepcopy
 from bencher.results.optuna_result import OptunaResult
 from bencher.variables.results import ResultVar
 from bencher.plotting.plot_filter import VarRange, PlotFilter
 
 from bencher.variables.results import (
     ResultReference,
 )
 
 from bencher.results.composable_container.composable_container_panel import ComposableContainerPanel
+from bencher.utils import listify
 
 # todo add plugins
 # https://gist.github.com/dorneanu/cce1cd6711969d581873a88e0257e312
 # https://kaleidoescape.github.io/decorated-plugins/
 
 
 class ReduceType(Enum):
@@ -50,58 +53,63 @@
 
 class BenchResultBase(OptunaResult):
     def result_samples(self) -> int:
         """The number of samples in the results dataframe"""
         return self.ds.count()
 
     def to_hv_dataset(
-        self, reduce: ReduceType = ReduceType.AUTO, result_var: ResultVar = None
+        self, reduce: ReduceType = ReduceType.AUTO, result_var: ResultVar = None, level: int = None
     ) -> hv.Dataset:
         """Generate a holoviews dataset from the xarray dataset.
 
         Args:
             reduce (ReduceType, optional): Optionally perform reduce options on the dataset.  By default the returned dataset will calculate the mean and standard devation over the "repeat" dimension so that the dataset plays nicely with most of the holoviews plot types.  Reduce.Sqeeze is used if there is only 1 repeat and you want the "reduce" variable removed from the dataset. ReduceType.None returns an unaltered dataset. Defaults to ReduceType.AUTO.
 
         Returns:
             hv.Dataset: results in the form of a holoviews dataset
         """
 
         if reduce == ReduceType.NONE:
             kdims = [i.name for i in self.bench_cfg.all_vars]
-            return hv.Dataset(self.to_dataset(reduce, result_var), kdims=kdims)
-        return hv.Dataset(self.to_dataset(reduce, result_var))
+            return hv.Dataset(self.to_dataset(reduce, result_var, level), kdims=kdims)
+        return hv.Dataset(self.to_dataset(reduce, result_var, level))
 
     def to_dataset(
-        self, reduce: ReduceType = ReduceType.AUTO, result_var: ResultVar = None
+        self, reduce: ReduceType = ReduceType.AUTO, result_var: ResultVar = None, level: int = None
     ) -> xr.Dataset:
         """Generate a summarised xarray dataset.
 
         Args:
             reduce (ReduceType, optional): Optionally perform reduce options on the dataset.  By default the returned dataset will calculate the mean and standard devation over the "repeat" dimension so that the dataset plays nicely with most of the holoviews plot types.  Reduce.Sqeeze is used if there is only 1 repeat and you want the "reduce" variable removed from the dataset. ReduceType.None returns an unaltered dataset. Defaults to ReduceType.AUTO.
 
         Returns:
             xr.Dataset: results in the form of an xarray dataset
         """
         if reduce == ReduceType.AUTO:
             reduce = ReduceType.REDUCE if self.bench_cfg.repeats > 1 else ReduceType.SQUEEZE
 
-        ds = self.ds if result_var is None else self.ds[result_var.name]
+        ds_out = self.ds if result_var is None else self.ds[result_var.name]
 
         match (reduce):
             case ReduceType.REDUCE:
-                ds_reduce_mean = ds.mean(dim="repeat", keep_attrs=True)
-                ds_reduce_std = ds.std(dim="repeat", keep_attrs=True)
+                ds_reduce_mean = ds_out.mean(dim="repeat", keep_attrs=True)
+                ds_reduce_std = ds_out.std(dim="repeat", keep_attrs=True)
 
                 for v in ds_reduce_mean.data_vars:
                     ds_reduce_mean[f"{v}_std"] = ds_reduce_std[v]
-                return ds_reduce_mean
+                ds_out = ds_reduce_mean
             case ReduceType.SQUEEZE:
-                return ds.squeeze(drop=True)
-            case _:
-                return ds
+                ds_out = ds_out.squeeze(drop=True)
+        if level is not None:
+            coords_no_repeat = {}
+            for c, v in ds_out.coords.items():
+                if c != "repeat":
+                    coords_no_repeat[c] = with_level(v.to_numpy(), level)
+            return ds_out.sel(coords_no_repeat)
+        return ds_out
 
     def get_optimal_vec(
         self,
         result_var: ParametrizedSweep,
         input_vars: List[ParametrizedSweep],
     ) -> List[Any]:
         """Get the optimal values from the sweep as a vector.
@@ -401,14 +409,53 @@
             val = ref.obj
             if ref.container is not None:
                 return ref.container(val, **kwargs)
         if container is not None:
             return container(val, styles={"background": "white"}, **kwargs)
         return val
 
+    @staticmethod
+    def select_level(
+        dataset: xr.Dataset,
+        level: int,
+        include_types: List[type] = None,
+        exclude_names: List[str] = None,
+    ) -> xr.Dataset:
+        """Given a dataset, return a reduced dataset that only contains data from a specified level.  By default all types of variables are filtered at the specified level.  If you only want to get a reduced level for some types of data you can pass in a list of types to get filtered, You can also pass a list of variables names to exclude from getting filtered
+        Args:
+            dataset (xr.Dataset): dataset to filter
+            level (int): desired data resolution level
+            include_types (List[type], optional): Only filter data of these types. Defaults to None.
+            exclude_names (List[str], optional): Only filter data with these variable names. Defaults to None.
+
+        Returns:
+            xr.Dataset: A reduced dataset at the specified level
+
+        Example:  a dataset with float_var: [1,2,3,4,5] cat_var: [a,b,c,d,e]
+
+        select_level(ds,2) -> [1,5] [a,e]
+        select_level(ds,2,(float)) -> [1,5] [a,b,c,d,e]
+        select_level(ds,2,exclude_names=["cat_var]) -> [1,5] [a,b,c,d,e]
+
+        see test_bench_result_base.py -> test_select_level()
+        """
+        coords_no_repeat = {}
+        for c, v in dataset.coords.items():
+            if c != "repeat":
+                vals = v.to_numpy()
+                print(vals.dtype)
+                include = True
+                if include_types is not None and vals.dtype not in listify(include_types):
+                    include = False
+                if exclude_names is not None and c in listify(exclude_names):
+                    include = False
+                if include:
+                    coords_no_repeat[c] = with_level(v.to_numpy(), level)
+        return dataset.sel(coords_no_repeat)
+
     # MAPPING TO LOWER LEVEL BENCHCFG functions so they are available at a top level.
     def to_sweep_summary(self, **kwargs):
         return self.bench_cfg.to_sweep_summary(**kwargs)
 
     def to_title(self, panel_name: str = None) -> pn.pane.Markdown:
         return self.bench_cfg.to_title(panel_name)
```

### Comparing `holobench-1.8.0/bencher/results/composable_container/composable_container_base.py` & `holobench-1.9.0/bencher/results/composable_container/composable_container_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,19 @@
             return f"{var_name}={var_value}"
         if var_name is not None:
             return f"{var_name}"
         if var_value is not None:
             return f"{var_value}"
         return None
 
-    def __init__(self, horizontal: bool = True) -> None:
+    def __init__(
+        self, horizontal: bool = True, compose_method: ComposeType = ComposeType.right
+    ) -> None:
         self.horizontal: bool = horizontal
-        self.compose_method = ComposeType.right
+        self.compose_method = compose_method
         self.container = []
 
     def append(self, obj: Any) -> None:
         """Add an object to the container.  The relationship between the objects is defined by the ComposeType
 
         Args:
             obj (Any): Object to add to the container
```

### Comparing `holobench-1.8.0/bencher/results/composable_container/composable_container_panel.py` & `holobench-1.9.0/bencher/results/composable_container/composable_container_panel.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/composable_container/composable_container_video.py` & `holobench-1.9.0/bencher/results/composable_container/composable_container_video.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/float_formatter.py` & `holobench-1.9.0/bencher/results/float_formatter.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/holoview_result.py` & `holobench-1.9.0/bencher/results/holoview_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 
     def to_line(self, result_var: Parameter = None, **kwargs) -> Optional[pn.panel]:
         return self.filter(
             self.to_line_ds,
             float_range=VarRange(1, 1),
             cat_range=VarRange(0, None),
             repeats_range=VarRange(1, 1),
+            panel_range=VarRange(0, None),
             reduce=ReduceType.SQUEEZE,
             target_dimension=2,
             result_var=result_var,
             result_types=(ResultVar),
             **kwargs,
         )
```

### Comparing `holobench-1.8.0/bencher/results/optuna_result.py` & `holobench-1.9.0/bencher/results/optuna_result.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/panel_result.py` & `holobench-1.9.0/bencher/results/panel_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 from functools import partial
 import panel as pn
 from param import Parameter
+import holoviews as hv
 from bencher.results.bench_result_base import BenchResultBase, ReduceType
 from bencher.results.video_result import VideoControls
 from bencher.variables.results import (
     PANEL_TYPES,
 )
 
 
@@ -14,19 +15,29 @@
         vc = VideoControls()
         return pn.Column(
             vc.video_controls(),
             self.to_panes(result_var=result_var, container=vc.video_container, **kwargs),
         )
 
     def to_panes(
-        self, result_var: Parameter = None, target_dimension: int = 0, container=None, **kwargs
+        self,
+        result_var: Parameter = None,
+        hv_dataset=None,
+        target_dimension: int = 0,
+        container=None,
+        level: int = None,
+        **kwargs
     ) -> Optional[pn.pane.panel]:
         if container is None:
             container = pn.pane.panel
+        if hv_dataset is None:
+            hv_dataset = self.to_hv_dataset(ReduceType.SQUEEZE, level=level)
+        elif not isinstance(hv_dataset, hv.Dataset):
+            hv_dataset = hv.Dataset(hv_dataset)
         return self.map_plot_panes(
             partial(self.ds_to_container, container=container),
-            hv_dataset=self.to_hv_dataset(ReduceType.SQUEEZE),
+            hv_dataset=hv_dataset,
             target_dimension=target_dimension,
             result_var=result_var,
             result_types=PANEL_TYPES,
             **kwargs,
         )
```

### Comparing `holobench-1.8.0/bencher/results/plotly_result.py` & `holobench-1.9.0/bencher/results/plotly_result.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/video_result.py` & `holobench-1.9.0/bencher/results/video_result.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/results/video_summary.py` & `holobench-1.9.0/bencher/results/video_summary.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/utils.py` & `holobench-1.9.0/bencher/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     try:
         return any_callable.__name__
     except AttributeError:
         return str(any_callable)
 
 
 def listify(obj) -> list:
-    """Take an object and turn it into a list if its not already a list"""
+    """Take an object and turn it into a list if its not already a list.  However if the object is none, don't turn it into a list"""
     if obj is None:
         return None
     if isinstance(obj, list):
         return obj
     if isinstance(obj, tuple):
         return list(obj)
     return [obj]
```

### Comparing `holobench-1.8.0/bencher/variables/inputs.py` & `holobench-1.9.0/bencher/variables/inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,7 +187,12 @@
         return self.sample_values
 
 
 def box(name, center, width):
     var = FloatSweep(default=center, bounds=(center - width, center + width))
     var.name = name
     return var
+
+
+def with_level(arr: list, level) -> list:
+    return IntSweep(sample_values=arr).with_level(level).values()
+    # return tmp.with_sample_values(arr).with_level(level).values()
```

### Comparing `holobench-1.8.0/bencher/variables/parametrised_sweep.py` & `holobench-1.9.0/bencher/variables/parametrised_sweep.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/variables/results.py` & `holobench-1.9.0/bencher/variables/results.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/variables/sweep_base.py` & `holobench-1.9.0/bencher/variables/sweep_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         # TODO set up class properly. Slightly complicated due to slots
         output.samples = samples  # pylint: disable = attribute-defined-outside-init
         if hasattr(output, "step"):
             # hack TODO fix this
             output.step = None  # pylint: disable = attribute-defined-outside-init
         return output
 
-    def with_sample_values(self, sample_values: int) -> SweepBase:
+    def with_sample_values(self, sample_values: list) -> SweepBase:
         output = deepcopy(self)
         # TODO set up class properly. Slightly complicated due to slots
         try:
             output.sample_values = sample_values  # pylint: disable = attribute-defined-outside-init
         except AttributeError:
             output.objects = sample_values  # pylint: disable = attribute-defined-outside-init
         output.samples = len(sample_values)  # pylint: disable = attribute-defined-outside-init
```

### Comparing `holobench-1.8.0/bencher/variables/time.py` & `holobench-1.9.0/bencher/variables/time.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/bencher/video_writer.py` & `holobench-1.9.0/bencher/video_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         clip = moviepy.video.io.ImageSequenceClip.ImageSequenceClip(
             self.images, fps=30, with_mask=False, load_images=True
         )
         self.write_video_raw(clip)
         return self.filename
 
     @staticmethod
-    def create_label(label, width=None, height=20):
+    def create_label(label, width=None, height=14):
         if width is None:
             width = len(label) * 8
         new_img = Image.new("RGB", (width, height), (255, 255, 255))
         # ImageDraw.Draw(new_img).text((width/2, 0), label, (0, 0, 0),align="center",achor="ms")
         ImageDraw.Draw(new_img).text((width / 2.0, 0), label, (0, 0, 0), anchor="mt", font_size=12)
 
         return new_img
```

### Comparing `holobench-1.8.0/bencher/worker_job.py` & `holobench-1.9.0/bencher/worker_job.py`

 * *Files identical despite different names*

### Comparing `holobench-1.8.0/pyproject.toml` & `holobench-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "holobench"
-version = "1.8.0"
+version = "1.9.0"
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A package for benchmarking the performance of arbitrary functions"
 readme = "README.md"
 
 #incompatible with setuptools
 # requires-python = ">= 3.10"
```

### Comparing `holobench-1.8.0/PKG-INFO` & `holobench-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holobench
-Version: 1.8.0
+Version: 1.9.0
 Summary: A package for benchmarking the performance of arbitrary functions
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: holoviews>=1.15,<=1.18.1
 Requires-Dist: numpy>=1.0,<=1.26.3
 Requires-Dist: param>=1.13.0,<=2.0.2
 Requires-Dist: hvplot>=0.8,<=0.9.2
```

