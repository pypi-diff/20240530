# Comparing `tmp/aqtp-0.7.3.tar.gz` & `tmp/aqtp-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtp-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aqtp-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aqtp-0.7.3.tar` & `aqtp-0.7.4.tar`

### file list

```diff
@@ -1,272 +1,272 @@
--rw-r--r--   0        0        0       39 2024-05-13 01:45:52.043967 aqtp-0.7.3/.gitignore
--rw-r--r--   0        0        0      107 2024-05-13 01:45:52.043967 aqtp-0.7.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2024-05-13 01:45:52.043967 aqtp-0.7.3/LICENSE
--rw-r--r--   0        0        0    17310 2024-05-13 01:45:52.047967 aqtp-0.7.3/README.md
--rw-r--r--   0        0        0      641 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/__init__.py
--rw-r--r--   0        0        0      576 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/__init__.py
--rw-r--r--   0        0        0     4354 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_common.py
--rw-r--r--   0        0        0    16011 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_config.py
--rw-r--r--   0        0        0    13928 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_config_schedule_test.py
--rw-r--r--   0        0        0     5177 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_config_utils.py
--rw-r--r--   0        0        0    15655 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/emulated_floating_points.py
--rw-r--r--   0        0        0     5730 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/emulation_utils.py
--rw-r--r--   0        0        0      576 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/__init__.py
--rw-r--r--   0        0        0    13641 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_conv_general.py
--rw-r--r--   0        0        0    12151 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_conv_general_test.py
--rw-r--r--   0        0        0     8861 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_dot_general.py
--rw-r--r--   0        0        0    14977 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_dot_general_test.py
--rw-r--r--   0        0        0     3693 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_matmul.py
--rw-r--r--   0        0        0     3293 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_matmul_test.py
--rw-r--r--   0        0        0     1083 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_ops.py
--rw-r--r--   0        0        0    18180 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_tensor.py
--rw-r--r--   0        0        0     4751 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_tensor_test.py
--rw-r--r--   0        0        0     2705 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_utils.py
--rw-r--r--   0        0        0     4724 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_conv_general.py
--rw-r--r--   0        0        0    28934 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_dot_general.py
--rw-r--r--   0        0        0    37153 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_dot_general_test.py
--rw-r--r--   0        0        0     5315 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_quantizer.py
--rw-r--r--   0        0        0    10687 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_tensor.py
--rw-r--r--   0        0        0     2926 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_tensor_test.py
--rw-r--r--   0        0        0     2632 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/calibration.py
--rw-r--r--   0        0        0    20892 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/config.py
--rw-r--r--   0        0        0    37689 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/config_test.py
--rw-r--r--   0        0        0     5550 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/examples/examples.ipynb
--rw-r--r--   0        0        0    15825 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model.py
--rw-r--r--   0        0        0    27434 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model_test.py
--rw-r--r--   0        0        0     2703 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model.py
--rw-r--r--   0        0        0     5971 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model_test.py
--rw-r--r--   0        0        0    11994 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer.py
--rw-r--r--   0        0        0     2284 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer_test.py
--rw-r--r--   0        0        0    23224 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax.py
--rw-r--r--   0        0        0     7548 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_calibration.py
--rw-r--r--   0        0        0     3835 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_dg_core.py
--rw-r--r--   0        0        0     7966 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_test.py
--rw-r--r--   0        0        0     3183 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/freezer.py
--rw-r--r--   0        0        0     7422 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/freezer_test.py
--rw-r--r--   0        0        0     1672 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/README.md
--rw-r--r--   0        0        0     6896 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
--rw-r--r--   0        0        0     3997 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
--rw-r--r--   0        0        0     6354 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
--rw-r--r--   0        0        0     9016 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
--rw-r--r--   0        0        0     4739 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics.py
--rw-r--r--   0        0        0     8823 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics_test.py
--rw-r--r--   0        0        0     4459 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/int_numerics.py
--rw-r--r--   0        0        0     1434 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/no_numerics.py
--rw-r--r--   0        0        0     1338 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/numerics.py
--rw-r--r--   0        0        0     2539 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops.py
--rw-r--r--   0        0        0     2095 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops_test.py
--rw-r--r--   0        0        0     1862 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/stochastic_rounding.py
--rw-r--r--   0        0        0    15088 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/tiled_dot_general.py
--rw-r--r--   0        0        0     8820 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/tiled_dot_general_test.py
--rw-r--r--   0        0        0     6727 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/transpose.py
--rw-r--r--   0        0        0     4741 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/transpose_test.py
--rw-r--r--   0        0        0     3983 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/utils.py
--rw-r--r--   0        0        0     1590 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/__init__.py
--rw-r--r--   0        0        0    14397 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
--rw-r--r--   0        0        0     1921 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/__init__.py
--rw-r--r--   0        0        0    17225 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils.py
--rw-r--r--   0        0        0    24127 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils_test.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax/__init__.py
--rw-r--r--   0        0        0     5671 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax/struct.py
--rw-r--r--   0        0        0    35156 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention.py
--rw-r--r--   0        0        0    25400 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention_test.py
--rw-r--r--   0        0        0    43061 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers.py
--rw-r--r--   0        0        0    75454 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers_test.py
--rw-r--r--   0        0        0     6897 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast.py
--rw-r--r--   0        0        0     7682 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast_test.py
--rw-r--r--   0        0        0     9842 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds.py
--rw-r--r--   0        0        0    11477 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds_test.py
--rw-r--r--   0        0        0     3477 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils.py
--rw-r--r--   0        0        0     2570 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils_test.py
--rw-r--r--   0        0        0    10045 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/__init__.py
--rw-r--r--   0        0        0     1963 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/check_config_util.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/__init__.py
--rw-r--r--   0        0        0     7382 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/base_config.py
--rw-r--r--   0        0        0     1207 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
--rw-r--r--   0        0        0      853 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
--rw-r--r--   0        0        0     1230 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
--rw-r--r--   0        0        0     1439 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
--rw-r--r--   0        0        0     1231 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
--rw-r--r--   0        0        0     2000 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
--rw-r--r--   0        0        0     6443 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
--rw-r--r--   0        0        0     1647 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
--rw-r--r--   0        0        0     7476 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
--rw-r--r--   0        0        0      855 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
--rw-r--r--   0        0        0      855 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
--rw-r--r--   0        0        0      925 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
--rw-r--r--   0        0        0     1439 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
--rw-r--r--   0        0        0     1440 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
--rw-r--r--   0        0        0     1390 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
--rw-r--r--   0        0        0     1514 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
--rw-r--r--   0        0        0     1383 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
--rw-r--r--   0        0        0     1025 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
--rw-r--r--   0        0        0      925 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
--rw-r--r--   0        0        0     1232 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
--rw-r--r--   0        0        0     6856 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
--rw-r--r--   0        0        0     9732 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
--rw-r--r--   0        0        0     2423 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_test.py
--rw-r--r--   0        0        0     2130 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/hparams_config.py
--rw-r--r--   0        0        0   331485 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/imagenet.png
--rw-r--r--   0        0        0     8129 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/input_pipeline.py
--rw-r--r--   0        0        0     7345 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models.py
--rw-r--r--   0        0        0     9773 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models_test.py
--rw-r--r--   0        0        0    15474 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn.py
--rw-r--r--   0        0        0     3119 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
--rw-r--r--   0        0        0       62 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/requirements.txt
--rw-r--r--   0        0        0     5749 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
--rw-r--r--   0        0        0    19735 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train.py
--rw-r--r--   0        0        0     2611 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_benchmark.py
--rw-r--r--   0        0        0     2547 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_test.py
--rw-r--r--   0        0        0     7991 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_utils.py
--rw-r--r--   0        0        0     5854 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/primitives.py
--rw-r--r--   0        0        0     6508 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/primitives_test.py
--rw-r--r--   0        0        0     3927 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/quant_config.py
--rw-r--r--   0        0        0    63283 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/quantization.py
--rw-r--r--   0        0        0    45534 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/quantization_test.py
--rw-r--r--   0        0        0     1654 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/shape_utils.py
--rw-r--r--   0        0        0    22231 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
--rw-r--r--   0        0        0    23430 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
--rw-r--r--   0        0        0     9798 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/stats.py
--rw-r--r--   0        0        0     6060 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag.py
--rw-r--r--   0        0        0     9777 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag_test.py
--rw-r--r--   0        0        0    10461 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/stats_test.py
--rw-r--r--   0        0        0     4637 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/test_utils.py
--rw-r--r--   0        0        0     5435 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/train_utils.py
--rw-r--r--   0        0        0     6454 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/train_utils_test.py
--rw-r--r--   0        0        0      995 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/utils.py
--rw-r--r--   0        0        0     2888 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
--rw-r--r--   0        0        0     7056 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
--rw-r--r--   0        0        0    15134 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/decode.py
--rw-r--r--   0        0        0    12107 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
--rw-r--r--   0        0        0    11082 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
--rw-r--r--   0        0        0    13257 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
--rw-r--r--   0        0        0     6573 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
--rw-r--r--   0        0        0     1069 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1069 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1056 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1041 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
--rw-r--r--   0        0        0     1006 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1193 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
--rw-r--r--   0        0        0      954 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1101 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
--rw-r--r--   0        0        0     1002 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1042 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
--rw-r--r--   0        0        0     1002 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
--rw-r--r--   0        0        0     1060 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1175 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
--rw-r--r--   0        0        0     1244 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
--rw-r--r--   0        0        0     1664 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
--rw-r--r--   0        0        0     1661 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
--rw-r--r--   0        0        0     1662 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
--rw-r--r--   0        0        0     1662 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
--rw-r--r--   0        0        0     2172 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
--rw-r--r--   0        0        0     1600 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1849 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1323 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1448 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1344 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
--rw-r--r--   0        0        0     1568 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1801 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1584 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
--rw-r--r--   0        0        0     1479 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
--rw-r--r--   0        0        0     1495 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
--rw-r--r--   0        0        0     1531 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
--rw-r--r--   0        0        0     1046 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
--rw-r--r--   0        0        0     1245 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
--rw-r--r--   0        0        0     1245 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
--rw-r--r--   0        0        0     1549 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1380 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1380 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2052 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
--rw-r--r--   0        0        0     1340 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
--rw-r--r--   0        0        0     1340 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     2032 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1757 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
--rw-r--r--   0        0        0     1729 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
--rw-r--r--   0        0        0     2133 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
--rw-r--r--   0        0        0     1238 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     1238 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
--rw-r--r--   0        0        0     1587 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1379 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1379 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2123 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
--rw-r--r--   0        0        0     1213 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
--rw-r--r--   0        0        0     1213 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
--rw-r--r--   0        0        0     1554 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1375 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1375 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2063 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
--rw-r--r--   0        0        0     2523 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
--rw-r--r--   0        0        0      995 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
--rw-r--r--   0        0        0     1672 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
--rw-r--r--   0        0        0     2392 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
--rw-r--r--   0        0        0     1222 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
--rw-r--r--   0        0        0     2101 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
--rw-r--r--   0        0        0     3356 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
--rw-r--r--   0        0        0     1531 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
--rw-r--r--   0        0        0     1965 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
--rw-r--r--   0        0        0      382 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
--rw-r--r--   0        0        0     1096 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1014 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1096 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1018 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
--rw-r--r--   0        0        0      995 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
--rw-r--r--   0        0        0     1925 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
--rw-r--r--   0        0        0    23300 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
--rw-r--r--   0        0        0    33382 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models.py
--rw-r--r--   0        0        0    38051 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
--rw-r--r--   0        0        0     4055 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/predict.py
--rw-r--r--   0        0        0      160 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
--rw-r--r--   0        0        0    51590 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train.py
--rw-r--r--   0        0        0     5666 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
--rw-r--r--   0        0        0    10503 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
--rw-r--r--   0        0        0     3939 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
--rw-r--r--   0        0        0    25395 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
--rw-r--r--   0        0        0     3284 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
--rw-r--r--   0        0        0      118 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/requirements.txt
--rw-r--r--   0        0        0    10519 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/README.md
--rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/__init__.py
--rw-r--r--   0        0        0     4810 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils.py
--rw-r--r--   0        0        0     5109 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils_test.py
--rw-r--r--   0        0        0     1045 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/common.py
--rw-r--r--   0        0        0     8505 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils.py
--rw-r--r--   0        0        0    11978 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils_test.py
--rw-r--r--   0        0        0     6844 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/hparams_utils.py
--rw-r--r--   0        0        0    10185 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils.py
--rw-r--r--   0        0        0    10192 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils_test.py
--rw-r--r--   0        0        0    20428 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/report_utils.py
--rw-r--r--   0        0        0    23689 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/report_utils_test.py
--rw-r--r--   0        0        0     2538 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils.py
--rw-r--r--   0        0        0     3451 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils_test.py
--rw-r--r--   0        0        0     6640 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils.py
--rw-r--r--   0        0        0     4307 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils_test.py
--rw-r--r--   0        0        0    15648 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_conv_test_base.py
--rw-r--r--   0        0        0    11192 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_matmul_test_base.py
--rw-r--r--   0        0        0    12101 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_stats_test_base.py
--rw-r--r--   0        0        0    23072 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_tensor_test_base.py
--rw-r--r--   0        0        0     4694 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_test_shared_base.py
--rw-r--r--   0        0        0   129585 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/aqt/aqt.pdf
--rw-r--r--   0        0        0     1303 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/aqt/aqt.tex
--rw-r--r--   0        0        0     1468 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/pokebnn/README.md
--rw-r--r--   0        0        0     2862 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/pokebnn/cloudtpu_train_pokebnn.sh
--rw-r--r--   0        0        0   117523 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/pokebnn/tensorboard.ipynb
--rw-r--r--   0        0        0      727 2024-05-13 01:45:52.059967 aqtp-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1852 2024-05-13 01:45:52.059967 aqtp-0.7.3/setup.py
--rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-30 03:12:42.957254 aqtp-0.7.4/.gitignore
+-rw-r--r--   0        0        0      107 2024-05-30 03:12:42.957254 aqtp-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2024-05-30 03:12:42.957254 aqtp-0.7.4/LICENSE
+-rw-r--r--   0        0        0    17310 2024-05-30 03:12:42.957254 aqtp-0.7.4/README.md
+-rw-r--r--   0        0        0      641 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/__init__.py
+-rw-r--r--   0        0        0      576 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/__init__.py
+-rw-r--r--   0        0        0     4354 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/aqt_common.py
+-rw-r--r--   0        0        0    16011 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/aqt_config.py
+-rw-r--r--   0        0        0    13928 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/aqt_config_schedule_test.py
+-rw-r--r--   0        0        0     5177 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/aqt_config_utils.py
+-rw-r--r--   0        0        0    15655 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/emulated_floating_points.py
+-rw-r--r--   0        0        0     5730 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/common/emulation_utils.py
+-rw-r--r--   0        0        0      576 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/__init__.py
+-rw-r--r--   0        0        0    13641 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_conv_general.py
+-rw-r--r--   0        0        0    12151 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_conv_general_test.py
+-rw-r--r--   0        0        0     8861 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_dot_general.py
+-rw-r--r--   0        0        0    14977 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     3693 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_matmul.py
+-rw-r--r--   0        0        0     3293 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_matmul_test.py
+-rw-r--r--   0        0        0     1083 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_ops.py
+-rw-r--r--   0        0        0    18180 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_tensor.py
+-rw-r--r--   0        0        0     4751 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2705 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/aqt_utils.py
+-rw-r--r--   0        0        0     4724 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/aqt_conv_general.py
+-rw-r--r--   0        0        0    28934 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/aqt_dot_general.py
+-rw-r--r--   0        0        0    37227 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     5315 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/aqt_quantizer.py
+-rw-r--r--   0        0        0    10873 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/aqt_tensor.py
+-rw-r--r--   0        0        0     2926 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2774 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax/v2/calibration.py
+-rw-r--r--   0        0        0    20892 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/config.py
+-rw-r--r--   0        0        0    37689 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/config_test.py
+-rw-r--r--   0        0        0     5550 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/examples/examples.ipynb
+-rw-r--r--   0        0        0    15825 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/examples/flax_e2e_model.py
+-rw-r--r--   0        0        0    27434 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/examples/flax_e2e_model_test.py
+-rw-r--r--   0        0        0     2703 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model.py
+-rw-r--r--   0        0        0     5971 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model_test.py
+-rw-r--r--   0        0        0    11994 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer.py
+-rw-r--r--   0        0        0     2284 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer_test.py
+-rw-r--r--   0        0        0    24223 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax.py
+-rw-r--r--   0        0        0     7548 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax_calibration.py
+-rw-r--r--   0        0        0     3835 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax_dg_core.py
+-rw-r--r--   0        0        0    13504 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax_test.py
+-rw-r--r--   0        0        0     3183 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/freezer.py
+-rw-r--r--   0        0        0     7422 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/freezer_test.py
+-rw-r--r--   0        0        0     1672 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/intercept/README.md
+-rw-r--r--   0        0        0     6896 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
+-rw-r--r--   0        0        0     3997 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
+-rw-r--r--   0        0        0     6354 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
+-rw-r--r--   0        0        0     9016 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
+-rw-r--r--   0        0        0     4739 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/numerics/fp8_numerics.py
+-rw-r--r--   0        0        0     8943 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/numerics/fp8_numerics_test.py
+-rw-r--r--   0        0        0     4459 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/numerics/int_numerics.py
+-rw-r--r--   0        0        0     1434 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/numerics/no_numerics.py
+-rw-r--r--   0        0        0     1338 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/numerics/numerics.py
+-rw-r--r--   0        0        0     2539 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/pax/pax_base_ops.py
+-rw-r--r--   0        0        0     2095 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/pax/pax_base_ops_test.py
+-rw-r--r--   0        0        0     1862 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/stochastic_rounding.py
+-rw-r--r--   0        0        0    15439 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax/v2/tiled_dot_general.py
+-rw-r--r--   0        0        0     8820 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax/v2/tiled_dot_general_test.py
+-rw-r--r--   0        0        0     9167 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax/v2/transpose.py
+-rw-r--r--   0        0        0     5249 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax/v2/transpose_test.py
+-rw-r--r--   0        0        0     4308 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax/v2/utils.py
+-rw-r--r--   0        0        0     1590 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/__init__.py
+-rw-r--r--   0        0        0    14397 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
+-rw-r--r--   0        0        0     1921 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/__init__.py
+-rw-r--r--   0        0        0    17225 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/compute_cost_utils.py
+-rw-r--r--   0        0        0    24127 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/compute_cost_utils_test.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/flax/__init__.py
+-rw-r--r--   0        0        0     5671 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/flax/struct.py
+-rw-r--r--   0        0        0    35156 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/flax_attention.py
+-rw-r--r--   0        0        0    25400 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/flax_attention_test.py
+-rw-r--r--   0        0        0    43061 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/flax_layers.py
+-rw-r--r--   0        0        0    75454 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/flax_layers_test.py
+-rw-r--r--   0        0        0     6897 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/fp_cast.py
+-rw-r--r--   0        0        0     7682 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/fp_cast_test.py
+-rw-r--r--   0        0        0     9842 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/get_bounds.py
+-rw-r--r--   0        0        0    11477 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/get_bounds_test.py
+-rw-r--r--   0        0        0     3477 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/hlo_utils.py
+-rw-r--r--   0        0        0     2570 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/hlo_utils_test.py
+-rw-r--r--   0        0        0    10045 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/__init__.py
+-rw-r--r--   0        0        0     1963 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/check_config_util.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/__init__.py
+-rw-r--r--   0        0        0     7382 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/base_config.py
+-rw-r--r--   0        0        0     1207 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
+-rw-r--r--   0        0        0      853 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
+-rw-r--r--   0        0        0     1230 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
+-rw-r--r--   0        0        0     1439 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
+-rw-r--r--   0        0        0     1231 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
+-rw-r--r--   0        0        0     2000 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
+-rw-r--r--   0        0        0     6443 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
+-rw-r--r--   0        0        0     1647 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
+-rw-r--r--   0        0        0     7476 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
+-rw-r--r--   0        0        0      855 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
+-rw-r--r--   0        0        0      855 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
+-rw-r--r--   0        0        0      925 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
+-rw-r--r--   0        0        0     1439 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
+-rw-r--r--   0        0        0     1440 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
+-rw-r--r--   0        0        0     1390 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
+-rw-r--r--   0        0        0     1514 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
+-rw-r--r--   0        0        0     1383 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
+-rw-r--r--   0        0        0     1025 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
+-rw-r--r--   0        0        0      925 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
+-rw-r--r--   0        0        0     1232 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
+-rw-r--r--   0        0        0     6856 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
+-rw-r--r--   0        0        0     9732 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
+-rw-r--r--   0        0        0     2423 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_test.py
+-rw-r--r--   0        0        0     2130 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/hparams_config.py
+-rw-r--r--   0        0        0   331485 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/imagenet.png
+-rw-r--r--   0        0        0     8129 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/input_pipeline.py
+-rw-r--r--   0        0        0     7345 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/models.py
+-rw-r--r--   0        0        0     9773 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/models_test.py
+-rw-r--r--   0        0        0    15474 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/pokebnn.py
+-rw-r--r--   0        0        0     3119 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
+-rw-r--r--   0        0        0       62 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/requirements.txt
+-rw-r--r--   0        0        0     5749 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
+-rw-r--r--   0        0        0    19735 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train.py
+-rw-r--r--   0        0        0     2611 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train_benchmark.py
+-rw-r--r--   0        0        0     2547 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train_test.py
+-rw-r--r--   0        0        0     7991 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train_utils.py
+-rw-r--r--   0        0        0     5854 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/primitives.py
+-rw-r--r--   0        0        0     6508 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/primitives_test.py
+-rw-r--r--   0        0        0     3927 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/quant_config.py
+-rw-r--r--   0        0        0    63283 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/quantization.py
+-rw-r--r--   0        0        0    45534 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/quantization_test.py
+-rw-r--r--   0        0        0     1654 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/shape_utils.py
+-rw-r--r--   0        0        0    22231 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
+-rw-r--r--   0        0        0    23430 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
+-rw-r--r--   0        0        0     9798 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/stats.py
+-rw-r--r--   0        0        0     6060 2024-05-30 03:12:42.977254 aqtp-0.7.4/aqt/jax_legacy/jax/stats_tag.py
+-rw-r--r--   0        0        0     9777 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/stats_tag_test.py
+-rw-r--r--   0        0        0    10461 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/stats_test.py
+-rw-r--r--   0        0        0     4637 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/test_utils.py
+-rw-r--r--   0        0        0     5435 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/train_utils.py
+-rw-r--r--   0        0        0     6454 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/train_utils_test.py
+-rw-r--r--   0        0        0      995 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/utils.py
+-rw-r--r--   0        0        0     2888 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
+-rw-r--r--   0        0        0     7056 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
+-rw-r--r--   0        0        0    15134 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/decode.py
+-rw-r--r--   0        0        0    12107 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
+-rw-r--r--   0        0        0    11082 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
+-rw-r--r--   0        0        0    13257 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
+-rw-r--r--   0        0        0     6573 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
+-rw-r--r--   0        0        0     1069 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1069 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1056 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1041 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
+-rw-r--r--   0        0        0     1006 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1193 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
+-rw-r--r--   0        0        0      954 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1101 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
+-rw-r--r--   0        0        0     1002 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1042 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
+-rw-r--r--   0        0        0     1002 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-05-30 03:12:42.961254 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
+-rw-r--r--   0        0        0     1060 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1175 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
+-rw-r--r--   0        0        0     1244 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
+-rw-r--r--   0        0        0     1664 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
+-rw-r--r--   0        0        0     1661 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
+-rw-r--r--   0        0        0     1662 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
+-rw-r--r--   0        0        0     1662 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
+-rw-r--r--   0        0        0     2172 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
+-rw-r--r--   0        0        0     1600 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1849 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1323 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1448 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1344 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
+-rw-r--r--   0        0        0     1568 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1801 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1584 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
+-rw-r--r--   0        0        0     1479 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
+-rw-r--r--   0        0        0     1495 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
+-rw-r--r--   0        0        0     1531 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
+-rw-r--r--   0        0        0     1046 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
+-rw-r--r--   0        0        0     1245 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
+-rw-r--r--   0        0        0     1245 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
+-rw-r--r--   0        0        0     1549 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1380 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1380 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2052 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
+-rw-r--r--   0        0        0     1340 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
+-rw-r--r--   0        0        0     1340 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     2032 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1757 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
+-rw-r--r--   0        0        0     1729 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
+-rw-r--r--   0        0        0     2133 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1238 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1238 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1587 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1379 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1379 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2123 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1213 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1213 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1554 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1375 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1375 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2063 2024-05-30 03:12:42.965253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
+-rw-r--r--   0        0        0     2523 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
+-rw-r--r--   0        0        0      995 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1672 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
+-rw-r--r--   0        0        0     2392 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
+-rw-r--r--   0        0        0     1222 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
+-rw-r--r--   0        0        0     2101 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
+-rw-r--r--   0        0        0     3356 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
+-rw-r--r--   0        0        0     1531 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
+-rw-r--r--   0        0        0     1965 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
+-rw-r--r--   0        0        0      382 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
+-rw-r--r--   0        0        0     1096 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1014 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1096 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1018 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
+-rw-r--r--   0        0        0      995 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1925 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
+-rw-r--r--   0        0        0    23300 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
+-rw-r--r--   0        0        0    33382 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/models.py
+-rw-r--r--   0        0        0    38051 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
+-rw-r--r--   0        0        0     4055 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/predict.py
+-rw-r--r--   0        0        0      160 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
+-rw-r--r--   0        0        0    51590 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/train.py
+-rw-r--r--   0        0        0     5666 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
+-rw-r--r--   0        0        0    10503 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
+-rw-r--r--   0        0        0     3939 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
+-rw-r--r--   0        0        0    25395 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
+-rw-r--r--   0        0        0     3284 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
+-rw-r--r--   0        0        0      118 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/requirements.txt
+-rw-r--r--   0        0        0    10519 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/utils/README.md
+-rw-r--r--   0        0        0      577 2024-05-30 03:12:42.969253 aqtp-0.7.4/aqt/jax_legacy/utils/__init__.py
+-rw-r--r--   0        0        0     4810 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/analysis_utils.py
+-rw-r--r--   0        0        0     5109 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/analysis_utils_test.py
+-rw-r--r--   0        0        0     1045 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/common.py
+-rw-r--r--   0        0        0     8505 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/config_schema_utils.py
+-rw-r--r--   0        0        0    11978 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/config_schema_utils_test.py
+-rw-r--r--   0        0        0     6844 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/hparams_utils.py
+-rw-r--r--   0        0        0    10185 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/pandas_utils.py
+-rw-r--r--   0        0        0    10192 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/pandas_utils_test.py
+-rw-r--r--   0        0        0    20428 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/report_utils.py
+-rw-r--r--   0        0        0    23689 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/report_utils_test.py
+-rw-r--r--   0        0        0     2538 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/summary_utils.py
+-rw-r--r--   0        0        0     3451 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/summary_utils_test.py
+-rw-r--r--   0        0        0     6640 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/tfevent_utils.py
+-rw-r--r--   0        0        0     4307 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/jax_legacy/utils/tfevent_utils_test.py
+-rw-r--r--   0        0        0    15648 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/test/aqt_conv_test_base.py
+-rw-r--r--   0        0        0    11192 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/test/aqt_matmul_test_base.py
+-rw-r--r--   0        0        0    12101 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/test/aqt_stats_test_base.py
+-rw-r--r--   0        0        0    23072 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/test/aqt_tensor_test_base.py
+-rw-r--r--   0        0        0     4694 2024-05-30 03:12:42.973253 aqtp-0.7.4/aqt/test/aqt_test_shared_base.py
+-rw-r--r--   0        0        0   129585 2024-05-30 03:12:42.973253 aqtp-0.7.4/papers/aqt/aqt.pdf
+-rw-r--r--   0        0        0     1303 2024-05-30 03:12:42.973253 aqtp-0.7.4/papers/aqt/aqt.tex
+-rw-r--r--   0        0        0     1468 2024-05-30 03:12:42.973253 aqtp-0.7.4/papers/pokebnn/README.md
+-rw-r--r--   0        0        0     2862 2024-05-30 03:12:42.973253 aqtp-0.7.4/papers/pokebnn/cloudtpu_train_pokebnn.sh
+-rw-r--r--   0        0        0   117523 2024-05-30 03:12:42.977254 aqtp-0.7.4/papers/pokebnn/tensorboard.ipynb
+-rw-r--r--   0        0        0      727 2024-05-30 03:12:42.977254 aqtp-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1852 2024-05-30 03:12:42.977254 aqtp-0.7.4/setup.py
+-rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.4/PKG-INFO
```

### Comparing `aqtp-0.7.3/LICENSE` & `aqtp-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/README.md` & `aqtp-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/__init__.py` & `aqtp-0.7.4/aqt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Accurate Quantized Training library."""
 
-__version__ = "0.7.3"
+__version__ = "0.7.4"
```

### Comparing `aqtp-0.7.3/aqt/common/__init__.py` & `aqtp-0.7.4/aqt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/common/aqt_common.py` & `aqtp-0.7.4/aqt/common/aqt_common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/common/aqt_config.py` & `aqtp-0.7.4/aqt/common/aqt_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/common/aqt_config_schedule_test.py` & `aqtp-0.7.4/aqt/common/aqt_config_schedule_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/common/aqt_config_utils.py` & `aqtp-0.7.4/aqt/common/aqt_config_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/common/emulated_floating_points.py` & `aqtp-0.7.4/aqt/common/emulated_floating_points.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/common/emulation_utils.py` & `aqtp-0.7.4/aqt/common/emulation_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/__init__.py` & `aqtp-0.7.4/aqt/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_conv_general.py` & `aqtp-0.7.4/aqt/jax/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_conv_general_test.py` & `aqtp-0.7.4/aqt/jax/aqt_conv_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_dot_general.py` & `aqtp-0.7.4/aqt/jax/aqt_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_dot_general_test.py` & `aqtp-0.7.4/aqt/jax/aqt_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_matmul.py` & `aqtp-0.7.4/aqt/jax/aqt_matmul.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_matmul_test.py` & `aqtp-0.7.4/aqt/jax/aqt_matmul_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_ops.py` & `aqtp-0.7.4/aqt/jax/aqt_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_tensor.py` & `aqtp-0.7.4/aqt/jax/aqt_tensor.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_tensor_test.py` & `aqtp-0.7.4/aqt/jax/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/aqt_utils.py` & `aqtp-0.7.4/aqt/jax/aqt_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/aqt_conv_general.py` & `aqtp-0.7.4/aqt/jax/v2/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/aqt_dot_general.py` & `aqtp-0.7.4/aqt/jax/v2/aqt_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/aqt_dot_general_test.py` & `aqtp-0.7.4/aqt/jax/v2/aqt_dot_general_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,17 @@
   trityps = [trityp for trityp in jaxpr_to_trityp(f_jaxpr)]
   assert len(trityps) == len(dg_raws)
   for (lhs_sa, rhs_sa, out_sa), dg_raw in zip(trityps, dg_raws):
     # If cfg has None, the type is inherited from the arguments' type.
     def assert_dtype_eq(dtype1, dtype2):
       assert dtype1 == dtype2, f"dtype1 != dtype2: {dtype1=} != {dtype2=}"
 
-    assert isinstance(dg_raw.dg_quantizer, aqt.DefaultDotGeneralQuantizer)
+    assert isinstance(
+        dg_raw.dg_quantizer, aqt.DefaultDotGeneralQuantizer
+    ), f"Invalid dg_quantizer type. {type(dg_raw.dg_quantizer)=}"
 
     lhs_dtype = dg_raw.dg_quantizer.lhs.numerics.get_dtype()
     rhs_dtype = dg_raw.dg_quantizer.rhs.numerics.get_dtype()
     assert_dtype_eq(lhs_sa.dtype, lhs_dtype or float_dtype)
     assert_dtype_eq(rhs_sa.dtype, rhs_dtype or float_dtype)
     assert_dtype_eq(out_sa.dtype, dg_raw.dg_accumulator_dtype or float_dtype)
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/aqt_quantizer.py` & `aqtp-0.7.4/aqt/jax/v2/aqt_quantizer.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/aqt_tensor.py` & `aqtp-0.7.4/aqt/jax/v2/aqt_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,20 +86,24 @@
     """Returns a copy of the QTensor without the qvalue."""
     return self.replace(qvalue=None)  # pytype: disable=attribute-error
 
   def astype(self, dtype: jnp.dtype) -> Self:
     return self.replace(dequant_dtype=dtype)  # pytype: disable=attribute-error
 
   def quant(self, x):
+    """Quantizes the QTensor."""
     assert not self.is_full(), 'Already quantized QTensor.'
     assert self.scale is not None, 'Missing scales to be used for quantization.'
 
     qvalue = x
     for s in self.scale:
-      qvalue = qvalue * jax.lax.reciprocal(s)
+      # TODO(lew): We could store s_inv for faster activation quantization.
+      s_inv = jax.lax.reciprocal(s)
+      s_inv = jnp.where(jnp.isinf(s_inv), jnp.ones_like(s_inv), s_inv)
+      qvalue = qvalue * s_inv
 
     # TODO(lew): We should apply numerics here, so that 'quant' function
     # Can be considered a part of API.
     return self.replace(qvalue=qvalue)  # pytype: disable=attribute-error
 
   def dequant(self) -> jnp.ndarray:
     """Dequantizes the QTensor."""
@@ -161,15 +165,15 @@
   )
 
 
 def zeros_with_scale(
     shape: Sequence[int],
     calibration_axis: Sequence[utils.AxisIdx],
     *,
-    container_dtype: jnp.dtype | None = None,
+    container_dtype: jnp.dtype,
     scale_dtype: jnp.dtype | None = None,
     dequant_dtype: jnp.dtype = jnp.bfloat16,
 ) -> QTensor:
   """Initializes a QTensor with empty qvalue along with empty scale value."""
   scale_shape = list(shape)
   for axis in calibration_axis:
     scale_shape[axis] = 1
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/aqt_tensor_test.py` & `aqtp-0.7.4/aqt/jax/v2/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/calibration.py` & `aqtp-0.7.4/aqt/jax/v2/calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,11 +77,13 @@
         ' to set them.'
     )
     assert shared_axes is not None, msg
 
     # NOTE: If you want to clip, consider using clip and clip_gradient in
     # int_numerics.IntNumerics.
     abs_max = jnp.max(jnp.abs(x), axis=shared_axes, keepdims=True)
+    # TODO(yichizh): the zero filtering is not needed anymore because inf is
+    # filtered when calculating the reciprocal of scaline factor
     abs_max = jnp.where(abs_max == 0.0, jnp.ones_like(abs_max), abs_max)
     if self.scale is not None:
       abs_max = abs_max * self.scale
     return abs_max.astype(x.dtype)
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/config.py` & `aqtp-0.7.4/aqt/jax/v2/config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/config_test.py` & `aqtp-0.7.4/aqt/jax/v2/config_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/examples/examples.ipynb` & `aqtp-0.7.4/aqt/jax/v2/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model.py` & `aqtp-0.7.4/aqt/jax/v2/examples/flax_e2e_model.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model_test.py` & `aqtp-0.7.4/aqt/jax/v2/examples/flax_e2e_model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             "cpu": [
                 3.123474359512329101562500000000,
                 3.123474597930908203125000000000,
                 3.123473882675170898437500000000,  # colab
             ],
             "TPU v2": [3.198328018188476562500000000000],
             "TPU v3": [3.198328018188476562500000000000],
-            "TPU v4": [3.198297739028930664062500000000],
-            "TPU v5 lite": [3.198297977447509765625000000000],
+            "TPU v4": [3.198297500610351562500000000000],
+            "TPU v5 lite": [3.198297500610351562500000000000],
         },
         4: {
             "cpu": [2.258865118026733398437500000000],
             "TPU v2": [2.302409172058105468750000000000],
             "TPU v3": [2.302409172058105468750000000000],
             "TPU v4": [2.302409172058105468750000000000],
             "TPU v5 lite": [2.302409172058105468750000000000],
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model.py` & `aqtp-0.7.4/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model_test.py` & `aqtp-0.7.4/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer.py` & `aqtp-0.7.4/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer_test.py` & `aqtp-0.7.4/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax.py` & `aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,22 @@
 import jax.numpy as jnp
 
 
 NoShardingAxes = Sequence[utils.AxisIdx]
 AxisMetadataWrapper = Callable[
     [jnp.ndarray, NoShardingAxes], nn_meta.AxisMetadata
 ]
+DotGeneralTilingFn = Callable[
+    [jnp.ndarray, jnp.ndarray, jax.lax.DotDimensionNumbers],
+    tiled_dot_general.Cfg
+]
+EinsumTilingFn = Callable[
+    [tiled_dot_general.EinsumEqnLetter, jnp.ndarray, jnp.ndarray],
+    tiled_dot_general.Cfg
+]
 
 
 class FreezerMode(enum.Enum):
   NONE = 1
   CALIBRATION = 2
   CALIBRATION_AND_VALUE = 3
 
@@ -209,15 +217,18 @@
   # CALIBRATION_AND_VALUE to store both scales and quantized values.
   lhs_freeze_mode: FreezerMode = FreezerMode.NONE
   rhs_freeze_mode: FreezerMode = FreezerMode.NONE
 
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
+
+  # Tiling configs. tilling_fn is valid only when tiling_cfg is None.
   tiling_cfg: Optional[tiled_dot_general.Cfg] = None
+  tiling_fn: Optional[DotGeneralTilingFn] = None
 
   # If set to True, use the current Freezer. Otherwise, use the new
   # QuantFreezer.
   use_legacy_freezer: bool = True
 
   def make_aqt_dg(
       self,
@@ -293,24 +304,24 @@
           return qt
 
         scale_non_shard_axis_all = list(range(qt.ndim))
         scale_non_shard_axis_contracting = list(contracting_axis)
 
         qt = qt.replace(
             qvalue=axis_metadata_wrapper(qt.qvalue, []),
-            scale=jax.tree_map(
+            scale=jax.tree.map(
                 lambda x: axis_metadata_wrapper(
                     x, scale_non_shard_axis_contracting
                 ),
                 qt.scale,
             ),
             # Passing scale_non_shard_axis_contracting would be incorrect due to
             # scale transposition. scale_t is being removed from QTensor anyway
             # so we just pass scale_non_shard_axis_all.
-            scale_t=jax.tree_map(
+            scale_t=jax.tree.map(
                 lambda x: axis_metadata_wrapper(x, scale_non_shard_axis_all),
                 qt.scale_t,
             ),
         )
         return qt
 
       lhs_ca, rhs_ca = contr
@@ -446,19 +457,23 @@
       self,
       lhs,
       rhs,
       dimension_numbers,
       precision,
       preferred_element_type=None,
   ):
-    if self.tiling_cfg is not None:
+    tiling_cfg = self.tiling_cfg
+    if tiling_cfg is None and self.tiling_fn is not None:
+      tiling_cfg = self.tiling_fn(lhs, rhs, dimension_numbers)
+
+    if tiling_cfg is not None:
       # Extract tiled input shapes and dimension numbers from jaxpr
       def dummy_tiled_dg(lhs_in, rhs_in):
         return tiled_dot_general.tiled_dot_general(
-            self.tiling_cfg, lhs_in, rhs_in, dimension_numbers
+            tiling_cfg, lhs_in, rhs_in, dimension_numbers
         )
 
       tiled_dg_jaxpr = jax.make_jaxpr(dummy_tiled_dg)(lhs, rhs)
       dg_eqn = [eqn for eqn in tiled_dg_jaxpr.eqns if 'dot_general' in str(eqn)]
       assert len(dg_eqn) == 1, 'Multiple dg calls are found in tiled dg jaxpr.'
       lhs_invar, rhs_invar = dg_eqn[0].invars
       tiled_lhs_shape = lhs_invar.aval.shape
@@ -469,15 +484,15 @@
       aqt_dg = self.make_aqt_dg(
           tiled_lhs_shape, tiled_rhs_shape, tiled_dimension_numbers
       )
       # We integrate tiling here and not on Jax level, so that the Freezers
       # observe tiled shapes.
       ret_dg = functools.partial(
           tiled_dot_general.tiled_dot_general,
-          self.tiling_cfg,
+          tiling_cfg,
           dot_general=aqt_dg,
       )
     else:
       ret_dg = self.make_aqt_dg(lhs.shape, rhs.shape, dimension_numbers)
     return ret_dg(
         lhs,
         rhs,
@@ -520,14 +535,15 @@
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
 
   assert_eqn: Optional[str] = None
   assert_lhs_shape: Optional[utils.ShapeTemplate] = None
   assert_rhs_shape: Optional[utils.ShapeTemplate] = None
   tile_sizes: Optional[tiled_dot_general.EinsumTileSizes] = None
+  tiling_fn: Optional[EinsumTilingFn] = None
 
   # If set to True, use the current Freezer. Otherwise, use the new
   # QTensorFreezer.
   use_legacy_freezer: bool = True
 
   @nn.compact
   def __call__(
@@ -556,15 +572,23 @@
     lhs_in = jnp.zeros_like(lhs_g.qvalue) if lhs_is_qt else lhs_g
     rhs_in = jnp.zeros_like(rhs_g.qvalue) if rhs_is_qt else rhs_g
 
     # Set the types of dummy input to the same as original input, to prevent it
     # from being rejected by assertions in aqt_dot_general.py, line 522-526 and
     # 414.
     # TODO: b/322111904 - Handle this in more proper way.
-    lhs_in, rhs_in = nn.dtypes.promote_dtype(lhs_in, rhs_in)
+    # We hand-hold int4 because promote_dtype(int4, x) fails.
+    # (To avoid unintended promotion, 4-bit integers do not support
+    # implicit promotion.)
+    if lhs_in.dtype == jnp.int4:
+      lhs_in = jnp.float32(lhs_in)
+    if rhs_in.dtype == jnp.int4:
+      rhs_in = jnp.float32(rhs_in)
+    if lhs_in.dtype != jnp.int4 and rhs_in.dtype != jnp.int4:
+      lhs_in, rhs_in = nn.dtypes.promote_dtype(lhs_in, rhs_in)
 
     # yes_swap = whether einsum swaps [lhs,rhs] when passing them to dot_general
     einsum = functools.partial(aqt_dot_general.einsum, eqn=eqn)
     a = jax.make_jaxpr(einsum)(lhs=lhs_in, rhs=rhs_in)
     [lhs_g_id, rhs_g_id] = a.eqns[0].invars
     [lhs_l_id, rhs_l_id] = a.jaxpr.invars
     not_swap = lhs_g_id == lhs_l_id and rhs_g_id == rhs_l_id
@@ -590,14 +614,16 @@
     lhs_freeze_mode = self.lhs_freeze_mode
     rhs_freeze_mode = self.rhs_freeze_mode
 
     quant_collection = self.quant_collection
     tiling_config = None
     if self.tile_sizes is not None:
       tiling_config = tiled_dot_general.Cfg.from_einsum(eqn, self.tile_sizes)
+    elif self.tiling_fn is not None:
+      tiling_config = self.tiling_fn(eqn, lhs_in, rhs_in)
 
     if yes_swap:
       if cfg is not None:
         cfg = copy.deepcopy(cfg)
         cfg.fwd.lhs, cfg.fwd.rhs = cfg.fwd.rhs, cfg.fwd.lhs
         cfg.fwd.dg_quantizer.swap_lhs_and_rhs()
         cfg.dlhs, cfg.drhs = cfg.drhs, cfg.dlhs
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_calibration.py` & `aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax_calibration.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_dg_core.py` & `aqtp-0.7.4/aqt/jax/v2/flax/aqt_flax_dg_core.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/freezer.py` & `aqtp-0.7.4/aqt/jax/v2/flax/freezer.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/freezer_test.py` & `aqtp-0.7.4/aqt/jax/v2/flax/freezer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,16 @@
     value3 = {'sub1': jax.random.normal(subkeys[4], (1, 4)),
               'sub2': jax.random.normal(subkeys[5], (3, 6)),
               'sub3': jax.random.normal(subkeys[6], (7, 7))}
     return _CustomStructure(value1, value2, value3)
 
   def _assert_same_tree_shape_dtype(self, tree1, tree2):
     """Checks if the two given pytrees have the same structure with the same leaves' shapes and dtypes."""
-    leaves1, treedef1 = jax.tree_flatten(tree1)
-    leaves2, treedef2 = jax.tree_flatten(tree2)
+    leaves1, treedef1 = jax.tree.flatten(tree1)
+    leaves2, treedef2 = jax.tree.flatten(tree2)
 
     # 1. Check if they have the same tree structure.
     self.assertEqual(treedef1, treedef2)
 
     # 2. Check if the leaves are with the same shapes and dtypes.
     self.assertEqual(len(leaves1), len(leaves2))
     for leaf1, leaf2 in zip(leaves1, leaves2):
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/intercept/README.md` & `aqtp-0.7.4/aqt/jax/v2/flax/intercept/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py` & `aqtp-0.7.4/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py` & `aqtp-0.7.4/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py` & `aqtp-0.7.4/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py` & `aqtp-0.7.4/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 ),
             ],
             remaining_axes=[],
         ),
     )
     target_loss = {
         8: {
-            "TPU v5 lite": [3.222529888153076171875000000000],
+            "TPU v5 lite": [3.222228527069091796875000000000],
         },
         4: {
             "TPU v5 lite": [2.292296886444091796875000000000],
         },
     }
     # below 3 lines are differences between config_v4/v3 and fully_quantized
     config.set_stochastic_rounding(aqt_cfg, True, True, "jax.uniform")
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics.py` & `aqtp-0.7.4/aqt/jax/v2/numerics/fp8_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics_test.py` & `aqtp-0.7.4/aqt/jax/v2/numerics/fp8_numerics_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,31 +124,33 @@
     target_loss = {
         "e4m3": {
             "cpu": [
                 # Different CPU models are not bit exact and sometimes produce
                 # different losses under the same training setting.
                 3.167505979537963867187500000000,
                 3.167067050933837890625000000000,  # skylake, cascadelake
+                3.167066574096679687500000000000,  # colab
             ],
             "TPU v2": [3.210080146789550781250000000000],
             "TPU v3": [3.210082530975341796875000000000],
-            "TPU v4": [3.210082530975341796875000000000],
-            "TPU v5 lite": [3.212916374206542968750000000000],
+            "TPU v4": [3.213466644287109375000000000000],
+            "TPU v5 lite": [3.213290691375732421875000000000],
         },
         "e5m2": {
             "cpu": [
                 # Different CPU models are not bit exact and sometimes produce
                 # different losses under the same training setting.
                 3.112026929855346679687500000000,
                 3.112026691436767578125000000000,
+                3.112027168273925781250000000000,  # colab s
             ],
             "TPU v2": [3.181228160858154296875000000000],
             "TPU v3": [3.181227684020996093750000000000],
-            "TPU v4": [3.181228160858154296875000000000],
-            "TPU v5 lite": [3.181028842926025390625000000000],
+            "TPU v4": [3.181212902069091796875000000000],
+            "TPU v5 lite": [3.181214332580566406250000000000],
         },
     }
 
     # RNGs
     rng = jax.random.key(0)
     rng, init_rng = jax.random.split(rng)
     rng, image_rng = jax.random.split(rng)
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/numerics/int_numerics.py` & `aqtp-0.7.4/aqt/jax/v2/numerics/int_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/numerics/no_numerics.py` & `aqtp-0.7.4/aqt/jax/v2/numerics/no_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/numerics/numerics.py` & `aqtp-0.7.4/aqt/jax/v2/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops.py` & `aqtp-0.7.4/aqt/jax/v2/pax/pax_base_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops_test.py` & `aqtp-0.7.4/aqt/jax/v2/pax/pax_base_ops_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/stochastic_rounding.py` & `aqtp-0.7.4/aqt/jax/v2/stochastic_rounding.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/tiled_dot_general.py` & `aqtp-0.7.4/aqt/jax/v2/tiled_dot_general.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 
 # pylint: disable=g-explicit-bool-comparison
 # pylint: disable=g-explicit-length-test
 
 import copy
 import dataclasses
 import pprint
-from typing import Literal
+from typing import Iterable
 from absl import logging
 from aqt.jax.v2 import utils
 import jax
 import jax.numpy as jnp
-import numpy as np
 from typing_extensions import Self  # for python version < 3.11
 
 
 AxisIdx = utils.AxisIdx
 AxisSize = utils.AxisSize
 EinsumEqnLetter = str
 EinsumTileSizes = dict[EinsumEqnLetter, AxisSize]
@@ -162,102 +161,105 @@
   return map(lambda x, y: x * y, l, r)
 
 
 def get_ra(rank, ca, ba) -> list[AxisIdx]:
   return list(a for a in range(rank) if a not in ca + ba)
 
 
-def sort_ra_cfg(ra_tiling: list[AxisTiling]) -> list[AxisTiling]:
-  ra_axes = [a.axis for a in ra_tiling]
-  sorted_idx = np.argsort(ra_axes).tolist()
-  return [ra_tiling[i] for i in sorted_idx]
-
-
-def empty_list():
-  return dataclasses.field(default_factory=list)
+def maybe_add_one(i, min_i):
+  return i + int(i >= min_i)
 
 
 @dataclasses.dataclass(frozen=False, slots=True)
 class _Xhs:
   """Structure for bookkeeping of AxisIdx while tiling."""
 
   x: jnp.ndarray
 
   # Below are axes indices, similar to dimension_numbers
   # E.g.
-  #   xhs,shape == [10, 20, 30, ...] ca=[0,1,2], ca_tile=[]
-  #   After splitting axis 1 to 2 tiles, sized 10, we get
-  #   xhs,shape == [10, 2, 10, 30, ...], ca=[0,2,3], ca_tile=[1]
-  #   and other axes indices (ra, ra_tile, ba) also can be updated by +1.
-  ca: list[AxisIdx]
-  ra: list[AxisIdx]
-
-  ca_tile: list[AxisIdx] = empty_list()  # to be summed after DG
-  ra_tile: list[AxisIdx] = empty_list()  # to be reshaped after DG
-  ra_tile_other: list[AxisIdx] = empty_list()  # to be reshaped after DG
-  # There is no point in tiling dot_general's batch axes
-  ba: list[AxisIdx] = dataclasses.field(default_factory=list)
-
-  # axes waiting to be slitted
-  # tensor_tiling: TensorTiling # TODO(lew): use this
-  ca_to_be_tiled: list[AxisTiling] = empty_list()
-  ra_to_be_tiled: list[AxisTiling] = empty_list()
+  #   assert xhs.shape == [10, 20, 30, ...],
+  #   assert tile_map == {0:[0], 1:[1], 2:[2], ...}
+  # After splitting axis 1 to 2 tiles, sized 10, we get
+  #   assert xhs.shape == [10, 2, 10, 30, ...]
+  #   assert tile_map == {0:[0], 1:[1,2], 2:[3], ...}
+  tile_map: dict[AxisIdx | str, list[AxisIdx]] = utils.dataclass_field(dict)
+
+  def __post_init__(self):
+    for i in range(self.x.ndim):
+      # self.x is not yet split at all.
+      self.tile_map[i] = [i]
 
-  def tile_axis(self, at: AxisTiling, tile_axis_name: Literal['ca', 'ra']):
+  def tile_axis(self, at: AxisTiling):
     """Tiles (splits) one axis while maintaining all AxisIdx."""
+    tile_axis = self.tile_map[at.axis]
+    assert len(tile_axis) == 1, "can't tile the same axis twice."
+    tile_axis = tile_axis[0]
+
+    # Reshape self.x
     shape = list(self.x.shape)
-    msg = f'{shape[at.axis]=}, {at.tile_size=}, {at.tile_count=}'
-    assert shape[at.axis] == at.tile_size * at.tile_count, msg
-    shape[at.axis] = at.tile_size
-    shape.insert(at.axis, at.tile_count)
+    msg = f'{shape[tile_axis]=}, {at.tile_size=}, {at.tile_count=}'
+    assert shape[tile_axis] == at.tile_size * at.tile_count, msg
+    shape[tile_axis] = at.tile_size
+    shape.insert(tile_axis, at.tile_count)
     self.x = self.x.reshape(shape)
 
-    def update(axes):
-      for i in range(len(axes)):
-        axes[i] += int(axes[i] >= at.axis)
-
-    def update_tiling(axes):
-      for i in range(len(axes)):
-        axes[i].axis += int(axes[i].axis >= at.axis)
-
-    update(self.ca)
-    update(self.ca_tile)
-    update(self.ra)
-    update(self.ra_tile)
-    update(self.ra_tile_other)
-    update(self.ba)
-
-    update_tiling(self.ca_to_be_tiled)
-    update_tiling(self.ra_to_be_tiled)
-    # Append tile axis index at the beginning. This has to be after the update
-    match tile_axis_name:
-      case 'ca':
-        self.ca_tile.append(at.axis)
-      case 'ra':
-        self.ra_tile.append(at.axis)
+    # Update tile_map
+    for k in self.tile_map:
+      self.tile_map[k] = [
+          maybe_add_one(ai, tile_axis) for ai in self.tile_map[k]
+      ]
+    self.tile_map[at.axis] = [tile_axis, tile_axis + 1]
+
+  def tile_axes(self, ats: Iterable[AxisTiling]):
+    for at in ats:
+      self.tile_axis(at)
 
   def broadcast_to_other(self, bcast_shape: tuple[AxisSize, ...]):
     """Adds new axes (bcast_shape) on AxisIdx=0."""
-    assert self.ra_tile_other == list(), 'ra_tile_other already set'
-    self.ra_tile_other = list(range(len(bcast_shape)))
     self.x = jnp.broadcast_to(self.x, bcast_shape + self.x.shape)
-
-    def update(axes):
-      for i in range(len(axes)):
-        axes[i] += len(bcast_shape)
-
-    update(self.ca)
-    update(self.ca_tile)
-    update(self.ra)
-    update(self.ra_tile)
-    update(self.ba)
+    for k in self.tile_map:
+      self.tile_map[k] = [ai + len(bcast_shape) for ai in self.tile_map[k]]
+    keys = []
+    for i in range(len(bcast_shape)):
+      k = f'broadcast_{i}'
+      keys.append(k)
+      assert k not in self.tile_map
+      self.tile_map[k] = [i]
+    return keys
 
   def axes_shape(self, axes: list[AxisIdx]) -> tuple[AxisSize, ...]:
     return tuple(map(lambda a: self.x.shape[a], axes))
 
+  def to_tiled_axes_transposed(
+      self,
+      axes: Iterable[AxisIdx | str],
+      tile_level: int,
+  ) -> tuple[list[AxisIdx], ...]:
+    # pylint: disable=g-doc-args,g-doc-return-or-yield
+    """The given 'axes' parameter defines axes in untiled represented Array.
+
+    Function returns the corresponding AxisIdxs in self.x which is tiled. So for
+    each give element of axes we can have multiple tiled axes. Function requires
+    that the tile granularity is the same for all axes and equal to the given
+    tile_level.
+
+    tile_level = 1 for untiled axis
+    tile_level = 2 for normally (one axis split into two) tiled.
+    """
+    lsts = [self.tile_map[ai] for ai in axes]
+    msg = (
+        'all requested axes shoudl have the same tile level, but we have:'
+        f' {lsts=} for {axes=}'
+    )
+    assert all(map(lambda tiled_ais: len(tiled_ais) == tile_level, lsts)), msg
+    if lsts == []:
+      return ([],) * tile_level
+    return tuple(map(list, zip(*lsts)))
+
 
 def print_dimension_numbers(dimension_numbers, lhs, rhs, label) -> None:
   """Prints dimension numbers before and/or after tiling.
 
   Args:
     dimension_numbers: It contains the left and right hand side contraction axes
       and batch axes.
@@ -289,72 +291,69 @@
     dot_general=jax.lax.dot_general,
 ):
   """local dot_general."""
 
   logging.vlog(1, 'Tiling config cfg: %s', cfg)
   print_dimension_numbers(dimension_numbers, lhs, rhs, label='before tiling')
 
+  # Config pre-processing and verification
+
   cfg = copy.deepcopy(cfg)
   cfg = cfg.complete_missing(lhs.shape, rhs.shape, dimension_numbers)
   (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
   lhs_ra = get_ra(lhs.ndim, lhs_ca, lhs_ba)
   rhs_ra = get_ra(rhs.ndim, rhs_ca, rhs_ba)
   g_msg = (
       'Before tiling: \n'
       f'lhs: {lhs.shape=}, {lhs_ca=}, {lhs_ba=}, {lhs_ra=} \n'
       f'rhs: {rhs.shape=}, {rhs_ca=}, {rhs_ba=}, {rhs_ra=} \n'
       f'tiling cfg: {pprint.pformat(cfg)} \n'
   )
 
-  xlhs = _Xhs(
-      x=lhs,
-      ca=list(lhs_ca),
-      ra=lhs_ra,
-      ba=list(lhs_ba),
-      ca_to_be_tiled=cfg.lhs.contraction_axes,
-      ra_to_be_tiled=sort_ra_cfg(cfg.lhs.remaining_axes),
-  )
-  xrhs = _Xhs(
-      x=rhs,
-      ca=list(rhs_ca),
-      ra=rhs_ra,
-      ba=list(rhs_ba),
-      ca_to_be_tiled=cfg.rhs.contraction_axes,
-      ra_to_be_tiled=sort_ra_cfg(cfg.rhs.remaining_axes),
-  )
-
   # First tile_axis CA. CA tile_count axes will be first in xxhs.ba_tile
-  assert len(xlhs.ca_to_be_tiled) == len(xrhs.ca_to_be_tiled), g_msg
-  while len(xlhs.ca_to_be_tiled) > 0:
-    cfg_lhs_ca = xlhs.ca_to_be_tiled.pop(0)
-    cfg_rhs_ca = xrhs.ca_to_be_tiled.pop(0)
+  assert len(cfg.lhs.contraction_axes) == len(cfg.rhs.contraction_axes), g_msg
+  for cfg_lhs_ca, cfg_rhs_ca in zip(
+      cfg.lhs.contraction_axes, cfg.rhs.contraction_axes
+  ):
     msg = (
         'Contraction axis tile counts should be the same, but found lhs axis'
         f' {cfg_lhs_ca.axis} has a tile count of {cfg_lhs_ca.tile_count}, and'
         f' rhs axis {cfg_rhs_ca.axis} has a tile count of'
         f' {cfg_rhs_ca.tile_count}'
     )
     assert cfg_lhs_ca.tile_count == cfg_rhs_ca.tile_count, msg
-    xlhs.tile_axis(cfg_lhs_ca, 'ca')
-    xrhs.tile_axis(cfg_rhs_ca, 'ca')
 
-  while len(xlhs.ra_to_be_tiled) > 0:
-    cfg_lhs_ra = xlhs.ra_to_be_tiled.pop(0)
-    xlhs.tile_axis(cfg_lhs_ra, 'ra')
-  while len(xrhs.ra_to_be_tiled) > 0:
-    cfg_rhs_ra = xrhs.ra_to_be_tiled.pop(0)
-    xrhs.tile_axis(cfg_rhs_ra, 'ra')
+  # Tiling
 
-  xlhs.broadcast_to_other(xrhs.axes_shape(xrhs.ra_tile))
-  xrhs.broadcast_to_other(xlhs.axes_shape(xlhs.ra_tile))
+  xlhs = _Xhs(x=lhs)
+  xlhs.tile_axes(cfg.lhs.contraction_axes + cfg.lhs.remaining_axes)
+  xrhs = _Xhs(x=rhs)
+  xrhs.tile_axes(cfg.rhs.contraction_axes + cfg.rhs.remaining_axes)
+
+  # DotGeneral reshapeing
+
+  xlhs_ra_tile, _ = xlhs.to_tiled_axes_transposed(lhs_ra, 2)
+  xrhs_bcast = xrhs.broadcast_to_other(xlhs.axes_shape(xlhs_ra_tile))
+
+  xrhs_ra_tile, _ = xrhs.to_tiled_axes_transposed(rhs_ra, 2)
+  xlhs_bcast = xlhs.broadcast_to_other(xrhs.axes_shape(xrhs_ra_tile))
+
+  xlhs_ca_tile, xlhs_ca = xlhs.to_tiled_axes_transposed(lhs_ca, 2)
+  xlhs_ra_tile, xlhs_ra = xlhs.to_tiled_axes_transposed(lhs_ra, 2)
+  xrhs_ca_tile, xrhs_ca = xrhs.to_tiled_axes_transposed(rhs_ca, 2)
+  xrhs_ra_tile, xrhs_ra = xrhs.to_tiled_axes_transposed(rhs_ra, 2)
+  (xlhs_ra_tile_other,) = xlhs.to_tiled_axes_transposed(xlhs_bcast, 1)
+  (xrhs_ra_tile_other,) = xrhs.to_tiled_axes_transposed(xrhs_bcast, 1)
+  (xlhs_ba,) = xlhs.to_tiled_axes_transposed(lhs_ba, 1)
+  (xrhs_ba,) = xrhs.to_tiled_axes_transposed(rhs_ba, 1)
 
-  tiled_ca = (xlhs.ca, xrhs.ca)
+  tiled_ca = (xlhs_ca, xrhs_ca)
   tiled_ba = (
-      xlhs.ca_tile + xlhs.ba + xlhs.ra_tile + xlhs.ra_tile_other,
-      xrhs.ca_tile + xrhs.ba + xrhs.ra_tile_other + xrhs.ra_tile,
+      xlhs_ca_tile + xlhs_ba + xlhs_ra_tile + xlhs_ra_tile_other,
+      xrhs_ca_tile + xrhs_ba + xrhs_ra_tile_other + xrhs_ra_tile,
   )
   tiled_dimension_numbers = (tiled_ca, tiled_ba)
   tiled_lhs_ra = get_ra(xlhs.x.ndim, tiled_ca[0], tiled_ba[0])
   tiled_rhs_ra = get_ra(xrhs.x.ndim, tiled_ca[1], tiled_ba[1])
   g_msg += (
       'After tiling: \n'
       f' lhs: lhs.shape={xlhs.x.shape}, lhs_ca={tiled_ca[0]},'
@@ -371,48 +370,48 @@
   )
 
   print_dimension_numbers(
       tiled_dimension_numbers, xlhs.x, xrhs.x, label='after tiling'
   )
 
   # Some assertions
-  assert xlhs.axes_shape(xlhs.ca_tile) == xrhs.axes_shape(xrhs.ca_tile), g_msg
-  ca_tile_sh = xlhs.axes_shape(xlhs.ca_tile)
+  assert xlhs.axes_shape(xlhs_ca_tile) == xrhs.axes_shape(xrhs_ca_tile), g_msg
+  ca_tile_sh = xlhs.axes_shape(xlhs_ca_tile)
 
-  assert xlhs.axes_shape(xlhs.ba) == xrhs.axes_shape(xrhs.ba), g_msg
-  ba_sh = xlhs.axes_shape(xlhs.ba)
+  assert xlhs.axes_shape(xlhs_ba) == xrhs.axes_shape(xrhs_ba), g_msg
+  ba_sh = xlhs.axes_shape(xlhs_ba)
 
-  assert xlhs.axes_shape(xlhs.ra_tile) == xrhs.axes_shape(
-      xrhs.ra_tile_other
+  assert xlhs.axes_shape(xlhs_ra_tile) == xrhs.axes_shape(
+      xrhs_ra_tile_other
   ), g_msg
-  lhs_ra_tile_sh = xlhs.axes_shape(xlhs.ra_tile)
+  lhs_ra_tile_sh = xlhs.axes_shape(xlhs_ra_tile)
 
-  assert xlhs.axes_shape(xlhs.ra_tile_other) == xrhs.axes_shape(
-      xrhs.ra_tile
+  assert xlhs.axes_shape(xlhs_ra_tile_other) == xrhs.axes_shape(
+      xrhs_ra_tile
   ), g_msg
-  rhs_ra_tile_sh = xlhs.axes_shape(xlhs.ra_tile_other)
+  rhs_ra_tile_sh = xlhs.axes_shape(xlhs_ra_tile_other)
 
-  lhs_ra_sh = xlhs.axes_shape(xlhs.ra)
-  rhs_ra_sh = xrhs.axes_shape(xrhs.ra)
+  lhs_ra_sh = xlhs.axes_shape(xlhs_ra)
+  rhs_ra_sh = xrhs.axes_shape(xrhs_ra)
 
   g_msg += f'Tiled dg {out.shape=} \n'
   assert (
       out.shape
       == ca_tile_sh
       + ba_sh
       + lhs_ra_tile_sh
       + rhs_ra_tile_sh
       + lhs_ra_sh
       + rhs_ra_sh
   ), g_msg
 
   # Sum over ca_tile now.
   # all_ba() returns ca_tile as the first axes in ba.
-  assert len(xlhs.ca_tile) == len(xrhs.ca_tile)
-  out = out.sum(axis=range(len(xlhs.ca_tile)))
+  assert len(xlhs_ca_tile) == len(xrhs_ca_tile)
+  out = out.sum(axis=range(len(xlhs_ca_tile)))
 
   g_msg += f'After sum over tiles {out.shape=} \n'
   assert (
       out.shape
       == ba_sh + lhs_ra_tile_sh + rhs_ra_tile_sh + lhs_ra_sh + rhs_ra_sh
   ), g_msg
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/tiled_dot_general_test.py` & `aqtp-0.7.4/aqt/jax/v2/tiled_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax/v2/transpose_test.py` & `aqtp-0.7.4/aqt/jax/v2/transpose_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for transpose."""
 
+import math
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.jax.v2 import transpose
 import jax.numpy as jnp
 
 
 class AqtTransposeTest(parameterized.TestCase):
 
   @parameterized.parameters(
+      ((10, 1, 10), (0, 2, 1)),
+      ((10, 1, 5), (1, 0, 2)),
+      ((5, 1, 10), (0, 1, 2)),
+      ((10, 20, 30), (1, 2, 0)),
+      ((10, 1, 1), (0, 2, 1)),
+      ((10, 1, 1), (2, 1, 0)),
+      ((10, 1, 1), (1, 2, 0)),
+  )
+  def test_transpose(self, tensor_shape, transpose_axes):
+    t = jnp.arange(math.prod(tensor_shape)).reshape(tensor_shape)
+    t_t = transpose.transpose(t, transpose_axes)
+    self.assertTrue((t_t == jnp.transpose(t, transpose_axes)).all())
+
+  @parameterized.parameters(
       # 'bmnts,bsnh->bmtnh'
       (
           (2, 1, 4, 7, 1),
           (2, 6, 4, 7, 3),
           (2, 3, 4, 5),
           (((4,), (1,)), ((0, 2), (0, 2))),
           (2, 4, 1, 7, 1),
```

### Comparing `aqtp-0.7.3/aqt/jax/v2/utils.py` & `aqtp-0.7.4/aqt/jax/v2/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """utils contains all kinds of small pieces of code used throughout AQT.
 
 Code in this file can't depend on any other AQT file.
 However, it is acceptable to grow pieces of funcionality in this file and later
 promote them to dedicated files.
 """
 
+import dataclasses
 import difflib
 import enum
 import functools
 import pprint
 import re
 from typing import Any, Sequence
 import flax.struct
@@ -64,14 +65,23 @@
 # done. This will exist only temporarily while completing the
 # migration.
 flax_slots_kw_only_dataclass = functools.partial(
     flax_slots_dataclass, kw_only=True
 )
 
 
+def dataclass_field(default='no default value'):
+  # We can't use None as the default's default,
+  # because someone actually might want to have None as default of the field.
+  if default == 'no default value':
+    return dataclasses.field()
+  else:
+    return dataclasses.field(default_factory=default)
+
+
 class QuantMode(enum.Enum):
   TRAIN = 1
   CALIBRATE = 2
   CONVERT = 3
   SERVE = 4
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/README.md` & `aqtp-0.7.4/aqt/jax_legacy/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb` & `aqtp-0.7.4/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/README.md` & `aqtp-0.7.4/aqt/jax_legacy/jax/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/compute_cost_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/compute_cost_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/flax/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/flax/struct.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/flax/struct.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/flax_attention.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/flax_attention_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/flax_layers.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/flax_layers_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     if param.ndim != len(param_axes.names):
       raise ValueError('Length of param dimension does not match axes, '
                        f'{param.shape} != {param_axes.names}.')
     for dim, axis_name in zip(param.shape, param_axes.names):
       output.append(f'{axis_name}={dim}')
     return output
 
-  return jax.tree_map(_create_entry, params, params_axes)
+  return jax.tree.map(_create_entry, params, params_axes)
 
 
 class ConvAqtTest(parameterized.TestCase):
   """Tests for ConvAqt layer."""
 
   def setUp(self):
     super(ConvAqtTest, self).setUp()
@@ -1340,15 +1340,15 @@
             update_bounds=False, quantize_acts=True))
     x = jnp.ones((2, 5))
     y = layer_norm.apply({}, x)
     onp.testing.assert_equal(onp.array(y), onp.zeros(x.shape))
 
 
 def assert_same_tree(a, b):
-  jax.tree_map(
+  jax.tree.map(
       functools.partial(onp.testing.assert_allclose, atol=1e-6, rtol=1e-6), a,
       b)
 
 
 class DenseGeneralAqtTest(parameterized.TestCase):
   """Tests for DenseGeneralAqt layer."""
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/fp_cast.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/fp_cast_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/get_bounds.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/get_bounds_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/hlo_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/hlo_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/README.md` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/check_config_util.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/check_config_util.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/base_config.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/README.md` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/configs_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/hparams_config.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/hparams_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/imagenet.png` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/imagenet.png`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/input_pipeline.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/pokebnn.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/pokebnn_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 def restore_checkpoint(state):
   return checkpoints.restore_checkpoint(FLAGS.model_dir, state)
 
 
 def save_checkpoint(state):
   if jax.host_id() == 0:
     # get train state from the first replica
-    state = jax.device_get(jax.tree_map(lambda x: x[0], state))
+    state = jax.device_get(jax.tree.map(lambda x: x[0], state))
     step = int(state.step)
     checkpoints.save_checkpoint(FLAGS.model_dir, state, step, keep=3)
 
 
 def _get_state_dict_keys_from_flags():
   """Returns key suffixes to look up in flax state dict."""
   state_dict_keys = []
@@ -474,15 +474,15 @@
       do_log = do_log or ((step_in_epoch %
                            (steps_per_epoch // 16) == 0) and end_of_train)
       return do_log
 
     if should_log(step):
       epoch = step // steps_per_epoch
       epoch_metrics = common_utils.get_metrics(epoch_metrics)
-      summary = jax.tree_map(lambda x: x.mean(), epoch_metrics)
+      summary = jax.tree.map(lambda x: x.mean(), epoch_metrics)
       logging.info('train epoch: %d, loss: %.4f, accuracy: %.2f', epoch,
                    summary['loss'], summary['accuracy'] * 100)
       steps_per_sec = (step - last_log_step) / (time.time() - t_loop_start)
       last_log_step = step
       t_loop_start = time.time()
 
       # Write to TensorBoard
@@ -506,15 +506,15 @@
       # sync batch statistics across replicas
       state = imagenet_train_utils.sync_batch_stats(state)
       for _ in range(steps_per_eval):
         eval_batch = next(eval_iter)
         metrics = p_eval_step(state, eval_batch, quantize_weights)
         eval_metrics.append(metrics)
       eval_metrics = common_utils.get_metrics(eval_metrics)
-      summary = jax.tree_map(lambda x: x.mean(), eval_metrics)
+      summary = jax.tree.map(lambda x: x.mean(), eval_metrics)
       logging.info('eval epoch: %d, loss: %.4f, accuracy: %.2f', epoch,
                    summary['loss'], summary['accuracy'] * 100)
       if jax.host_id() == 0:
         for key, val in eval_metrics.items():
           tag = 'eval_%s' % key
           summary_writer.scalar(tag, val.mean(), step)
         summary_writer.flush()
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_benchmark.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train_benchmark.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         8,
         224,
         jnp.float32,
         hparams.model_hparams,
         train=True)
     x = random.normal(random.PRNGKey(1), (8, 224, 224, 3))
     y, new_state = model.apply(state, x, mutable=True)
-    state = jax.tree_map(onp.shape, state)
-    new_state = jax.tree_map(onp.shape, new_state)
+    state = jax.tree.map(onp.shape, state)
+    new_state = jax.tree.map(onp.shape, new_state)
     self.assertEqual(state, new_state)
     self.assertEqual(y.shape, (8, 1000))
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/imagenet/train_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     logits, new_model_state = model.apply(
         variables, batch['image'], mutable=['batch_stats', 'get_bounds'])
     # TODO(yichi): use the checkpoint and the 8-bit model to compute logits
     teacher_logits = teacher['model'](teacher['variables'], batch['image'],
                                       batch['label'])
     # TODO(yichi): replace cross_entropy_loss with KL div loss
     loss = kl_div_loss(logits, teacher_logits)
-    weight_penalty_params = jax.tree_leaves(params)
+    weight_penalty_params = jax.tree.leaves(params)
     weight_decay = hparams.weight_decay
     weight_l2 = sum(
         [jnp.sum(x**2) for x in weight_penalty_params if x.ndim > 1])
     weight_penalty = weight_decay * 0.5 * weight_l2
     loss = loss + weight_penalty
     return loss, (new_model_state, logits)
 
@@ -139,19 +139,19 @@
       opt_state=new_opt_state,
       dynamic_scale=dynamic_scale)
 
   if dynamic_scale:
     # if is_fin == False the gradients contain Inf/NaNs and the old optimizer
     # state should be restored.
     new_state = new_state.replace(
-        opt_state=jax.tree_map(
+        opt_state=jax.tree.map(
             functools.partial(jnp.where, is_fin),
             new_state.opt_state,
             state.opt_state),
-        params=jax.tree_map(
+        params=jax.tree.map(
             functools.partial(jnp.where, is_fin),
             new_state.params,
             state.params))
     metrics['scale'] = dynamic_scale.scale
 
   return new_state, metrics
 
@@ -177,15 +177,15 @@
     # Use _numpy() for zero-copy conversion between TF and NumPy.
     x = x._numpy()  # pylint: disable=protected-access
 
     # reshape (host_batch_size, height, width, 3) to
     # (local_devices, device_batch_size, height, width, 3)
     return x.reshape((local_device_count, -1) + x.shape[1:])
 
-  return jax.tree_map(_prepare, xs)
+  return jax.tree.map(_prepare, xs)
 
 
 def create_input_iter(batch_size, data_dir, image_size, dtype, train, cache):
   """Creates input data iterator."""
   ds = input_pipeline.load_split(
       batch_size,
       data_dir=data_dir,
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/primitives.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/primitives.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/primitives_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/primitives_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/quant_config.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/quant_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/quantization.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/quantization_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/quantization_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/shape_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/shape_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/stats.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/stats_tag.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/stats_tag_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/stats_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/stats_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/test_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/test_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/train_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/train_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/utils.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/README.md` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/bleu.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/bleu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/decode.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
   def gather_fn(x):
     if x.ndim == 0:  # ignore scalars (e.g. cache index)
       return x
     else:
       return x[batch_indices, beam_indices]
 
-  return jax.tree_map(gather_fn, nested)
+  return jax.tree.map(gather_fn, nested)
 
 
 def gather_topk_beams(nested, score_or_log_prob, batch_size, new_beam_size):
   """Gathers the top-k beam slices given by score_or_log_prob array.
 
   Args:
     nested: pytree of arrays or scalars (the latter ignored).
@@ -166,15 +166,15 @@
   live_logprobs0 = jnp.tile(
       jnp.array([0.0] + [NEG_INF] * (beam_size - 1)), [batch_size, 1])
   finished_scores0 = jnp.ones((batch_size, beam_size)) * NEG_INF
   live_seqs0 = jnp.zeros((batch_size, beam_size, max_decode_len), jnp.int32)
   finished_seqs0 = jnp.zeros((batch_size, beam_size, max_decode_len), jnp.int32)
   finished_flags0 = jnp.zeros((batch_size, beam_size), jnp.bool_)
   # add beam dimension to attention cache pytree elements
-  beam_cache0 = jax.tree_map(lambda x: add_beam_dim(x, beam_size), cache)
+  beam_cache0 = jax.tree.map(lambda x: add_beam_dim(x, beam_size), cache)
   return BeamState(
       cur_index=cur_index0,
       live_logprobs=live_logprobs0,
       finished_scores=finished_scores0,
       live_seqs=live_seqs0,
       finished_seqs=finished_seqs0,
       finished_flags=finished_flags0,
@@ -249,26 +249,26 @@
     # dimension for feeding into the model.
     # --> [batch * beam, 1]
     flat_ids = flatten_beam_dim(
         lax.dynamic_slice(state.live_seqs, (0, 0, state.cur_index),
                           (batch_size, beam_size, 1)))
     # Flatten beam dimension into batch to be compatible with model.
     # {[batch, beam, ...], ...} --> {[batch * beam, ...], ...}
-    flat_cache = jax.tree_map(flatten_beam_dim, state.cache)
+    flat_cache = jax.tree.map(flatten_beam_dim, state.cache)
 
     # Call fast-decoder model on current tokens to get next-position logits.
     # --> [batch * beam, vocab]
     flat_logits, new_flat_cache = tokens_to_logits(flat_ids, flat_cache)
 
     # unflatten beam dimension
     # [batch * beam, vocab] --> [batch, beam, vocab]
     logits = unflatten_beam_dim(flat_logits, batch_size, beam_size)
     # Unflatten beam dimension in attention cache arrays
     # {[batch * beam, ...], ...} --> {[batch, beam, ...], ...}
-    new_cache = jax.tree_map(
+    new_cache = jax.tree.map(
         lambda x: unflatten_beam_dim(x, batch_size, beam_size), new_flat_cache)
 
     # Gather log probabilities from logits
     candidate_log_probs = jax.nn.log_softmax(logits)
     # Add new logprobs to existing prefix logprobs.
     # --> [batch, beam, vocab]
     log_probs = (
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 def _restore_from_checkpoint(model, checkpoint_file: str):
   with tf.io.gfile.GFile(checkpoint_file, 'rb') as fp:
     checkpoint = serialization.msgpack_restore(fp.read())
     if 'target' not in checkpoint:
       raise ValueError('Invalid checkpoint %s: no top-level "target".' %
                        checkpoint_file)
     checkpoint_model = checkpoint['target']
-    checkpoint_model = jax.tree_map(jnp.array, checkpoint_model)
+    checkpoint_model = jax.tree.map(jnp.array, checkpoint_model)
     return serialization.from_state_dict(model, checkpoint_model)
 
 
 def encoder_from_file(config: config_dict.ConfigDict,
                       batch_size: int = 8,
                       encode_length: int = 16,
                       use_bfloat16: bool = True,
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/predict.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/predict.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,23 +646,23 @@
              transformer_kwargs: Mapping[str, Any],
              hparams: training_hparams.TrainingHParams) -> Dict[str, Any]:
   """Compute evaluation metrics for a given dataset."""
   eval_metrics = []
   eval_iter = iter(ds)
   dynamic_context = get_dynamic_context(hparams, step, train=False)
   for _, eval_batch in zip(range(num_steps), eval_iter):
-    eval_batch = jax.tree_map(lambda x: x._numpy(), eval_batch)  # pylint: disable=protected-access
+    eval_batch = jax.tree.map(lambda x: x._numpy(), eval_batch)  # pylint: disable=protected-access
     eval_batch = common_utils.shard(eval_batch)
     metrics = p_eval_step(params, eval_batch, state, transformer_kwargs,
                           hparams.model_hparams, dynamic_context)
     eval_metrics.append(metrics)
   eval_metrics = common_utils.get_metrics(eval_metrics)
-  eval_metrics_sums = jax.tree_map(jnp.sum, eval_metrics)
+  eval_metrics_sums = jax.tree.map(jnp.sum, eval_metrics)
   eval_denominator = eval_metrics_sums.pop('denominator')
-  eval_summary = jax.tree_map(
+  eval_summary = jax.tree.map(
       lambda x: x / eval_denominator,  # pylint: disable=cell-var-from-loop
       eval_metrics_sums)
   eval_summary['perplexity'] = jnp.clip(
       jnp.exp(eval_summary['loss']), a_max=1.0e4)
   if summary_writer is not None:
     if jax.host_id() == 0:
       for key, val in eval_summary.items():
@@ -709,20 +709,20 @@
                   params, write_beam_hlo, step: int):
   """Runs inference (ie, translates) over the given dataset."""
 
   predict_iter = iter(ds)
   sources, references, predictions = [], [], []
   dynamic_context = get_dynamic_context(hparams, step, train=False)
   for _, pred_batch in enumerate(predict_iter):
-    pred_batch = jax.tree_map(lambda x: x._numpy(), pred_batch)  # pylint: disable=protected-access
+    pred_batch = jax.tree.map(lambda x: x._numpy(), pred_batch)  # pylint: disable=protected-access
     # Handle final odd-sized batch by padding instead of dropping it.
     cur_pred_batch_size = pred_batch['inputs'].shape[0]
     if cur_pred_batch_size != FLAGS.eval_batch_size:
       logging.info('Translation: uneven batch size %d.', cur_pred_batch_size)
-      pred_batch = jax.tree_map(
+      pred_batch = jax.tree.map(
           lambda x: pad_examples(x, FLAGS.eval_batch_size), pred_batch)
     pred_batch = common_utils.shard(pred_batch)
     per_device_batchsize = pred_batch['inputs'].shape[1]
     unreplicated_cache = initialize_cache(per_device_batchsize,
                                           flax.core.freeze(transformer_kwargs),
                                           hparams.model_hparams)
 
@@ -897,15 +897,15 @@
 
 
 def run_train_step(*, training_state: TrainingState, step: int, batch: Any,
                    hparams: training_hparams.TrainingHParams):
   """Run a single step of training."""
   dynamic_context = get_dynamic_context(hparams, step, train=True)
   # Shard data to devices and do a training step.
-  batch = common_utils.shard(jax.tree_map(lambda x: x._numpy(), batch))  # pylint: disable=protected-access
+  batch = common_utils.shard(jax.tree.map(lambda x: x._numpy(), batch))  # pylint: disable=protected-access
   flax_state, optimizer, metrics, dropout_rngs = p_train_step(
       training_state.optimizer,
       batch,
       dynamic_context,
       training_state.transformer_kwargs,
       WrapHashably(hparams),
       state=training_state.flax_state,
@@ -1229,17 +1229,17 @@
       # Training Metrics
       if FLAGS.compute_train_metrics:
         metrics_all = common_utils.get_metrics(metrics_all)
         state_dict_summary_all = common_utils.get_metrics(
             state_dict_summary_all)
         lr = metrics_all.pop('learning_rate').mean()
 
-        metrics_sums = jax.tree_map(jnp.sum, metrics_all)
+        metrics_sums = jax.tree.map(jnp.sum, metrics_all)
         denominator = metrics_sums.pop('denominator')
-        summary = jax.tree_map(lambda x: x / denominator, metrics_sums)  # pylint: disable=cell-var-from-loop
+        summary = jax.tree.map(lambda x: x / denominator, metrics_sums)  # pylint: disable=cell-var-from-loop
         summary['learning_rate'] = lr
         if FLAGS.log_sparsity_scalars:
           apply_sparsity = metrics_all.pop('apply_sparsity').mean()
           update_weight_sparsity = metrics_all.pop(
               'update_weight_sparsity').mean()
           update_act_sparsity = metrics_all.pop('update_act_sparsity').mean()
           num_update_sparsity = metrics_all.pop('num_update_sparsity').mean()
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/train_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,19 +140,19 @@
                         training_state_initial.flax_state)
     with np.testing.assert_raises(AssertionError):
       np.testing.assert_array_equal(training_state.dropout_rngs,
                                     training_state_initial.dropout_rngs)
     training_state_restored = training_state_initial.restore_checkpoint(
         model_dir=ckpt_dir)
 
-    leaf_equality_tree = jax.tree_map(lambda x, y: jnp.all(x == y),
+    leaf_equality_tree = jax.tree.map(lambda x, y: jnp.all(x == y),
                                            training_state.flax_state,
                                            training_state_restored.flax_state)
     self.assertTrue(
-        all(jax.tree_leaves(leaf_equality_tree)),
+        all(jax.tree.leaves(leaf_equality_tree)),
         'Training state was altered during restoration.')
 
     np.testing.assert_array_equal(training_state.dropout_rngs,
                                   training_state_restored.dropout_rngs)
 
 
 class LearningRateSchedulerTest(absltest.TestCase):
```

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py` & `aqtp-0.7.4/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/README.md` & `aqtp-0.7.4/aqt/jax_legacy/utils/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/__init__.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/analysis_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/common.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/config_schema_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/config_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/hparams_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/hparams_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/pandas_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/report_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/report_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/report_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/tfevent_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils_test.py` & `aqtp-0.7.4/aqt/jax_legacy/utils/tfevent_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/test/aqt_conv_test_base.py` & `aqtp-0.7.4/aqt/test/aqt_conv_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/test/aqt_matmul_test_base.py` & `aqtp-0.7.4/aqt/test/aqt_matmul_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/test/aqt_stats_test_base.py` & `aqtp-0.7.4/aqt/test/aqt_stats_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/test/aqt_tensor_test_base.py` & `aqtp-0.7.4/aqt/test/aqt_tensor_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/aqt/test/aqt_test_shared_base.py` & `aqtp-0.7.4/aqt/test/aqt_test_shared_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/papers/aqt/aqt.pdf` & `aqtp-0.7.4/papers/aqt/aqt.pdf`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/papers/aqt/aqt.tex` & `aqtp-0.7.4/papers/aqt/aqt.tex`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/papers/pokebnn/README.md` & `aqtp-0.7.4/papers/pokebnn/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/papers/pokebnn/cloudtpu_train_pokebnn.sh` & `aqtp-0.7.4/papers/pokebnn/cloudtpu_train_pokebnn.sh`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/papers/pokebnn/tensorboard.ipynb` & `aqtp-0.7.4/papers/pokebnn/tensorboard.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/pyproject.toml` & `aqtp-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/setup.py` & `aqtp-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.3/PKG-INFO` & `aqtp-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtp
-Version: 0.7.3
+Version: 0.7.4
 Summary: Accurate Quantized Training library.
 Author-email: Lukasz Lew <lew@google.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

