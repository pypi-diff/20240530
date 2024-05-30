# Comparing `tmp/onediff-1.1.0.dev202405280128.tar.gz` & `tmp/onediff-1.1.0.dev202405290129.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.1.0.dev202405280128.tar", last modified: Tue May 28 01:28:28 2024, max compression
+gzip compressed data, was "onediff-1.1.0.dev202405290129.tar", last modified: Wed May 29 01:29:53 2024, max compression
```

## Comparing `onediff-1.1.0.dev202405280128.tar` & `onediff-1.1.0.dev202405290129.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.653484 onediff-1.1.0.dev202405280128/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 01:28:28.653484 onediff-1.1.0.dev202405280128/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:28:28.653484 onediff-1.1.0.dev202405280128/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.637484 onediff-1.1.0.dev202405280128/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.641484 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.641484 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.641484 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.641484 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.641484 onediff-1.1.0.dev202405280128/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.645484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.645484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.645484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/nexfort/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/nexfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/nexfort/nexfort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.645484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.645484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/param_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/torch_utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/torch_utils/module_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/src/onediff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/src/onediff/utils/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.653484 onediff-1.1.0.dev202405280128/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 01:28:28.000000 onediff-1.1.0.dev202405280128/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-28 01:28:28.000000 onediff-1.1.0.dev202405280128/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:28:28.000000 onediff-1.1.0.dev202405280128/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:28:28.000000 onediff-1.1.0.dev202405280128/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 01:28:28.000000 onediff-1.1.0.dev202405280128/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:28.649484 onediff-1.1.0.dev202405280128/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 01:28:21.000000 onediff-1.1.0.dev202405280128/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.784242 onediff-1.1.0.dev202405290129/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.788241 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.788241 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.788241 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.788241 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.788241 onediff-1.1.0.dev202405290129/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.788241 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.792242 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.792242 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/nexfort/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/nexfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/nexfort/nexfort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.792242 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.796242 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/param_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.796242 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.796242 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.796242 onediff-1.1.0.dev202405290129/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.796242 onediff-1.1.0.dev202405290129/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.796242 onediff-1.1.0.dev202405290129/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/src/onediff/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/torch_utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/torch_utils/module_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/src/onediff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/src/onediff/utils/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-29 01:29:53.000000 onediff-1.1.0.dev202405290129/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-29 01:29:53.000000 onediff-1.1.0.dev202405290129/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:29:53.000000 onediff-1.1.0.dev202405290129/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 01:29:53.000000 onediff-1.1.0.dev202405290129/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 01:29:53.000000 onediff-1.1.0.dev202405290129/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:53.800242 onediff-1.1.0.dev202405290129/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-29 01:29:48.000000 onediff-1.1.0.dev202405290129/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.1.0.dev202405280128/LICENSE` & `onediff-1.1.0.dev202405290129/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/PKG-INFO` & `onediff-1.1.0.dev202405290129/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405280128
+Version: 1.1.0.dev202405290129
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405280128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405290129 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405280128/README.md` & `onediff-1.1.0.dev202405290129/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/setup.py` & `onediff-1.1.0.dev202405290129/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.1.0.dev202405290129/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/compiler.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/nexfort/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/nexfort/nexfort.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/nexfort/nexfort.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/dual_module.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/env_var.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/graph.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/oneflow.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/param_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.1.0.dev202405290129/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/optimization/attention_processor.py` & `onediff-1.1.0.dev202405290129/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/optimization/quant_optimizer.py` & `onediff-1.1.0.dev202405290129/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.1.0.dev202405290129/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/quantization/load_quantized_model.py` & `onediff-1.1.0.dev202405290129/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.1.0.dev202405290129/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.1.0.dev202405290129/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/quantization/quantize_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/torch_utils/model_inplace_assign.py` & `onediff-1.1.0.dev202405290129/src/onediff/torch_utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/torch_utils/module_operations.py` & `onediff-1.1.0.dev202405290129/src/onediff/torch_utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/utils/env_var.py` & `onediff-1.1.0.dev202405290129/src/onediff/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff/utils/log_utils.py` & `onediff-1.1.0.dev202405290129/src/onediff/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/src/onediff.egg-info/PKG-INFO` & `onediff-1.1.0.dev202405290129/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405280128
+Version: 1.1.0.dev202405290129
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405280128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405290129 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405280128/src/onediff.egg-info/SOURCES.txt` & `onediff-1.1.0.dev202405290129/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/tests/test_dual_module_list.py` & `onediff-1.1.0.dev202405290129/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.1.0.dev202405290129/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/tests/test_quantitative_quality.py` & `onediff-1.1.0.dev202405290129/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405280128/tests/test_quantize_custom_model.py` & `onediff-1.1.0.dev202405290129/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

